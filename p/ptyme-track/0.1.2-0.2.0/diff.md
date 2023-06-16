# Comparing `tmp/ptyme_track-0.1.2.tar.gz` & `tmp/ptyme_track-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptyme_track-0.1.2.tar", max compression
+gzip compressed data, was "ptyme_track-0.2.0.tar", max compression
```

## Comparing `ptyme_track-0.1.2.tar` & `ptyme_track-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2023-06-01 04:30:12.754795 ptyme_track-0.1.2/LICENSE
--rw-r--r--   0        0        0     2020 2023-06-01 04:30:12.754795 ptyme_track-0.1.2/README.md
--rw-r--r--   0        0        0       43 2023-06-01 04:30:12.754795 ptyme_track-0.1.2/ptyme_track/__init__.py
--rw-r--r--   0        0        0     1021 2023-06-01 04:30:12.754795 ptyme_track-0.1.2/ptyme_track/cement.py
--rw-r--r--   0        0        0     6818 2023-06-01 04:30:12.754795 ptyme_track-0.1.2/ptyme_track/client.py
--rw-r--r--   0        0        0      221 2023-06-01 04:30:12.754795 ptyme_track-0.1.2/ptyme_track/cur_times.py
--rw-r--r--   0        0        0     2771 2023-06-01 04:30:12.754795 ptyme_track-0.1.2/ptyme_track/git_ci_diff.py
--rw-r--r--   0        0        0     3333 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/ptyme_track/main.py
--rw-r--r--   0        0        0      936 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/ptyme_track/ptyme_env.py
--rw-r--r--   0        0        0      234 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/ptyme_track/secret.py
--rw-r--r--   0        0        0     2993 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/ptyme_track/server.py
--rw-r--r--   0        0        0      204 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/ptyme_track/signature.py
--rw-r--r--   0        0        0      300 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/ptyme_track/signed_time.py
--rw-r--r--   0        0        0     1951 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/ptyme_track/time_blocks.py
--rw-r--r--   0        0        0     1231 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/ptyme_track/validation.py
--rw-r--r--   0        0        0      798 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 ptyme_track-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2184 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/README.md
+-rw-r--r--   0        0        0       43 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/__init__.py
+-rw-r--r--   0        0        0     1021 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/cement.py
+-rw-r--r--   0        0        0     7050 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/client.py
+-rw-r--r--   0        0        0      221 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/cur_times.py
+-rw-r--r--   0        0        0     2771 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/git_ci_diff.py
+-rw-r--r--   0        0        0     3906 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/main.py
+-rw-r--r--   0        0        0      936 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/ptyme_env.py
+-rw-r--r--   0        0        0     1222 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/secret.py
+-rw-r--r--   0        0        0     2561 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/server.py
+-rw-r--r--   0        0        0      204 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/signature.py
+-rw-r--r--   0        0        0      300 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/signed_time.py
+-rw-r--r--   0        0        0     2091 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/time_blocks.py
+-rw-r--r--   0        0        0     1829 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/ptyme_track/validation.py
+-rw-r--r--   0        0        0      798 2023-06-16 22:52:42.240030 ptyme_track-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2818 1970-01-01 00:00:00.000000 ptyme_track-0.2.0/PKG-INFO
```

### Comparing `ptyme_track-0.1.2/LICENSE` & `ptyme_track-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.1.2/README.md` & `ptyme_track-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,23 @@
 
 ## Usage
 
 ### Installation
 `pip install ptyme-track`
 
 ### Server / client
+For the server, generate a secret first with `ptyme-track --ensure-secret`
+
 Simply run the server with `ptyme_track --server`
 
 For the client, use `ptyme_track --client`
 
 ### Running locally
+Run `ptyme-track --ensure-secret` to generate a secret and update the .gitignore file.
+
 Simply run `ptyme_track --standalone` in the background.
 
 ### Setting directories to watch
 By default, the current working directory is used and hidden directories are ignored. To manually set paths, use the `PTYME_WATCHED_DIRS` environment variable.
 
 ## Cementing work
 To cement your time record, use `ptyme_track --cement <name>`. It is recommended name is your github name. Note this is a filename so it needs to be filename safe (and unique from others). This will create a file `.ptyme_track/<name>`
```

### Comparing `ptyme_track-0.1.2/ptyme_track/cement.py` & `ptyme_track-0.2.0/ptyme_track/cement.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.1.2/ptyme_track/client.py` & `ptyme_track-0.2.0/ptyme_track/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from typing import Dict, Iterator, List, Optional, Tuple, Union
 
 from ptyme_track.cur_times import CEMENTED_PATH, CUR_TIMES_PATH
 from ptyme_track.ptyme_env import (
     PTYME_TRACK_DIR,
     PTYME_WATCH_INTERVAL_MIN,
 )
+from ptyme_track.secret import validate_secret_file_exists
 from ptyme_track.server import sign_time
 from ptyme_track.signed_time import SignedTime
 
 COUNT_MOD = 10  # when to take a small break when hashing files
 IGNORED_COUNT_MOD = 1000  # when to take a small break when ignoring files
 
 logger = logging.getLogger(__name__)
@@ -135,15 +136,15 @@
     def prep_ptyme_dir(self) -> None:
         track_dir = Path(PTYME_TRACK_DIR)
         if not track_dir.exists():
             logger.info(f"Creating {PTYME_TRACK_DIR}")
             track_dir.mkdir()
         git_ignore = track_dir / ".gitignore"
         if not git_ignore.exists():
-            git_ignore.write_text("!.gitignore\n.*")
+            git_ignore.write_text("!.gitignore\n!.cemented\n.*\n")
 
     def _retrieve_signed_time(self) -> SignedTime:
         # retrieve the current time from the server using the built-in urllib module
         response = urllib.request.urlopen(self.server_url)
         logger.debug("Got signed time")
         return json.loads(response.read().decode("utf-8"))
 
@@ -170,9 +171,13 @@
             cur_time_log.write("\n")
 
 
 class StandalonePtymeClient(PtymeClient):
     def __init__(self, watched_dirs: List[str], ignored_dirs: List[str]) -> None:
         super().__init__("", watched_dirs, ignored_dirs)
 
+    def run_forever(self, cemented_file=Path(CEMENTED_PATH)) -> None:
+        validate_secret_file_exists()
+        return super().run_forever(cemented_file)
+
     def _retrieve_signed_time(self) -> SignedTime:
         return sign_time()
```

### Comparing `ptyme_track-0.1.2/ptyme_track/git_ci_diff.py` & `ptyme_track-0.2.0/ptyme_track/git_ci_diff.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.1.2/ptyme_track/main.py` & `ptyme_track-0.2.0/ptyme_track/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,25 +22,35 @@
 
 
 def main() -> None:
     parser = argparse.ArgumentParser(description="ptyme_track")
     parser.add_argument(
         "--generate-secret", action="store_true", help="Generate a secret and update gitignore"
     )
+    parser.add_argument(
+        "--ensure-secret", action="store_true", help="Like generate-secret but only if missing"
+    )
     parser.add_argument("--server", action="store_true", help="Run as server")
     parser.add_argument("--client", action="store_true", help="Run as client")
     # cement takes a parameter which is the name of the file to cement to
     parser.add_argument("--cement", help="Cement to file")
     # time-blocks takes a file to extract the time blocks from
     parser.add_argument("--time-blocks", help="Extract time blocks from file")
     parser.add_argument(
+        "--no-validate",
+        action="store_true",
+        help="Do not validate time blocks against the known secret. This currently only affects --time-blocks",
+    )
+    parser.add_argument(
         "--standalone", action="store_true", help="Run as both a client and a server"
     )
     parser.add_argument(
-        "--git-ci-times", action="store_true", help="Get the current times on this PR from git"
+        "--git-ci-times",
+        action="store_true",
+        help="Get the current times on this PR from git. Note that currently times are not validated",
     )
 
     args = parser.parse_args()
 
     if args.server:
         from ptyme_track.server import run_forever
 
@@ -55,23 +65,30 @@
     if args.git_ci_times:
         base_branch = PTYME_TRACK_BASE_BRANCH
         if not base_branch:
             raise Exception("PTYME_TRACK_BASE_BRANCH environment variable not set.")
         feature_branch = PTYME_TRACK_FEATURE_BRANCH
         display_git_ci_diff_times(base_branch, feature_branch)
         return
+    if args.ensure_secret:
+        from ptyme_track.secret import ensure_secret
+
+        ensure_secret()
+        return
     if args.generate_secret:
-        from ptyme_track.server import generate_secret
+        from ptyme_track.secret import generate_secret
 
         generate_secret()
         return
     if args.time_blocks:
         from ptyme_track.time_blocks import get_time_blocks
 
-        time_blocks = get_time_blocks(Path(args.time_blocks), get_secret())
+        time_blocks = get_time_blocks(
+            Path(args.time_blocks), get_secret(), check_against_secret=(not args.no_validate)
+        )
         total_time = timedelta(minutes=0)
         for block in time_blocks:
             total_time += block.duration
             print(
                 json.dumps(
                     {
                         "start": str(block.start_time),
```

### Comparing `ptyme_track-0.1.2/ptyme_track/ptyme_env.py` & `ptyme_track-0.2.0/ptyme_track/ptyme_env.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.1.2/ptyme_track/server.py` & `ptyme_track-0.2.0/ptyme_track/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import datetime
 import json
-import uuid
 from dataclasses import asdict
 from http.server import BaseHTTPRequestHandler, HTTPServer
-from pathlib import Path
 from urllib.parse import urlparse
 
-from ptyme_track.ptyme_env import SECRET_PATH, SERVER_ID, SERVER_URL
-from ptyme_track.secret import get_secret
+from ptyme_track.ptyme_env import SERVER_ID, SERVER_URL
+from ptyme_track.secret import get_secret, validate_secret_file_exists
 from ptyme_track.signature import signature_from_time
 from ptyme_track.signed_time import SignedTime
 from ptyme_track.validation import validate_signed_time_given_secret
 
 
 class MyRequestHandler(BaseHTTPRequestHandler):
     def do_GET(self) -> None:
@@ -61,28 +59,16 @@
 
 
 def _signature_from_time(time_as_str: str) -> str:
     return signature_from_time(get_secret(), time_as_str)
 
 
 def run_forever(server_class=HTTPServer, handler_class=MyRequestHandler) -> None:
+    validate_secret_file_exists()
     server_host = urlparse(SERVER_URL).hostname
     server_port = urlparse(SERVER_URL).port
     httpd = server_class((server_host, server_port), handler_class)
     httpd.serve_forever()
 
 
-def generate_secret() -> None:
-    with open(SECRET_PATH, "w") as f:
-        f.write(str(uuid.uuid4()))
-    git_ignore = Path(".gitignore")
-    if git_ignore.exists():
-        contents = git_ignore.read_text()
-        if SECRET_PATH not in contents:
-            to_write = contents + "\n# ptyme server secret\n" + SECRET_PATH
-            if contents.endswith("\n"):
-                to_write += "\n"
-            git_ignore.write_text(to_write)
-
-
 if __name__ == "__main__":
     run_forever()
```

### Comparing `ptyme_track-0.1.2/ptyme_track/time_blocks.py` & `ptyme_track-0.2.0/ptyme_track/time_blocks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 from dataclasses import dataclass
 from pathlib import Path
 from typing import List, Optional
 
 from ptyme_track.signed_time import SignedTime
-from ptyme_track.validation import validate_entries
+from ptyme_track.validation import load_entries, validate_entries
 
 
 @dataclass
 class TimeBlock:
     start_time: datetime.datetime
     end_time: datetime.datetime
 
@@ -19,16 +19,20 @@
 
 def get_time_blocks(
     file: Path,
     secret: str,
     buffer_minutes: int = 5,
     start_time_utc: Optional[datetime.datetime] = None,
     end_time_utc: Optional[datetime.datetime] = None,
+    check_against_secret: bool = True,
 ) -> List[TimeBlock]:
-    valid, invalid = validate_entries(file, secret)
+    if check_against_secret:
+        valid, invalid = validate_entries(file, secret)
+    else:
+        valid, invalid = load_entries(file)
     considered = []
     for record in valid:
         signed_time = SignedTime(**record["signed_time"])
         if start_time_utc and signed_time.dt <= start_time_utc:
             continue
         if end_time_utc and signed_time.dt >= end_time_utc:
             continue
```

### Comparing `ptyme_track-0.1.2/ptyme_track/validation.py` & `ptyme_track-0.2.0/ptyme_track/validation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 import json
 from pathlib import Path
-from typing import List, Tuple
+from typing import Callable, List, NamedTuple, Optional, Tuple, Union
 
 from ptyme_track.signature import signature_from_time
 from ptyme_track.signed_time import SignedTime
 
+_SecretAndValidator = NamedTuple(
+    "_SecretAndValidator", [("secret", str), ("validator", Callable)]
+)
+
 
 def validate_signed_time_given_secret(secret: str, signed_time: SignedTime) -> dict:
     server_id_matches = signed_time.server_id == signed_time.server_id
     hash_sig = signature_from_time(secret, signed_time.time)
     return {
         "server_id_match": server_id_matches,
         "time": signed_time.time,
         "sig_matches": hash_sig == signed_time.sig,
     }
 
 
-def validate_entries(file: Path, secret: str) -> Tuple[List[dict], List[dict]]:
-    valid = []
-    invalid = []
+def validate_entries(file: Path, secret: str) -> Tuple[List[dict], List[Union[dict, str]]]:
+    return load_entries(file, _SecretAndValidator(secret, validate_signed_time_given_secret))
+
+
+def load_entries(
+    file: Path, secret_and_validator: Optional[_SecretAndValidator] = None
+) -> Tuple[List[dict], List[Union[dict, str]]]:
+    valid: List[dict] = []
+    invalid: List[Union[dict, str]] = []
     with file.open() as times_file:
         for line in times_file.readlines():
             try:
-                record = json.loads(line)
-                result = validate_signed_time_given_secret(
-                    secret, SignedTime(**record["signed_time"])
-                )
+                record: dict = json.loads(line)
+                if secret_and_validator:
+                    result = secret_and_validator.validator(
+                        secret_and_validator.secret, SignedTime(**record["signed_time"])
+                    )
+                else:
+                    valid.append(record)
+                    continue
             except (json.JSONDecodeError, ValueError, KeyError):
-                invalid.append(record)
+                invalid.append(line)
             else:
                 if result["sig_matches"]:
                     valid.append(record)
                 else:
                     invalid.append(record)
     return valid, invalid
```

### Comparing `ptyme_track-0.1.2/pyproject.toml` & `ptyme_track-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 # soft limit, wrap just before 100 chars
 line-length = 98
 
 [tool.poetry]
 name = "ptyme-track"
-version = "0.1.2"
+version = "0.2.0"
 description = "The obnoxiously named time tracking based on file modifications and signed reporting. The P is silent like in Pterodactyl"
 authors = ["James Hutchison <JamesGHutchison@proton.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "ptyme_track" }]
 
 [tool.poetry.dependencies]
```

### Comparing `ptyme_track-0.1.2/PKG-INFO` & `ptyme_track-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptyme-track
-Version: 0.1.2
+Version: 0.2.0
 Summary: The obnoxiously named time tracking based on file modifications and signed reporting. The P is silent like in Pterodactyl
 License: MIT
 Author: James Hutchison
 Author-email: JamesGHutchison@proton.me
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,19 +19,23 @@
 
 ## Usage
 
 ### Installation
 `pip install ptyme-track`
 
 ### Server / client
+For the server, generate a secret first with `ptyme-track --ensure-secret`
+
 Simply run the server with `ptyme_track --server`
 
 For the client, use `ptyme_track --client`
 
 ### Running locally
+Run `ptyme-track --ensure-secret` to generate a secret and update the .gitignore file.
+
 Simply run `ptyme_track --standalone` in the background.
 
 ### Setting directories to watch
 By default, the current working directory is used and hidden directories are ignored. To manually set paths, use the `PTYME_WATCHED_DIRS` environment variable.
 
 ## Cementing work
 To cement your time record, use `ptyme_track --cement <name>`. It is recommended name is your github name. Note this is a filename so it needs to be filename safe (and unique from others). This will create a file `.ptyme_track/<name>`
```

