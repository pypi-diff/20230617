# Comparing `tmp/fastq_dl-2.0.1.tar.gz` & `tmp/fastq_dl-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastq_dl-2.0.1.tar", max compression
+gzip compressed data, was "fastq_dl-2.0.2.tar", max compression
```

## Comparing `fastq_dl-2.0.1.tar` & `fastq_dl-2.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1076 2023-05-08 03:35:04.772854 fastq_dl-2.0.1/LICENSE
--rw-r--r--   0        0        0    10364 2023-05-08 03:35:04.772854 fastq_dl-2.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-08 03:35:04.772854 fastq_dl-2.0.1/fastq_dl/__init__.py
--rwxr-xr-x   0        0        0    20611 2023-05-08 03:35:04.772854 fastq_dl-2.0.1/fastq_dl/fastq_dl.py
--rw-r--r--   0        0        0      854 2023-05-08 03:35:04.776854 fastq_dl-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    11469 1970-01-01 00:00:00.000000 fastq_dl-2.0.1/setup.py
--rw-r--r--   0        0        0    11324 1970-01-01 00:00:00.000000 fastq_dl-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-17 19:34:34.132264 fastq_dl-2.0.2/LICENSE
+-rw-r--r--   0        0        0    10364 2023-06-17 19:34:34.132264 fastq_dl-2.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-17 19:34:34.132264 fastq_dl-2.0.2/fastq_dl/__init__.py
+-rwxr-xr-x   0        0        0    25349 2023-06-17 19:34:34.132264 fastq_dl-2.0.2/fastq_dl/fastq_dl.py
+-rw-r--r--   0        0        0      917 2023-06-17 19:34:34.132264 fastq_dl-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0    11469 1970-01-01 00:00:00.000000 fastq_dl-2.0.2/setup.py
+-rw-r--r--   0        0        0    11324 1970-01-01 00:00:00.000000 fastq_dl-2.0.2/PKG-INFO
```

### Comparing `fastq_dl-2.0.1/LICENSE` & `fastq_dl-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastq_dl-2.0.1/README.md` & `fastq_dl-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fastq_dl-2.0.1/fastq_dl/fastq_dl.py` & `fastq_dl-2.0.2/fastq_dl/fastq_dl.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,26 +24,28 @@
                 "--provider",
                 "--group-by-experiment",
                 "--group-by-sample",
                 "--outdir",
                 "--prefix",
                 "--cpus",
                 "--max-attempts",
+                "--force",
                 "--only-provider",
+                "--only-download-metadata",
                 "--silent",
                 "--version",
                 "--verbose",
                 "--help",
             ],
         },
     ]
 }
 
 PROGRAM = "fastq-dl"
-VERSION = "2.0.1"
+VERSION = "2.0.2"
 ENA_FAILED = "ENA_NOT_FOUND"
 SRA_FAILED = "SRA_NOT_FOUND"
 SRA = "SRA"
 ENA = "ENA"
 ENA_URL = "https://www.ebi.ac.uk/ena/portal/api/search?result=read_run&format=tsv"
 
 
@@ -90,79 +92,124 @@
             logging.debug(command.decoded_stdout)
             logging.debug(command.decoded_stderr)
 
             if capture_stdout:
                 return command.decoded_stdout
             else:
                 return command.returncode
-        except ExternalCommandFailed as error:
+        except ExternalCommandFailed:
             logging.error(f'"{cmd}" return exit code {command.returncode}')
 
             if is_sra and command.returncode == 3:
                 # The FASTQ isn't on SRA for some reason, try to download from ENA
                 error_msg = command.decoded_stderr.split("\n")[0]
                 logging.error(error_msg)
                 return SRA_FAILED
 
             if attempt < max_attempts:
                 logging.error(f"Retry execution ({attempt} of {max_attempts})")
                 time.sleep(10)
             else:
-                raise error
+                if is_sra:
+                    return SRA_FAILED
+                else:
+                    return ENA_FAILED
 
 
 def sra_download(
-    accession: str, outdir: str, cpus: int = 1, max_attempts: int = 10
+    accession: str,
+    outdir: str,
+    cpus: int = 1,
+    max_attempts: int = 10,
+    force: bool = False,
 ) -> dict:
     """Download FASTQs from SRA using fasterq-dump.
 
     Args:
         accession (str): The accession to download associated FASTQs.
         outdir (str): Directory to write FASTQs to.
         cpus (int, optional): Number of CPUs to use. Defaults to 1.
         max_attempts (int, optional): Maximum number of download attempts. Defaults to 10.
 
     Returns:
         dict: A dictionary of the FASTQs and their paired status.
     """
     fastqs = {"r1": "", "r2": "", "single_end": True}
     se = f"{outdir}/{accession}.fastq.gz"
-    pe = f"{outdir}/{accession}_2.fastq.gz"
+    pe1 = f"{outdir}/{accession}_1.fastq.gz"
+    pe2 = f"{outdir}/{accession}_2.fastq.gz"
+
+    # remove existing files if force is selected.
+    # TODO: only remove if the MD5 checksum is different.
+    if force and Path(se).exists():
+        Path(se).unlink()
+        logging.warning(f"Overwriting existing file: {se}")
+    if force and Path(pe1).exists() and Path(pe2).exists():
+        Path(pe1).unlink()
+        Path(pe2).unlink()
+        logging.warning(f"Overwriting existing file: {pe1}")
+        logging.warning(f"Overwriting existing file: {pe2}")
 
-    if not Path(se).exists() and not Path(pe).exists():
+    if not Path(se).exists() and not (Path(pe1).exists() and Path(pe2).exists()):
         Path(outdir).mkdir(parents=True, exist_ok=True)
+
+        # TODO: add check of read count as a proxy for checksum?
         outcome = execute(
-            f"fasterq-dump {accession} --split-files --threads {cpus}",
+            f"prefetch {accession} --max-size 10T -o {accession}.sra",
             max_attempts=max_attempts,
             directory=outdir,
             is_sra=True,
         )
+
+        if outcome == SRA_FAILED:
+            return outcome
+        else:
+            outcome = execute(
+                f"fasterq-dump {accession} --split-3 --mem 1G --threads {cpus}",
+                max_attempts=max_attempts,
+                directory=outdir,
+                is_sra=True,
+            )
+
         if outcome == SRA_FAILED:
             return outcome
         else:
             execute(f"pigz --force -p {cpus} -n {accession}*.fastq", directory=outdir)
+            Path(f"{outdir}/{accession}.sra").unlink()
+    else:
+        if Path(se).exists():
+            logging.debug(f"Skipping re-download of existing file: {se}")
+        elif Path(pe1).exists() and Path(pe2).exists():
+            logging.debug(f"Skipping re-download of existing file: {pe1}")
+            logging.debug(f"Skipping re-download of existing file: {pe2}")
 
     if Path(f"{outdir}/{accession}_2.fastq.gz").exists():
         # Paired end
         fastqs["r1"] = f"{outdir}/{accession}_1.fastq.gz"
         fastqs["r2"] = f"{outdir}/{accession}_2.fastq.gz"
-        fastqs["single_end"] = False
+        if Path(f"{outdir}/{accession}.fastq.gz").exists():
+            fastqs["single_end"] = f"{outdir}/{accession}.fastq.gz"
+        else:
+            fastqs["single_end"] = False
     else:
         fastqs["r1"] = f"{outdir}/{accession}.fastq.gz"
 
     return fastqs
 
 
-def ena_download(run: str, outdir: str, max_attempts: int = 10) -> dict:
+def ena_download(
+    run: str, outdir: str, max_attempts: int = 10, force: bool = False
+) -> dict:
     """Download FASTQs from ENA FTP using wget.
 
     Args:
         accession (str): The accession to download associated FASTQs.
         outdir (str): Directory to write FASTQs to.
         max_attempts (int, optional): Maximum number of download attempts. Defaults to 10.
+        force: (bool, optional): Whether to overwrite existing files if the MD5's do not match
 
     Returns:
         dict: A dictionary of the FASTQs and their paired status.
     """
     fastqs = {"r1": "", "r2": "", "single_end": True}
     ftp = run["fastq_ftp"]
     if not ftp:
@@ -190,19 +237,18 @@
                 exp_fq = f'{run["run_accession"]}.fastq.gz'
                 if len(ftp) != 1 and obs_fq != exp_fq:
                     continue
 
         # Download Run
         if md5[i]:
             fastq = download_ena_fastq(
-                ftp[i],
-                outdir,
-                md5[i],
-                max_attempts=max_attempts,
+                ftp[i], outdir, md5[i], max_attempts=max_attempts, force=force
             )
+            if fastq == ENA_FAILED:
+                return ENA_FAILED
 
             if is_r2:
                 fastqs["r2"] = fastq
                 fastqs["single_end"] = False
             else:
                 fastqs["r1"] = fastq
 
@@ -234,54 +280,70 @@
 
 
 def download_ena_fastq(
     ftp: str,
     outdir: str,
     md5: str,
     max_attempts: int = 10,
+    force: bool = False,
 ) -> str:
     """Download FASTQs from ENA using FTP.
 
     Args:
         ftp (str): The FTP address of the FASTQ file.
         outdir (str): Directory to download the FASTQ to.
         md5 (str): Expected MD5 checksum of the FASTQ.
         max_attempts (int, optional): Maximum number of download attempts. Defaults to 10.
+        force: (bool, optional): Whether to overwrite existing files if the MD5's do not match
 
     Returns:
         str: Path to the downloaded FASTQ.
     """
     success = False
     attempt = 0
     fastq = f"{outdir}/{Path(ftp).name}"
 
+    if Path(fastq).exists() and force:
+        logging.warning(f"Overwriting existing file: {fastq}")
+        Path(fastq).unlink()
+
     if not Path(fastq).exists():
         Path(outdir).mkdir(parents=True, exist_ok=True)
 
         while not success:
             logging.info(f"\t\t{Path(ftp).name} FTP download attempt {attempt + 1}")
-            execute(f"wget --quiet -O {fastq} ftp://{ftp}", max_attempts=max_attempts)
-
-            fastq_md5 = md5sum(fastq)
-            if fastq_md5 != md5:
-                logging.debug(f"MD5s, Observed: {fastq_md5}, Expected: {md5}")
-                attempt += 1
-                if Path(fastq).exists():
-                    Path(fastq).unlink()
-                if attempt > max_attempts:
-                    logging.error(
-                        f"Download failed after {max_attempts} attempts. "
-                        "Please try again later or manually from SRA/ENA."
-                    )
-                    sys.exit(1)
+            outcome = execute(
+                f"wget --quiet -O {fastq} ftp://{ftp}", max_attempts=max_attempts
+            )
+            if outcome == ENA_FAILED:
+                return ENA_FAILED
 
-                # Hiccup? Wait a bit before trying again.
-                time.sleep(10)
-            else:
+            if force:
+                logging.debug(f"--force used, skipping MD5sum check for {fastq}")
                 success = True
+            else:
+                fastq_md5 = md5sum(fastq)
+                if fastq_md5 != md5:
+                    logging.debug(f"MD5s, Observed: {fastq_md5}, Expected: {md5}")
+                    attempt += 1
+                    if Path(fastq).exists():
+                        Path(fastq).unlink()
+                    if attempt > max_attempts:
+                        logging.error(
+                            f"Download failed after {max_attempts} attempts. "
+                            "Please try again later or manually from SRA/ENA."
+                        )
+                        sys.exit(1)
+
+                    # Hiccup? Wait a bit before trying again.
+                    time.sleep(10)
+                else:
+                    success = True
+    else:
+        logging.debug(f"Skipping re-download of existing file: {fastq}")
 
     return fastq
 
 
 def merge_runs(runs: list, output: str) -> None:
     """Merge runs from an experiment or sample.
 
@@ -341,42 +403,66 @@
                 else:
                     col_names = cols
         return [True, data]
     else:
         return [False, [r.status_code, r.text]]
 
 
-def get_run_info(accession: str, query: str) -> tuple:
+def get_run_info(
+    accession: str, query: str, provider: str, only_provider: bool
+) -> tuple:
     """Retrieve a list of samples available from ENA.
 
     The first attempt will be against ENA, and if that fails, SRA will be queried. This should
     capture those samples not yet synced between ENA and SRA.
 
     Args:
         accession (str): The accession to search for.
         query (str): A formatted query for ENA searches.
+        provider (str): Limit queries only to the specified provider (requires only_provider be true)
+        only_provider (bool): If true, limit queries to the specified provider
 
     Returns:
         tuple: Records associated with the accession.
     """
 
     logging.debug("Querying ENA for metadata...")
-    success, ena_data = get_ena_metadata(query)
-    if success:
-        return ENA, ena_data
+
+    if only_provider:
+        logging.debug(f"--only-provider supplied, limiting queries to {provider}")
+        if provider.lower() == "ena":
+            success, ena_data = get_ena_metadata(query)
+            if success:
+                return ENA, ena_data
+            else:
+                logging.error("There was an issue querying ENA, exiting...")
+                logging.error(f"STATUS: {ena_data[0]}")
+                logging.error(f"TEXT: {ena_data[1]}")
+                sys.exit(1)
+        else:
+            success, sra_data = get_sra_metadata(accession)
+            if success:
+                return SRA, sra_data
+            else:
+                logging.error("There was an issue querying SRA, exiting...")
+                sys.exit(1)
     else:
-        logging.debug("Failed to get metadata from ENA. Trying SRA...")
-        success, sra_data = get_sra_metadata(accession)
-        if not success:
-            logging.error("There was an issue querying ENA and SRA, exiting...")
-            logging.error(f"STATUS: {ena_data[0]}")
-            logging.error(f"TEXT: {ena_data[1]}")
-            sys.exit(1)
+        success, ena_data = get_ena_metadata(query)
+        if success:
+            return ENA, ena_data
         else:
-            return SRA, sra_data
+            logging.debug("Failed to get metadata from ENA. Trying SRA...")
+            success, sra_data = get_sra_metadata(accession)
+            if not success:
+                logging.error("There was an issue querying ENA and SRA, exiting...")
+                logging.error(f"STATUS: {ena_data[0]}")
+                logging.error(f"TEXT: {ena_data[1]}")
+                sys.exit(1)
+            else:
+                return SRA, sra_data
 
 
 def write_tsv(data: dict, output: str) -> None:
     """Write a TSV file.
 
     Args:
         data (dict): Data to be written to TSV.
@@ -481,20 +567,29 @@
     "--max-attempts",
     "-m",
     default=10,
     show_default=True,
     help="Maximum number of download attempts.",
 )
 @click.option(
-    "-F",
+    "--force",
+    is_flag=True,
+    help="Overwrite existing files if their MD5 checksums do not match.",
+)
+@click.option(
     "--only-provider",
     is_flag=True,
     help="Only attempt download from specified provider.",
 )
 @click.option(
+    "--only-download-metadata",
+    is_flag=True,
+    help="Skip FASTQ downloads, and retrieve only the metadata.",
+)
+@click.option(
     "--cpus",
     default=1,
     show_default=True,
     help="Total cpus used for downloading from SRA.",
 )
 @click.option("--silent", is_flag=True, help="Only critical errors will be printed.")
 @click.option("--verbose", "-v", is_flag=True, help="Print debug related text.")
@@ -503,15 +598,17 @@
     accession,
     provider,
     group_by_experiment,
     group_by_sample,
     outdir,
     prefix,
     max_attempts,
+    force,
     only_provider,
+    only_download_metadata,
     cpus,
     silent,
     verbose,
 ):
     """Download FASTQ files from ENA or SRA."""
     # Setup logs
     logging.basicConfig(
@@ -523,117 +620,128 @@
     )
 
     logging.getLogger().setLevel(
         logging.ERROR if silent else logging.DEBUG if verbose else logging.INFO
     )
     # Start Download Process
     query = validate_query(accession)
-    data_from, ena_data = get_run_info(accession, query)
+    data_from, ena_data = get_run_info(accession, query, provider, only_provider)
 
     logging.info(f"Query: {accession}")
     logging.info(f"Archive: {provider}")
-    logging.info(f"Total Runs To Download: {len(ena_data)}")
+    if only_download_metadata:
+        logging.info(f"Total Runs Found: {len(ena_data)}")
+        logging.debug("--only-download-metadata used, skipping FASTQ downloads")
+    else:
+        logging.info(f"Total Runs To Download: {len(ena_data)}")
     downloaded = {}
     runs = {} if group_by_experiment or group_by_sample else None
     outdir = Path.cwd() if outdir == "./" else f"{outdir}"
 
-    for i, run_info in enumerate(ena_data):
-        run_acc = run_info["run_accession"]
-        if run_acc not in downloaded:
-            downloaded[run_acc] = True
-        else:
-            logging.warning(f"Duplicate run {run_acc} found, skipping re-download...")
-            continue
-        logging.info(f"\tWorking on run {run_acc}...")
-        fastqs = None
-        if provider == "ena" and data_from == ENA:
-            fastqs = ena_download(
-                run_info,
-                outdir,
-                max_attempts=max_attempts,
-            )
-
-            if fastqs == ENA_FAILED:
-                if only_provider:
-                    logging.error(f"\tNo fastqs found in ENA for {run_acc}")
-                    ena_data[i]["error"] = ENA_FAILED
-                    fastqs = None
-                else:
-                    # Retry download from SRA
-                    logging.info(f"\t{run_acc} not found on ENA, retrying from SRA")
-
-                    fastqs = sra_download(
-                        run_acc,
-                        outdir,
-                        cpus=cpus,
-                        max_attempts=max_attempts,
-                    )
-                    if fastqs == SRA_FAILED:
-                        logging.error(f"\t{run_acc} not found on SRA")
-                        ena_data[i]["error"] = f"{ENA_FAILED}&{SRA_FAILED}"
-                        fastqs = None
+    if only_download_metadata:
+        Path(outdir).mkdir(parents=True, exist_ok=True)
+        logging.info(f"Writing metadata to {outdir}/{prefix}-run-info.tsv")
+        write_tsv(ena_data, f"{outdir}/{prefix}-run-info.tsv")
+    else:
+        for i, run_info in enumerate(ena_data):
+            run_acc = run_info["run_accession"]
+            if run_acc not in downloaded:
+                downloaded[run_acc] = True
+            else:
+                logging.warning(
+                    f"Duplicate run {run_acc} found, skipping re-download..."
+                )
+                continue
+            logging.info(f"\tWorking on run {run_acc}...")
+            fastqs = None
+            if provider.lower() == "ena" and data_from == ENA:
+                fastqs = ena_download(
+                    run_info, outdir, max_attempts=max_attempts, force=force
+                )
 
-        else:
-            fastqs = sra_download(
-                run_acc,
-                outdir,
-                cpus=cpus,
-                max_attempts=max_attempts,
-            )
-            if fastqs == SRA_FAILED:
-                if only_provider or data_from == SRA:
-                    logging.error(f"\t{run_acc} not found on SRA or ENA")
-                    ena_data[i]["error"] = SRA_FAILED
-                    fastqs = None
-                else:
-                    # Retry download from ENA
-                    logging.info(f"\t{run_acc} not found on SRA, retrying from ENA")
-                    fastqs = ena_download(
-                        run_info,
-                        outdir,
-                        max_attempts=max_attempts,
-                    )
-                    if fastqs == ENA_FAILED:
+                if fastqs == ENA_FAILED:
+                    if only_provider:
                         logging.error(f"\tNo fastqs found in ENA for {run_acc}")
-                        ena_data[i]["error"] = f"{SRA_FAILED}&{ENA_FAILED}"
+                        ena_data[i]["error"] = ENA_FAILED
                         fastqs = None
+                    else:
+                        # Retry download from SRA
+                        logging.info(f"\t{run_acc} not found on ENA, retrying from SRA")
+
+                        fastqs = sra_download(
+                            run_acc,
+                            outdir,
+                            cpus=cpus,
+                            max_attempts=max_attempts,
+                        )
+                        if fastqs == SRA_FAILED:
+                            logging.error(f"\t{run_acc} not found on SRA")
+                            ena_data[i]["error"] = f"{ENA_FAILED}&{SRA_FAILED}"
+                            fastqs = None
 
-        # Add the download results
-        if fastqs:
-            if group_by_experiment or group_by_sample:
-                name = run_info["sample_accession"]
-                if group_by_experiment:
-                    name = run_info["experiment_accession"]
-
-                if name not in runs:
-                    runs[name] = {"r1": [], "r2": []}
-
-                if fastqs["single_end"]:
-                    runs[name]["r1"].append(fastqs["r1"])
-                else:
-                    runs[name]["r1"].append(fastqs["r1"])
-                    runs[name]["r2"].append(fastqs["r2"])
-
-    # If applicable, merge runs
-    if runs:
-        for name, vals in runs.items():
-            if len(vals["r1"]) and len(vals["r2"]):
-                # Not all runs labeled as paired are actually paired.
-                if len(vals["r1"]) == len(vals["r2"]):
-                    logging.info(f"\tMerging paired end runs to {name}...")
-                    merge_runs(vals["r1"], f"{outdir}/{name}_R1.fastq.gz")
-                    merge_runs(vals["r2"], f"{outdir}/{name}_R2.fastq.gz")
+            else:
+                fastqs = sra_download(
+                    run_acc,
+                    outdir,
+                    cpus=cpus,
+                    max_attempts=max_attempts,
+                )
+                if fastqs == SRA_FAILED:
+                    if only_provider or data_from == SRA:
+                        logging.error(f"\t{run_acc} not found on SRA or ENA")
+                        ena_data[i]["error"] = SRA_FAILED
+                        fastqs = None
+                    else:
+                        # Retry download from ENA
+                        logging.info(f"\t{run_acc} not found on SRA, retrying from ENA")
+                        fastqs = ena_download(
+                            run_info, outdir, max_attempts=max_attempts, force=force
+                        )
+                        if fastqs == ENA_FAILED:
+                            logging.error(f"\tNo fastqs found in ENA for {run_acc}")
+                            ena_data[i]["error"] = f"{SRA_FAILED}&{ENA_FAILED}"
+                            fastqs = None
+
+            # Add the download results
+            if fastqs:
+                if group_by_experiment or group_by_sample:
+                    name = run_info["sample_accession"]
+                    if group_by_experiment:
+                        name = run_info["experiment_accession"]
+
+                    if name not in runs:
+                        runs[name] = {"r1": [], "r2": []}
+
+                    if fastqs["single_end"]:
+                        runs[name]["r1"].append(fastqs["r1"])
+                    else:
+                        runs[name]["r1"].append(fastqs["r1"])
+                        runs[name]["r2"].append(fastqs["r2"])
+
+        # If applicable, merge runs
+        if runs:
+            for name, vals in runs.items():
+                if len(vals["r1"]) and len(vals["r2"]):
+                    # Not all runs labeled as paired are actually paired.
+                    if len(vals["r1"]) == len(vals["r2"]):
+                        logging.info(f"\tMerging paired end runs to {name}...")
+                        merge_runs(vals["r1"], f"{outdir}/{name}_R1.fastq.gz")
+                        merge_runs(vals["r2"], f"{outdir}/{name}_R2.fastq.gz")
+                    else:
+                        logging.info("\tMerging single end runs to experiment...")
+                        merge_runs(vals["r1"], f"{outdir}/{name}.fastq.gz")
                 else:
                     logging.info("\tMerging single end runs to experiment...")
                     merge_runs(vals["r1"], f"{outdir}/{name}.fastq.gz")
-            else:
-                logging.info("\tMerging single end runs to experiment...")
-                merge_runs(vals["r1"], f"{outdir}/{name}.fastq.gz")
-        write_tsv(runs, f"{outdir}/{prefix}-run-mergers.tsv")
-    write_tsv(ena_data, f"{outdir}/{prefix}-run-info.tsv")
+            logging.info(
+                f"Writing merged run info to {outdir}/{prefix}-run-mergers.tsv"
+            )
+            write_tsv(runs, f"{outdir}/{prefix}-run-mergers.tsv")
+        logging.info(f"Writing metadata to {outdir}/{prefix}-run-info.tsv")
+        write_tsv(ena_data, f"{outdir}/{prefix}-run-info.tsv")
 
 
 def main():
     fastqdl()
 
 
 if __name__ == "__main__":
```

### Comparing `fastq_dl-2.0.1/pyproject.toml` & `fastq_dl-2.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [tool.poetry]
 name = "fastq-dl"
-version = "2.0.1"
+version = "2.0.2"
 description = "Download FASTQ files from SRA or ENA repositories."
 authors = [
     "Robert A. Petit III <robbie.petit@gmail.com>",
-    "Michael B. Hall <michael@mbh.sh>"
+    "Michael B. Hall <michael@mbh.sh>",
+    "Gerry Tonkin-Hill",
+    "Jie Zhu",
+    "Timothy D. Read"
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rpetit3/fastq-dl"
 repository = "https://github.com/rpetit3/fastq-dl"
 keywords = ["bioinformatics", "fastq", "download", "SRA", "ENA"]
 
 [tool.poetry.scripts]
 fastq-dl = "fastq_dl.fastq_dl:main"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
-requests = "^2.28.2"
+requests = "^2.31.0"
 pysradb = "^1.4"
 rich-click = "^1.6.1"
 executor = "^23.2"
 rich = "^13.3.1"
 markdown-it-py = "2.2.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `fastq_dl-2.0.1/setup.py` & `fastq_dl-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['executor>=23.2,<24.0',
  'markdown-it-py==2.2.0',
  'pysradb>=1.4,<2.0',
- 'requests>=2.28.2,<3.0.0',
+ 'requests>=2.31.0,<3.0.0',
  'rich-click>=1.6.1,<2.0.0',
  'rich>=13.3.1,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['fastq-dl = fastq_dl.fastq_dl:main']}
 
 setup_kwargs = {
     'name': 'fastq-dl',
-    'version': '2.0.1',
+    'version': '2.0.2',
     'description': 'Download FASTQ files from SRA or ENA repositories.',
     'long_description': "[![GitHub release (latest by date)](https://img.shields.io/github/v/release/rpetit3/fastq-dl)](https://github.com/bactopia/rpetit3/fastq-dl)\n[![Anaconda-Server Badge](https://anaconda.org/bioconda/fastq-dl/badges/downloads.svg)](https://anaconda.org/bioconda/fastq-dl)\n[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/rpetit3/fastq-dl)\n\n# fastq-dl\n\nDownload FASTQ files from the [European Nucleotide Archive](https://www.ebi.ac.uk/ena) or the\n[Sequence Read Archive](https://www.ncbi.nlm.nih.gov/sra) repositories.\n\n## Introduction\n\n`fastq-dl` takes an ENA/SRA accession (Study, Sample, Experiment, or Run) and queries ENA (via\n[Data Warehouse API](https://www.ebi.ac.uk/ena/browse/search-rest)) to determine the associated\nmetadata. It then downloads FASTQ files for each Run. For Samples or Experiments with multiple\nRuns, users can optionally merge the runs.\n\n## Installation\n\n### Bioconda\n\n`fastq-dl` is available from [Bioconda](https://bioconda.github.io/) and I highly recommend you\ngo this route to for installation.\n\n```{bash}\nconda create -n fastq-dl -c conda-forge -c bioconda fastq-dl\nconda activate fastq-dl \n```\n\n## Usage\n\n```{bash}\nfastq-dl --help\n                                                                                          \n Usage: fastq-dl [OPTIONS]                                                                \n                                                                                          \n Download FASTQ files from ENA or SRA.                                                    \n                                                                                          \n╭─ Required Options ─────────────────────────────────────────────────────────────────────╮\n│ *  --accession  -a  TEXT  ENA/SRA accession to query. (Study, Sample, Experiment, Run  │\n│                           accession) [required]                                        │\n╰────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ───────────────────────────────────────────────────────────────────╮\n│ --provider                 [ena|sra]  Specify which provider (ENA or SRA) to use.      │\n│                                       [default: ena]                                   │\n│ --group-by-experiment                 Group Runs by experiment accession.              │\n│ --group-by-sample                     Group Runs by sample accession.                  │\n│ --outdir               -o  TEXT       Directory to output downloads to. [default: ./]  │\n│ --prefix                   TEXT       Prefix to use for naming log files.              │\n│                                       [default: fastq]                                 │\n│ --cpus                     INTEGER    Total cpus used for downloading from SRA.        │\n│                                       [default: 1]                                     │\n│ --max-attempts         -m  INTEGER    Maximum number of download attempts.             │\n│                                       [default: 10]                                    │\n│ --only-provider        -F             Only attempt download from specified provider.   │\n│ --silent                              Only critical errors will be printed.            │\n│ --version              -V             Show the version and exit.                       │\n│ --verbose              -v             Print debug related text.                        │\n│ --help                 -h             Show this message and exit.                      │\n╰────────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n*fastq-dl* requires a single ENA/SRA Study, Sample, Experiment, or Run accession and FASTQs\nfor all Runs that fall under the given accession will be downloaded. For example, if a Study\naccession is given all Runs under that studies umbrella will be downloaded. By default, \n`fastq-dl` will try to download from ENA first, then SRA.\n\n### --accession\n\nThe accession you would like to download associated FASTQS for. Currently the following types\nof accessions are accepted.\n\n| Accession Type | Prefixes            | Example                                  |\n|----------------|---------------------|------------------------------------------|\n| BioProject     | PRJEB, PRJNA, PRJDB | PRJEB42779, PRJNA480016, PRJDB14838      |\n| Study          | ERP, DRP, SRP       | ERP126685, DRP009283, SRP158268          |\n| BioSample      | SAMD, SAME, SAMN    | SAMD00258402, SAMEA7997453, SAMN06479985 |\n| Sample         | ERS, DRS, SRS       | ERS5684710, DRS259711, SRS2024210        |\n| Experiment     | ERX, DRX, SRX       | ERX5050800, DRX406443, SRX4563689        |\n| Run            | ERR, DRR, SRR       | ERR5260405, DRR421224, SRR7706354        |\n\nThe accessions are using regular expressions from the [ENA Training Modules - Accession Numbers](https://ena-docs.readthedocs.io/en/latest/submit/general-guide/accessions.html#accession-numbers) section.\n\n### --provider\n\n`fastq-dl` gives you the option to download from ENA or SRA. the `--provider` option will\nspecify which provider you would like to attempt downloads from first. If a download fails\nfrom the first provider, additional attempts will be made using the other provider.\n\nENA was selected as the default provider because the FASTQs are available directly without\nthe need for conversion.\n\n### --only-provider\n\nBy default, `fastq-dl` will fallback on a secondary provider to attempt downloads. There\nmay be cases where you would prefer to disable this feature, and that is exactly the\npurpose of `--only-provider`. When provided, if a FASTQ cannot be downloaded from the\noriginal provider, no additional attempts will be made.\n\n### --group-by-experiment & --group-by-sample\n\nThere maybe times you might want to group Run accessions based on a Experiment or Sample\naccessions. This will merge FASTQs associated with a Run accession based its associated\nExperiment accession (`--group-by-experiment`) or Sample accession (`--group-by-sample`).\n\n## Output Files\n\n| Extension          | Description                                                                              |\n|--------------------|------------------------------------------------------------------------------------------|\n| `-run-info.tsv`    | Tab-delimited file containing metadata for each Run downloaded                           |\n| `-run-mergers.tsv` | Tab-delimited file merge information from `--group-by-experiment` or `--group-by-sample` |\n| `.fastq.gz`        | FASTQ files downloaded from ENA or SRA                                                   |\n\n## Example Usage\n\n#### Download FASTQs associated with a Study\n\nSometimes you might be reading a paper and they very kindly provided a Bioproject of all\nthe samples they sequenced. So, you decide you want to download FASTQs for all the samples\nasscociated with the Bioproject. `fastq-dl` can help you with that! \n\n```{bash}\nfastq-dl --accession PRJNA248678 --provider SRA\nfastq-dl --accession PRJNA248678\n```\n\nThe above commands will download the 3 Runs that fall under Study accession [PRJNA248678](https://www.ebi.ac.uk/ena/browser/view/PRJNA248678)\nfrom either SRA (`--provider SRA`) or ENA (without `--provider`).\n\n#### Download FASTQs associated with an Experiment\n\nLet's say instead of the whole Bioproject you just want a single Experiment. You can do\nthat as well.\n\n```{bash}\nfastq-dl --accession SRX477044\n```\n\nThe above command would download the Run accessions from ENA that fall under Experiment SRX477044.\n\nThe relationship of Experiment to Run is a 1-to-many relationship, or there can be many Run accessions\nassociated with a single Experiment Accession (e.g. re-sequencing the same sample). Although in most\ncases, it is a 1-to-1 relationship, you can use `--group-by-experiment` to merge multiple runs\nassociated with an Experiment accession into a single FASTQ file.\n\n#### Download FASTQs associated with an Sample\n\nOk, this time you just want a single Sample, or Biosample.\n\n```{bash}\nfastq-dl --accession SRS1904245 --provider SRA\n```\n\nThe above command would download the Run accessions from SRA that fall under Sample SRS1904245.\n\nSimilar to Experiment accessions, the relationship of Sample to Run is a 1-to-many relationship,\nor there can be many Run accessions associated with a single Sample Accession. Although in most\ncases, it is a 1-to-1 relationship, you can use `--group-by-sample` to merge multiple runs\nassociated with an Sample accession into a single FASTQ file.\n\n_Warning! For some type strains (e.g. S. aureus USA300) a Biosample accession might be associated with\n100s or 1000s of Run accessions. These Runs are likely associated with many different conditions and\nreally should not fall under a single BioSample accession. Please consider this when using\n`--group-by-sample`.\n\n#### Download FASTQs associated with a Run\n\nLet's keep it super simple and just download a Run.\n\n```\nfastq-dl --accession SRR1178105 --provider SRA\n```\n\nThe above command would download the Run SRR1178105 from SRA. Run accessions are the end of the\nline (1-to-1 relationship), so you will always get the expected Run.\n\n## Alternatives\n`fastq-dl`, is a spin-off of [ena-dl](https://github.com/rpetit3/ena-dl), that has been developed for\nusage with [Bactopia](https://github.com/bactopia/bactopia). With this in mind, EBI/NCBI and provide\ntheir own tools ([enaBrowserTools](https://github.com/enasequence/enaBrowserTools) and\n[SRA Toolkit](https://github.com/ncbi/sra-tools)) that offer more extensive access to their databases.\n",
     'author': 'Robert A. Petit III',
     'author_email': 'robbie.petit@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/rpetit3/fastq-dl',
```

### Comparing `fastq_dl-2.0.1/PKG-INFO` & `fastq_dl-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastq-dl
-Version: 2.0.1
+Version: 2.0.2
 Summary: Download FASTQ files from SRA or ENA repositories.
 Home-page: https://github.com/rpetit3/fastq-dl
 License: MIT
 Keywords: bioinformatics,fastq,download,SRA,ENA
 Author: Robert A. Petit III
 Author-email: robbie.petit@gmail.com
 Requires-Python: >=3.7.1,<4.0.0
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: executor (>=23.2,<24.0)
 Requires-Dist: markdown-it-py (==2.2.0)
 Requires-Dist: pysradb (>=1.4,<2.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.3.1,<14.0.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Project-URL: Repository, https://github.com/rpetit3/fastq-dl
 Description-Content-Type: text/markdown
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/rpetit3/fastq-dl)](https://github.com/bactopia/rpetit3/fastq-dl)
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/fastq-dl/badges/downloads.svg)](https://anaconda.org/bioconda/fastq-dl)
```

