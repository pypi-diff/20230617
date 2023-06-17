# Comparing `tmp/wgd-2.0.16.tar.gz` & `tmp/wgd-2.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wgd-2.0.16.tar", last modified: Tue Jun  6 13:41:28 2023, max compression
+gzip compressed data, was "dist/wgd-2.0.17.tar", last modified: Sat Jun 17 12:42:31 2023, max compression
```

## Comparing `wgd-2.0.16.tar` & `wgd-2.0.17.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-06 13:41:28.610749 wgd-2.0.16/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.16/LICENSE
--rwxrwxrwx   0 heche     (1000) heche     (1000)    44508 2023-06-06 13:41:28.610749 wgd-2.0.16/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)    39901 2023-06-02 15:36:16.000000 wgd-2.0.16/README.md
--rwxrwxrwx   0 heche     (1000) heche     (1000)    50452 2023-05-30 15:36:15.000000 wgd-2.0.16/cli.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-06-06 13:41:28.610749 wgd-2.0.16/setup.cfg
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1904 2023-06-06 13:40:10.000000 wgd-2.0.16/setup.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-06 13:41:28.580312 wgd-2.0.16/test/
--rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-05-08 19:45:47.000000 wgd-2.0.16/test/test_core.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-06 13:41:28.600718 wgd-2.0.16/wgd/
--rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.16/wgd/__init__.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.16/wgd/beast.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.16/wgd/cluster.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     8819 2022-12-04 21:40:23.000000 wgd-2.0.16/wgd/codeml.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   134238 2023-05-19 10:45:47.000000 wgd-2.0.16/wgd/core.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    17148 2023-03-17 14:15:45.000000 wgd-2.0.16/wgd/mcmctree.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.16/wgd/mix.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   103616 2023-06-05 09:26:29.000000 wgd-2.0.16/wgd/peak.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     8792 2023-06-03 13:38:23.000000 wgd-2.0.16/wgd/syn.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    28648 2022-09-30 07:30:21.000000 wgd-2.0.16/wgd/utils.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   113240 2023-05-28 17:34:16.000000 wgd-2.0.16/wgd/viz.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-06 13:41:28.602237 wgd-2.0.16/wgd.egg-info/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    44508 2023-06-06 13:41:28.000000 wgd-2.0.16/wgd.egg-info/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)      369 2023-06-06 13:41:28.000000 wgd-2.0.16/wgd.egg-info/SOURCES.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-06-06 13:41:28.000000 wgd-2.0.16/wgd.egg-info/dependency_links.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       51 2023-06-06 13:41:28.000000 wgd-2.0.16/wgd.egg-info/entry_points.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)      749 2023-06-06 13:41:28.000000 wgd-2.0.16/wgd.egg-info/requires.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2023-06-06 13:41:28.000000 wgd-2.0.16/wgd.egg-info/top_level.txt
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-17 12:42:31.427053 wgd-2.0.17/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.17/LICENSE
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    47387 2023-06-17 12:42:31.427053 wgd-2.0.17/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    47149 2023-06-17 12:28:46.000000 wgd-2.0.17/README.md
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    52222 2023-06-17 12:17:36.000000 wgd-2.0.17/cli.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-06-17 12:42:31.428059 wgd-2.0.17/setup.cfg
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1904 2023-06-10 17:45:36.000000 wgd-2.0.17/setup.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-17 12:42:31.406718 wgd-2.0.17/test/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-06-06 22:05:06.000000 wgd-2.0.17/test/test_core.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-17 12:42:31.419542 wgd-2.0.17/wgd/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.17/wgd/__init__.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.17/wgd/beast.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.17/wgd/cluster.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     8819 2022-12-04 21:40:23.000000 wgd-2.0.17/wgd/codeml.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   135263 2023-06-15 13:48:21.000000 wgd-2.0.17/wgd/core.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    17148 2023-03-17 14:15:45.000000 wgd-2.0.17/wgd/mcmctree.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.17/wgd/mix.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   103616 2023-06-06 22:05:06.000000 wgd-2.0.17/wgd/peak.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     4722 2023-06-06 22:05:06.000000 wgd-2.0.17/wgd/postplot.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    17378 2023-06-15 09:47:26.000000 wgd-2.0.17/wgd/syn.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    28647 2023-06-06 22:05:06.000000 wgd-2.0.17/wgd/utils.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   144926 2023-06-17 12:20:32.000000 wgd-2.0.17/wgd/viz.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-17 12:42:31.425546 wgd-2.0.17/wgd.egg-info/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    47387 2023-06-17 12:42:31.000000 wgd-2.0.17/wgd.egg-info/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      385 2023-06-17 12:42:31.000000 wgd-2.0.17/wgd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-06-17 12:42:31.000000 wgd-2.0.17/wgd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       32 2023-06-17 12:42:31.000000 wgd-2.0.17/wgd.egg-info/entry_points.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      749 2023-06-17 12:42:31.000000 wgd-2.0.17/wgd.egg-info/requires.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2023-06-17 12:42:31.000000 wgd-2.0.17/wgd.egg-info/top_level.txt
```

### Comparing `wgd-2.0.16/LICENSE` & `wgd-2.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `wgd-2.0.16/PKG-INFO` & `wgd-2.0.17/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,556 +1,625 @@
-Metadata-Version: 2.1
-Name: wgd
-Version: 2.0.16
-Summary: wgd
-Home-page: http://github.com/heche-psb/wgd
-Author: Hengchi Chen
-Author-email: heche@psb.vib-ugent.be
-License: GPL
-Description: <div align="center">
-        
-        # `wgd v2` : a suite tool of WGD inference and timing
-        
-        **Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
-        
-        [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
-        
-        [**Introduction**](#Introduction) | 
-        [**Installation**](#Installation) | 
-        [**Parameters**](#Parameters) | 
-        [**Usage**](#Usage) | 
-        [**Illustration**](#Illustration) |
-        [**Citation**](#Citation)
-        
-        </div>
-        
-        `wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
-        
-        ## Introduction
-        
-        Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
-        
-        The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
-        
-        ## Installation
-        
-        The easiest way to install `wgd v2` is using PYPI
-        
-        ```
-        pip install wgd
-        ```
-        
-        To install `wgd v2` in a virtual environment, the following command lines could be used.
-        
-        ```
-        git clone <wgd repo>
-        cd wgd
-        virtualenv -p=python3 ENV (or python3 -m venv ENV)
-        source ENV/bin/activate
-        pip install -r requirements.txt
-        pip install .
-        ```
-        
-        When met with permission problem in installation, please try the following command line.
-        
-        ```
-        pip install -e .
-        ```
-        
-        If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
-        
-        ```
-        export PATH="$PATH:~/.local/bin/wgd"
-        ```
-        
-        Note that the version of `numpy` is important (for many other packages are the same of course), especially for `fastcluster` package. In our test, the `numpy` 1.19.0 works fine on `python3.6/8`. If you met some errors or warnings about numpy, maybe considering pre-install `numpy` as 1.19.0 or other close-by versions before you install `wgd`.
-        
-        ## Parameters
-        
-        There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
-        
-        The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
-        ```
-        wgd dmd sequences (option)
-        --------------------------------------------------------------------------------
-        -o, --outdir, the output directory, default wgd_dmd
-        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
-        -c, --cscore, the c-score to restrict the homologs of MRBHs, default None, if None was given, the c-score funcion won't be activated
-        -I, --inflation, the inflation factor for MCL program, default 2.0
-        -e, --eval, the e-value cut-off for similarity in diamond and/or hmmer, default 1e-10
-        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
-        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
-        -f, --focus, the species to be merged on local MRBHs, default None, if None was given, the local MRBHs won't be inferred
-        -ap, --anchorpoints, the anchor points data file, default None
-        -coc, --collinearcoalescence, flag option, whether to initiate the collinear coalescence analysis, if the flag was set, the analysis will be initiated
-        -sm, --segments, the segments data file used in collinear coalescence analysis if initiated, default None
-        -le, --listelements, the listsegments data file used in collinear coalescence analysis if initiated, default None
-        -gt, --genetable, the gene table datafile used in collinear coalescence analysis if initiated, default None
-        -kf, --keepfasta, flag option, whether to output the sequence information of MRBHs, if the flag was set, the sequences of MRBHs will be in output
-        -kd, --keepduplicates, flag option, whether to allow the same gene to occur in different MRBHs, if the flag was set, the same gene can be assigned to different MRBHs
-        -gm, --globalmrbh, flag option, whether to initiate global MRBHs construction, if the flag was set, the --focus option will be ignored and only global MRBHs will be built
-        -n, --nthreads, the number of threads to use, default 4
-        -oi, --orthoinfer, flag option, whether to initiate orthogroup infernece, if the flag was set, the orthogroup infernece program will be initiated
-        -oo, --onlyortho, flag option, whether to only conduct orthogroup infernece, if the flag was set, only the orthogroup infernece program will be conducted while the other analysis won't be initiated
-        -gn, --getnsog, flag option, whether to initiate the searching for nested single-copy gene families (NSOGs), if the flag was set, additional NSOGs analysis will be performed besides the basic orthogroup infernece
-        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
-        -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
-        -mc, --msogcut, the ratio cutoff for mostly single-copy family and species representation in collinear coalescence inference, default 0.8.
-        -ga, --geneassign, flag option, whether to initiate the gene-to-family assignment analysis, if the flag was set, the analysis will be initiated
-        -am, --assign_method, which method to conduct the gene-to-family assignment analysis, default hmmer
-        -sa, --seq2assign, the queried sequences data file in gene-to-family assignment analysis, default None, this option can be provided multiple times
-        -fa, --fam2assign, the queried familiy data file in gene-to-family assignment analysis, default None
-        -cc, --concat, flag option, whether to initiate the concatenation pipeline for orthogroup infernece, if the flag was set, the analysis will be initiated
-        -te, --testsog, flag option, whether to initiate the unbiased test of single-copy gene families, if the flag was set, the analysis will be initiated
-        -bs, --bins, the number of bins divided in gene length normalization, default 100
-        -np, --normalizedpercent, the percentage of upper hits used for gene length normalization, default 5
-        -nn, --nonormalization, flag option, whether to call off the normalization, if the flag was set, no normalization will be conducted
-        -bsog, --buscosog, flag option, whether to initiate the busco-guided single-copy gene family analysis, if the flag was set, the analysis will be initiated
-        -bhmm, --buscohmm, the HMM profile datafile in the busco-guided single-copy gene family analysis, default None
-        -bctf, --buscocutoff, the HMM score cutoff datafile in the busco-guided single-copy gene family analysis, default None
-        ```
-        
-        The program `wgd focus` can realize the concatenation-based and coalescence-based phylogenetic inference, functional annotation of gene families and phylogenetic dating of WGDs.
-        ```
-        wgd focus families sequences (option)
-        --------------------------------------------------------------------------------
-        -o, --outdir, the output directory, default wgd_focus
-        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
-        -n, --nthreads, the number of threads to use, default 4
-        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
-        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
-        --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
-        -a, --aligner, which alignment program to use, default mafft
-        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
-        -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
-        --concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
-        --coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
-        -sp, --speciestree, species tree darafile for dating, default None
-        -d, --dating, which molecular dating program to use, default none
-        -ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
-        -ns, --nsites, the nsites information for r8s dating, default None
-        -ot, --outgroup, the outgroup information for r8s dating, default None
-        -pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
-        -am, --aamodel, which protein model to be used in mcmctree, default poisson
-        -ks, flag option, whether to initiate Ks analysis
-        --annotation, which annotation program to use, default none
-        --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
-        -ed, --eggnogdata, the eggnog annotation datafile, default None
-        --pfam, which option to use for pfam annotation, default none
-        --dmnb, the diamond database for annotation, default None
-        --hmm, the HMM profile for annotation, default None
-        --evalue, the e-value cut-off for annotation, default 1e-10
-        --exepath, the path to the interproscan executable, default None
-        -f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
-         -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
-        -cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
-        --beastlgjar, the path to beastLG.jar, default None
-        --beagle, flag option, whether to use beagle in Beast, if the flag was set, beagle will be used
-        --protdating, flag option, whether to only initiate the protein-concatenation based dating analysis, if the flag was set, the analysis will be initiated
-        ```
-        
-        The program `wgd ksd` can realize the construction of *K*<sub>S</sub> age distribution and rate correction.
-        ```
-        wgd ksd families sequences (option)
-        --------------------------------------------------------------------------------
-        -o, --outdir, the output directory, default wgd_ksd
-        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
-        -n, --nthreads, the number of threads to use, default 4
-        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
-        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
-        --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
-        --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
-        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
-        -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
-        -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
-        -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
-        -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
-        ```
-        
-        The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
-        ```
-        wgd mix ks_datafile (option)
-        --------------------------------------------------------------------------------
-        -f, --filters, the cutoff alignment length, default 300
-        -r, --ks_range, the Ks range to be considered, default (0.005, 3)
-        -b, --bins, the number of bins in Ks distribution, default 50
-        -o, --outdir, the output directory, default wgd_mix
-        --method, which mixture model to use, default gmm
-        -n, --components, the range of the number of components to fit, default (1, 4)
-        -g, --gamma, the gamma parameter for bgmm models, default 0.001
-        -ni, --n_init, the number of k-means initializations, default 200
-        -mi, --max_iter, the maximum number of iterations, default 1000
-        ```
-        
-        The program `wgd peak` can realize the search of crediable *K*<sub>S</sub> range used in WGD dating.
-        ```
-        wgd peak ks_datafile (option)
-        --------------------------------------------------------------------------------
-        -ap, --anchorpoints, the anchor points datafile, default None
-        -sm, --segments, the segments datafile, default None
-        -le, --listelements, the listsegments datafile, default None 
-        -mp, --multipliconpairs, the multipliconpairs datafile, default None
-        -o, --outdir, the output directory, default wgd_peak
-        -af, --alignfilter, cutoff for alignment identity, length and coverage, default 0.0, 0, 0.0
-        -r, --ksrange, range of Ks to be analyzed, default (0, 5)
-        -bw, --bin_width, bandwidth of Ks distribution, default 0.1
-        -ic, --weights_outliers_included, flag option, whether to include Ks outliers, if the flag was set, Ks outliers will be included in the analysis
-        -m, --method, which mixture model to use, default gmm
-        --seed, random seed given to initialization, default 2352890
-        -ei, --em_iter, the number of EM iterations to perform, default 200
-        -ni, --n_init, the number of k-means initializations, default 200
-        -n, --components, the range of the number of components to fit, default (1, 4)
-        --boots, the number of bootstrap replicates of kde, default 200
-        --weighted, flag option, whether to use node-weighted method of de-redundancy, if the flag was set, the node-weighted method will be used
-        -p, --plot, the plotting method to be used, default identical
-        -bm, --bw_method, the bandwidth method to be used, default silverman
-        --n_medoids, the number of medoids to fit, default 2
-        -km, --kdemethod, the kde method to be used, default scipy
-        --n_clusters, the number of clusters to plot Elbow loss function, default 5
-        --kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
-        -gd, --guide, the regime residing anchors, default: segment
-        -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
-        -kd, --kstodate, the range of Ks to be dated, default (0.5, 1.5)
-        -f, --family, the family to filter Ks upon, default None
-        --manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
-        -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
-        --ci, the confidence level of log-normal distribution to date, default 95
-        --hdr, the highest densidy region (HDR) in a given distribution to date, default 95
-        --heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
-        -kc, --kscutoff, the Ks saturation cutoff in dating, default 5
-        ```
-        
-        The program `wgd syn` can realize the intra- and inter-specific synteny inference.
-        ```
-        wgd syn families gffs (option)
-        --------------------------------------------------------------------------------
-        -ks, --ks_distribution, ks distribution datafile, default None
-        -o, --outdir, the output directory, default wgd_syn
-        -f, --feature, the feature for parsing gene IDs from GFF files, default gene
-        -a, --attribute, the attribute for parsing the gene IDs from the GFF files, default ID
-        -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
-        -ms, --maxsize, the maximum family size to include, default 200
-        -r, --ks_range, the Ks range in colored dotplot, default (0, 5)
-        --iadhore_options, the parameter setting in iadhore, default 
-        -ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
-        -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
-        -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
-        ```
-        
-        The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
-        ```
-        wgd viz (option)
-        --------------------------------------------------------------------------------
-        -d, --datafile, the Ks datafile, default None
-        -o, --outdir, the output directory, default wgd_viz
-        -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
-        -gs, --gsmap, the gene name-species name map, default None
-        -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
-        -pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
-        -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
-        -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
-        -iter, --em_iterations, the maximum EM iterations, default 200
-        -init, --em_initializations, the maximum EM initializations, default 200
-        -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
-        -sm, --segments, the segments data file, default None
-        -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
-        -ms, --maxsize, the maximum family size to include, default 200
-        -ap, --anchorpoints, the anchor points datafile, default None
-        -mt, --multiplicon, the multiplicons datafile, default None
-        -gt, --genetable, the gene table datafile, default None
-        -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
-        -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
-        -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
-        ```
-        
-        ## Usage
-        
-        Here we provided the basic usage for each program.
-        
-        ### wgd dmd
-        
-        **The delineation of whole paranome**
-        ```
-        wgd dmd sequence
-        ``` 
-        
-        **The delineation of RBHs**
-        ```
-        wgd dmd sequence1 sequence2
-        ```
-        
-        **The delineation of local MRBHs**
-        ```
-        wgd dmd sequence1 sequence2 sequence3 -f sequence1
-        ```
-        
-        **The delineation of global MRBHs**
-        ```
-        wgd dmd sequence1 sequence2 sequence3 -gm
-        ```
-        
-        **The delineation of orthogroups**
-        ```
-        wgd dmd sequence1 sequence2 sequence3 -oi (option)
-        ```
-        Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
-        
-        **The collinear coalescence inference of phylogeny**
-        ```
-        wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
-        ```
-        
-        Note that there should be no duplicated gene IDs in the sequence file.
-        
-        ### wgd focus
-        
-        **The concatenation-based/coalescence-based phylogenetic inference**
-        ```
-        wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
-        ```
-        
-        **The functional annotation of gene families**
-        ```
-        wgd focus families sequence1 sequence2 sequence3 --annotation eggnog -ed eddata --dmnb dbdata
-        ```
-        
-        **The phylogenetic dating of WGDs**
-        ```
-        wgd focus families sequence1 sequence2 sequence3 -d mcmctree -sp spdata
-        ```
-        
-        ### wgd ksd
-        
-        **The construction of whole paranome *K*<sub>S</sub> age distribution**
-        ```
-        wgd ksd families sequence
-        ```
-        
-        **The construction of orthologous *K*<sub>S</sub> age distribution**
-        ```
-        wgd ksd families sequence1 sequence2
-        ```
-        
-        **The construction of *K*<sub>S</sub> age distribution with rate correction**
-        ```
-        wgd ksd families sequence1 sequence2 sequence3 -sr srdata -sp spdata
-        ```
-        
-        ### wgd mix
-        
-        **The mixture model clustering analysis of *K*<sub>S</sub> age distribution**
-        ```
-        wgd mix ksdata
-        ```
-        
-        ### wgd peak
-        
-        **The search of crediable *K*<sub>S</sub> range used in WGD dating**
-        ```
-        wgd peak ksdata -ap apdata -sm smdata -le ledata -mp mpdata
-        ```
-        Note that users can add the flag --heuristic to implement the heuristic search analysis
-        
-        ### wgd syn
-        
-        **The intra-specific synteny inference**
-        ```
-        wgd syn families gff
-        ```
-        
-        **The inter-specific synteny inference**
-        ```
-        wgd syn families gff1 gff2
-        ```
-        
-        ### wgd viz
-        
-        **The visualization of *K*<sub>S</sub> age distribution**
-        ```
-        wgd viz -d ksdata
-        ```
-        
-        **The visualization of *K*<sub>S</sub> age distribution with rate correction**
-        ```
-        wgd viz -d ksdata -sr srdata -sp spdata -gs gsdata
-        ```
-        
-        **The visualization of synteny**
-        ```
-        wgd viz -ap apdata -sm smdata -mt mtdata -gt gtdata
-        ```
-        
-        ## Illustration
-        
-        We illustrate our program on an exemplary WGD inference and dating upon species *Aquilegia coerulea*.
-        
-        The *Aquilegia coerulea* was reported to experience an paleo-polyploidization event after the divergence of core eudicots, which is likely shared by all Ranunculales.
-        
-        First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
-        
-        ```
-        wgd dmd Aquilegia_coerulea
-        wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
-        ```
-        
-        The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1 but not clear.
-        
-        ![](data/Aquilegia_coerulea.tsv.ksd_wp.svg)
-        
-        We then construct the anchor *K*<sub>S</sub> age distribution using the command line below.
-        
-        ```
-        wgd syn -f mRNA -a Name wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea.gff3 -ks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
-        ```
-        
-        As shown below, there are some retained anchor pairs with *K*<sub>S</sub> between 1 and 2, which seems to suggest a WGD event.
-        
-        ![](data/Aquilegia_coerulea.tsv.ksd_wp_ap.svg)
-        
-        The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes, except for the chr_07, which seems to experience more severe fragmentization than the other chromosomes.
-        
-        ![](data/Aquilegia_coerulea_Aquilegia_coerulea_multiplicons_level.svg)
-        
-        The associated dotplot in oxford grid also presents numerous densely aggregated anchor points throughout most of the chromosomes.
-        
-        ![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
-        
-        A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
-        
-        ![](data/Syndepth.svg)
-        
-        We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
-        
-        ```
-        wgd viz -d wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
-        ```
-        
-        The result of ELMM mixture model clustering shows that there is a likely WGD component at *K*<sub>S</sub> 1.19.
-        
-        ![](data/elmm_Aquilegia_coerulea.tsv.ks.tsv_best_models_weighted.svg)
-        
-        Let's do a mixture model clustering for anchor *K*<sub>S</sub> too, using the command line below.
-        
-        ```
-        wgd peak wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv --anchorpoints wgd_syn/iadhore-out/anchorpoints.txt --segments wgd_syn/iadhore-out/segments.txt --listelements wgd_syn/iadhore-out/list_elements.txt --multipliconpairs wgd_syn/iadhore-out/multiplicon_pairs.txt --weighted
-        ```
-        
-        The anchor *K*<sub>S</sub> age distribution also has a likely WGD component with mode 1.28.
-        
-        ![](data/Original_AnchorKs_GMM_Component3_node_weighted_Lognormal.svg)
-        
-        Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis. First, we built a global MRBH family using the command below.
-        
-        ```
-        wgd dmd --globalmrbh Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera -o wgd_globalmrbh
-        ```
-        
-        In the global MRBH family, every pair of orthologous genes is the reciprocal best hit, suggesting true orthologous relationships. We would use the *K*<sub>S</sub> values associated with these orthologous pairs to delimit the divergence *K*<sub>S</sub> peak. Together with the whole paranome *K*<sub>S</sub> distribution, we conduct the rate correction using the command below.
-        
-        ```
-        wgd ksd wgd_globalmrbh/global_MRBH.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
-        ```
-        
-        The file `speciestree.nw` is the text file of species tree in newick that rate correction would be conducted on. Its content is as below. Users need to provide the species pairs to be plotted. We suggest adding the option `--reweight` to recalculate the weight per species pair such that the weight of orthologous gene pairs will become 1 as the paralogous gene pairs. The flag `--plotkde` can be added when the kde curve of orthologous *K*<sub>S</sub> is desired. Extra collinear data can be added by the option `-ap`.
-        
-        ```
-        (((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
-        ```
-        
-        ![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
-        
-        As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
-        
-        If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
-        
-        ```
-        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
-        ```
-        
-        Note that we can easily show that *Aquilegia coerulea* has higher substitution rate than *Protea cynaroides* and *Vitis vinifera* by comparing their substitution distance in regard to the same divergence event with outgroup species *Acorus_americanus*, using command below.
-        
-        ```
-        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_viz_Compare_rate --spair "Acorus_americanus;Protea_cynaroides" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Vitis_vinifera;Acorus_americanus" --gsmap gene_species.map --plotkde
-        ```
-        
-        ![](data/Raw_Orthologues_Compare_rate.ksd.svg)
-        
-        As displayed above, the orthologous *K*<sub>S</sub> values bewteen *Aquilegia coerulea* and *Acorus americanus* has the highest mode, indicatingthe faster substitution rate of *Aquilegia coerulea* compared to *Protea cynaroides* and *Vitis vinifera*.
-        
-        Note that a necessary gene-species map file is needed for its implementation in `wgd viz`, which should be automately produced by the last `wgd ksd` step. The `gene_species.map` has contents as below in which each line is the joined string of gene name and species name by space.
-        
-        ```
-        Aqcoe6G057800.1 Aquilegia_coerulea
-        Vvi_VIT_201s0011g01530.1 Vitis_vinifera
-        Pcy_Procy01g08510 Protea_cynaroides
-        Aam_Acora.04G142900.1 Acorus_americanus
-        ```
-        
-        A more complex plot can be made by add the flag `--plotelmm` such that the ELMM mixture modeling of provided paranome *K*<sub>S</sub> can be superimposed, using the command below.
-        
-        ```
-        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm
-        ```
-        
-        ![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Corrected.ksd.svg)
-        
-        From the mixed *K*<sub>S</sub> plot above, we can see that the optimized lognormal component b with mode 1.2 is younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera* (1.39 and 1.47, respectively).
-        
-        Besides, we can also add the GMM mixture modeling of anchor *K*<sub>S</sub> values with the flag `--plotapgmm`, using the command below.
-        
-        ```
-        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotapgmmm
-        ```
-        
-        ![](data/Aquilegia_coerulea_GlobalmrbhKs_Apgmm_Corrected.ksd.svg)
-        
-        As manifested above, the anchor *K*<sub>S</sub> component 2 with mode 1.28 is also younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera*. But we need to be of course cautious that such distinction comes with the uncertainties introduced from the applied mixture modeling methodology in terms of for instance different initialization points and the issue of overfitting and the sister speciess adopted in that there might be species with more disparate substitution rates than the one we chose.
-        
-        Adding both ELMM result for paranome and GMM result for anchor *K*<sub>S</sub> can be achieved just by add the two flags mentioned above, using the command below.
-        
-        ```
-        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm --plotapgmmm
-        ```
-        
-        ![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Apgmm_Corrected.ksd.svg)
-        
-        An alternative way to calculate the orthologous *K*<sub>S</sub> is to directly use the orthogroups instead of global MRBH family. That way we don't use the pre-inferred paranome *K*<sub>S</sub> but the paralogous gene pairs inside each orthogroup instead. To achieve that, we first need to infer orthogroups using the command below.
-        
-        ```
-        wgd dmd Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera --orthoinfer -o wgd_ortho (--onlyortho) 
-        ```
-        
-        Users can decide to only conduct the orthogroup analysis while skipping other analysis by adding the flag `--onlyortho`. Next step is the same with global MRBH family except that we don't use the extra pre-inferred paranome *K*<sub>S</sub> anymore. We infer the *K*<sub>S</sub> using the command below. Note that the program `wgd viz` can plot the same just as shown above.
-        
-        ```
-        wgd ksd wgd_ortho/Orthogroups.sp.tsv -sp speciestree.nw --reweight -o wgd_ortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
-        ```
-        
-        ![](data/Aquilegia_coerulea_OrthoKs_Corrected.ksd.svg)
-        
-        As shown above, the number of both paralogous gene pairs and orthologous gene pairs is different than the one from global MRBH family in that here we plotted all orthologous gene pairs instead of only global MRBH and potentially new paralogous gene pairs might be produced in the orthogroup inference step, together with different recalculated weights.
-        
-        If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, as we have already shown above, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
-        
-        ```
-        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --gsmap gene_species.map
-        ```
-        
-        We can clearly see that *Vitis vinifera* has higher substitution rate than *Protea cynaroides* in that their orthologous *K*<sub>S</sub> peaks with *Aquilegia coerulea*, although representing the same divergence event, differed in substitution distance.
-        ![](data/Raw_Orthologues.ksd.svg)
-        
-        ## Citation
-         
-        Please cite us at https://doi.org/10.1093/bioinformatics/bty915
-        
-        ```
-        Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
-        
-        Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
-        ```
-        
-        For citation of the tools used in wgd, please consult the documentation at
-        https://wgd.readthedocs.io/en/latest/index.html#citation.
-        
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+<div align="center">
+
+# `wgd v2` : a suite tool of WGD inference and timing
+
+[![Build Status](https://app.travis-ci.com/heche-psb/wgd.svg?branch=phylodating)](https://app.travis-ci.com/heche-psb/wgd)
+[![Documentation Status](https://readthedocs.org/projects/wgdv2/badge/?version=latest)](https://wgdv2.readthedocs.io/en/latest/?badge=latest)
+[![license](https://img.shields.io/pypi/l/wgd.svg)](https://pypi.python.org/pypi/wgd)
+[![Latest PyPI version](https://img.shields.io/pypi/v/wgd.svg)](https://pypi.python.org/pypi/wgd)
+[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/wgd/README.html)
+[![Downloads](https://pepy.tech/badge/wgd)](https://pepy.tech/project/wgd)
+
+**Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
+
+[**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
+
+[**Introduction**](#Introduction) | 
+[**Installation**](#Installation) | 
+[**Parameters**](#Parameters) | 
+[**Usage**](#Usage) | 
+[**Illustration**](#Illustration) |
+[**Documentation**](https://wgdv2.readthedocs.io/en/latest/?badge=latest) |
+[**Citation**](#Citation)
+
+
+</div>
+
+`wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
+
+## Introduction
+
+Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
+
+The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
+
+## Installation
+
+The easiest way to install `wgd v2` is using PYPI
+
+```
+pip install wgd
+```
+
+To install `wgd v2` in a virtual environment, the following command lines could be used.
+
+```
+git clone <wgd repo>
+cd wgd
+virtualenv -p=python3 ENV (or python3 -m venv ENV)
+source ENV/bin/activate
+pip install -r requirements.txt
+pip install .
+```
+
+When met with permission problem in installation, please try the following command line.
+
+```
+pip install -e .
+```
+
+If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
+
+```
+export PATH="$PATH:~/.local/bin/wgd"
+```
+
+Note that the version of `numpy` is important (for many other packages are the same of course), especially for `fastcluster` package. In our test, the `numpy` 1.19.0 works fine on `python3.6/8`. If you met some errors or warnings about numpy, maybe considering pre-install `numpy` as 1.19.0 or other close-by versions before you install `wgd`.
+
+## Parameters
+
+There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
+
+The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
+```
+wgd dmd sequences (option)
+--------------------------------------------------------------------------------
+-o, --outdir, the output directory, default wgd_dmd
+-t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+-c, --cscore, the c-score to restrict the homologs of MRBHs, default None, if None was given, the c-score funcion won't be activated
+-I, --inflation, the inflation factor for MCL program, default 2.0
+-e, --eval, the e-value cut-off for similarity in diamond and/or hmmer, default 1e-10
+--to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+--cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+-f, --focus, the species to be merged on local MRBHs, default None, if None was given, the local MRBHs won't be inferred
+-ap, --anchorpoints, the anchor points data file, default None
+-coc, --collinearcoalescence, flag option, whether to initiate the collinear coalescence analysis, if the flag was set, the analysis will be initiated
+-sm, --segments, the segments data file used in collinear coalescence analysis if initiated, default None
+-le, --listelements, the listsegments data file used in collinear coalescence analysis if initiated, default None
+-gt, --genetable, the gene table datafile used in collinear coalescence analysis if initiated, default None
+-kf, --keepfasta, flag option, whether to output the sequence information of MRBHs, if the flag was set, the sequences of MRBHs will be in output
+-kd, --keepduplicates, flag option, whether to allow the same gene to occur in different MRBHs, if the flag was set, the same gene can be assigned to different MRBHs
+-gm, --globalmrbh, flag option, whether to initiate global MRBHs construction, if the flag was set, the --focus option will be ignored and only global MRBHs will be built
+-n, --nthreads, the number of threads to use, default 4
+-oi, --orthoinfer, flag option, whether to initiate orthogroup infernece, if the flag was set, the orthogroup infernece program will be initiated
+-oo, --onlyortho, flag option, whether to only conduct orthogroup infernece, if the flag was set, only the orthogroup infernece program will be conducted while the other analysis won't be initiated
+-gn, --getnsog, flag option, whether to initiate the searching for nested single-copy gene families (NSOGs), if the flag was set, additional NSOGs analysis will be performed besides the basic orthogroup infernece
+-tree, --tree_method, which gene tree inference program to invoke, default fasttree
+-ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
+-mc, --msogcut, the ratio cutoff for mostly single-copy family and species representation in collinear coalescence inference, default 0.8.
+-ga, --geneassign, flag option, whether to initiate the gene-to-family assignment analysis, if the flag was set, the analysis will be initiated
+-am, --assign_method, which method to conduct the gene-to-family assignment analysis, default hmmer
+-sa, --seq2assign, the queried sequences data file in gene-to-family assignment analysis, default None, this option can be provided multiple times
+-fa, --fam2assign, the queried familiy data file in gene-to-family assignment analysis, default None
+-cc, --concat, flag option, whether to initiate the concatenation pipeline for orthogroup infernece, if the flag was set, the analysis will be initiated
+-te, --testsog, flag option, whether to initiate the unbiased test of single-copy gene families, if the flag was set, the analysis will be initiated
+-bs, --bins, the number of bins divided in gene length normalization, default 100
+-np, --normalizedpercent, the percentage of upper hits used for gene length normalization, default 5
+-nn, --nonormalization, flag option, whether to call off the normalization, if the flag was set, no normalization will be conducted
+-bsog, --buscosog, flag option, whether to initiate the busco-guided single-copy gene family analysis, if the flag was set, the analysis will be initiated
+-bhmm, --buscohmm, the HMM profile datafile in the busco-guided single-copy gene family analysis, default None
+-bctf, --buscocutoff, the HMM score cutoff datafile in the busco-guided single-copy gene family analysis, default None
+```
+
+The program `wgd focus` can realize the concatenation-based and coalescence-based phylogenetic inference, functional annotation of gene families and phylogenetic dating of WGDs.
+```
+wgd focus families sequences (option)
+--------------------------------------------------------------------------------
+-o, --outdir, the output directory, default wgd_focus
+-t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+-n, --nthreads, the number of threads to use, default 4
+--to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+--cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+--strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
+-a, --aligner, which alignment program to use, default mafft
+-tree, --tree_method, which gene tree inference program to invoke, default fasttree
+-ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
+--concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
+--coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
+-sp, --speciestree, species tree datafile for dating, default None
+-d, --dating, which molecular dating program to use, default none
+-ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
+-ns, --nsites, the nsites information for r8s dating, default None
+-ot, --outgroup, the outgroup information for r8s dating, default None
+-pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
+-am, --aamodel, which protein model to be used in mcmctree, default poisson
+-ks, flag option, whether to initiate Ks calculation
+--annotation, which annotation program to use, default None
+--pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
+-ed, --eggnogdata, the eggnog annotation datafile, default None
+--pfam, which option to use for pfam annotation, default None
+--dmnb, the diamond database for annotation, default None
+--hmm, the HMM profile for annotation, default None
+--evalue, the e-value cut-off for annotation, default 1e-10
+--exepath, the path to the interproscan executable, default None
+-f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
+ -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
+-cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
+--beastlgjar, the path to beastLG.jar, default None
+--beagle, flag option, whether to use beagle in Beast, if the flag was set, beagle will be used
+--protdating, flag option, whether to only initiate the protein-concatenation based dating analysis, if the flag was set, the analysis will be initiated
+```
+
+The program `wgd ksd` can realize the construction of *K*<sub>S</sub> age distribution and rate correction.
+```
+wgd ksd families sequences (option)
+--------------------------------------------------------------------------------
+-o, --outdir, the output directory, default wgd_ksd
+-t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+-n, --nthreads, the number of threads to use, default 4
+--to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+--cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+--pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
+--strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
+-tree, --tree_method, which gene tree inference program to invoke, default fasttree
+-sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
+-sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
+-rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
+-or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+-epk, --extraparanomeks, extra paranome Ks data to plot in the mixed Ks distribution, default None
+-ap, --anchorpoints, anchorpoints.txt file to plot anchor Ks in the mixed Ks distribution, default None
+-pk, --plotkde, flag option, whether to plot kde curve of orthologous Ks distribution over histogram in the mixed Ks distribution, if the flag was set, the kde curve will be plotted
+-pag, --plotapgmm, flag option, whether to plot mixture modeling of anchor Ks in the mixed Ks distribution, if the flag was set, the mixture modeling of anchor Ks will be plotted
+-pem, --plotelmm, flag option, whether to plot elmm mixture modeling of paranome Ks in the mixed Ks distribution, if the flag was set, the elmm mixture modeling of paranome Ks will be plotted
+-c, --components, the range of the number of components to fit in anchor Ks mixture modeling, default (1,4)
+```
+
+The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
+```
+wgd mix ks_datafile (option)
+--------------------------------------------------------------------------------
+-f, --filters, the cutoff alignment length, default 300
+-r, --ks_range, the Ks range to be considered, default (0, 5)
+-b, --bins, the number of bins in Ks distribution, default 50
+-o, --outdir, the output directory, default wgd_mix
+--method, which mixture model to use, default gmm
+-n, --components, the range of the number of components to fit, default (1, 4)
+-g, --gamma, the gamma parameter for bgmm models, default 0.001
+-ni, --n_init, the number of k-means initializations, default 200
+-mi, --max_iter, the maximum number of iterations, default 1000
+```
+
+The program `wgd peak` can realize the search of crediable *K*<sub>S</sub> range used in WGD dating.
+```
+wgd peak ks_datafile (option)
+--------------------------------------------------------------------------------
+-ap, --anchorpoints, the anchor points datafile, default None
+-sm, --segments, the segments datafile, default None
+-le, --listelements, the listsegments datafile, default None 
+-mp, --multipliconpairs, the multipliconpairs datafile, default None
+-o, --outdir, the output directory, default wgd_peak
+-af, --alignfilter, cutoff for alignment identity, length and coverage, default 0.0, 0, 0.0
+-r, --ksrange, range of Ks to be analyzed, default (0, 5)
+-bw, --bin_width, bandwidth of Ks distribution, default 0.1
+-ic, --weights_outliers_included, flag option, whether to include Ks outliers, if the flag was set, Ks outliers will be included in the analysis
+-m, --method, which mixture model to use, default gmm
+--seed, random seed given to initialization, default 2352890
+-ei, --em_iter, the number of EM iterations to perform, default 200
+-ni, --n_init, the number of k-means initializations, default 200
+-n, --components, the range of the number of components to fit, default (1, 4)
+--boots, the number of bootstrap replicates of kde, default 200
+--weighted, flag option, whether to use node-weighted method of de-redundancy, if the flag was set, the node-weighted method will be used
+-p, --plot, the plotting method to be used, default identical
+-bm, --bw_method, the bandwidth method to be used, default silverman
+--n_medoids, the number of medoids to fit, default 2
+-km, --kdemethod, the kde method to be used, default scipy
+--n_clusters, the number of clusters to plot Elbow loss function, default 5
+--kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
+-gd, --guide, the regime residing anchors, default: segment
+-prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
+-kd, --kstodate, the range of Ks to be dated in heuristic search, default (0.5, 1.5)
+-f, --family, the family to filter Ks upon, default None
+--manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
+-rh, --rel_height, the relative height at which the peak width is measured, default 0.4
+--ci, the confidence level of log-normal distribution to date, default 95
+--hdr, the highest density region (HDR) in a given distribution to date, default 95
+--heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
+-kc, --kscutoff, the Ks saturation cutoff in dating, default 5
+-g, --gamma, the gamma parameter for bgmm models, default 1e-3
+```
+
+The program `wgd syn` can realize the intra- and inter-specific synteny inference.
+```
+wgd syn families gffs (option)
+--------------------------------------------------------------------------------
+-ks, --ks_distribution, ks distribution datafile, default None
+-o, --outdir, the output directory, default wgd_syn
+-f, --feature, the feature for parsing gene IDs from GFF files, default gene
+-a, --attribute, the attribute for parsing the gene IDs from the GFF files, default ID
+-ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
+-ms, --maxsize, the maximum family size to include, default 200
+-r, --ks_range, the Ks range in colored dotplot, default (0, 5)
+--iadhore_options, the parameter setting in iadhore, default 
+-ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
+-mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
+-kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+```
+
+The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
+```
+wgd viz (option)
+--------------------------------------------------------------------------------
+-d, --datafile, the Ks datafile, default None
+-o, --outdir, the output directory, default wgd_viz
+-sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
+-gs, --gsmap, the gene name-species name map, default None
+-sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
+-pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
+-rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
+-or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+-iter, --em_iterations, the maximum EM iterations, default 200
+-init, --em_initializations, the maximum EM initializations, default 200
+-prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
+-sm, --segments, the segments data file, default None
+-ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffolds will be set
+-ms, --maxsize, the maximum family size to include, default 200
+-ap, --anchorpoints, the anchor points datafile, default None
+-mt, --multiplicon, the multiplicons datafile, default None
+-gt, --genetable, the gene table datafile, default None
+-rh, --rel_height, the relative height at which the peak width is measured, default 0.4
+-mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
+-kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+-epk, --extraparanomeks, extra paranome Ks data to plot in the mixed Ks distribution, default None
+-pag, --plotapgmm, flag option, whether to plot mixture modeling of anchor Ks in the mixed Ks distribution, if the flag was set, the mixture modeling of anchor Ks will be plotted
+-pem, --plotelmm, flag option, whether to plot elmm mixture modeling of paranome Ks in the mixed Ks distribution, if the flag was set, the elmm mixture modeling of paranome Ks will be plotted
+-c, --components, the range of the number of components to fit in anchor Ks mixture modeling, default (1,4)
+```
+
+## Usage
+
+Here we provided the basic usage for each program.
+
+### wgd dmd
+
+**The delineation of whole paranome**
+```
+wgd dmd sequence
+``` 
+
+**The delineation of RBHs**
+```
+wgd dmd sequence1 sequence2
+```
+
+**The delineation of local MRBHs**
+```
+wgd dmd sequence1 sequence2 sequence3 -f sequence1
+```
+
+**The delineation of global MRBHs**
+```
+wgd dmd sequence1 sequence2 sequence3 -gm
+```
+
+**The delineation of orthogroups**
+```
+wgd dmd sequence1 sequence2 sequence3 -oi (option)
+```
+Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
+
+**The collinear coalescence inference of phylogeny**
+```
+wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
+```
+
+Note that there should be no duplicated gene IDs in the sequence file.
+
+### wgd focus
+
+**The concatenation-based/coalescence-based phylogenetic inference**
+```
+wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
+```
+
+**The functional annotation of gene families**
+```
+wgd focus families sequence1 sequence2 sequence3 --annotation eggnog -ed eddata --dmnb dbdata
+```
+
+**The phylogenetic dating of WGDs**
+```
+wgd focus families sequence1 sequence2 sequence3 -d mcmctree -sp spdata
+```
+
+### wgd ksd
+
+**The construction of whole paranome *K*<sub>S</sub> age distribution**
+```
+wgd ksd families sequence
+```
+
+**The construction of orthologous *K*<sub>S</sub> age distribution**
+```
+wgd ksd families sequence1 sequence2
+```
+
+**The construction of *K*<sub>S</sub> age distribution with rate correction**
+```
+wgd ksd families sequence1 sequence2 sequence3 -sr srdata -sp spdata
+```
+
+### wgd mix
+
+**The mixture model clustering analysis of *K*<sub>S</sub> age distribution**
+```
+wgd mix ksdata
+```
+
+### wgd peak
+
+**The search of crediable *K*<sub>S</sub> range used in WGD dating**
+```
+wgd peak ksdata -ap apdata -sm smdata -le ledata -mp mpdata
+```
+Note that users can add the flag --heuristic to implement the heuristic search analysis
+
+### wgd syn
+
+**The intra-specific synteny inference**
+```
+wgd syn families gff
+```
+
+**The inter-specific synteny inference**
+```
+wgd syn families gff1 gff2
+```
+
+### wgd viz
+
+**The visualization of *K*<sub>S</sub> age distribution**
+```
+wgd viz -d ksdata
+```
+
+**The visualization of *K*<sub>S</sub> age distribution with rate correction**
+```
+wgd viz -d ksdata -sr srdata -sp spdata -gs gsdata
+```
+
+**The visualization of synteny**
+```
+wgd viz -ap apdata -sm smdata -mt mtdata -gt gtdata
+```
+
+## Illustration
+
+We illustrate our program on an exemplary WGD inference and dating upon species *Aquilegia coerulea*.
+
+The *Aquilegia coerulea* was reported to experience an paleo-polyploidization event after the divergence of core eudicots, which is likely shared by all Ranunculales.
+
+First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
+
+```
+wgd dmd Aquilegia_coerulea
+wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
+```
+
+The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1 but not clear.
+
+![](data/Aquilegia_coerulea.tsv.ksd_wp.svg)
+
+We then construct the anchor *K*<sub>S</sub> age distribution using the command line below.
+
+```
+wgd syn -f mRNA -a Name wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea.gff3 -ks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+```
+
+As shown below, there are some retained anchor pairs with *K*<sub>S</sub> between 1 and 2, which seems to suggest a WGD event.
+
+![](data/Aquilegia_coerulea.tsv.ksd_wp_ap.svg)
+
+The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes.
+
+![](data/Aquilegia_coerulea_Aquilegia_coerulea_multiplicons_level.svg)
+
+We implemented two types of dot plots in oxford grid: one in the unit of bases and the other in the unit of genes, which can be colored by *K*<sub>S</sub> values given *K*<sub>S</sub> data.
+
+![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea_Ks.dot_unit_gene.png)
+
+As shown above, the dot plot in the unit of genes presents numerous densely aggregated (line-like) anchor points at most of the chromosomes with consistent *K*<sub>S</sub> age between 1 and 2. The dot plot in the unit of bases shows the same pattern, as manifested below.
+
+![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea_Ks.dot.png)
+
+The dot plots without *K*<sub>S</sub> annotation will also be automately produced, as shown below.
+
+![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot_unit_gene.png)
+
+![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
+
+A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
+
+![](data/Syndepth.svg)
+
+We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
+
+```
+wgd viz -d wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+```
+
+The result of ELMM mixture model clustering shows that there is a likely WGD component at *K*<sub>S</sub> 1.19.
+
+![](data/elmm_Aquilegia_coerulea.tsv.ks.tsv_best_models_weighted.svg)
+
+Let's do a mixture model clustering for anchor *K*<sub>S</sub> too, using the command line below.
+
+```
+wgd peak wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv --anchorpoints wgd_syn/iadhore-out/anchorpoints.txt --segments wgd_syn/iadhore-out/segments.txt --listelements wgd_syn/iadhore-out/list_elements.txt --multipliconpairs wgd_syn/iadhore-out/multiplicon_pairs.txt --weighted
+```
+
+The anchor *K*<sub>S</sub> age distribution also has a likely WGD component with mode 1.28.
+
+![](data/Original_AnchorKs_GMM_Component3_node_weighted_Lognormal.svg)
+
+Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis. First, we built a global MRBH family using the command below.
+
+```
+wgd dmd --globalmrbh Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera -o wgd_globalmrbh
+```
+
+In the global MRBH family, every pair of orthologous genes is the reciprocal best hit, suggesting true orthologous relationships. We would use the *K*<sub>S</sub> values associated with these orthologous pairs to delimit the divergence *K*<sub>S</sub> peak. Together with the whole paranome *K*<sub>S</sub> distribution, we conduct the rate correction using the command below.
+
+```
+wgd ksd wgd_globalmrbh/global_MRBH.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
+```
+
+The file `speciestree.nw` is the text file of species tree in newick that rate correction would be conducted on. Its content is as below. Users need to provide the species pairs to be plotted. We suggest adding the option `--reweight` to recalculate the weight per species pair such that the weight of orthologous gene pairs will become 1 as the paralogous gene pairs. The flag `--plotkde` can be added when the kde curve of orthologous *K*<sub>S</sub> is desired. Extra collinear data can be added by the option `-ap`.
+
+```
+(((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
+```
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
+
+As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
+
+If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
+```
+
+Note that we can easily show that *Aquilegia coerulea* has higher substitution rate than *Protea cynaroides* and *Vitis vinifera* by comparing their substitution distance in regard to the same divergence event with outgroup species *Acorus_americanus*, using command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_viz_Compare_rate --spair "Acorus_americanus;Protea_cynaroides" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Vitis_vinifera;Acorus_americanus" --gsmap gene_species.map --plotkde
+```
+
+![](data/Raw_Orthologues_Compare_rate.ksd.svg)
+
+As displayed above, the orthologous *K*<sub>S</sub> values bewteen *Aquilegia coerulea* and *Acorus americanus* has the highest mode, indicatingthe faster substitution rate of *Aquilegia coerulea* compared to *Protea cynaroides* and *Vitis vinifera*.
+
+Note that a necessary gene-species map file is needed for its implementation in `wgd viz`, which should be automately produced by the last `wgd ksd` step. The `gene_species.map` has contents as below in which each line is the joined string of gene name and species name by space.
+
+```
+Aqcoe6G057800.1 Aquilegia_coerulea
+Vvi_VIT_201s0011g01530.1 Vitis_vinifera
+Pcy_Procy01g08510 Protea_cynaroides
+Aam_Acora.04G142900.1 Acorus_americanus
+```
+
+A more complex plot can be made by add the flag `--plotelmm` such that the ELMM mixture modeling of provided paranome *K*<sub>S</sub> can be superimposed, using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm
+```
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Corrected.ksd.svg)
+
+From the mixed *K*<sub>S</sub> plot above, we can see that the optimized lognormal component b with mode 1.2 is younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera* (1.39 and 1.47, respectively).
+
+Besides, we can also add the GMM mixture modeling of anchor *K*<sub>S</sub> values with the flag `--plotapgmm`, using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotapgmmm
+```
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Apgmm_Corrected.ksd.svg)
+
+As manifested above, the anchor *K*<sub>S</sub> component 2 with mode 1.28 is also younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera*. But we need to be of course cautious that such distinction comes with the uncertainties introduced from the applied mixture modeling methodology in terms of for instance different initialization points and the issue of overfitting and the sister speciess adopted in that there might be species with more disparate substitution rates than the one we chose.
+
+Adding both ELMM result for paranome and GMM result for anchor *K*<sub>S</sub> can be achieved just by add the two flags mentioned above, using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm --plotapgmmm
+```
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Apgmm_Corrected.ksd.svg)
+
+An alternative way to calculate the orthologous *K*<sub>S</sub> is to directly use the orthogroups instead of global MRBH family. That way we don't use the pre-inferred paranome *K*<sub>S</sub> but the paralogous gene pairs inside each orthogroup instead. To achieve that, we first need to infer orthogroups using the command below.
+
+```
+wgd dmd Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera --orthoinfer -o wgd_ortho (--onlyortho) 
+```
+
+Users can decide to only conduct the orthogroup analysis while skipping other analysis by adding the flag `--onlyortho`. Next step is the same with global MRBH family except that we don't use the extra pre-inferred paranome *K*<sub>S</sub> anymore. We infer the *K*<sub>S</sub> using the command below. Note that the program `wgd viz` can plot the same just as shown above.
+
+```
+wgd ksd wgd_ortho/Orthogroups.sp.tsv -sp speciestree.nw --reweight -o wgd_ortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
+```
+
+![](data/Aquilegia_coerulea_OrthoKs_Corrected.ksd.svg)
+
+As shown above, the number of both paralogous gene pairs and orthologous gene pairs is different than the one from global MRBH family in that here we plotted all orthologous gene pairs instead of only global MRBH and potentially new paralogous gene pairs might be produced in the orthogroup inference step, together with different recalculated weights.
+
+If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, as we have already shown above, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --gsmap gene_species.map
+```
+
+We can clearly see that *Vitis vinifera* has higher substitution rate than *Protea cynaroides* in that their orthologous *K*<sub>S</sub> peaks with *Aquilegia coerulea*, although representing the same divergence event, differed in substitution distance.
+![](data/Raw_Orthologues.ksd.svg)
+
+After the phylogenetic timing of the Ranunculales WGD, we can further infer its absolute age. First we infer the credible range of anchor pairs by *K*<sub>S</sub> heuristically using the program `wgd peak`.
+
+```
+wgd peak --heuristic wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -ap wgd_syn/iadhore-out/anchorpoints.txt -sm wgd_syn/iadhore-out/segments.txt -le wgd_syn/iadhore-out/list_elements.txt -mp wgd_syn/iadhore-out/multiplicon_pairs.txt -o wgd_peak
+```
+
+![](data/AnchorKs_PeakCI_Aquilegia_coerulea.tsv.ks.tsv_node_weighted.svg)
+
+As shown above, we assumed a lognormal distribution at the peak location detected by the `signal` module of `scipy` library. The 95% confidence level of the lognormal distribution was applied, i.e., 0.68-2.74, in further molecular dating. The file `Aquilegia_coerulea.tsv.ks.tsv_95%CI_AP_for_dating_weighted_format.tsv` is what we need for next step. To build the orthogroups used in phylogenetic dating, we need to select some species and form a starting tree with proper fossil calibrations. We provide one in mcmctree format as below.
+
+```
+17 1
+((((Potamogeton_acutifolius,(Spirodela_intermedia,Amorphophallus_konjac)),(Acanthochlamys_bracteata,(Dioscorea_alata,Dioscorea_rotundata))'>0.5600<1.2863')'>0.8360<1.2863',(Acorus_americanus,Acorus_tatarinowii))'>0.8360<1.2863',((((Tetracentron_sinense,Trochodendron_aralioides),(Buxus_austroyunnanensis,Buxus_sinica))'>1.1080<1.2863',(Nelumbo_nucifera,(Telopea_speciosissima,Protea_cynaroides)))'>1.1080<1.2863',(Aquilegia_coerulea_ap1,Aquilegia_coerulea_ap2))'>1.1080<1.2863')'>1.2720<2.4720';
+```
+
+As presented above, the focus species that is about to be dated needs to be replaced with `(Aquilegia_coerulea_ap1,Aquilegia_coerulea_ap2)`. With this starting tree and predownloaded cds files of all the species, we can build the orthogroup used in the final molecular dating using the command as below.
+
+```
+wgd dmd -f Aquilegia_coerulea -ap wgd_peak/Aquilegia_coerulea.tsv.ks.tsv_95%CI_AP_for_dating_weighted_format.tsv -o wgd_dmd_ortho Potamogeton_acutifolius Spirodela_intermedia Amorphophallus_konjac Acanthochlamys_bracteata Dioscorea_alata Dioscorea_rotundata Acorus_americanus Acorus_tatarinowii Tetracentron_sinense Trochodendron_aralioides Buxus_austroyunnanensis Buxus_sinica Nelumbo_nucifera Telopea_speciosissima Protea_cynaroides Aquilegia_coerulea
+```
+
+The result file `merge_focus_ap.tsv` is what we need for the final step of molecular dating in program `wgd focus`.
+
+```
+wgd focus --protdating --aamodel lg wgd_dmd_ortho/merge_focus_ap.tsv -sp dating_tree.nw -o wgd_dating -d mcmctree -ds 'burnin = 2000' -ds 'sampfreq = 1000' -ds 'nsample = 20000' Potamogeton_acutifolius Spirodela_intermedia Amorphophallus_konjac Acanthochlamys_bracteata Dioscorea_alata Dioscorea_rotundata Acorus_americanus Acorus_tatarinowii Tetracentron_sinense Trochodendron_aralioides Buxus_austroyunnanensis Buxus_sinica Nelumbo_nucifera Telopea_speciosissima Protea_cynaroides Aquilegia_coerulea
+```
+
+Here we only implemented the concatenation analysis using protein sequence by adding the flag `--protdating` and we set the parameter for `mcmctree` via the option `-ds`. Note that other dating program such as `r8s` and `beast` are also available given some mandatory parameters. The final log of the successful run is as below.
+
+```
+16:04:25 INFO     Running mcmctree using Hessian matrix of LG+Gamma  core.py:967
+                  for protein model
+23:49:37 INFO     Posterior mean for the ages of wgd is 1.128945 mcmctree.py:296
+                  billion years from Concatenated peptide
+                  alignment and 95% credibility intervals (CI)
+                  is 1.01224-1.23121 billion years
+         INFO     Total run time: 29175s                              cli.py:241
+         INFO     Done                                                cli.py:242
+```
+
+To visualize the date, we also provided a python script to plot the WGD dates in the `wgd` folder. Users need to extract the raw dates from the `mcmc.txt` for the WGD node first and save it as file `dates.txt` (or whatever preferred name). An example command is as below.
+
+```
+python $PATH/postplot.py postdis dates.txt --percentile 90 --title "WGD date" --hpd -o "Ranunculales_WGD_date.svg"
+```
+
+![](data/Ranunculales_WGD_date.svg)
+
+The posterior mean, median and mode of the Ranunculales WGD age is 112.92, 113.44 and 112.54 mya, with 90% HPD 105.07 - 122.32 mya as manifested above.
+
+## Citation
+ 
+Please cite us at https://doi.org/10.1093/bioinformatics/bty915
+
+```
+Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
+
+Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
+```
+
+For citation of the tools used in wgd, please consult the documentation at
+https://wgdv2.readthedocs.io/en/latest/citation.html.
+
```

### Comparing `wgd-2.0.16/README.md` & `wgd-2.0.17/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,42 @@
+Metadata-Version: 2.1
+Name: wgd
+Version: 2.0.17
+Summary: wgd
+Home-page: http://github.com/heche-psb/wgd
+Author: Hengchi Chen
+Author-email: heche@psb.vib-ugent.be
+License: GPL
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 
 # `wgd v2` : a suite tool of WGD inference and timing
 
+[![Build Status](https://app.travis-ci.com/heche-psb/wgd.svg?branch=phylodating)](https://app.travis-ci.com/heche-psb/wgd)
+[![Documentation Status](https://readthedocs.org/projects/wgdv2/badge/?version=latest)](https://wgdv2.readthedocs.io/en/latest/?badge=latest)
+[![license](https://img.shields.io/pypi/l/wgd.svg)](https://pypi.python.org/pypi/wgd)
+[![Latest PyPI version](https://img.shields.io/pypi/v/wgd.svg)](https://pypi.python.org/pypi/wgd)
+[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/wgd/README.html)
+[![Downloads](https://pepy.tech/badge/wgd)](https://pepy.tech/project/wgd)
+
 **Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
 
 [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
 
 [**Introduction**](#Introduction) | 
 [**Installation**](#Installation) | 
 [**Parameters**](#Parameters) | 
 [**Usage**](#Usage) | 
 [**Illustration**](#Illustration) |
+[**Documentation**](https://wgdv2.readthedocs.io/en/latest/?badge=latest) |
 [**Citation**](#Citation)
 
+
 </div>
 
 `wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
 
 ## Introduction
 
 Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
@@ -112,26 +132,26 @@
 --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
 --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
 -a, --aligner, which alignment program to use, default mafft
 -tree, --tree_method, which gene tree inference program to invoke, default fasttree
 -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
 --concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
 --coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
--sp, --speciestree, species tree darafile for dating, default None
+-sp, --speciestree, species tree datafile for dating, default None
 -d, --dating, which molecular dating program to use, default none
 -ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
 -ns, --nsites, the nsites information for r8s dating, default None
 -ot, --outgroup, the outgroup information for r8s dating, default None
 -pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
 -am, --aamodel, which protein model to be used in mcmctree, default poisson
--ks, flag option, whether to initiate Ks analysis
---annotation, which annotation program to use, default none
+-ks, flag option, whether to initiate Ks calculation
+--annotation, which annotation program to use, default None
 --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
 -ed, --eggnogdata, the eggnog annotation datafile, default None
---pfam, which option to use for pfam annotation, default none
+--pfam, which option to use for pfam annotation, default None
 --dmnb, the diamond database for annotation, default None
 --hmm, the HMM profile for annotation, default None
 --evalue, the e-value cut-off for annotation, default 1e-10
 --exepath, the path to the interproscan executable, default None
 -f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
  -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
 -cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
@@ -152,22 +172,28 @@
 --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
 --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
 -tree, --tree_method, which gene tree inference program to invoke, default fasttree
 -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
 -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
 -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
 -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+-epk, --extraparanomeks, extra paranome Ks data to plot in the mixed Ks distribution, default None
+-ap, --anchorpoints, anchorpoints.txt file to plot anchor Ks in the mixed Ks distribution, default None
+-pk, --plotkde, flag option, whether to plot kde curve of orthologous Ks distribution over histogram in the mixed Ks distribution, if the flag was set, the kde curve will be plotted
+-pag, --plotapgmm, flag option, whether to plot mixture modeling of anchor Ks in the mixed Ks distribution, if the flag was set, the mixture modeling of anchor Ks will be plotted
+-pem, --plotelmm, flag option, whether to plot elmm mixture modeling of paranome Ks in the mixed Ks distribution, if the flag was set, the elmm mixture modeling of paranome Ks will be plotted
+-c, --components, the range of the number of components to fit in anchor Ks mixture modeling, default (1,4)
 ```
 
 The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
 ```
 wgd mix ks_datafile (option)
 --------------------------------------------------------------------------------
 -f, --filters, the cutoff alignment length, default 300
--r, --ks_range, the Ks range to be considered, default (0.005, 3)
+-r, --ks_range, the Ks range to be considered, default (0, 5)
 -b, --bins, the number of bins in Ks distribution, default 50
 -o, --outdir, the output directory, default wgd_mix
 --method, which mixture model to use, default gmm
 -n, --components, the range of the number of components to fit, default (1, 4)
 -g, --gamma, the gamma parameter for bgmm models, default 0.001
 -ni, --n_init, the number of k-means initializations, default 200
 -mi, --max_iter, the maximum number of iterations, default 1000
@@ -197,22 +223,23 @@
 -bm, --bw_method, the bandwidth method to be used, default silverman
 --n_medoids, the number of medoids to fit, default 2
 -km, --kdemethod, the kde method to be used, default scipy
 --n_clusters, the number of clusters to plot Elbow loss function, default 5
 --kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
 -gd, --guide, the regime residing anchors, default: segment
 -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
--kd, --kstodate, the range of Ks to be dated, default (0.5, 1.5)
+-kd, --kstodate, the range of Ks to be dated in heuristic search, default (0.5, 1.5)
 -f, --family, the family to filter Ks upon, default None
 --manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
 -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
 --ci, the confidence level of log-normal distribution to date, default 95
---hdr, the highest densidy region (HDR) in a given distribution to date, default 95
+--hdr, the highest density region (HDR) in a given distribution to date, default 95
 --heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
 -kc, --kscutoff, the Ks saturation cutoff in dating, default 5
+-g, --gamma, the gamma parameter for bgmm models, default 1e-3
 ```
 
 The program `wgd syn` can realize the intra- and inter-specific synteny inference.
 ```
 wgd syn families gffs (option)
 --------------------------------------------------------------------------------
 -ks, --ks_distribution, ks distribution datafile, default None
@@ -240,22 +267,26 @@
 -pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
 -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
 -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
 -iter, --em_iterations, the maximum EM iterations, default 200
 -init, --em_initializations, the maximum EM initializations, default 200
 -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
 -sm, --segments, the segments data file, default None
--ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
+-ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffolds will be set
 -ms, --maxsize, the maximum family size to include, default 200
 -ap, --anchorpoints, the anchor points datafile, default None
 -mt, --multiplicon, the multiplicons datafile, default None
 -gt, --genetable, the gene table datafile, default None
 -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
 -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
 -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+-epk, --extraparanomeks, extra paranome Ks data to plot in the mixed Ks distribution, default None
+-pag, --plotapgmm, flag option, whether to plot mixture modeling of anchor Ks in the mixed Ks distribution, if the flag was set, the mixture modeling of anchor Ks will be plotted
+-pem, --plotelmm, flag option, whether to plot elmm mixture modeling of paranome Ks in the mixed Ks distribution, if the flag was set, the elmm mixture modeling of paranome Ks will be plotted
+-c, --components, the range of the number of components to fit in anchor Ks mixture modeling, default (1,4)
 ```
 
 ## Usage
 
 Here we provided the basic usage for each program.
 
 ### wgd dmd
@@ -394,19 +425,29 @@
 wgd syn -f mRNA -a Name wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea.gff3 -ks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
 ```
 
 As shown below, there are some retained anchor pairs with *K*<sub>S</sub> between 1 and 2, which seems to suggest a WGD event.
 
 ![](data/Aquilegia_coerulea.tsv.ksd_wp_ap.svg)
 
-The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes, except for the chr_07, which seems to experience more severe fragmentization than the other chromosomes.
+The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes.
 
 ![](data/Aquilegia_coerulea_Aquilegia_coerulea_multiplicons_level.svg)
 
-The associated dotplot in oxford grid also presents numerous densely aggregated anchor points throughout most of the chromosomes.
+We implemented two types of dot plots in oxford grid: one in the unit of bases and the other in the unit of genes, which can be colored by *K*<sub>S</sub> values given *K*<sub>S</sub> data.
+
+![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea_Ks.dot_unit_gene.png)
+
+As shown above, the dot plot in the unit of genes presents numerous densely aggregated (line-like) anchor points at most of the chromosomes with consistent *K*<sub>S</sub> age between 1 and 2. The dot plot in the unit of bases shows the same pattern, as manifested below.
+
+![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea_Ks.dot.png)
+
+The dot plots without *K*<sub>S</sub> annotation will also be automately produced, as shown below.
+
+![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot_unit_gene.png)
 
 ![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
 
 A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
 
 ![](data/Syndepth.svg)
 
@@ -526,20 +567,70 @@
 ```
 wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --gsmap gene_species.map
 ```
 
 We can clearly see that *Vitis vinifera* has higher substitution rate than *Protea cynaroides* in that their orthologous *K*<sub>S</sub> peaks with *Aquilegia coerulea*, although representing the same divergence event, differed in substitution distance.
 ![](data/Raw_Orthologues.ksd.svg)
 
+After the phylogenetic timing of the Ranunculales WGD, we can further infer its absolute age. First we infer the credible range of anchor pairs by *K*<sub>S</sub> heuristically using the program `wgd peak`.
+
+```
+wgd peak --heuristic wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -ap wgd_syn/iadhore-out/anchorpoints.txt -sm wgd_syn/iadhore-out/segments.txt -le wgd_syn/iadhore-out/list_elements.txt -mp wgd_syn/iadhore-out/multiplicon_pairs.txt -o wgd_peak
+```
+
+![](data/AnchorKs_PeakCI_Aquilegia_coerulea.tsv.ks.tsv_node_weighted.svg)
+
+As shown above, we assumed a lognormal distribution at the peak location detected by the `signal` module of `scipy` library. The 95% confidence level of the lognormal distribution was applied, i.e., 0.68-2.74, in further molecular dating. The file `Aquilegia_coerulea.tsv.ks.tsv_95%CI_AP_for_dating_weighted_format.tsv` is what we need for next step. To build the orthogroups used in phylogenetic dating, we need to select some species and form a starting tree with proper fossil calibrations. We provide one in mcmctree format as below.
+
+```
+17 1
+((((Potamogeton_acutifolius,(Spirodela_intermedia,Amorphophallus_konjac)),(Acanthochlamys_bracteata,(Dioscorea_alata,Dioscorea_rotundata))'>0.5600<1.2863')'>0.8360<1.2863',(Acorus_americanus,Acorus_tatarinowii))'>0.8360<1.2863',((((Tetracentron_sinense,Trochodendron_aralioides),(Buxus_austroyunnanensis,Buxus_sinica))'>1.1080<1.2863',(Nelumbo_nucifera,(Telopea_speciosissima,Protea_cynaroides)))'>1.1080<1.2863',(Aquilegia_coerulea_ap1,Aquilegia_coerulea_ap2))'>1.1080<1.2863')'>1.2720<2.4720';
+```
+
+As presented above, the focus species that is about to be dated needs to be replaced with `(Aquilegia_coerulea_ap1,Aquilegia_coerulea_ap2)`. With this starting tree and predownloaded cds files of all the species, we can build the orthogroup used in the final molecular dating using the command as below.
+
+```
+wgd dmd -f Aquilegia_coerulea -ap wgd_peak/Aquilegia_coerulea.tsv.ks.tsv_95%CI_AP_for_dating_weighted_format.tsv -o wgd_dmd_ortho Potamogeton_acutifolius Spirodela_intermedia Amorphophallus_konjac Acanthochlamys_bracteata Dioscorea_alata Dioscorea_rotundata Acorus_americanus Acorus_tatarinowii Tetracentron_sinense Trochodendron_aralioides Buxus_austroyunnanensis Buxus_sinica Nelumbo_nucifera Telopea_speciosissima Protea_cynaroides Aquilegia_coerulea
+```
+
+The result file `merge_focus_ap.tsv` is what we need for the final step of molecular dating in program `wgd focus`.
+
+```
+wgd focus --protdating --aamodel lg wgd_dmd_ortho/merge_focus_ap.tsv -sp dating_tree.nw -o wgd_dating -d mcmctree -ds 'burnin = 2000' -ds 'sampfreq = 1000' -ds 'nsample = 20000' Potamogeton_acutifolius Spirodela_intermedia Amorphophallus_konjac Acanthochlamys_bracteata Dioscorea_alata Dioscorea_rotundata Acorus_americanus Acorus_tatarinowii Tetracentron_sinense Trochodendron_aralioides Buxus_austroyunnanensis Buxus_sinica Nelumbo_nucifera Telopea_speciosissima Protea_cynaroides Aquilegia_coerulea
+```
+
+Here we only implemented the concatenation analysis using protein sequence by adding the flag `--protdating` and we set the parameter for `mcmctree` via the option `-ds`. Note that other dating program such as `r8s` and `beast` are also available given some mandatory parameters. The final log of the successful run is as below.
+
+```
+16:04:25 INFO     Running mcmctree using Hessian matrix of LG+Gamma  core.py:967
+                  for protein model
+23:49:37 INFO     Posterior mean for the ages of wgd is 1.128945 mcmctree.py:296
+                  billion years from Concatenated peptide
+                  alignment and 95% credibility intervals (CI)
+                  is 1.01224-1.23121 billion years
+         INFO     Total run time: 29175s                              cli.py:241
+         INFO     Done                                                cli.py:242
+```
+
+To visualize the date, we also provided a python script to plot the WGD dates in the `wgd` folder. Users need to extract the raw dates from the `mcmc.txt` for the WGD node first and save it as file `dates.txt` (or whatever preferred name). An example command is as below.
+
+```
+python $PATH/postplot.py postdis dates.txt --percentile 90 --title "WGD date" --hpd -o "Ranunculales_WGD_date.svg"
+```
+
+![](data/Ranunculales_WGD_date.svg)
+
+The posterior mean, median and mode of the Ranunculales WGD age is 112.92, 113.44 and 112.54 mya, with 90% HPD 105.07 - 122.32 mya as manifested above.
+
 ## Citation
  
 Please cite us at https://doi.org/10.1093/bioinformatics/bty915
 
 ```
 Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
 
 Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
 ```
 
 For citation of the tools used in wgd, please consult the documentation at
-https://wgd.readthedocs.io/en/latest/index.html#citation.
+https://wgdv2.readthedocs.io/en/latest/citation.html.
```

### Comparing `wgd-2.0.16/cli.py` & `wgd-2.0.17/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # CLI entry point
 @click.group(context_settings={'help_option_names': ['-h', '--help']})
 @click.option('--verbosity', '-v', type=click.Choice(['info', 'debug']),
     default='info', help="Verbosity level, default = info.")
 def cli(verbosity):
     """
-    wgd - Copyright (C) 2023-2024 Hengchi Chen\n
+    wgd v2 - Copyright (C) 2023-2024 Hengchi Chen\n
     Contact: heche@psb.vib-ugent.be
     """
     logging.basicConfig(
         format='%(message)s',
         handlers=[RichHandler()],
         datefmt='%H:%M:%S',
         level=verbosity.upper())
@@ -329,15 +329,15 @@
 @click.option('--guide', '-gd', type=click.Choice(['multiplicon', 'basecluster', 'segment']), default='segment', show_default=True, help="regime residing anchors")
 @click.option('--prominence_cutoff', '-prct', type=float, default=0.1, show_default=True, help='prominence cutoff of acceptable peaks')
 @click.option('--kstodate', '-kd', nargs=2, type=float, default=(0.5, 1.5), show_default=True, help='range of Ks to be dated')
 @click.option('--family', '-f', default=None, show_default=True, help='family to filter Ks upon')
 @click.option('--manualset', is_flag=True,help="Manually set Ks range of anchor pairs or multiplicons as CI")
 @click.option('--rel_height', '-rh', type=float, default=0.4, show_default=True, help='relative height at which the peak width is measured')
 @click.option('--ci', default=95, show_default=True,type=int, help='confidence level of log-normal distribution to date')
-@click.option('--hdr', default=95, show_default=True,type=int, help='highest densidy region (HDR) in a given distribution to date')
+@click.option('--hdr', default=95, show_default=True,type=int, help='highest density region (HDR) in a given distribution to date')
 @click.option('--heuristic', is_flag=True,help="heuristic CI for dating")
 @click.option('--kscutoff', '-kc', default=5, show_default=True, type=float, help='Ks Saturation cutoff for genes in Dating')
 def peak(**kwargs):
     """
     Infer peak and CI of Ks distribution.
     """
     _peak(**kwargs)
@@ -422,18 +422,19 @@
     default='fasttree', show_default=True,
     help="Tree inference method for node weighting")
 @click.option('--spair', '-sr', multiple=True, default=None, show_default=True,help='species pair to be plotted')
 @click.option('--speciestree', '-sp', default=None, show_default=True,help='species tree to perform rate correction')
 @click.option('--reweight', '-rw', is_flag=True, help='recalculate the weight per species pair')
 @click.option('--onlyrootout', '-or', is_flag=True, help='only consider the outgroup at root')
 @click.option('--extraparanomeks', '-epk', default=None, help='extra paranome ks data')
-@click.option('--anchorpoints', '-ap', default=None, show_default=True, help='anchorpoints.txt file')
+@click.option('--anchorpoints', '-ap', default=None, show_default=True, help='anchorpoints.txt file to plot anchor Ks')
 @click.option('--plotkde', '-pk', is_flag=True, help='plot kde curve over histogram')
-@click.option('--plotapgmm', '-pag', is_flag=True, help='plot mixture modeling of anchor pairs')
-@click.option('--components', '-c', nargs=2, default=(1, 4), show_default=True, help="range of number of components to fit")
+@click.option('--plotapgmm', '-pag', is_flag=True, help='plot mixture modeling of anchor Ks')
+@click.option('--plotelmm', '-pem', is_flag=True, help='plot elmm mixture modeling')
+@click.option('--components', '-c', nargs=2, default=(1, 4), show_default=True, help="range of the number of components to fit in anchor Ks mixture modeling")
 def ksd(**kwargs):
     """
     Paranome and one-to-one ortholog Ks distribution inference pipeline.
 
     Example 1 - whole-paranome:
 
         wgd ksd families.mcl cds.fasta
@@ -444,15 +445,15 @@
 
     If you want to keep intermediate (temporary) files, please provide a directory
     name for the `--tmpdir` option.
     """
     _ksd(**kwargs)
 
 def _ksd(families, sequences, outdir, tmpdir, nthreads, to_stop, cds, pairwise,
-        strip_gaps, tree_method,spair, speciestree, reweight, onlyrootout, extraparanomeks, anchorpoints, plotkde, plotapgmm, components):
+        strip_gaps, tree_method,spair, speciestree, reweight, onlyrootout, extraparanomeks, anchorpoints, plotkde, plotapgmm, plotelmm, components):
     from wgd.core import get_gene_families, SequenceData, KsDistributionBuilder
     from wgd.core import read_gene_families, merge_seqs
     from wgd.viz import default_plot, apply_filters,multi_sp_plot
     start = timer()
     if tmpdir != None and not os.path.isdir(tmpdir): os.mkdir(tmpdir)
     if len(sequences) == 0: 
         logging.error("Please provide at least one sequence file")
@@ -479,15 +480,15 @@
     logging.info("Making plots")
     df = apply_filters(ksdb.df, [("dS", 0., 5.)])
     ylabel = "Duplications"
     if len(sequences) == 2:
         ylabel = "RBH orthologs"
     elif len(sequences) > 2:
         ylabel = "Homologous pairs"
-    if len(spair)!= 0:  multi_sp_plot(df,spair,spgenemap,outdir,onlyrootout,title=prefix,ylabel=ylabel,ksd=True,reweight=reweight,sptree=speciestree,extraparanomeks=extraparanomeks, ap = anchorpoints,plotkde=plotkde,plotapgmm=plotapgmm,components=components)
+    if len(spair)!= 0:  multi_sp_plot(df,spair,spgenemap,outdir,onlyrootout,title=prefix,ylabel=ylabel,ksd=True,reweight=reweight,sptree=speciestree,extraparanomeks=extraparanomeks, ap = anchorpoints,plotkde=plotkde,plotapgmm=plotapgmm,plotelmm=plotelmm,components=components)
     fig = default_plot(df, title=prefix, bins=50, ylabel=ylabel)
     fig.savefig(os.path.join(outdir, "{}.ksd.svg".format(prefix)))
     fig.savefig(os.path.join(outdir, "{}.ksd.pdf".format(prefix)))
     plt.close()
     if tmpdir is None:
         [x.remove_tmp(prompt=False) for x in seqs]
     end = timer()
@@ -508,44 +509,61 @@
 @click.option('--em_initializations', '-init', type=int, default=200, show_default=True, help='maximum EM initializations')
 @click.option('--prominence_cutoff', '-prct', type=float, default=0.1, show_default=True, help='prominence cutoff of acceptable peaks')
 @click.option('--segments', '-sm', default=None,show_default=True,help='segments.txt file')
 @click.option('--minlen', '-ml', default=-1, show_default=True, help="minimum length of a genomic element to be included in dotplot")
 @click.option('--maxsize', '-ms', default=200, show_default=True, help="maximum family size to include in analysis")
 @click.option('--anchorpoints', '-ap', default=None, show_default=True, help='anchorpoints.txt file')
 @click.option('--multiplicon', '-mt', default=None, show_default=True, help='multiplicons.txt file')
+@click.option('--multipliconpairs', '-mp', default=None, show_default=True, help='multipliconpairs information')
 @click.option('--genetable', '-gt', default=None, show_default=True, help='gene-table.csv file')
 @click.option('--rel_height', '-rh', type=float, default=0.4, show_default=True, help='relative height at which the peak width is measured')
 @click.option('--minseglen', '-mg', default=10000, show_default=True, help="minimum length (ratio if <=1) of segments to show in marco-synteny")
 @click.option('--keepredun', '-kr', is_flag=True, help='keep redundant multiplicons')
 @click.option('--extraparanomeks', '-epk', default=None, help='extra paranome ks data')
 @click.option('--plotapgmm', '-pag', is_flag=True, help='plot mixture modeling of anchor pairs')
 @click.option('--plotelmm', '-pem', is_flag=True, help='plot elmm mixture modeling')
 @click.option('--components', '-n', nargs=2, default=(1, 4), show_default=True, help="range of number of components to fit")
+@click.option('--mingenenum', '-mgn', default=30, type=int, show_default=True, help="min number of genes on segments to be considered")
+@click.option('--plotsyn', '-psy', is_flag=True, help='plot synteny')
 def viz(**kwargs):
     """
     Visualization of Ks distribution or synteny
     """
     _viz(**kwargs)
 
-def _viz(datafile,spair,outdir,gsmap,plotkde,reweight,em_iterations,em_initializations,prominence_cutoff,segments,minlen,maxsize,anchorpoints,multiplicon,genetable,rel_height,speciestree,onlyrootout,minseglen,keepredun,extraparanomeks,plotapgmm,plotelmm,components):
-    from wgd.viz import elmm_plot, apply_filters, multi_sp_plot, default_plot,all_dotplots,filter_by_minlength
+def _viz(datafile,spair,outdir,gsmap,plotkde,reweight,em_iterations,em_initializations,prominence_cutoff,segments,minlen,maxsize,anchorpoints,multiplicon,genetable,rel_height,speciestree,onlyrootout,minseglen,keepredun,extraparanomeks,plotapgmm,plotelmm,components,multipliconpairs,mingenenum,plotsyn):
+    from wgd.viz import elmm_plot, apply_filters, multi_sp_plot, default_plot,all_dotplots,filter_by_minlength,dotplotunitgene,dotplotingene,filter_mingenumber
     from wgd.core import _mkdir
-    from wgd.syn import get_anchors,get_multi,get_segments_profile
+    from wgd.syn import get_anchors,get_multi,get_segments_profile,get_chrom_gene,get_mp_geneorder,transformunit
+    from wgd.peak import formatv2
     if datafile!=None: prefix = os.path.basename(datafile)
     _mkdir(outdir)
-    if datafile ==None:
+    if plotsyn:
+        df = None
+        if datafile!=None:
+            ksdb_df = pd.read_csv(datafile,header=0,index_col=0,sep='\t')
+            ksdb_df = formatv2(ksdb_df)
+            df = apply_filters(ksdb_df, [("dS", 0., 5.)])
         table = pd.read_csv(genetable,header=0,index_col=0,sep=',')
-        df_anchor,df_multi = get_anchors('',userdf=anchorpoints),get_multi('',userdf2=multiplicon)
+        table_orig = table.copy()
+        df_anchor,orig_anchors = get_anchors('',userdf=anchorpoints)
+        df_multi = get_multi('',userdf2=multiplicon)
+        ordered_genes_perchrom_allsp, gene_orders = get_chrom_gene(table,outdir)
+        ordered_mp = get_mp_geneorder(gene_orders,'',outdir,table,userdf4=multipliconpairs)
         segs = get_segments_profile(df_multi,keepredun,'',userdf3=segments)
-        segs,table,df_multi = filter_by_minlength(table,segs,minlen,df_multi,keepredun,outdir,minseglen)
-        figs = all_dotplots(table, segs, df_multi, minseglen, anchors=df_anchor, maxsize=maxsize, minlen=minlen, outdir=outdir)
+        segs,table,df_multi,removed_scfa = filter_by_minlength(table,segs,minlen,df_multi,keepredun,outdir,minseglen)
+        segs_gene_unit, gene_order_dict_allsp = transformunit(segs,ordered_genes_perchrom_allsp,outdir)
+        segs = filter_mingenumber(segs_gene_unit,mingenenum)
+        dotplotingene(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=df_anchor,ksdf=df,maxsize=maxsize)
+        #dotplotunitgene(ordered_genes_perchrom_allsp,segs_gene_unit,removed_scfa,outdir,mingenenum,table_orig,ordered_mp,ksdf=df)
+        figs = all_dotplots(table, segs, df_multi, minseglen, anchors=df_anchor, maxsize=maxsize, minlen=minlen, outdir=outdir, Ks = df)
         for k, v in figs.items():
             v.savefig(os.path.join(outdir, "{}.dot.svg".format(k)))
             v.savefig(os.path.join(outdir, "{}.dot.pdf".format(k)))
-            v.savefig(os.path.join(outdir, "{}.dot.png".format(k)))
+            v.savefig(os.path.join(outdir, "{}.dot.png".format(k)),dpi=1200)
         logging.info('Done')
         exit()
     ksdb_df = pd.read_csv(datafile,header=0,index_col=0,sep='\t')
     df = apply_filters(ksdb_df, [("dS", 0., 5.)])
     ylabel = "Duplications" if spair == () else "Homologous pairs"
     if len(spair)!= 0: multi_sp_plot(df,spair,gsmap,outdir,onlyrootout,title=prefix,ylabel=ylabel,viz=True,plotkde=plotkde,reweight=reweight,sptree=speciestree,ap = anchorpoints, extraparanomeks=extraparanomeks,plotapgmm=plotapgmm,plotelmm=plotelmm,components=components,max_EM_iterations=em_iterations,num_EM_initializations=em_initializations,peak_threshold=prominence_cutoff,rel_height=rel_height)
     fig = default_plot(df, title=prefix, bins=50, ylabel=ylabel)
@@ -576,74 +594,91 @@
     help="maximum family size to include in analysis.")
 @click.option('--ks_range', '-r', nargs=2, default=(0, 5), show_default=True,
     type=float, help='Ks range to use for colored dotplot')
 @click.option('--iadhore_options', default="",
     help="other options for I-ADHoRe, as a comma separated string, "
          "e.g. gap_size=30,q_value=0.75,prob_cutoff=0.05")
 @click.option('--ancestor', '-ac', default=None,show_default=True,help='assumed ancestor species')
-@click.option('--minseglen', '-mg', default=100000, show_default=True, help="min length of segments in ratio if <= 1")
+@click.option('--minseglen', '-mg', default=10000, show_default=True, help="min length of segments in ratio if <= 1")
 @click.option('--keepredun', '-kr', is_flag=True, help='keep redundant multiplicons')
+@click.option('--mingenenum', '-mgn', default=30, type=int, show_default=True, help="min number of genes on segments to be considered")
 def syn(**kwargs):
     """
     Co-linearity and anchor inference using I-ADHoRe.
     """
     _syn(**kwargs)
 
 def _syn(families, gff_files, ks_distribution, outdir, feature, attribute,
-        minlen, maxsize, ks_range, iadhore_options, ancestor, minseglen, keepredun):
+        minlen, maxsize, ks_range, iadhore_options, ancestor, minseglen, keepredun, mingenenum):
     """
     Co-linearity and anchor inference using I-ADHoRe.
     """
     from wgd.syn import make_gene_table, configure_adhore, run_adhore
-    from wgd.syn import get_anchors, get_anchor_ksd, get_segments_profile, get_multi
-    from wgd.viz import default_plot, apply_filters, all_dotplots, syntenic_dotplot_ks_colored,filter_by_minlength
+    from wgd.syn import get_anchors, get_anchor_ksd, get_segments_profile, get_multi, get_chrom_gene, transformunit, get_mp_geneorder
+    from wgd.viz import default_plot, apply_filters, all_dotplots, syntenic_dotplot_ks_colored,filter_by_minlength,dotplotunitgene,dotplotingene,filter_mingenumber
+    from wgd.peak import formatv2
     # non-default options for I-ADHoRe
     iadhore_opts = {x.split("=")[0].strip(): x.split("=")[1].strip()
                for x in iadhore_options.split(",") if x != ""}
     if len(iadhore_opts) > 0:
         logging.info("I-ADHoRe 3.0 options: {}".format(iadhore_opts))
     # read families and make table
     prefix = os.path.basename(families)
     fams = pd.read_csv(families, index_col=0, sep="\t")
     table = make_gene_table(gff_files, fams, feature, attribute)
+    table_orig = table.copy()
     if len(table.dropna().index) == 0:
         logging.error("No genes from families file `{}` found in the GFF file "
                 "for `feature={}` and `attribute={}`, please double check command " 
                 "settings.".format(families, feature, attribute))
         exit(1)
     if len(table.dropna()) < 1000:
         logging.warning("Few genes from families `{}` found in the GFF file, better "
                 "Double check your command.".format(families))
 
     # I-ADHoRe
     logging.info("Configuring I-ADHoRe co-linearity search")
     conf, out_path = configure_adhore(table, outdir, **iadhore_opts)
+    ordered_genes_perchrom_allsp, gene_orders = get_chrom_gene(table,outdir)
     table.to_csv(os.path.join(outdir, "gene-table.csv"))
     logging.info("Running I-ADHoRe")
     run_adhore(conf)
 
     # general post-processing
     logging.info("Processing I-ADHoRe output")
-    anchors = get_anchors(out_path)
+    ordered_mp = get_mp_geneorder(gene_orders,out_path,outdir,table)
+    anchors,orig_anchors = get_anchors(out_path)
     multi = get_multi(out_path)
     if anchors is None:
         logging.warning("No anchors found, terminating! Please inspect your input files "
                 "and the I-ADHoRe results in `{}`".format(out_path))
         exit(1)
-
     anchors.to_csv(os.path.join(outdir, "anchors.csv"))
+    #ap_order_permlt = getmltorder(orig_anchors,multi,gene_orders)
     segs = get_segments_profile(multi,keepredun,out_path)
-    segs,table,multi = filter_by_minlength(table,segs,minlen,multi,keepredun,outdir,minseglen)
+    #segmentpair_order = get_segmentpair_order(orig_anchors,segs,table,gene_orders)
+    segs,table,multi,removed_scfa = filter_by_minlength(table,segs,minlen,multi,keepredun,outdir,minseglen)
+    segs_gene_unit, gene_order_dict_allsp = transformunit(segs,ordered_genes_perchrom_allsp,outdir)
+    segs = filter_mingenumber(segs_gene_unit,mingenenum)
+    #if ks_distribution: segs_gene_unit_ks = getsegks(segs_gene_unit,ks_distribution,ordered_genes_perchrom_allsp)
+    df_ks = None
+    if ks_distribution!=None:
+        ksdb_df = pd.read_csv(ks_distribution,header=0,index_col=0,sep='\t')
+        ksdb_df = formatv2(ksdb_df)
+        df_ks = apply_filters(ksdb_df, [("dS", 0., 5.)])
+    dotplotingene(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=anchors,ksdf=df_ks,maxsize=maxsize)
+    #dotplotunitgene(ordered_genes_perchrom_allsp,segs_gene_unit,removed_scfa,outdir,mingenenum,table_orig,ordered_mp,ksdf=df_ks)
     # dotplot
     #logging.info("Generating dot plots")
-    figs = all_dotplots(table, segs, multi, minseglen, anchors=anchors, maxsize=maxsize, minlen=minlen, outdir=outdir, ancestor=ancestor) 
+    figs = all_dotplots(table, segs, multi, minseglen, anchors=anchors, maxsize=maxsize, minlen=minlen, outdir=outdir, ancestor=ancestor, Ks = df_ks) 
     for k, v in figs.items():
         v.savefig(os.path.join(outdir, "{}.dot.svg".format(k)))
         v.savefig(os.path.join(outdir, "{}.dot.pdf".format(k)))
         v.savefig(os.path.join(outdir, "{}.dot.png".format(k)))
+    plt.close()
 
     # anchor Ks distributions
     if ks_distribution:
         ylabel = "Duplications"
         if len(gff_files) == 2:
             ylabel = "RBH orthologs"
         ksd = pd.read_csv(ks_distribution, sep="\t", index_col=0)
@@ -651,46 +686,28 @@
         anchor_ks.to_csv(os.path.join(outdir, "{}.anchors.ks.tsv".format(prefix)),sep='\t')
         a = apply_filters(ksd,       [("dS", 0, 5.)])
         b = apply_filters(anchor_ks, [("dS", 0, 5.)])
         logging.info("Generating anchor Ks distribution")
         fig = default_plot(a, b, title=prefix, bins=50, ylabel=ylabel)
         fig.savefig(os.path.join(outdir, "{}.ksd.svg".format(prefix)))
         fig.savefig(os.path.join(outdir, "{}.ksd.pdf".format(prefix)))
-        # Ks colored dotplot
-        logging.info("Generating Ks colored (median Ks) dotplot")
-        #multiplicons = pd.read_csv(os.path.join(
-        #    outdir, 'iadhore-out', 'multiplicons.txt'), sep='\t')
-        #anchor_points = pd.read_csv(os.path.join(
-        #    outdir, 'iadhore-out', 'anchorpoints.txt'), sep='\t')
-        dotplot_out = os.path.join(outdir, '{}.dotplot.ks.svg'.format(
-                os.path.basename(families)))
-        syntenic_dotplot_ks_colored(
-                multi, anchors, anchor_ks, min_ks=ks_range[0],
-                max_ks=ks_range[1], output_file=dotplot_out,
-                min_length=minlen
-        )
-        #figs2=Ks_dotplots(segs,multiplicons, table, anchor_ks, anchor_points, anchors,min_ks=ks_range[0],max_ks=ks_range[1], maxsize=maxsize, minlen=minlen,outdir = outdir)
-        #for k, v in figs2.items():
-        #    v.savefig(os.path.join(outdir, "{}.ks.dot.svg".format(k)))
-        #    v.savefig(os.path.join(outdir, "{}.ks.dot.pdf".format(k)))
-        #    v.savefig(os.path.join(outdir, "{}.ks.dot.png".format(k)))
     logging.info("Done")    
 
 # MIXTURE MODELING
 @cli.command(context_settings={'help_option_names': ['-h', '--help']})
 @click.argument(
         'ks_distribution', type=click.Path(exists=True), default=None
 )
 @click.option(
         '--filters', '-f', type=int, default=300,
         help="Alignment length",
         show_default=True
 )
 @click.option(
-        '--ks_range', '-r', nargs=2, default=(0.005, 3), show_default=True,
+        '--ks_range', '-r', nargs=2, default=(0, 5), show_default=True,
         type=float,
         help='Ks range to use for modeling'
 )
 @click.option(
         '--bins', '-b', default=50, show_default=True, type=int,
         help="Number of histogram bins."
 )
@@ -811,11 +828,8 @@
     logging.info("Writing component-wise probabilities to file")
     new_df = get_component_probabilities(df, best)
     new_df.round(5).to_csv(os.path.join(
             output_dir, "ks_{}.tsv".format(method)), sep="\t")
 
 
 if __name__ == '__main__':
-    start = timer()
     cli()
-    end = timer()
-    logging.info("Total run time: {}s".format(int(end-start)))
```

### Comparing `wgd-2.0.16/setup.py` & `wgd-2.0.17/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='wgd',
-    version='2.0.16',
+    version='2.0.17',
     packages=['wgd'],
     url='http://github.com/heche-psb/wgd',
     license='GPL',
     author='Hengchi Chen',
     author_email='heche@psb.vib-ugent.be',
     description='wgd',
     long_description=long_description,
```

### Comparing `wgd-2.0.16/test/test_core.py` & `wgd-2.0.17/test/test_core.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.16/wgd/__init__.py` & `wgd-2.0.17/wgd/__init__.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.16/wgd/beast.py` & `wgd-2.0.17/wgd/beast.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.16/wgd/cluster.py` & `wgd-2.0.17/wgd/cluster.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.16/wgd/codeml.py` & `wgd-2.0.17/wgd/codeml.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.16/wgd/core.py` & `wgd-2.0.17/wgd/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1642,16 +1642,31 @@
 
 def hmmer4g2f(outdir,s,nthreads,querys,df,eval,fam2assign):
     hmmerbuild(df,s,outdir,nthreads)
     hmmf = concathmm(outdir,df)
     c_f = reference_hmmscan(df,s,hmmf,outdir,eval)
     outs = hmmerscan(outdir,querys,hmmf,eval,nthreads,skipress=True)
     df = modifydf(df,outs,outdir,fam2assign,use_cf=c_f)
+    fromgene2count(df,outdir,fam2assign)
     getassignfasta(df,s,querys,outdir)
 
+def fromgene2count(df,outdir,fam2assign):
+    fname = os.path.join(outdir,os.path.basename(fam2assign)+'.assigned.genecount')
+    Index = df.index
+    columns = {c:[] for c in df.columns}
+    for indice in df.index:
+        for c in df.columns:
+            if type(df.loc[indice,c]) != str:
+                columns[c].append(0)
+            else:
+                columns[c].append(len(df.loc[indice,c].split(", ")))
+    df_out = pd.DataFrame.from_dict(columns)
+    df_out.index = Index
+    df_out.to_csv(fname,header=True,index=True,sep='\t')
+
 def rmtmp(tmpdir,outdir,querys):
     if tmpdir == None:
         [x.remove_tmp(prompt=False) for x in querys]
         bf = os.path.join(outdir,'rm.sh')
         with open(bf,'w') as f: f.write('rm *.hmm *.dom *.pfam *.pep *.aln *.txt *.tbl Full.hmm*')
         cwd = os.getcwd()
         os.chdir(outdir)
@@ -2089,15 +2104,15 @@
         ratios.append(ratio)
         Multiplicons_matrix.append(Multiplicon_matrix)
         if Ratios.get(ratio) == None: Ratios[ratio] = 1
         else: Ratios[ratio] = Ratios[ratio] + 1
     profile['ratio'] = ratios
     profile[text] = ratios
     profile['level'] = levels
-    return text,Multiplicons_matrix
+    return text,Multiplicons_matrix,profile
 
 def multipliconid2aps(Multiplicons_ids,anchorpoints):
     df = pd.read_csv(anchorpoints, sep="\t", index_col=0, header=0)
     df.set_index("multiplicon")
 
 #def getWGDderivedmultiplicons(profile,WGDingroup,outgroup):
 
@@ -2325,14 +2340,15 @@
     dfs_container = []
     minimum_sp = num_sp*cutoff
     if minimum_sp-int(minimum_sp) != 0: logging.info('Only consider multiplcons containing at least {} species'.format(int(minimum_sp)+1))
     else: logging.info('Only consider multiplcons containing at least {} species'.format(int(minimum_sp)))
     for mid,df in zip(Mids,Aps_per_Mul):
         df = df.drop_duplicates(subset=['gene_x', 'gene_y']).copy()
         level = list(df['level'])[0]
+        # Here I used the 'gene_y' column as grouping proxy because the structure of anchorpoints.txt is that the 'gene_y' column will be fixed as only one segment, while the 'gene_x' column is variable in segments. (For instance there is 10 segments in a multiplicon, the 'gene_y' column will always be the genes from segment 1, while the 'gene_x' column will be genes from the other 9(or 10 if self-collinearity) segments)
         occurs_gl = df.groupby('gene_y')[['gl_x','gene_x']].aggregate(lambda x:list(x))
         for gy in occurs_gl.index: occurs_gl.loc[gy,'gene_x'] = occurs_gl.loc[gy,'gene_x'] + [gy]
         occurs_gl = occurs_gl.rename(columns={"gl_x": "gl_x_y",'gene_x':'gene_xy'})
         for gy in occurs_gl.index: occurs_gl.loc[gy,'gl_x_y'] = occurs_gl.loc[gy,'gl_x_y'] + [gene_sp_gl[gy][1]]
         occurs_gl['num_gl_x_y'] = [len(i) for i in occurs_gl['gl_x_y']]
         occurs_sp = df.groupby('gene_y')['sp_x'].aggregate(lambda x:set(x))
         occurs_sp.name = 'sp_x_y'
@@ -2492,15 +2508,15 @@
     #segs_anchors = le.groupby('segment')['anchors'].aggregate(lambda x: ", ".join([i for i in x])).to_frame()
     #segs_orders = le.groupby('segment')['position'].aggregate(lambda x: ", ".join([str(i) for i in x])).to_frame()
     df = pd.read_csv(segments, sep="\t", index_col=0)
     df['segment'] = df.index
     counted = df.groupby(["multiplicon", "genome"])["segment"].aggregate(lambda x: len(set(x)))
     df = df.loc[:,['multiplicon','segment','genome']]
     profile = counted.unstack(level=-1).fillna(0)
-    text,MP_matrix = Allratio(profile,Ratios)
+    text,MP_matrix,profile = Allratio(profile,Ratios)
     MP_matrix_array = np.transpose(MP_matrix)
     hierarchy_dendrogram(MP_matrix_array,text.split(':'),outdir)
     hierarchy_dendrogram(MP_matrix_array,text.split(':'),outdir,label=False)
     #profile = profile.loc[:,text]
     #minimum_portion = 0.75
     species_ratio = []
     for i in profile.index: species_ratio.append(sum(map(lambda x:int(x)!=0,profile.loc[i,profile.columns[:-3]]))/num_sp)
```

### Comparing `wgd-2.0.16/wgd/mcmctree.py` & `wgd-2.0.17/wgd/mcmctree.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.16/wgd/mix.py` & `wgd-2.0.17/wgd/mix.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.16/wgd/peak.py` & `wgd-2.0.17/wgd/peak.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.16/wgd/utils.py` & `wgd-2.0.17/wgd/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import numpy as np
 import json
 import subprocess
 from progressbar import ProgressBar
 from numpy import mean, std
 from scipy.spatial.distance import cdist
 
-
 def can_i_run_software(software):
     """
     Test if external software is executable
 
     :param software: list or string of executable(s)
     :return: 1 (failure) or 0 (success)
     """
```

### Comparing `wgd-2.0.16/wgd/viz.py` & `wgd-2.0.17/wgd/viz.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import seaborn as sns
 import pandas as pd
 import os
 from matplotlib.patches import Rectangle
 from matplotlib.path import Path
 import matplotlib.patches as patches
 from matplotlib.pyplot import cm
+from matplotlib.cm import ScalarMappable
 from scipy import stats,interpolate,signal
 from io import StringIO
 from Bio import Phylo
 from sklearn import mixture
 
 def node_averages(df):
     # note that this returns a df with fewer rows, i.e. one for every
@@ -1590,20 +1591,526 @@
     ax.spines['bottom'].set_visible(False)
     fig.tight_layout()
     fig.savefig(fname)
     fig.savefig(fnamep)
     fig.savefig(fnames)
     plt.close()
 
+def judgeoverlap(startx,lastx,starty,lasty,start_lastxy):
+    Assumeoverlap = False
+    for i,j,k in start_lastxy:
+        if i[0] < startx and i[1] < lastx and j[0] < starty and j[1] < lasty:
+            Assumeoverlap = True
+            break
+    return Assumeoverlap
+
+def determineoverlap(plotted_xy,xy):
+    x,y = xy[0],xy[1]
+    overlap = False
+    for occuredx,occuredy in plotted_xy:
+        occuredsx,occuredlx,occuredsy,occuredly = occuredx[0],occuredx[1],occuredy[0],occuredy[1]
+        if occuredsx <= x[0] and x[1] <= occuredlx and occuredsy <= y[0] and y[1] <= occuredly:
+            overlap = True
+            logging.info("Skip fully overlapped segment pair ({0},{1}) ({2},{3})".format(x[0],y[0],x[1],y[1]))
+            break
+    return overlap
+
+def mergeoverlapped(plotted_xy,xy):
+    x,y = xy[0],xy[1]
+    for occuredx,occuredy in plotted_xy:
+        occuredsx,occuredlx,occuredsy,occuredly = occuredx[0],occuredx[1],occuredy[0],occuredy[1]
+        if x[0] > occuredlx or occuredsx > x[1]:
+            continue
+        if y[0] > occuredly or occuredsy > y[1]:
+            continue
+        x = [min([occuredsx,occuredlx,x[0],x[1]]),max([occuredsx,occuredlx,x[0],x[1]])]
+        y = [min([occuredsy,occuredly,y[0],y[1]]),max([occuredsy,occuredly,y[0],y[1]])]
+    return x,y
+
+def mergedxy(i_infox,i_infoy,i_orien,i_color,j_infox,j_infoy,j_orien,j_color):
+    if i_infox[0] > j_infox[1] or i_infox[1] < j_infox[0]:
+        return i_infox,i_infoy,i_orien,i_color,j_infox,j_infoy,j_orien,j_color
+    if i_infoy[0] > j_infoy[1] or i_infoy[1] < j_infoy[0]:
+        return i_infox,i_infoy,i_orien,i_color,j_infox,j_infoy,j_orien,j_color
+    sizei = (i_infox[1]-i_infox[0]) * (i_infoy[1]-i_infoy[0])
+    sizej = (j_infox[1]-j_infox[0]) * (j_infoy[1]-j_infoy[0])
+    infox = [min([i_infox[0],i_infox[1],j_infox[0],j_infox[1]]),max([i_infox[0],i_infox[1],j_infox[0],j_infox[1]])]
+    infoy = [min([i_infoy[0],i_infoy[1],j_infoy[0],j_infoy[1]]),max([i_infoy[0],i_infoy[1],j_infoy[0],j_infoy[1]])]
+    if sizei > sizej:
+        return infox,infoy,i_orien,i_color,None,None,None,None
+    else:
+        return infox,infoy,j_orien,j_color,None,None,None,None
+
+def loopmerge(working):
+    merged_startxy = []
+    for i in range(len(working)):
+        for j in range(i+1,len(working)):
+            i_infox,i_infoy,i_orien = working[i]
+            j_infox,j_infoy,j_orien = working[j]
+            result = mergedxy(i_infox,i_infoy,i_orien,j_infox,j_infoy,j_orien)
+            if result[3] == None:
+                merged_startxy.append((result[0],result[1],result[2]))
+            else:
+                if (result[0],result[1],result[2]) not in merged_startxy:
+                    merged_startxy.append((result[0],result[1],result[2]))
+                if (result[3],result[4],result[5]) not in merged_startxy:
+                    merged_startxy.append((result[3],result[4],result[5]))
+    if working == merged_startxy:
+        return merged_startxy
+    else:
+        return loopmerge(merged_startxy)
+
+def singlemerge(working):
+    merged_startxy = []
+    for i in range(len(working)):
+        for j in range(i+1,len(working)):
+            i_infox,i_infoy,i_orien,i_color = working[i]
+            j_infox,j_infoy,j_orien,j_color = working[j]
+            result = mergedxy(i_infox,i_infoy,i_orien,i_color,j_infox,j_infoy,j_orien,j_color)
+            if result[4] == None:
+                merged_startxy.append((result[0],result[1],result[2],result[3]))
+            else:
+                if (result[0],result[1],result[2],result[3]) not in merged_startxy:
+                    merged_startxy.append((result[0],result[1],result[2],result[3]))
+                if (result[4],result[5],result[6],result[7]) not in merged_startxy:
+                    merged_startxy.append((result[4],result[5],result[6],result[7]))
+    return merged_startxy
+
+def filteroverlapped(segs_filter,xtick_addable_dict,ytick_addable_dict,spx_given,spy_given):
+    seg_pairs = {}
+    for mlt, df in list(segs_filter.groupby('multiplicon')):
+        for i,indicex in enumerate(df.index):
+            for indicey in df.index[i+1:]:
+                spx,spy = df.loc[indicex,'genome'],df.loc[indicey,'genome']
+                list_x,list_y = df.loc[indicex,'list'],df.loc[indicey,'list']
+                pair_id = "__".join(sorted([spx,spy])) + "__" + "__".join(sorted([list_x,list_y]))
+                if spx != spx_given and spx != spy_given:
+                    continue
+                if spy != spx_given and spy != spy_given:
+                    continue
+                if spx_given == spy_given:
+                    infox,infoy = [df.loc[indicex,'first_coordinate']+xtick_addable_dict[list_x],df.loc[indicex,'last_coordinate']+xtick_addable_dict[list_x]], [df.loc[indicey,'first_coordinate']+xtick_addable_dict[list_y],df.loc[indicey,'last_coordinate']+xtick_addable_dict[list_y]]
+                else:
+                    if spx==spx_given:
+                        if spy == spy_given:
+                            infox,infoy = [df.loc[indicex,'first_coordinate']+xtick_addable_dict["{}_".format(spx)+list_x],df.loc[indicex,'last_coordinate']+xtick_addable_dict["{}_".format(spx)+list_x]], [df.loc[indicey,'first_coordinate']+ytick_addable_dict["{}_".format(spy)+list_y],df.loc[indicey,'last_coordinate']+ytick_addable_dict["{}_".format(spy)+list_y]]
+                        else:
+                            infox,infoy = [df.loc[indicex,'first_coordinate']+xtick_addable_dict["{}_".format(spx)+list_x],df.loc[indicex,'last_coordinate']+xtick_addable_dict["{}_".format(spx)+list_x]], [df.loc[indicey,'first_coordinate']+xtick_addable_dict["{}_".format(spy)+list_y],df.loc[indicey,'last_coordinate']+xtick_addable_dict["{}_".format(spy)+list_y]]
+                    else:
+                        if spy == spy_given:
+                            infox,infoy = [df.loc[indicex,'first_coordinate']+ytick_addable_dict["{}_".format(spx)+list_x],df.loc[indicex,'last_coordinate']+ytick_addable_dict["{}_".format(spx)+list_x]], [df.loc[indicey,'first_coordinate']+ytick_addable_dict["{}_".format(spy)+list_y],df.loc[indicey,'last_coordinate']+ytick_addable_dict["{}_".format(spy)+list_y]]
+                        else:
+                            infox,infoy = [df.loc[indicex,'first_coordinate']+ytick_addable_dict["{}_".format(spx)+list_x],df.loc[indicex,'last_coordinate']+ytick_addable_dict["{}_".format(spx)+list_x]], [df.loc[indicey,'first_coordinate']+xtick_addable_dict["{}_".format(spy)+list_y],df.loc[indicey,'last_coordinate']+xtick_addable_dict["{}_".format(spy)+list_y]]
+                if seg_pairs.get(pair_id) == None:
+                    seg_pairs[pair_id] = [(infox,infoy,(indicex,indicey))]
+                    #if spx_given == spy_given:
+                    #    seg_pairs[pair_id] = [(infoy,infox,(indicex,indicey))]
+                else:
+                    seg_pairs[pair_id].append((infox,infoy,(indicex,indicey)))
+                    #if spx_given == spy_given:
+                    #    seg_pairs[pair_id].append((infoy,infox,(indicex,indicey)))
+    indice_torm = []
+    indice_tomerge = {}
+    for key,value in seg_pairs.items():
+        if len(value) == 1:
+            continue
+        for i in range(len(value)):
+            for j in range(len(value)):
+                if i == j:
+                    continue
+                i_info,j_info = value[i],value[j]
+                if i_info[0][1] >= j_info[0][1] and i_info[0][0] <= j_info[0][0] and i_info[1][1] >= j_info[1][1] and i_info[1][0] <= j_info[1][0]:
+                    indice_torm.append(j_info[2])
+                if j_info[0][1] >= i_info[0][1] and j_info[0][0] <= i_info[0][0] and j_info[1][1] >= i_info[1][1] and j_info[1][0] <= i_info[1][0]:
+                    indice_torm.append(i_info[2])
+                #if i_info[0][1] >= j_info[0][0] and i_info[0][0] <= j_info[0][1]:
+                    # x label overlap
+                #    if i_info[1][1] >= j_info[1][0] and i_info[1][0] <= j_info[1][1]:
+                        # y label overlap
+                #        if i_info[0][1] >= j_info[0][1]:
+                            # only consider the overlap ratio of x
+                #            overlap_ratio_i = (j_info[0][1]-i_info[0][0])/(i_info[0][1]-i_info[0][0])
+                #            overlap_ratio_j = (j_info[0][1]-i_info[0][0])/(j_info[0][1]-j_info[0][0])
+                #        else:
+                #            overlap_ratio_i = (i_info[0][1]-j_info[0][0])/(i_info[0][1]-i_info[0][0])
+                #            overlap_ratio_j = (i_info[0][1]-j_info[0][0])/(j_info[0][1]-j_info[0][0])
+                #        if overlap_ratio_i <= 0.3 and overlap_ratio_j <= 0.3:
+                #            continue
+                #        newx = [min([i_info[0][1],j_info[0][0],i_info[0][0],j_info[0][1]]),max([i_info[0][1],j_info[0][0],i_info[0][0],j_info[0][1]])]
+                #        newy = [min([i_info[1][1],j_info[1][0],i_info[1][0],j_info[1][1]]),max([i_info[1][1],j_info[1][0],i_info[1][0],j_info[1][1]])]
+                #        if overlap_ratio_i > overlap_ratio_j:
+                #            indice_torm.append(i_info[2])
+                #            indice_tomerge[j_info[2]] = (newx,newy)
+                #        else:
+                #            indice_torm.append(j_info[2])
+                #            indice_tomerge[i_info[2]] = (newx,newy)
+                #if spx_given == spy_given:
+                #    if i_info[0][1] >= j_info[1][0] and i_info[0][0] <= j_info[1][1]:
+                        # x label overlap
+                #        if i_info[1][1] >= j_info[0][0] and i_info[1][0] <= j_info[0][1]:
+                            # y label overlap
+                #            if i_info[0][1] >= j_info[1][1]:
+                                # only consider the overlap ratio of x
+                #                overlap_ratio_i = (j_info[1][1]-i_info[0][0])/(i_info[0][1]-i_info[0][0])
+                #                overlap_ratio_j = (j_info[1][1]-i_info[0][0])/(j_info[1][1]-j_info[1][0])
+                #            else:
+                #                overlap_ratio_i = (i_info[0][1]-j_info[1][0])/(i_info[0][1]-i_info[0][0])
+                #                overlap_ratio_j = (i_info[0][1]-j_info[1][0])/(j_info[1][1]-j_info[1][0])
+                #            if overlap_ratio_i <= 0.01 and overlap_ratio_j <= 0.01:
+                #                continue
+                #            newx = [min([i_info[0][1],j_info[1][0],i_info[0][0],j_info[1][1]]),max([i_info[0][1],j_info[1][0],i_info[0][0],j_info[1][1]])]
+                #            newy = [min([i_info[1][1],j_info[0][0],i_info[1][0],j_info[0][1]]),max([i_info[1][1],j_info[0][0],i_info[1][0],j_info[0][1]])]
+                #            if overlap_ratio_i > overlap_ratio_j:
+                #                indice_torm.append(i_info[2])
+                #                indice_tomerge[j_info[2]] = (newx,newy)
+                #            else:
+                #                indice_torm.append(j_info[2])
+                #                indice_tomerge[i_info[2]] = (newx,newy)
+    return indice_torm, indice_tomerge
+
+def getksage(MP_unit,ksdf):
+    pairs = ["__".join(sorted([x,y])) for x,y in zip(MP_unit['gene_x'],MP_unit['gene_y'])]
+    ksdf = ksdf.dropna(subset=['dS'])
+    Ks_dict = {pair:ks for pair,ks in zip(ksdf.index,ksdf['dS'])}
+    Ks = []
+    for p in pairs:
+        if Ks_dict.get(p,False):
+            Ks.append(Ks_dict[p])
+    if len(Ks) == 0:
+        return None
+    else:
+        return np.median(Ks)
+
+def getpairks(pair,ksdf):
+    Ks_dict = {pair:ks for pair,ks in zip(ksdf.index,ksdf['dS'])}
+    return Ks_dict.get(pair,None)
+
+def plotdp_ig(ax,dfx,dfy,spx,spy,table,gene_orders,anchor=None,ksdf=None,maxsize=200,showks=False):
+    dfx,dfy = dfx.set_index('Coordinates'),dfy.set_index('Coordinates')
+    leng_info_x,leng_info_y = {},{}
+    gene_list = {gene:li for gene,li in zip(table.index,table['scaffold'])}
+    if spx != spy:
+        gene_list = {spx:{},spy:{}}
+        for gene,sp,li in zip(table.index,table['species'],table['scaffold']):
+            if sp != spx and sp != spy:
+                continue
+            gene_list[sp][gene] = li
+    for scfa in dfx.columns: leng_info_x[scfa] = len(dfx[scfa].dropna())
+    for scfa in dfy.columns: leng_info_y[scfa] = len(dfy[scfa].dropna())
+    sorted_labels_x = [i[0] for i in sorted(leng_info_x.items(),key=lambda x: x[1],reverse=True)]
+    sorted_leng_x = [i[1] for i in sorted(leng_info_x.items(),key=lambda x: x[1],reverse=True)]
+    sorted_labels_y = [i[0] for i in sorted(leng_info_y.items(),key=lambda x: x[1],reverse=True)]
+    sorted_leng_y = [i[1] for i in sorted(leng_info_y.items(),key=lambda x: x[1],reverse=True)]
+    xtick,ytick = list(np.cumsum(sorted_leng_x)),list(np.cumsum(sorted_leng_y))
+    xtick_addable, ytick_addable = [0]+xtick[:-1], [0]+ytick[:-1]
+    xtick_addable_dict = {scfa:scfastart for scfa,scfastart in zip(sorted_labels_x,xtick_addable)}
+    ytick_addable_dict = {scfa:scfastart for scfa,scfastart in zip(sorted_labels_y,ytick_addable)}
+    xs,ys,co,xs_ap,ys_ap,co_ap,Ks_ages = [],[],[],[],[],[],[]
+    if showks: Ks_dict = {pair:ks for pair,ks in zip(ksdf.index,ksdf['dS'])}
+    for fam, df_tmp in list(table.groupby('family')):
+        if len(df_tmp[df_tmp['species']==spx]) >= maxsize or len(df_tmp[df_tmp['species']==spy]) >= maxsize:
+            continue
+        if len(df_tmp[df_tmp['species']==spx]) == 0 or len(df_tmp[df_tmp['species']==spy]) == 0:
+            continue
+        gx,gy = list(df_tmp[df_tmp['species']==spx].index),list(df_tmp[df_tmp['species']==spy].index)
+        if spx != spy:
+            gx_coori = [gene_orders[g] + xtick_addable_dict[gene_list[spx][g]] for g in gx]
+            gy_coori = [gene_orders[g] + ytick_addable_dict[gene_list[spy][g]] for g in gy]
+        else:
+            gx_coori = [gene_orders[g] + xtick_addable_dict[gene_list[g]] for g in gx]
+            gy_coori = [gene_orders[g] + ytick_addable_dict[gene_list[g]] for g in gy]
+        for (ggx,ggy), (x, y) in zip(itertools.product(gx,gy),itertools.product(gx_coori,gy_coori)):
+            if x == y:
+                continue
+            if showks:
+                if not (ksdf is None):
+                    ks = Ks_dict.get("__".join(sorted([ggx,ggy])),None)
+                    if ks is None:
+                        continue
+                    Ks_ages.append(ks)
+            xs.append(x)
+            ys.append(y)
+            if showks: co.append(ks)
+            if not (anchor is None):
+                if "__".join(sorted([ggx,ggy])) in anchor.index:
+                    xs_ap.append(x)
+                    ys_ap.append(y)
+                    if showks: co_ap.append(ks)
+    if showks:
+        if not (ksdf is None):
+            norm = matplotlib.colors.Normalize(vmin=np.min(Ks_ages), vmax=np.max(Ks_ages))
+            c_m = matplotlib.cm.rainbow
+            s_m = ScalarMappable(cmap=c_m, norm=norm)
+            s_m.set_array([])
+    if not showks:
+        ax.scatter(xs, ys, s=0.4, color = 'k', alpha=0.01)
+        ax.scatter(xs_ap, ys_ap, s=0.4, color = 'r', alpha=1)
+    else:
+        ax.scatter(xs, ys, s=0.4, color=[c_m(norm(c)) for c in co], alpha=0.01)
+        ax.scatter(xs_ap, ys_ap, s=0.4, color=[c_m(norm(c)) for c in co_ap], alpha=1)
+    #ax.scatter(xs_ap, ys_ap, s=0.4, alpha=0.5)
+    xlim,ylim = xtick[-1],ytick[-1]
+    ax.set_xlim(0, xlim)
+    ax.set_ylim(0, ylim)
+    ax.vlines(xtick, ymin=0, ymax=ylim, alpha=0.8, color="k")
+    ax.hlines(ytick, xmin=0, xmax=xlim, alpha=0.8, color="k")
+    ax.set_xlabel("{}".format(spx))
+    ax.set_ylabel("{}".format(spy))
+    ax.set_xticks(xtick)
+    ax.set_xticklabels(sorted_labels_x,rotation=45)
+    ax.set_yticks(ytick)
+    ax.set_yticklabels(sorted_labels_y,rotation=45)
+    ax2 = ax.twinx()
+    ax3 = ax.twiny()
+    ax2.set_yticks(ytick)
+    ax2.set_ylabel("{} (genes)".format(spy))
+    ax2.tick_params(axis='y', labelrotation=45)
+    ax3.set_xticks(xtick)
+    ax3.set_xlabel("{} (genes)".format(spx))
+    ax3.tick_params(axis='x', labelrotation=45)
+    if showks:
+        if not (ksdf is None): plt.colorbar(s_m, label="$K_\mathrm{S}$", orientation="vertical",fraction=0.03,pad=0.1)
+    return ax
+
+def plotbb_dpug(ax,dfx,dfy,spx,spy,segs,mingenenum,mp,gene_genome,ksdf=None):
+    dfx,dfy = dfx.set_index('Coordinates'),dfy.set_index('Coordinates')
+    leng_info_x,leng_info_y = {},{}
+    for scfa in dfx.columns: leng_info_x[scfa] = len(dfx[scfa].dropna())
+    for scfa in dfy.columns: leng_info_y[scfa] = len(dfy[scfa].dropna())
+    sorted_labels_x = [i[0] for i in sorted(leng_info_x.items(),key=lambda x: x[1],reverse=True)]
+    sorted_leng_x = [i[1] for i in sorted(leng_info_x.items(),key=lambda x: x[1],reverse=True)]
+    sorted_labels_y = [i[0] for i in sorted(leng_info_y.items(),key=lambda x: x[1],reverse=True)]
+    sorted_leng_y = [i[1] for i in sorted(leng_info_y.items(),key=lambda x: x[1],reverse=True)]
+    xtick,ytick = list(np.cumsum(sorted_leng_x)),list(np.cumsum(sorted_leng_y))
+    xtick_addable, ytick_addable = [0]+xtick[:-1], [0]+ytick[:-1]
+    if spx == spy:
+        xtick_addable_dict = {scfa:scfastart for scfa,scfastart in zip(sorted_labels_x,xtick_addable)}
+        ytick_addable_dict = {scfa:scfastart for scfa,scfastart in zip(sorted_labels_y,ytick_addable)}
+    else:
+        xtick_addable_dict = {"{}_".format(spx)+scfa:scfastart for scfa,scfastart in zip(sorted_labels_x,xtick_addable)}
+        ytick_addable_dict = {"{}_".format(spy)+scfa:scfastart for scfa,scfastart in zip(sorted_labels_y,ytick_addable)}
+    xlim,ylim = xtick[-1],ytick[-1]
+    ax.set_xlim(0, xlim)
+    ax.set_ylim(0, ylim)
+    tmp = segs.groupby('multiplicon')['genome'].agg(lambda x:set(x))
+    good_mlt = []
+    for mlt,genome in zip(tmp.index,tmp):
+        if spx in genome and spy in genome: good_mlt.append(mlt)
+    segs_filter = segs[segs['multiplicon'].isin(good_mlt)].copy()
+    segs_filter.loc[:,'length'] = [l-s for s,l in zip(segs_filter['first_coordinate'],segs_filter['last_coordinate'])]
+    indice_notplot,indice_tomerge = filteroverlapped(segs_filter,xtick_addable_dict,ytick_addable_dict,spx,spy)
+    MP = mp.copy()
+    if spx != spy:
+        segs_filter.loc[:,'list'] = ["{}_{}".format(g,l) for g,l in zip(segs_filter['genome'],segs_filter['list'])]
+        MP['genome_x'],MP['genome_y'] = MP['gene_x'].apply(lambda x:gene_genome[x]),MP['gene_y'].apply(lambda x:gene_genome[x])
+        MP.loc[:,'scaffold_x'] = ["{}_{}".format(g,l) for g,l in zip(MP['genome_x'],MP['scaffold_x'])]
+        MP.loc[:,'scaffold_y'] = ["{}_{}".format(g,l) for g,l in zip(MP['genome_y'],MP['scaffold_y'])]
+    Num_segments_plotted = 0
+    start_lastxy = []
+    Ks_ages = []
+    for mlt, df_tmp in sorted(list(segs_filter.groupby('multiplicon')),key=lambda x:max(x[1]['length'])):
+        MP_tmp = MP[MP['multiplicon']==mlt]
+        df_tmp = df_tmp[[any([i,j]) for i,j in zip(df_tmp['genome']==spx,df_tmp['genome']==spy)]]
+        indice = 0
+        if spx != spy:
+            df_tmp.loc[:,'sp_order'] = [[spx,spy].index(g) for g in df_tmp['genome']]
+            df_tmp = df_tmp.sort_values(by=['sp_order'])
+        logging.debug("Checking multiplicon {}".format(mlt))
+        for i in df_tmp.index:
+            indice = indice + 1
+            if abs(df_tmp.loc[i,'last_coordinate'] - df_tmp.loc[i,'first_coordinate']) + 1 < mingenenum:
+                continue
+            for j in df_tmp.index[indice:]:
+                if abs(df_tmp.loc[j,'last_coordinate'] - df_tmp.loc[j,'first_coordinate']) + 1 < mingenenum:
+                    continue
+                if spx != spy and df_tmp.loc[i,'genome'] == df_tmp.loc[j,'genome']:
+                    continue
+                if (i,j) in indice_notplot:
+                    logging.debug("Skip due to overlap")
+                    continue
+                for unit,MP_unit in list(MP_tmp.groupby('unit')):
+                    scaf_xy = [list(MP_unit['scaffold_x'])[0],list(MP_unit['scaffold_y'])[0]]
+                    if df_tmp.loc[i,'list'] in scaf_xy and df_tmp.loc[j,'list'] in scaf_xy:
+                        if list(MP_unit['orientation'])[0] == "x":
+                            continue
+                        if df_tmp.loc[i,'list'] == list(MP_unit['scaffold_x'])[0]:
+                            minimum,maximum = df_tmp.loc[i,'first_coordinate'],df_tmp.loc[i,'last_coordinate']
+                            if sum([minimum<cx<maximum for cx in MP_unit['coordinate_x']]) >= 2:
+                                minimum,maximum = df_tmp.loc[j,'first_coordinate'],df_tmp.loc[j,'last_coordinate']
+                                if sum([minimum<cx<maximum for cx in MP_unit['coordinate_y']]) >= 2:
+                                    ksage = getksage(MP_unit,ksdf) if type(ksdf) == pd.core.frame.DataFrame else None
+                                    color = ksage if ksage != None else None
+                                    if ksage != None: Ks_ages.append(ksage)
+                                    if (i,j) in indice_tomerge:
+                                        logging.debug("plot merged segment pair")
+                                        newx,newy = indice_tomerge[(i,j)]
+                                        startx,lastx = newx[0], newx[1]
+                                        starty,lasty = newy[0], newy[1]
+                                    else:
+                                        startx,lastx = df_tmp.loc[i,'first_coordinate'] + xtick_addable_dict[df_tmp.loc[i,'list']],df_tmp.loc[i,'last_coordinate'] + xtick_addable_dict[df_tmp.loc[i,'list']]
+                                        starty,lasty = df_tmp.loc[j,'first_coordinate'] + ytick_addable_dict[df_tmp.loc[j,'list']],df_tmp.loc[j,'last_coordinate'] + ytick_addable_dict[df_tmp.loc[j,'list']]
+                                    #if judgeoverlap(startx,lastx,starty,lasty,start_lastxy):
+                                    #    continue
+                                    start_lastxy.append(([startx,lastx],[starty,lasty],list(MP_unit['orientation'])[0],color))
+                                    lengx = abs(df_tmp.loc[i,'last_coordinate'] - df_tmp.loc[i,'first_coordinate']) + 1
+                                    lengy = abs(df_tmp.loc[j,'last_coordinate'] - df_tmp.loc[j,'first_coordinate']) + 1
+                                    logging.debug("Add coor ({0},{1}) ({2},{3}) {4} of scaffold ({5},{6}) segment ({7},{8}) length ({9},{10})".format(startx,starty,lastx,lasty,list(MP_unit['orientation'])[0],df_tmp.loc[i,'list'],df_tmp.loc[j,'list'],df_tmp.loc[i,'segment'],df_tmp.loc[j,'segment'],lengx,lengy))
+                        else:
+                            minimum,maximum = df_tmp.loc[i,'first_coordinate'],df_tmp.loc[i,'last_coordinate']
+                            if sum([minimum<cx<maximum for cx in MP_unit['coordinate_y']]) >= 2:
+                                minimum,maximum = df_tmp.loc[j,'first_coordinate'],df_tmp.loc[j,'last_coordinate']
+                                if sum([minimum<cx<maximum for cx in MP_unit['coordinate_x']]) >= 2:
+                                    ksage = getksage(MP_unit,ksdf) if type(ksdf) == pd.core.frame.DataFrame else None
+                                    color=ksage if ksage != None else None
+                                    if ksage != None: Ks_ages.append(ksage)
+                                    if (i,j) in indice_tomerge:
+                                        logging.debug("plot merged segment pair")
+                                        newx,newy = indice_tomerge[(i,j)]
+                                        startx,lastx = newx[0], newx[1]
+                                        starty,lasty = newy[0], newy[1]
+                                    else:
+                                        startx,lastx = df_tmp.loc[i,'first_coordinate'] + xtick_addable_dict[df_tmp.loc[i,'list']],df_tmp.loc[i,'last_coordinate'] + xtick_addable_dict[df_tmp.loc[i,'list']]
+                                        starty,lasty = df_tmp.loc[j,'first_coordinate'] + ytick_addable_dict[df_tmp.loc[j,'list']],df_tmp.loc[j,'last_coordinate'] + ytick_addable_dict[df_tmp.loc[j,'list']]
+                                    start_lastxy.append(([startx,lastx],[starty,lasty],list(MP_unit['orientation'])[0],color))
+                                    lengx = abs(df_tmp.loc[j,'last_coordinate'] - df_tmp.loc[j,'first_coordinate']) + 1
+                                    lengy = abs(df_tmp.loc[i,'last_coordinate'] - df_tmp.loc[i,'first_coordinate']) + 1
+                                    logging.debug("Add coor ({0},{1}) ({2},{3}) {4} of scaffold ({5},{6}) segment ({7},{8}) length ({9},{10})".format(startx,starty,lastx,lasty,list(MP_unit['orientation'])[0],df_tmp.loc[j,'list'],df_tmp.loc[i,'list'],df_tmp.loc[j,'segment'],df_tmp.loc[i,'segment'],lengx,lengy))
+    plotted_xy = []
+    #working = sorted(start_lastxy,key=lambda x:max([abs(x[0][0]-x[0][1]),abs(x[1][0]-x[1][1])]),reverse=True)
+    #working_nooverlapped = []
+    #for infox,infoy,orien,color in working:
+    #    if determineoverlap(plotted_xy,(infox,infoy)):
+    #        continue
+    #    plotted_xy.append((infox,infoy))
+    #    working_nooverlapped.append((infox,infoy,orien,color))
+    #for i in range(10):
+    #    working_nooverlapped = singlemerge(working_nooverlapped)
+    #plotted_xy = []
+    #final_merged = loopmerge(working)
+    #for infox,infoy,orien in sorted(final_merged,key=lambda x:max([abs(x[0][0]-x[0][1]),abs(x[1][0]-x[1][1])]),reverse=True):
+    #sm = ScalarMappable(cmap='seismic', norm=plt.Normalize(vmin=min(Ks_ages), vmax=max(Ks_ages)))
+    if type(ksdf) == pd.core.frame.DataFrame:
+        norm = matplotlib.colors.Normalize(vmin=np.min(Ks_ages), vmax=np.max(Ks_ages))
+        c_m = matplotlib.cm.rainbow
+        s_m = ScalarMappable(cmap=c_m, norm=norm)
+        s_m.set_array([])
+    #for infox,infoy,orien,color in working_nooverlapped:
+    start_xy_sorted = sorted(start_lastxy,key=lambda x:max([abs(x[0][0]-x[0][1]),abs(x[1][0]-x[1][1])]),reverse=False)
+    for i in range(len(start_xy_sorted)):
+        line1_x, line1_y, line1_orien, line1_color = start_xy_sorted[i]
+        if line1_color == None and type(ksdf) == pd.core.frame.DataFrame:
+            continue
+        remove_line = False
+        for j in range(len(start_xy_sorted)):
+            if j != i:
+                line2_x, line2_y, line2_orien, line2_color = start_xy_sorted[j]
+                if line2_color == None and type(ksdf) == pd.core.frame.DataFrame:
+                    continue
+                if max(line2_x) >= max(line1_x) and min(line1_x) >= min(line2_x) and max(line2_y) >= max(line1_y) and min(line1_y) >= min(line2_y):
+                    remove_line = True
+                    break
+                if max(line2_y) >= max(line1_x) and min(line1_x) >= min(line2_y) and max(line2_x) >= max(line1_y) and min(line1_y) >= min(line2_x) and spx == spy:
+                    remove_line = True
+                    break
+        if not remove_line:
+            Num_segments_plotted = Num_segments_plotted + 1
+            if line1_orien == '-': line1_y.reverse()
+            if type(ksdf) != pd.core.frame.DataFrame: c = 'b'
+            else: c = c_m(norm(line1_color))
+            ax.plot(line1_x, line1_y, alpha=1, linewidth=0.8, color = c)
+            logging.debug("plot segment pair ({0},{1}) ({2},{3})".format(line1_x[0],line1_x[1],line1_y[0],line1_y[1]))
+            if spx == spy: ax.plot(line1_y, line1_x, alpha=1, linewidth=0.8, color = c)
+            logging.debug("plot segment pair ({0},{1}) ({2},{3})".format(line1_y[0],line1_y[1],line1_x[0],line1_x[1]))
+    #for infox,infoy,orien,color in sorted(start_lastxy,key=lambda x:max([abs(x[0][0]-x[0][1]),abs(x[1][0]-x[1][1])]),reverse=True):
+    #    if color == None:
+    #        logging.info("Skip segment pair ({0},{1}) ({2},{3}) {4} due to no Ks data".format(infox[0],infoy[0],infox[1],infoy[1],orien))
+    #        continue
+    #    if determineoverlap(plotted_xy,(infox,infoy)):
+    #        continue
+    #    Num_segments_plotted = Num_segments_plotted + 1
+    #    if orien == '-': infoy.reverse()
+    #    plotted_xy.append((infox,infoy))
+    #    ax.plot(infox, infoy, alpha=0.9, linewidth=0.8,color = c_m(norm(color)))
+    #    if spx == spy: ax.plot(infoy, infox, alpha=0.9, linewidth=0.8,color = c_m(norm(color)))
+    if type(ksdf) == pd.core.frame.DataFrame: plt.colorbar(s_m, label="$K_\mathrm{S}$", orientation="vertical",fraction=0.03,pad=0.03)
+    logging.info("In total {} segment pairs were plotted".format(Num_segments_plotted))
+    ax.vlines(xtick, ymin=0, ymax=ylim, alpha=0.8, color="k")
+    ax.hlines(ytick, xmin=0, xmax=xlim, alpha=0.8, color="k")
+    ax.set_xlabel("{}".format(spx))
+    ax.set_ylabel("{}".format(spy))
+    ax.set_xticks(xtick)
+    ax.set_xticklabels(sorted_labels_x,rotation=45)
+    ax.set_yticks(ytick)
+    ax.set_yticklabels(sorted_labels_y,rotation=45)
+    return ax
+
+def plotbackbone_dpug(spx,spy,ordered_genes_perchrom_allsp,removed_scfa,segs,mingenenum,MP,gene_genome,ksdf=None):
+    fig, ax = plt.subplots(1, 1, figsize=(10,10))
+    dfx = ordered_genes_perchrom_allsp[spx].copy().drop(removed_scfa[spx],axis=1)
+    dfy = ordered_genes_perchrom_allsp[spy].copy().drop(removed_scfa[spy],axis=1)
+    ax = plotbb_dpug(ax,dfx,dfy,spx,spy,segs,mingenenum,MP,gene_genome,ksdf=ksdf)
+    fig.tight_layout()
+    return fig, ax
+
+def dotplotunitgene(ordered_genes_perchrom_allsp,segs,removed_scfa,outdir,mingenenum,table,MP,ksdf=None):
+    sp_list = list(ordered_genes_perchrom_allsp.keys())
+    gene_list = {gene:li for gene,li in zip(table.index,table['scaffold'])}
+    gene_genome = {gene:sp for gene,sp in zip(table.index,table['species'])}
+    figs = {}
+    #orig_anchors['list_y'] = orig_anchors['gene_y'].apply(lambda x:gene_list[x])
+    #orig_anchors['list_x'] = orig_anchors['gene_x'].apply(lambda x:gene_list[x])
+    for i in range(len(sp_list)):
+        for j in range(i,len(sp_list)):
+            spx,spy = sp_list[i],sp_list[j]
+            fig, ax = plotbackbone_dpug(spx,spy,ordered_genes_perchrom_allsp,removed_scfa,segs,mingenenum,MP,gene_genome,ksdf=ksdf)
+            figs[spx + "-vs-" + spy] = fig
+    for prefix, fig in figs.items():
+        fname = os.path.join(outdir, "{}.line_unit_gene.svg".format(prefix))
+        fig.savefig(fname)
+
+def plotdotplotingene(spx,spy,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=None,ksdf=None,maxsize=200,showks=False):
+    fig, ax = plt.subplots(1, 1, figsize=(10,10))
+    dfx = ordered_genes_perchrom_allsp[spx].copy().drop(removed_scfa[spx],axis=1)
+    dfy = ordered_genes_perchrom_allsp[spy].copy().drop(removed_scfa[spy],axis=1)
+    ax = plotdp_ig(ax,dfx,dfy,spx,spy,table,gene_orders,anchor=anchor,ksdf=ksdf,maxsize=maxsize,showks=showks)
+    fig.tight_layout()
+    return fig, ax
+
+def dotplotingene(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=None,ksdf=None,maxsize=200):
+    sp_list = list(ordered_genes_perchrom_allsp.keys())
+    gene_list = {gene:li for gene,li in zip(table.index,table['scaffold'])}
+    gene_genome = {gene:sp for gene,sp in zip(table.index,table['species'])}
+    figs = {}
+    logging.info("Making dotplot (in unit of genes)")
+    for i in range(len(sp_list)):
+        for j in range(i,len(sp_list)):
+            spx,spy = sp_list[i],sp_list[j]
+            logging.info("{0} vs. {1}".format(spx,spy))
+            fig, ax = plotdotplotingene(spx,spy,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=anchor,ksdf=ksdf)
+            figs[spx + "-vs-" + spy] = fig
+            if not (ksdf is None):
+                figks, ax = plotdotplotingene(spx,spy,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=anchor,ksdf=ksdf,showks=True)
+                figs[spx + "-vs-" + spy + "_Ks"] = figks
+    for prefix, fig in figs.items():
+        fname = os.path.join(outdir, "{}.dot_unit_gene.svg".format(prefix))
+        fig.savefig(fname)
+        fname = os.path.join(outdir, "{}.dot_unit_gene.png".format(prefix))
+        fig.savefig(fname,dpi=1200)
+        fname = os.path.join(outdir, "{}.dot_unit_gene.pdf".format(prefix))
+        fig.savefig(fname)
+    plt.close()
+
 # dot plot stuff
-def all_dotplots(df, segs, multi, minseglen, anchors=None, ancestor=None, **kwargs):
+def all_dotplots(df, segs, multi, minseglen, anchors=None, ancestor=None, Ks=None, **kwargs):
     """
     Generate dot plots for all pairs of species in `df`, coloring anchor pairs.
     """
     # Note that the Chr ID in gff3 file should not be alleen int or float
+    if not (Ks is None):
+        ks_dict = {pair:ks for pair,ks in zip(Ks.index,Ks['dS'])}
     gdf = list(df.groupby("species"))
     n = len(gdf)
     figs = {}
     if ancestor != None:
         logging.info("Making ancestral karyotype plot")
         gdf_ances = df[df['species']==ancestor]
         color_scaff = AK_plot(ancestor,gdf_ances,ancestor,backbone=True,**kwargs)
@@ -1613,19 +2120,20 @@
     logging.info("Making dupStack plot")
     for i in range(n):
         for j in range(n):
             spx, dfx = gdf[i]
             spy, dfy = gdf[j]
             logging.info("{} vs. {}".format(spx, spy))
             get_dots(dfx, dfy, segs, multi, minseglen, dupStack = True, **kwargs)
-    logging.info("Making dotplots and marco-synteny plots")
+    logging.info("Making dotplots (in unit of bases) and marco-synteny plots")
     getscafflength(n,gdf,**kwargs)
     if n > 1: get_marco_whole(list(map(lambda x:x[1],gdf)),segs, multi, minseglen,**kwargs)
     for i in range(n):
         for j in range(i, n):
+            xxs,yys,ksages,xxs_ap,yys_ap,ksages_ap,Ksages = [],[],[],[],[],[],[]
             fig, ax = plt.subplots(1, 1, figsize=(10,10))
             ax2 = ax.twinx()
             ax3 = ax.twiny()
             spx, dfx = gdf[i]
             spy, dfy = gdf[j]
             logging.info("{} vs. {}".format(spx, spy))
             get_marco(dfx, dfy, segs, multi, minseglen, **kwargs)
@@ -1633,82 +2141,108 @@
             #print(xs)
             #print(ys)
             #for i,j in zip(df.x,df.y): print((i,j))
             if df is None:  # HACK, in case we're dealing with RBH orthologs...
                 continue
             #for x,y in zip(df.x,df.y): ax.scatter(x, y, s=1, color="k", alpha=0.1)
             #print((len(list(itertools.chain(df.x))),len(list(itertools.chain(df.y)))))
-            ax.scatter(list(itertools.chain(df.x)), list(itertools.chain(df.y)), s=1, color="k", alpha=0.1)
+            ax.scatter(list(itertools.chain(df.x)), list(itertools.chain(df.y)), s=0.4, color="k", alpha=0.01)
+            if not (Ks is None):
+                for i,x,y in zip(df.index,df['x'],df['y']):
+                    ksage = ks_dict.get(i,None)
+                    if ksage == None:
+                        continue
+                    ksages.append(ksage)
+                    Ksages.append(ksage)
+                    xxs.append(x)
+                    yys.append(y)
             #ax.scatter(np.array(df.x,dtype=float), np.array(df.y,dtype=float), s=1, color="k", alpha=0.1)
             if not (anchors is None):
                 andf = df.join(anchors, how="inner")
                 #for x,y in zip(andf.x,andf.y): ax.scatter(x, y, s=1, color="r", alpha=0.9)
-                ax.scatter(list(itertools.chain(andf.x)), list(itertools.chain(andf.y)), s=1, color="r", alpha=0.9)
-                #ax.scatter(np.array(andf.x,dtype=float), np.array(andf.y,dtype=float), s=1, color="red", alpha=0.9)
+                ax.scatter(list(itertools.chain(andf.x)), list(itertools.chain(andf.y)), s=0.4, color="r", alpha=1)
+                if not (Ks is None):
+                    for i,x,y in zip(andf.index,andf['x'],andf['y']):
+                        ksage = ks_dict.get(i,None)
+                        if ksage == None:
+                            continue
+                        ksages_ap.append(ksage)
+                        xxs_ap.append(x)
+                        yys_ap.append(y)
             xlim = max(scaffxtick)
             ylim = max(scaffytick)
             ax.set_xlim(0, xlim)
             ax.set_ylim(0, ylim)
             ymin, ymax = ax.get_ylim()
             xmin, xmax = ax.get_xlim()
-            #ax.vlines(xs, ymin=0, ymax=ys[-1], alpha=0.8, color="k")
-            #ax.vlines(xs, ymin=0, ymax=ylim, alpha=0.8, color="k")
             ax.vlines(xs+[xmax], ymin=0, ymax=ylim, alpha=0.8, color="k")
-            #ax.vlines(scaffxtick, ymin=0, ymax=ylim, alpha=0.8, color="k")
-            #ax.hlines(ys, xmin=0, xmax=xs[-1], alpha=0.8, color="k")
-            #ax.hlines(ys, xmin=0, xmax=xlim, alpha=0.8, color="k")
             ax.hlines(ys+[ymax], xmin=0, xmax=xlim, alpha=0.8, color="k")
-            #ax.hlines(scaffytick, xmin=0, xmax=xlim, alpha=0.8, color="k")
-            #xlim = max(scaffxtick)
-            #ax.set_xlim(0, xs[-1])
-            #ax.set_xlim(0, xlim)
-            #ylim = max(scaffytick)
-            #ax.set_ylim(0, ys[-1])
-            #ax.set_ylim(0, ylim)
-            #ax.set_xlabel("${}$ (Mb)".format(spx))
-            #ax.set_ylabel("${}$ (Mb)".format(spy))
             ax.set_xlabel("{}".format(spx))
             ax.set_ylabel("{}".format(spy))
-            ax2.set_ylabel("{} (Mb)".format(spy))
-            ax2.yaxis.label.set_fontsize(18)
             ax2.set_yticklabels(ax.get_yticks() / 1e6)
-            ax2.tick_params(axis='both', which='major', labelsize=16)
-            ax3.set_xlabel("{} (Mb)".format(spx))
-            ax3.xaxis.label.set_fontsize(18)
             ax3.set_xticklabels(ax.get_xticks() / 1e6)
-            ax3.tick_params(axis='both', which='major', labelsize=16)
-            ax.xaxis.label.set_fontsize(18)
-            ax.yaxis.label.set_fontsize(18)
-            ax.tick_params(axis='both', which='major', labelsize=16)
+            ax.tick_params(axis='both', which='major')
             ax.set_xticks(scaffxtick)
             ax.set_xticklabels(scaffxlabels,rotation=45)
-            #ax.set_xticklabels(ax.get_xticks() / 1e6)  # in Mb
-            #ax.set_yticklabels(ax.get_yticks() / 1e6)  # in Mb
             ax.set_yticks(scaffytick)
             ax.set_yticklabels(scaffylabels,rotation=45)
+            ax2.set_ylabel("{} (Mb)".format(spy))
+            ax3.set_xlabel("{} (Mb)".format(spx))
             fig.tight_layout()
             figs[spx + "-vs-" + spy] = fig
+            if not (Ks is None):
+                figks, axks = plt.subplots(1, 1, figsize=(10,10))
+                axks2 = axks.twinx()
+                axks3 = axks.twiny()
+                norm = matplotlib.colors.Normalize(vmin=np.min(Ksages), vmax=np.max(Ksages))
+                c_m = matplotlib.cm.rainbow
+                s_m = ScalarMappable(cmap=c_m, norm=norm)
+                s_m.set_array([])
+                axks.scatter(xxs, yys, s=0.4, color=[c_m(norm(c)) for c in ksages], alpha=0.01)
+                axks.scatter(xxs_ap, yys_ap, s=0.4, color=[c_m(norm(c)) for c in ksages_ap], alpha=1)
+                axks.set_xlim(0, xlim)
+                axks.set_ylim(0, ylim)
+                axks.vlines(xs+[xmax], ymin=0, ymax=ylim, alpha=0.8, color="k")
+                axks.hlines(ys+[ymax], xmin=0, xmax=xlim, alpha=0.8, color="k")
+                axks.set_xlabel("{}".format(spx))
+                axks.set_ylabel("{}".format(spy))
+                axks2.set_yticklabels(axks.get_yticks() / 1e6)
+                axks3.set_xticklabels(axks.get_xticks() / 1e6)
+                axks.tick_params(axis='both', which='major')
+                axks.set_xticks(scaffxtick)
+                axks.set_xticklabels(scaffxlabels,rotation=45)
+                axks.set_yticks(scaffytick)
+                axks.set_yticklabels(scaffylabels,rotation=45)
+                axks2.set_ylabel("{} (Mb)".format(spy))
+                axks3.set_xlabel("{} (Mb)".format(spx))
+                plt.colorbar(s_m, label="$K_\mathrm{S}$", orientation="vertical",fraction=0.03,pad=0.1)
+                figks.tight_layout()
+                figs[spx + "-vs-" + spy + "_Ks"] = figks
     return figs
 
 def filter_by_minlength(genetable,segs,minlen,multi,keepredun,outdir,minseglen):
     gdf,Index_torm,I2,I3,I4 = list(genetable.copy().groupby("species")),[],[],[],[]
     Sf_len_lab_persp = {sp:{} for sp,df in gdf}
+    removed_scfa = {}
     for sp,df in gdf:
         lens = df.groupby("scaffold")["start"].agg(max)
         lens.name = "len"
         lens = pd.DataFrame(lens).sort_values("len", ascending=False)
+        orig_scfa = set(lens.index)
         noriginal = len(lens.index)
         if minlen < 0:
             Minlen = lens.len.max() * 0.1
             logging.info("`minlen` not set, taking 10% of longest scaffold ({}) for {}".format(Minlen,sp))
             lens = lens.loc[lens.len > Minlen]
             logging.info("Dropped {} scaffolds in {} because they are on scaffolds shorter than {}".format(noriginal-len(lens.index),sp,Minlen))
         else:
             lens = lens.loc[lens.len > minlen]
             logging.info("Dropped {} scaffolds in {} because they are on scaffolds shorter than {}".format(noriginal-len(lens.index),sp,minlen))
+        removed = list(orig_scfa - set(lens.index))
+        removed_scfa[sp] = removed
         segs_tmp = segs.loc[(segs['genome']==sp) & (~segs['list'].isin(lens.index)),:]
         gt_tmp = genetable.loc[(genetable['species']==sp) & (~genetable['scaffold'].isin(lens.index)),:]
         multi_tmpx = multi.loc[(multi['genome_x']==sp) & (~multi['list_x'].isin(lens.index)),:]
         multi_tmpy = multi.loc[(multi['genome_y']==sp) & (~multi['list_y'].isin(lens.index)),:]
         for i in segs_tmp.index: Index_torm.append(i)
         for j in gt_tmp.index: I2.append(j)
         for lab in lens.index: Sf_len_lab_persp[sp][lab] = lens.loc[lab,'len']
@@ -1727,15 +2261,23 @@
     segs = Filter_miniseglen(segs,Sf_len_lab_persp,minseglen,genetable)
     counted = segs.groupby(["multiplicon", "genome"])["segment"].aggregate(lambda x: len(set(x)))
     profile = counted.unstack(level=-1).fillna(0)
     fig = syntenic_depth_plot(profile)
     fig.savefig(os.path.join(outdir, "Syndepth.svg"),bbox_inches='tight')
     fig.savefig(os.path.join(outdir, "Syndepth.pdf"),bbox_inches='tight')
     profile.to_csv(os.path.join(outdir, "Segprofile.csv"))
-    return segs,genetable,multi
+    return segs,genetable,multi,removed_scfa
+
+def filter_mingenumber(segs,mingenenum):
+    rm_indice = []
+    for indice, f, l in zip(segs.index,segs['first_coordinate'],segs['last_coordinate']):
+        if (l-f+1) < mingenenum:
+            rm_indice.append(indice)
+    segs = segs.drop(rm_indice)
+    return segs
 
 def Filter_miniseglen(segs,scaf_info,minseglen,genetable):
     rm_indice = []
     gene_start_info = {sp:{} for sp in scaf_info.keys()}
     work1 = genetable.reset_index().loc[:,['gene','species','start']]
     work2 = work1.groupby('species')
     for i,j,k in map(lambda x:(x[0],x[1]['gene'],x[1]['start']) ,work2):
@@ -1745,103 +2287,14 @@
         if minseglen <= 1:
             if seg_len < scaf_info[sp][sf_la] * minseglen: rm_indice.append(indice)
         else:
             if seg_len < minseglen: rm_indice.append(indice)
     segs = segs.drop(rm_indice)
     return segs
 
-def Ks_dotplots(segs,dff, df, ks, an, minseglen, anchors=None, color_map='Spectral',min_ks=0.05, max_ks=5, minlen=250, maxsize=25, outdir='', **kwargs):
-    """
-    Generate Ks colored dot plots for all pairs of species in `df`.
-    """
-    cmap = plt.get_cmap(color_map)
-    if len(an["gene_x"]) == 0:
-        logging.warning("No multiplicons found!")
-        return
-    an["pair"] = an.apply(lambda x: '__'.join(
-            sorted([x["gene_x"], x["gene_y"]])), axis=1)
-    genomic_elements_ = {
-        x: 0 for x in list(set(dff['list_x']) | set(dff['list_y']))
-        if type(x) == str
-    }
-
-    ks_multiplicons = {}
-    all_ks = []
-    for i in range(len(dff)):
-        row = dff.iloc[i]
-        pairs = an[an['multiplicon'] == row['id']]['pair']
-        med_ks = np.median(ks.loc[ks.index.intersection(pairs)]['dS'])
-        ks_multiplicons[row['id']] = med_ks
-        all_ks.append(med_ks)
-
-    z = [[0, 0], [0, 0]]
-    levels = range(0, 101, 1)
-    tmp = plt.contourf(z, levels, cmap=cmap)
-    plt.clf()
-    
-    for key in sorted(genomic_elements_.keys()):
-        length = max(list(dff[dff['list_x'] == key]['end_x']) + list(
-                dff[dff['list_y'] == key]['end_y']))
-        if length >= minlen:
-            genomic_elements_[key] = length
-
-    previous = 0
-    genomic_elements = {}
-    sorted_ge = sorted(genomic_elements_.items(), key=lambda x: x[1],
-                       reverse=True)
-    labels = [kv[0] for kv in sorted_ge if kv[1] >= minlen]
-
-    for kv in sorted_ge:
-        genomic_elements[kv[0]] = previous
-        previous += kv[1]
-
-    gdf = list(df.groupby("species"))
-    n = len(gdf)
-    figs = {}
-    for i in range(n):
-        for j in range(i, n):
-            fig, ax = plt.subplots(1, 1, figsize=(10,10))
-            spx, dfx = gdf[i]
-            spy, dfy = gdf[j]
-            logging.info("{} vs. {}".format(spx, spy))
-            df, xs, ys, scafflabels, scaffylabels, scaffxtick, scaffytick = get_dots(dfx, dfy, segs, dff, minseglen, minlen=minlen, maxsize=maxsize, outdir = outdir)
-            if df is None:  # HACK, in case we're dealing with RBH orthologs...
-                continue
-            ax.scatter(df.x, df.y, s=0.1, color="k", alpha=0.5)
-            if not (anchors is None):
-                andf = df.join(anchors, how="inner")
-                for k in range(len(dff)):
-                    row = dff.iloc[k]
-                    list_x, list_y = row['list_x'], row['list_y']
-                    if type(list_x) != float:
-                        curr_list_x = list_x
-                    x = [genomic_elements[curr_list_x] + x for x in [row['begin_x'], row['end_x']]]
-                    y = [genomic_elements[list_y] + x for x in [row['begin_y'], row['end_y']]]                     
-                    med_ks = ks_multiplicons[row['id']]
-                    if min_ks < med_ks <= max_ks:
-                        ax.scatter(andf.x, andf.y, s=0.2, color=cmap(ks_multiplicons[row['id']] / 5), alpha=0.9)
-            ax.vlines(xs, ymin=0, ymax=ys[-1], alpha=0.1, color="k")
-            ax.hlines(ys, xmin=0, xmax=xs[-1], alpha=0.1, color="k")
-            ax.set_xlim(0, xs[-1])
-            ax.set_ylim(0, ys[-1])
-            ax.set_xlabel("${}$ (Mb)".format(spx))
-            ax.set_ylabel("${}$ (Mb)".format(spy))
-            ax.xaxis.label.set_fontsize(18)
-            ax.yaxis.label.set_fontsize(18)
-            ax.tick_params(axis='both', which='major', labelsize=16)
-            ax.set_xticklabels(ax.get_xticks() / 1e6)  # in Mb
-            ax.set_yticklabels(ax.get_yticks() / 1e6)  # in Mb
-            figs[spx + "-vs-" + spy] = fig
-
-    # colorbar
-    cbar = plt.colorbar(tmp, fraction=0.02, pad=0.01)
-    cbar.ax.set_yticklabels(['{:.2f}'.format(x) for x in np.linspace(0, 5, 11)])
-
-    return figs
-
 def get_dots(dfx, dfy, seg, multi, minseglen, minlen=-1, maxsize=200, outdir = '', dupStack = False):
     spx=dfx.loc[:,'species'][0]
     spy=dfy.loc[:,'species'][0]
     if dupStack: sankey_plot(spx, dfx, spy, dfy, minseglen, minlen, outdir, seg)
     else:
         dfx,scaffxtick = filter_data_dotplot(dfx, minlen)
         dfy,scaffytick = filter_data_dotplot(dfy, minlen)
@@ -1929,86 +2382,103 @@
     cmap = plt.get_cmap(color_map)
     if len(an) == 0:
         logging.warning("No multiplicons found!")
         return
     #an["pair"] = an.apply(lambda x: '__'.join(
     #        sorted([x["gene_x"], x["gene_y"]])), axis=1)
     an = an.reset_index()
+    # Get all occurred scaffolds in multiplicons
     genomic_elements_ = {
         x: 0 for x in list(set(df['list_x']) | set(df['list_y']))
         if type(x) == str
     }
-
+    # Here the age is per multiplicon instead of per segment
     ks_multiplicons = {}
     all_ks = []
     for i in range(len(df)):
         row = df.iloc[i]
+        # from anchor.csv file get the anchor pairs information per multiplicon
         pairs = an[an['multiplicon'] == row['id']]['pair']
-        med_ks = np.median(ks.loc[ks.index.intersection(pairs)]['dS'])
+        if len(pairs) == 0:
+            logging.info("Multiplicon {} has 0 anchor pairs left after filtering duplicated anchor pairs".format(row['id']))
+            continue
+        # from anchor_ks file get all the associated Ks information per multiplicon
+        # The anchor pairs are filtered at the very begining that no duplicated pairs are allowed, thus there might be multiplicon with 0,1,2 anchor pairs with Ks data, since not all anchor pairs have Ks data
+        index_retained = ks.index.intersection(pairs)
+        if len(index_retained) == 0:
+            logging.info("The anchor pairs on multiplicon {} have no Ks estimation".format(row['id']))
+            continue
+        med_ks = np.median(ks.loc[index_retained]['dS']) # this step will counter RuntimeWarning: Mean of empty slice and RuntimeWarning: invalid value encountered in double_scalars
         ks_multiplicons[row['id']] = med_ks
         all_ks.append(med_ks)
 
     z = [[0, 0], [0, 0]]
     levels = range(0, 101, 1)
     tmp = plt.contourf(z, levels, cmap=cmap)
     plt.clf()
 
     fig = plt.figure(figsize=(6.5, 6))
     ax = fig.add_subplot(111)
 
     for key in sorted(genomic_elements_.keys()):
+        # find the longest multiplicon per scaffold, instead of the real length of that scaffold
         length = max(list(df[df['list_x'] == key]['end_x']) + list(
                 df[df['list_y'] == key]['end_y']))
         if length >= min_length:
             genomic_elements_[key] = length
 
     previous = 0
     genomic_elements = {}
     sorted_ge = sorted(genomic_elements_.items(), key=lambda x: x[1],
                        reverse=True)
     labels = [kv[0] for kv in sorted_ge if kv[1] >= min_length]
-
+    # accumulate the scaffold length, now = now + previous, to prepare the tick, starting from 0
     for kv in sorted_ge:
         genomic_elements[kv[0]] = previous
         previous += kv[1]
 
     # plot layout
     x = [genomic_elements[key] for key in sorted(genomic_elements.keys())] + \
         [previous]
-    x = sorted(list(set(x)))
+    x = sorted(list(set(x))) # starting from 0
     ax.vlines(ymin=0, ymax=previous, x=x, linestyles='dotted', alpha=0.2)
     ax.hlines(xmin=0, xmax=previous, y=x, linestyles='dotted', alpha=0.2)
-    ax.plot(x, x, color='k', alpha=0.2)
+    ax.plot(x, x, color='k', alpha=0.2) # diagonal line
     ax.set_xticks(x)
     ax.set_yticks(x)
     ax.set_xticklabels([])
     ax.set_yticklabels([])
     ax.set_xlim(0, max(x))
     ax.set_ylim(0, max(x))
-    ax.set_xticks([(x[i] + x[i - 1]) / 2 for i in range(1, len(x))], minor=True)
+    ax.set_xticks([(x[i] + x[i - 1]) / 2 for i in range(1, len(x))], minor=True) # here there are two sets of ticks
     ax.set_xticklabels(labels, minor=True, rotation=45)
     ax.set_yticks([(x[i] + x[i - 1]) / 2 for i in range(1, len(x))], minor=True)
     ax.set_yticklabels(labels, minor=True, rotation=45)
+    # hide the tick shape and center the label
     for tick in ax.xaxis.get_minor_ticks():
         tick.tick1line.set_markersize(0)
         tick.tick2line.set_markersize(0)
         tick.label1.set_horizontalalignment('center')
     for tick in ax.yaxis.get_minor_ticks():
         tick.tick1line.set_markersize(0)
         tick.tick2line.set_markersize(0)
         # tick.label1.set_horizontalalignment('center')
 
     # the actual dots (or better, line segments)
     for i in range(len(df)):
         row = df.iloc[i]
+        if ks_multiplicons.get(row['id']) == None:
+            logging.info("Skipping multiplicon {} which has no Ks information of retained unique anchor pairs".format(row['id']))
+            continue
         list_x, list_y = row['list_x'], row['list_y']
         if type(list_x) != float:
+            # The first multiplicon of all children multiplicons has the list_x info astype str instead of float
             curr_list_x = list_x
         x = [genomic_elements[curr_list_x] + x for x in
-             [row['begin_x'], row['end_x']]]
+             [row['begin_x'], row['end_x']]] # return a list of two elements, for instance [607, 1720]
         y = [genomic_elements[list_y] + x for x in
              [row['begin_y'], row['end_y']]]
         med_ks = ks_multiplicons[row['id']]
         if min_ks < med_ks <= max_ks:
             ax.plot(x, y, alpha=0.9, linewidth=1.5,
                     color=cmap(ks_multiplicons[row['id']] / 5)),
             # path_effects=[pe.Stroke(linewidth=4, foreground='k'), pe.Normal()])
```

### Comparing `wgd-2.0.16/wgd.egg-info/PKG-INFO` & `wgd-2.0.17/wgd.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,556 +1,636 @@
 Metadata-Version: 2.1
 Name: wgd
-Version: 2.0.16
+Version: 2.0.17
 Summary: wgd
 Home-page: http://github.com/heche-psb/wgd
 Author: Hengchi Chen
 Author-email: heche@psb.vib-ugent.be
 License: GPL
-Description: <div align="center">
-        
-        # `wgd v2` : a suite tool of WGD inference and timing
-        
-        **Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
-        
-        [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
-        
-        [**Introduction**](#Introduction) | 
-        [**Installation**](#Installation) | 
-        [**Parameters**](#Parameters) | 
-        [**Usage**](#Usage) | 
-        [**Illustration**](#Illustration) |
-        [**Citation**](#Citation)
-        
-        </div>
-        
-        `wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
-        
-        ## Introduction
-        
-        Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
-        
-        The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
-        
-        ## Installation
-        
-        The easiest way to install `wgd v2` is using PYPI
-        
-        ```
-        pip install wgd
-        ```
-        
-        To install `wgd v2` in a virtual environment, the following command lines could be used.
-        
-        ```
-        git clone <wgd repo>
-        cd wgd
-        virtualenv -p=python3 ENV (or python3 -m venv ENV)
-        source ENV/bin/activate
-        pip install -r requirements.txt
-        pip install .
-        ```
-        
-        When met with permission problem in installation, please try the following command line.
-        
-        ```
-        pip install -e .
-        ```
-        
-        If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
-        
-        ```
-        export PATH="$PATH:~/.local/bin/wgd"
-        ```
-        
-        Note that the version of `numpy` is important (for many other packages are the same of course), especially for `fastcluster` package. In our test, the `numpy` 1.19.0 works fine on `python3.6/8`. If you met some errors or warnings about numpy, maybe considering pre-install `numpy` as 1.19.0 or other close-by versions before you install `wgd`.
-        
-        ## Parameters
-        
-        There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
-        
-        The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
-        ```
-        wgd dmd sequences (option)
-        --------------------------------------------------------------------------------
-        -o, --outdir, the output directory, default wgd_dmd
-        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
-        -c, --cscore, the c-score to restrict the homologs of MRBHs, default None, if None was given, the c-score funcion won't be activated
-        -I, --inflation, the inflation factor for MCL program, default 2.0
-        -e, --eval, the e-value cut-off for similarity in diamond and/or hmmer, default 1e-10
-        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
-        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
-        -f, --focus, the species to be merged on local MRBHs, default None, if None was given, the local MRBHs won't be inferred
-        -ap, --anchorpoints, the anchor points data file, default None
-        -coc, --collinearcoalescence, flag option, whether to initiate the collinear coalescence analysis, if the flag was set, the analysis will be initiated
-        -sm, --segments, the segments data file used in collinear coalescence analysis if initiated, default None
-        -le, --listelements, the listsegments data file used in collinear coalescence analysis if initiated, default None
-        -gt, --genetable, the gene table datafile used in collinear coalescence analysis if initiated, default None
-        -kf, --keepfasta, flag option, whether to output the sequence information of MRBHs, if the flag was set, the sequences of MRBHs will be in output
-        -kd, --keepduplicates, flag option, whether to allow the same gene to occur in different MRBHs, if the flag was set, the same gene can be assigned to different MRBHs
-        -gm, --globalmrbh, flag option, whether to initiate global MRBHs construction, if the flag was set, the --focus option will be ignored and only global MRBHs will be built
-        -n, --nthreads, the number of threads to use, default 4
-        -oi, --orthoinfer, flag option, whether to initiate orthogroup infernece, if the flag was set, the orthogroup infernece program will be initiated
-        -oo, --onlyortho, flag option, whether to only conduct orthogroup infernece, if the flag was set, only the orthogroup infernece program will be conducted while the other analysis won't be initiated
-        -gn, --getnsog, flag option, whether to initiate the searching for nested single-copy gene families (NSOGs), if the flag was set, additional NSOGs analysis will be performed besides the basic orthogroup infernece
-        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
-        -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
-        -mc, --msogcut, the ratio cutoff for mostly single-copy family and species representation in collinear coalescence inference, default 0.8.
-        -ga, --geneassign, flag option, whether to initiate the gene-to-family assignment analysis, if the flag was set, the analysis will be initiated
-        -am, --assign_method, which method to conduct the gene-to-family assignment analysis, default hmmer
-        -sa, --seq2assign, the queried sequences data file in gene-to-family assignment analysis, default None, this option can be provided multiple times
-        -fa, --fam2assign, the queried familiy data file in gene-to-family assignment analysis, default None
-        -cc, --concat, flag option, whether to initiate the concatenation pipeline for orthogroup infernece, if the flag was set, the analysis will be initiated
-        -te, --testsog, flag option, whether to initiate the unbiased test of single-copy gene families, if the flag was set, the analysis will be initiated
-        -bs, --bins, the number of bins divided in gene length normalization, default 100
-        -np, --normalizedpercent, the percentage of upper hits used for gene length normalization, default 5
-        -nn, --nonormalization, flag option, whether to call off the normalization, if the flag was set, no normalization will be conducted
-        -bsog, --buscosog, flag option, whether to initiate the busco-guided single-copy gene family analysis, if the flag was set, the analysis will be initiated
-        -bhmm, --buscohmm, the HMM profile datafile in the busco-guided single-copy gene family analysis, default None
-        -bctf, --buscocutoff, the HMM score cutoff datafile in the busco-guided single-copy gene family analysis, default None
-        ```
-        
-        The program `wgd focus` can realize the concatenation-based and coalescence-based phylogenetic inference, functional annotation of gene families and phylogenetic dating of WGDs.
-        ```
-        wgd focus families sequences (option)
-        --------------------------------------------------------------------------------
-        -o, --outdir, the output directory, default wgd_focus
-        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
-        -n, --nthreads, the number of threads to use, default 4
-        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
-        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
-        --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
-        -a, --aligner, which alignment program to use, default mafft
-        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
-        -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
-        --concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
-        --coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
-        -sp, --speciestree, species tree darafile for dating, default None
-        -d, --dating, which molecular dating program to use, default none
-        -ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
-        -ns, --nsites, the nsites information for r8s dating, default None
-        -ot, --outgroup, the outgroup information for r8s dating, default None
-        -pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
-        -am, --aamodel, which protein model to be used in mcmctree, default poisson
-        -ks, flag option, whether to initiate Ks analysis
-        --annotation, which annotation program to use, default none
-        --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
-        -ed, --eggnogdata, the eggnog annotation datafile, default None
-        --pfam, which option to use for pfam annotation, default none
-        --dmnb, the diamond database for annotation, default None
-        --hmm, the HMM profile for annotation, default None
-        --evalue, the e-value cut-off for annotation, default 1e-10
-        --exepath, the path to the interproscan executable, default None
-        -f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
-         -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
-        -cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
-        --beastlgjar, the path to beastLG.jar, default None
-        --beagle, flag option, whether to use beagle in Beast, if the flag was set, beagle will be used
-        --protdating, flag option, whether to only initiate the protein-concatenation based dating analysis, if the flag was set, the analysis will be initiated
-        ```
-        
-        The program `wgd ksd` can realize the construction of *K*<sub>S</sub> age distribution and rate correction.
-        ```
-        wgd ksd families sequences (option)
-        --------------------------------------------------------------------------------
-        -o, --outdir, the output directory, default wgd_ksd
-        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
-        -n, --nthreads, the number of threads to use, default 4
-        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
-        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
-        --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
-        --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
-        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
-        -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
-        -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
-        -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
-        -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
-        ```
-        
-        The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
-        ```
-        wgd mix ks_datafile (option)
-        --------------------------------------------------------------------------------
-        -f, --filters, the cutoff alignment length, default 300
-        -r, --ks_range, the Ks range to be considered, default (0.005, 3)
-        -b, --bins, the number of bins in Ks distribution, default 50
-        -o, --outdir, the output directory, default wgd_mix
-        --method, which mixture model to use, default gmm
-        -n, --components, the range of the number of components to fit, default (1, 4)
-        -g, --gamma, the gamma parameter for bgmm models, default 0.001
-        -ni, --n_init, the number of k-means initializations, default 200
-        -mi, --max_iter, the maximum number of iterations, default 1000
-        ```
-        
-        The program `wgd peak` can realize the search of crediable *K*<sub>S</sub> range used in WGD dating.
-        ```
-        wgd peak ks_datafile (option)
-        --------------------------------------------------------------------------------
-        -ap, --anchorpoints, the anchor points datafile, default None
-        -sm, --segments, the segments datafile, default None
-        -le, --listelements, the listsegments datafile, default None 
-        -mp, --multipliconpairs, the multipliconpairs datafile, default None
-        -o, --outdir, the output directory, default wgd_peak
-        -af, --alignfilter, cutoff for alignment identity, length and coverage, default 0.0, 0, 0.0
-        -r, --ksrange, range of Ks to be analyzed, default (0, 5)
-        -bw, --bin_width, bandwidth of Ks distribution, default 0.1
-        -ic, --weights_outliers_included, flag option, whether to include Ks outliers, if the flag was set, Ks outliers will be included in the analysis
-        -m, --method, which mixture model to use, default gmm
-        --seed, random seed given to initialization, default 2352890
-        -ei, --em_iter, the number of EM iterations to perform, default 200
-        -ni, --n_init, the number of k-means initializations, default 200
-        -n, --components, the range of the number of components to fit, default (1, 4)
-        --boots, the number of bootstrap replicates of kde, default 200
-        --weighted, flag option, whether to use node-weighted method of de-redundancy, if the flag was set, the node-weighted method will be used
-        -p, --plot, the plotting method to be used, default identical
-        -bm, --bw_method, the bandwidth method to be used, default silverman
-        --n_medoids, the number of medoids to fit, default 2
-        -km, --kdemethod, the kde method to be used, default scipy
-        --n_clusters, the number of clusters to plot Elbow loss function, default 5
-        --kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
-        -gd, --guide, the regime residing anchors, default: segment
-        -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
-        -kd, --kstodate, the range of Ks to be dated, default (0.5, 1.5)
-        -f, --family, the family to filter Ks upon, default None
-        --manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
-        -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
-        --ci, the confidence level of log-normal distribution to date, default 95
-        --hdr, the highest densidy region (HDR) in a given distribution to date, default 95
-        --heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
-        -kc, --kscutoff, the Ks saturation cutoff in dating, default 5
-        ```
-        
-        The program `wgd syn` can realize the intra- and inter-specific synteny inference.
-        ```
-        wgd syn families gffs (option)
-        --------------------------------------------------------------------------------
-        -ks, --ks_distribution, ks distribution datafile, default None
-        -o, --outdir, the output directory, default wgd_syn
-        -f, --feature, the feature for parsing gene IDs from GFF files, default gene
-        -a, --attribute, the attribute for parsing the gene IDs from the GFF files, default ID
-        -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
-        -ms, --maxsize, the maximum family size to include, default 200
-        -r, --ks_range, the Ks range in colored dotplot, default (0, 5)
-        --iadhore_options, the parameter setting in iadhore, default 
-        -ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
-        -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
-        -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
-        ```
-        
-        The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
-        ```
-        wgd viz (option)
-        --------------------------------------------------------------------------------
-        -d, --datafile, the Ks datafile, default None
-        -o, --outdir, the output directory, default wgd_viz
-        -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
-        -gs, --gsmap, the gene name-species name map, default None
-        -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
-        -pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
-        -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
-        -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
-        -iter, --em_iterations, the maximum EM iterations, default 200
-        -init, --em_initializations, the maximum EM initializations, default 200
-        -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
-        -sm, --segments, the segments data file, default None
-        -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
-        -ms, --maxsize, the maximum family size to include, default 200
-        -ap, --anchorpoints, the anchor points datafile, default None
-        -mt, --multiplicon, the multiplicons datafile, default None
-        -gt, --genetable, the gene table datafile, default None
-        -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
-        -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
-        -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
-        ```
-        
-        ## Usage
-        
-        Here we provided the basic usage for each program.
-        
-        ### wgd dmd
-        
-        **The delineation of whole paranome**
-        ```
-        wgd dmd sequence
-        ``` 
-        
-        **The delineation of RBHs**
-        ```
-        wgd dmd sequence1 sequence2
-        ```
-        
-        **The delineation of local MRBHs**
-        ```
-        wgd dmd sequence1 sequence2 sequence3 -f sequence1
-        ```
-        
-        **The delineation of global MRBHs**
-        ```
-        wgd dmd sequence1 sequence2 sequence3 -gm
-        ```
-        
-        **The delineation of orthogroups**
-        ```
-        wgd dmd sequence1 sequence2 sequence3 -oi (option)
-        ```
-        Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
-        
-        **The collinear coalescence inference of phylogeny**
-        ```
-        wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
-        ```
-        
-        Note that there should be no duplicated gene IDs in the sequence file.
-        
-        ### wgd focus
-        
-        **The concatenation-based/coalescence-based phylogenetic inference**
-        ```
-        wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
-        ```
-        
-        **The functional annotation of gene families**
-        ```
-        wgd focus families sequence1 sequence2 sequence3 --annotation eggnog -ed eddata --dmnb dbdata
-        ```
-        
-        **The phylogenetic dating of WGDs**
-        ```
-        wgd focus families sequence1 sequence2 sequence3 -d mcmctree -sp spdata
-        ```
-        
-        ### wgd ksd
-        
-        **The construction of whole paranome *K*<sub>S</sub> age distribution**
-        ```
-        wgd ksd families sequence
-        ```
-        
-        **The construction of orthologous *K*<sub>S</sub> age distribution**
-        ```
-        wgd ksd families sequence1 sequence2
-        ```
-        
-        **The construction of *K*<sub>S</sub> age distribution with rate correction**
-        ```
-        wgd ksd families sequence1 sequence2 sequence3 -sr srdata -sp spdata
-        ```
-        
-        ### wgd mix
-        
-        **The mixture model clustering analysis of *K*<sub>S</sub> age distribution**
-        ```
-        wgd mix ksdata
-        ```
-        
-        ### wgd peak
-        
-        **The search of crediable *K*<sub>S</sub> range used in WGD dating**
-        ```
-        wgd peak ksdata -ap apdata -sm smdata -le ledata -mp mpdata
-        ```
-        Note that users can add the flag --heuristic to implement the heuristic search analysis
-        
-        ### wgd syn
-        
-        **The intra-specific synteny inference**
-        ```
-        wgd syn families gff
-        ```
-        
-        **The inter-specific synteny inference**
-        ```
-        wgd syn families gff1 gff2
-        ```
-        
-        ### wgd viz
-        
-        **The visualization of *K*<sub>S</sub> age distribution**
-        ```
-        wgd viz -d ksdata
-        ```
-        
-        **The visualization of *K*<sub>S</sub> age distribution with rate correction**
-        ```
-        wgd viz -d ksdata -sr srdata -sp spdata -gs gsdata
-        ```
-        
-        **The visualization of synteny**
-        ```
-        wgd viz -ap apdata -sm smdata -mt mtdata -gt gtdata
-        ```
-        
-        ## Illustration
-        
-        We illustrate our program on an exemplary WGD inference and dating upon species *Aquilegia coerulea*.
-        
-        The *Aquilegia coerulea* was reported to experience an paleo-polyploidization event after the divergence of core eudicots, which is likely shared by all Ranunculales.
-        
-        First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
-        
-        ```
-        wgd dmd Aquilegia_coerulea
-        wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
-        ```
-        
-        The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1 but not clear.
-        
-        ![](data/Aquilegia_coerulea.tsv.ksd_wp.svg)
-        
-        We then construct the anchor *K*<sub>S</sub> age distribution using the command line below.
-        
-        ```
-        wgd syn -f mRNA -a Name wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea.gff3 -ks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
-        ```
-        
-        As shown below, there are some retained anchor pairs with *K*<sub>S</sub> between 1 and 2, which seems to suggest a WGD event.
-        
-        ![](data/Aquilegia_coerulea.tsv.ksd_wp_ap.svg)
-        
-        The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes, except for the chr_07, which seems to experience more severe fragmentization than the other chromosomes.
-        
-        ![](data/Aquilegia_coerulea_Aquilegia_coerulea_multiplicons_level.svg)
-        
-        The associated dotplot in oxford grid also presents numerous densely aggregated anchor points throughout most of the chromosomes.
-        
-        ![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
-        
-        A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
-        
-        ![](data/Syndepth.svg)
-        
-        We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
-        
-        ```
-        wgd viz -d wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
-        ```
-        
-        The result of ELMM mixture model clustering shows that there is a likely WGD component at *K*<sub>S</sub> 1.19.
-        
-        ![](data/elmm_Aquilegia_coerulea.tsv.ks.tsv_best_models_weighted.svg)
-        
-        Let's do a mixture model clustering for anchor *K*<sub>S</sub> too, using the command line below.
-        
-        ```
-        wgd peak wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv --anchorpoints wgd_syn/iadhore-out/anchorpoints.txt --segments wgd_syn/iadhore-out/segments.txt --listelements wgd_syn/iadhore-out/list_elements.txt --multipliconpairs wgd_syn/iadhore-out/multiplicon_pairs.txt --weighted
-        ```
-        
-        The anchor *K*<sub>S</sub> age distribution also has a likely WGD component with mode 1.28.
-        
-        ![](data/Original_AnchorKs_GMM_Component3_node_weighted_Lognormal.svg)
-        
-        Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis. First, we built a global MRBH family using the command below.
-        
-        ```
-        wgd dmd --globalmrbh Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera -o wgd_globalmrbh
-        ```
-        
-        In the global MRBH family, every pair of orthologous genes is the reciprocal best hit, suggesting true orthologous relationships. We would use the *K*<sub>S</sub> values associated with these orthologous pairs to delimit the divergence *K*<sub>S</sub> peak. Together with the whole paranome *K*<sub>S</sub> distribution, we conduct the rate correction using the command below.
-        
-        ```
-        wgd ksd wgd_globalmrbh/global_MRBH.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
-        ```
-        
-        The file `speciestree.nw` is the text file of species tree in newick that rate correction would be conducted on. Its content is as below. Users need to provide the species pairs to be plotted. We suggest adding the option `--reweight` to recalculate the weight per species pair such that the weight of orthologous gene pairs will become 1 as the paralogous gene pairs. The flag `--plotkde` can be added when the kde curve of orthologous *K*<sub>S</sub> is desired. Extra collinear data can be added by the option `-ap`.
-        
-        ```
-        (((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
-        ```
-        
-        ![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
-        
-        As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
-        
-        If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
-        
-        ```
-        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
-        ```
-        
-        Note that we can easily show that *Aquilegia coerulea* has higher substitution rate than *Protea cynaroides* and *Vitis vinifera* by comparing their substitution distance in regard to the same divergence event with outgroup species *Acorus_americanus*, using command below.
-        
-        ```
-        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_viz_Compare_rate --spair "Acorus_americanus;Protea_cynaroides" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Vitis_vinifera;Acorus_americanus" --gsmap gene_species.map --plotkde
-        ```
-        
-        ![](data/Raw_Orthologues_Compare_rate.ksd.svg)
-        
-        As displayed above, the orthologous *K*<sub>S</sub> values bewteen *Aquilegia coerulea* and *Acorus americanus* has the highest mode, indicatingthe faster substitution rate of *Aquilegia coerulea* compared to *Protea cynaroides* and *Vitis vinifera*.
-        
-        Note that a necessary gene-species map file is needed for its implementation in `wgd viz`, which should be automately produced by the last `wgd ksd` step. The `gene_species.map` has contents as below in which each line is the joined string of gene name and species name by space.
-        
-        ```
-        Aqcoe6G057800.1 Aquilegia_coerulea
-        Vvi_VIT_201s0011g01530.1 Vitis_vinifera
-        Pcy_Procy01g08510 Protea_cynaroides
-        Aam_Acora.04G142900.1 Acorus_americanus
-        ```
-        
-        A more complex plot can be made by add the flag `--plotelmm` such that the ELMM mixture modeling of provided paranome *K*<sub>S</sub> can be superimposed, using the command below.
-        
-        ```
-        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm
-        ```
-        
-        ![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Corrected.ksd.svg)
-        
-        From the mixed *K*<sub>S</sub> plot above, we can see that the optimized lognormal component b with mode 1.2 is younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera* (1.39 and 1.47, respectively).
-        
-        Besides, we can also add the GMM mixture modeling of anchor *K*<sub>S</sub> values with the flag `--plotapgmm`, using the command below.
-        
-        ```
-        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotapgmmm
-        ```
-        
-        ![](data/Aquilegia_coerulea_GlobalmrbhKs_Apgmm_Corrected.ksd.svg)
-        
-        As manifested above, the anchor *K*<sub>S</sub> component 2 with mode 1.28 is also younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera*. But we need to be of course cautious that such distinction comes with the uncertainties introduced from the applied mixture modeling methodology in terms of for instance different initialization points and the issue of overfitting and the sister speciess adopted in that there might be species with more disparate substitution rates than the one we chose.
-        
-        Adding both ELMM result for paranome and GMM result for anchor *K*<sub>S</sub> can be achieved just by add the two flags mentioned above, using the command below.
-        
-        ```
-        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm --plotapgmmm
-        ```
-        
-        ![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Apgmm_Corrected.ksd.svg)
-        
-        An alternative way to calculate the orthologous *K*<sub>S</sub> is to directly use the orthogroups instead of global MRBH family. That way we don't use the pre-inferred paranome *K*<sub>S</sub> but the paralogous gene pairs inside each orthogroup instead. To achieve that, we first need to infer orthogroups using the command below.
-        
-        ```
-        wgd dmd Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera --orthoinfer -o wgd_ortho (--onlyortho) 
-        ```
-        
-        Users can decide to only conduct the orthogroup analysis while skipping other analysis by adding the flag `--onlyortho`. Next step is the same with global MRBH family except that we don't use the extra pre-inferred paranome *K*<sub>S</sub> anymore. We infer the *K*<sub>S</sub> using the command below. Note that the program `wgd viz` can plot the same just as shown above.
-        
-        ```
-        wgd ksd wgd_ortho/Orthogroups.sp.tsv -sp speciestree.nw --reweight -o wgd_ortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
-        ```
-        
-        ![](data/Aquilegia_coerulea_OrthoKs_Corrected.ksd.svg)
-        
-        As shown above, the number of both paralogous gene pairs and orthologous gene pairs is different than the one from global MRBH family in that here we plotted all orthologous gene pairs instead of only global MRBH and potentially new paralogous gene pairs might be produced in the orthogroup inference step, together with different recalculated weights.
-        
-        If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, as we have already shown above, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
-        
-        ```
-        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --gsmap gene_species.map
-        ```
-        
-        We can clearly see that *Vitis vinifera* has higher substitution rate than *Protea cynaroides* in that their orthologous *K*<sub>S</sub> peaks with *Aquilegia coerulea*, although representing the same divergence event, differed in substitution distance.
-        ![](data/Raw_Orthologues.ksd.svg)
-        
-        ## Citation
-         
-        Please cite us at https://doi.org/10.1093/bioinformatics/bty915
-        
-        ```
-        Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
-        
-        Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
-        ```
-        
-        For citation of the tools used in wgd, please consult the documentation at
-        https://wgd.readthedocs.io/en/latest/index.html#citation.
-        
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center">
+
+# `wgd v2` : a suite tool of WGD inference and timing
+
+[![Build Status](https://app.travis-ci.com/heche-psb/wgd.svg?branch=phylodating)](https://app.travis-ci.com/heche-psb/wgd)
+[![Documentation Status](https://readthedocs.org/projects/wgdv2/badge/?version=latest)](https://wgdv2.readthedocs.io/en/latest/?badge=latest)
+[![license](https://img.shields.io/pypi/l/wgd.svg)](https://pypi.python.org/pypi/wgd)
+[![Latest PyPI version](https://img.shields.io/pypi/v/wgd.svg)](https://pypi.python.org/pypi/wgd)
+[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/wgd/README.html)
+[![Downloads](https://pepy.tech/badge/wgd)](https://pepy.tech/project/wgd)
+
+**Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
+
+[**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
+
+[**Introduction**](#Introduction) | 
+[**Installation**](#Installation) | 
+[**Parameters**](#Parameters) | 
+[**Usage**](#Usage) | 
+[**Illustration**](#Illustration) |
+[**Documentation**](https://wgdv2.readthedocs.io/en/latest/?badge=latest) |
+[**Citation**](#Citation)
+
+
+</div>
+
+`wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
+
+## Introduction
+
+Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
+
+The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
+
+## Installation
+
+The easiest way to install `wgd v2` is using PYPI
+
+```
+pip install wgd
+```
+
+To install `wgd v2` in a virtual environment, the following command lines could be used.
+
+```
+git clone <wgd repo>
+cd wgd
+virtualenv -p=python3 ENV (or python3 -m venv ENV)
+source ENV/bin/activate
+pip install -r requirements.txt
+pip install .
+```
+
+When met with permission problem in installation, please try the following command line.
+
+```
+pip install -e .
+```
+
+If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
+
+```
+export PATH="$PATH:~/.local/bin/wgd"
+```
+
+Note that the version of `numpy` is important (for many other packages are the same of course), especially for `fastcluster` package. In our test, the `numpy` 1.19.0 works fine on `python3.6/8`. If you met some errors or warnings about numpy, maybe considering pre-install `numpy` as 1.19.0 or other close-by versions before you install `wgd`.
+
+## Parameters
+
+There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
+
+The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
+```
+wgd dmd sequences (option)
+--------------------------------------------------------------------------------
+-o, --outdir, the output directory, default wgd_dmd
+-t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+-c, --cscore, the c-score to restrict the homologs of MRBHs, default None, if None was given, the c-score funcion won't be activated
+-I, --inflation, the inflation factor for MCL program, default 2.0
+-e, --eval, the e-value cut-off for similarity in diamond and/or hmmer, default 1e-10
+--to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+--cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+-f, --focus, the species to be merged on local MRBHs, default None, if None was given, the local MRBHs won't be inferred
+-ap, --anchorpoints, the anchor points data file, default None
+-coc, --collinearcoalescence, flag option, whether to initiate the collinear coalescence analysis, if the flag was set, the analysis will be initiated
+-sm, --segments, the segments data file used in collinear coalescence analysis if initiated, default None
+-le, --listelements, the listsegments data file used in collinear coalescence analysis if initiated, default None
+-gt, --genetable, the gene table datafile used in collinear coalescence analysis if initiated, default None
+-kf, --keepfasta, flag option, whether to output the sequence information of MRBHs, if the flag was set, the sequences of MRBHs will be in output
+-kd, --keepduplicates, flag option, whether to allow the same gene to occur in different MRBHs, if the flag was set, the same gene can be assigned to different MRBHs
+-gm, --globalmrbh, flag option, whether to initiate global MRBHs construction, if the flag was set, the --focus option will be ignored and only global MRBHs will be built
+-n, --nthreads, the number of threads to use, default 4
+-oi, --orthoinfer, flag option, whether to initiate orthogroup infernece, if the flag was set, the orthogroup infernece program will be initiated
+-oo, --onlyortho, flag option, whether to only conduct orthogroup infernece, if the flag was set, only the orthogroup infernece program will be conducted while the other analysis won't be initiated
+-gn, --getnsog, flag option, whether to initiate the searching for nested single-copy gene families (NSOGs), if the flag was set, additional NSOGs analysis will be performed besides the basic orthogroup infernece
+-tree, --tree_method, which gene tree inference program to invoke, default fasttree
+-ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
+-mc, --msogcut, the ratio cutoff for mostly single-copy family and species representation in collinear coalescence inference, default 0.8.
+-ga, --geneassign, flag option, whether to initiate the gene-to-family assignment analysis, if the flag was set, the analysis will be initiated
+-am, --assign_method, which method to conduct the gene-to-family assignment analysis, default hmmer
+-sa, --seq2assign, the queried sequences data file in gene-to-family assignment analysis, default None, this option can be provided multiple times
+-fa, --fam2assign, the queried familiy data file in gene-to-family assignment analysis, default None
+-cc, --concat, flag option, whether to initiate the concatenation pipeline for orthogroup infernece, if the flag was set, the analysis will be initiated
+-te, --testsog, flag option, whether to initiate the unbiased test of single-copy gene families, if the flag was set, the analysis will be initiated
+-bs, --bins, the number of bins divided in gene length normalization, default 100
+-np, --normalizedpercent, the percentage of upper hits used for gene length normalization, default 5
+-nn, --nonormalization, flag option, whether to call off the normalization, if the flag was set, no normalization will be conducted
+-bsog, --buscosog, flag option, whether to initiate the busco-guided single-copy gene family analysis, if the flag was set, the analysis will be initiated
+-bhmm, --buscohmm, the HMM profile datafile in the busco-guided single-copy gene family analysis, default None
+-bctf, --buscocutoff, the HMM score cutoff datafile in the busco-guided single-copy gene family analysis, default None
+```
+
+The program `wgd focus` can realize the concatenation-based and coalescence-based phylogenetic inference, functional annotation of gene families and phylogenetic dating of WGDs.
+```
+wgd focus families sequences (option)
+--------------------------------------------------------------------------------
+-o, --outdir, the output directory, default wgd_focus
+-t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+-n, --nthreads, the number of threads to use, default 4
+--to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+--cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+--strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
+-a, --aligner, which alignment program to use, default mafft
+-tree, --tree_method, which gene tree inference program to invoke, default fasttree
+-ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
+--concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
+--coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
+-sp, --speciestree, species tree datafile for dating, default None
+-d, --dating, which molecular dating program to use, default none
+-ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
+-ns, --nsites, the nsites information for r8s dating, default None
+-ot, --outgroup, the outgroup information for r8s dating, default None
+-pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
+-am, --aamodel, which protein model to be used in mcmctree, default poisson
+-ks, flag option, whether to initiate Ks calculation
+--annotation, which annotation program to use, default None
+--pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
+-ed, --eggnogdata, the eggnog annotation datafile, default None
+--pfam, which option to use for pfam annotation, default None
+--dmnb, the diamond database for annotation, default None
+--hmm, the HMM profile for annotation, default None
+--evalue, the e-value cut-off for annotation, default 1e-10
+--exepath, the path to the interproscan executable, default None
+-f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
+ -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
+-cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
+--beastlgjar, the path to beastLG.jar, default None
+--beagle, flag option, whether to use beagle in Beast, if the flag was set, beagle will be used
+--protdating, flag option, whether to only initiate the protein-concatenation based dating analysis, if the flag was set, the analysis will be initiated
+```
+
+The program `wgd ksd` can realize the construction of *K*<sub>S</sub> age distribution and rate correction.
+```
+wgd ksd families sequences (option)
+--------------------------------------------------------------------------------
+-o, --outdir, the output directory, default wgd_ksd
+-t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+-n, --nthreads, the number of threads to use, default 4
+--to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+--cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+--pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
+--strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
+-tree, --tree_method, which gene tree inference program to invoke, default fasttree
+-sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
+-sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
+-rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
+-or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+-epk, --extraparanomeks, extra paranome Ks data to plot in the mixed Ks distribution, default None
+-ap, --anchorpoints, anchorpoints.txt file to plot anchor Ks in the mixed Ks distribution, default None
+-pk, --plotkde, flag option, whether to plot kde curve of orthologous Ks distribution over histogram in the mixed Ks distribution, if the flag was set, the kde curve will be plotted
+-pag, --plotapgmm, flag option, whether to plot mixture modeling of anchor Ks in the mixed Ks distribution, if the flag was set, the mixture modeling of anchor Ks will be plotted
+-pem, --plotelmm, flag option, whether to plot elmm mixture modeling of paranome Ks in the mixed Ks distribution, if the flag was set, the elmm mixture modeling of paranome Ks will be plotted
+-c, --components, the range of the number of components to fit in anchor Ks mixture modeling, default (1,4)
+```
+
+The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
+```
+wgd mix ks_datafile (option)
+--------------------------------------------------------------------------------
+-f, --filters, the cutoff alignment length, default 300
+-r, --ks_range, the Ks range to be considered, default (0, 5)
+-b, --bins, the number of bins in Ks distribution, default 50
+-o, --outdir, the output directory, default wgd_mix
+--method, which mixture model to use, default gmm
+-n, --components, the range of the number of components to fit, default (1, 4)
+-g, --gamma, the gamma parameter for bgmm models, default 0.001
+-ni, --n_init, the number of k-means initializations, default 200
+-mi, --max_iter, the maximum number of iterations, default 1000
+```
+
+The program `wgd peak` can realize the search of crediable *K*<sub>S</sub> range used in WGD dating.
+```
+wgd peak ks_datafile (option)
+--------------------------------------------------------------------------------
+-ap, --anchorpoints, the anchor points datafile, default None
+-sm, --segments, the segments datafile, default None
+-le, --listelements, the listsegments datafile, default None 
+-mp, --multipliconpairs, the multipliconpairs datafile, default None
+-o, --outdir, the output directory, default wgd_peak
+-af, --alignfilter, cutoff for alignment identity, length and coverage, default 0.0, 0, 0.0
+-r, --ksrange, range of Ks to be analyzed, default (0, 5)
+-bw, --bin_width, bandwidth of Ks distribution, default 0.1
+-ic, --weights_outliers_included, flag option, whether to include Ks outliers, if the flag was set, Ks outliers will be included in the analysis
+-m, --method, which mixture model to use, default gmm
+--seed, random seed given to initialization, default 2352890
+-ei, --em_iter, the number of EM iterations to perform, default 200
+-ni, --n_init, the number of k-means initializations, default 200
+-n, --components, the range of the number of components to fit, default (1, 4)
+--boots, the number of bootstrap replicates of kde, default 200
+--weighted, flag option, whether to use node-weighted method of de-redundancy, if the flag was set, the node-weighted method will be used
+-p, --plot, the plotting method to be used, default identical
+-bm, --bw_method, the bandwidth method to be used, default silverman
+--n_medoids, the number of medoids to fit, default 2
+-km, --kdemethod, the kde method to be used, default scipy
+--n_clusters, the number of clusters to plot Elbow loss function, default 5
+--kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
+-gd, --guide, the regime residing anchors, default: segment
+-prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
+-kd, --kstodate, the range of Ks to be dated in heuristic search, default (0.5, 1.5)
+-f, --family, the family to filter Ks upon, default None
+--manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
+-rh, --rel_height, the relative height at which the peak width is measured, default 0.4
+--ci, the confidence level of log-normal distribution to date, default 95
+--hdr, the highest density region (HDR) in a given distribution to date, default 95
+--heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
+-kc, --kscutoff, the Ks saturation cutoff in dating, default 5
+-g, --gamma, the gamma parameter for bgmm models, default 1e-3
+```
+
+The program `wgd syn` can realize the intra- and inter-specific synteny inference.
+```
+wgd syn families gffs (option)
+--------------------------------------------------------------------------------
+-ks, --ks_distribution, ks distribution datafile, default None
+-o, --outdir, the output directory, default wgd_syn
+-f, --feature, the feature for parsing gene IDs from GFF files, default gene
+-a, --attribute, the attribute for parsing the gene IDs from the GFF files, default ID
+-ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
+-ms, --maxsize, the maximum family size to include, default 200
+-r, --ks_range, the Ks range in colored dotplot, default (0, 5)
+--iadhore_options, the parameter setting in iadhore, default 
+-ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
+-mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
+-kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+```
+
+The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
+```
+wgd viz (option)
+--------------------------------------------------------------------------------
+-d, --datafile, the Ks datafile, default None
+-o, --outdir, the output directory, default wgd_viz
+-sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
+-gs, --gsmap, the gene name-species name map, default None
+-sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
+-pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
+-rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
+-or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+-iter, --em_iterations, the maximum EM iterations, default 200
+-init, --em_initializations, the maximum EM initializations, default 200
+-prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
+-sm, --segments, the segments data file, default None
+-ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffolds will be set
+-ms, --maxsize, the maximum family size to include, default 200
+-ap, --anchorpoints, the anchor points datafile, default None
+-mt, --multiplicon, the multiplicons datafile, default None
+-gt, --genetable, the gene table datafile, default None
+-rh, --rel_height, the relative height at which the peak width is measured, default 0.4
+-mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
+-kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+-epk, --extraparanomeks, extra paranome Ks data to plot in the mixed Ks distribution, default None
+-pag, --plotapgmm, flag option, whether to plot mixture modeling of anchor Ks in the mixed Ks distribution, if the flag was set, the mixture modeling of anchor Ks will be plotted
+-pem, --plotelmm, flag option, whether to plot elmm mixture modeling of paranome Ks in the mixed Ks distribution, if the flag was set, the elmm mixture modeling of paranome Ks will be plotted
+-c, --components, the range of the number of components to fit in anchor Ks mixture modeling, default (1,4)
+```
+
+## Usage
+
+Here we provided the basic usage for each program.
+
+### wgd dmd
+
+**The delineation of whole paranome**
+```
+wgd dmd sequence
+``` 
+
+**The delineation of RBHs**
+```
+wgd dmd sequence1 sequence2
+```
+
+**The delineation of local MRBHs**
+```
+wgd dmd sequence1 sequence2 sequence3 -f sequence1
+```
+
+**The delineation of global MRBHs**
+```
+wgd dmd sequence1 sequence2 sequence3 -gm
+```
+
+**The delineation of orthogroups**
+```
+wgd dmd sequence1 sequence2 sequence3 -oi (option)
+```
+Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
+
+**The collinear coalescence inference of phylogeny**
+```
+wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
+```
+
+Note that there should be no duplicated gene IDs in the sequence file.
+
+### wgd focus
+
+**The concatenation-based/coalescence-based phylogenetic inference**
+```
+wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
+```
+
+**The functional annotation of gene families**
+```
+wgd focus families sequence1 sequence2 sequence3 --annotation eggnog -ed eddata --dmnb dbdata
+```
+
+**The phylogenetic dating of WGDs**
+```
+wgd focus families sequence1 sequence2 sequence3 -d mcmctree -sp spdata
+```
+
+### wgd ksd
+
+**The construction of whole paranome *K*<sub>S</sub> age distribution**
+```
+wgd ksd families sequence
+```
+
+**The construction of orthologous *K*<sub>S</sub> age distribution**
+```
+wgd ksd families sequence1 sequence2
+```
+
+**The construction of *K*<sub>S</sub> age distribution with rate correction**
+```
+wgd ksd families sequence1 sequence2 sequence3 -sr srdata -sp spdata
+```
+
+### wgd mix
+
+**The mixture model clustering analysis of *K*<sub>S</sub> age distribution**
+```
+wgd mix ksdata
+```
+
+### wgd peak
+
+**The search of crediable *K*<sub>S</sub> range used in WGD dating**
+```
+wgd peak ksdata -ap apdata -sm smdata -le ledata -mp mpdata
+```
+Note that users can add the flag --heuristic to implement the heuristic search analysis
+
+### wgd syn
+
+**The intra-specific synteny inference**
+```
+wgd syn families gff
+```
+
+**The inter-specific synteny inference**
+```
+wgd syn families gff1 gff2
+```
+
+### wgd viz
+
+**The visualization of *K*<sub>S</sub> age distribution**
+```
+wgd viz -d ksdata
+```
+
+**The visualization of *K*<sub>S</sub> age distribution with rate correction**
+```
+wgd viz -d ksdata -sr srdata -sp spdata -gs gsdata
+```
+
+**The visualization of synteny**
+```
+wgd viz -ap apdata -sm smdata -mt mtdata -gt gtdata
+```
+
+## Illustration
+
+We illustrate our program on an exemplary WGD inference and dating upon species *Aquilegia coerulea*.
+
+The *Aquilegia coerulea* was reported to experience an paleo-polyploidization event after the divergence of core eudicots, which is likely shared by all Ranunculales.
+
+First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
+
+```
+wgd dmd Aquilegia_coerulea
+wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
+```
+
+The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1 but not clear.
+
+![](data/Aquilegia_coerulea.tsv.ksd_wp.svg)
+
+We then construct the anchor *K*<sub>S</sub> age distribution using the command line below.
+
+```
+wgd syn -f mRNA -a Name wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea.gff3 -ks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+```
+
+As shown below, there are some retained anchor pairs with *K*<sub>S</sub> between 1 and 2, which seems to suggest a WGD event.
+
+![](data/Aquilegia_coerulea.tsv.ksd_wp_ap.svg)
+
+The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes.
+
+![](data/Aquilegia_coerulea_Aquilegia_coerulea_multiplicons_level.svg)
+
+We implemented two types of dot plots in oxford grid: one in the unit of bases and the other in the unit of genes, which can be colored by *K*<sub>S</sub> values given *K*<sub>S</sub> data.
+
+![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea_Ks.dot_unit_gene.png)
+
+As shown above, the dot plot in the unit of genes presents numerous densely aggregated (line-like) anchor points at most of the chromosomes with consistent *K*<sub>S</sub> age between 1 and 2. The dot plot in the unit of bases shows the same pattern, as manifested below.
+
+![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea_Ks.dot.png)
+
+The dot plots without *K*<sub>S</sub> annotation will also be automately produced, as shown below.
+
+![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot_unit_gene.png)
+
+![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
+
+A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
+
+![](data/Syndepth.svg)
+
+We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
+
+```
+wgd viz -d wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+```
+
+The result of ELMM mixture model clustering shows that there is a likely WGD component at *K*<sub>S</sub> 1.19.
+
+![](data/elmm_Aquilegia_coerulea.tsv.ks.tsv_best_models_weighted.svg)
+
+Let's do a mixture model clustering for anchor *K*<sub>S</sub> too, using the command line below.
+
+```
+wgd peak wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv --anchorpoints wgd_syn/iadhore-out/anchorpoints.txt --segments wgd_syn/iadhore-out/segments.txt --listelements wgd_syn/iadhore-out/list_elements.txt --multipliconpairs wgd_syn/iadhore-out/multiplicon_pairs.txt --weighted
+```
+
+The anchor *K*<sub>S</sub> age distribution also has a likely WGD component with mode 1.28.
+
+![](data/Original_AnchorKs_GMM_Component3_node_weighted_Lognormal.svg)
+
+Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis. First, we built a global MRBH family using the command below.
+
+```
+wgd dmd --globalmrbh Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera -o wgd_globalmrbh
+```
+
+In the global MRBH family, every pair of orthologous genes is the reciprocal best hit, suggesting true orthologous relationships. We would use the *K*<sub>S</sub> values associated with these orthologous pairs to delimit the divergence *K*<sub>S</sub> peak. Together with the whole paranome *K*<sub>S</sub> distribution, we conduct the rate correction using the command below.
+
+```
+wgd ksd wgd_globalmrbh/global_MRBH.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
+```
+
+The file `speciestree.nw` is the text file of species tree in newick that rate correction would be conducted on. Its content is as below. Users need to provide the species pairs to be plotted. We suggest adding the option `--reweight` to recalculate the weight per species pair such that the weight of orthologous gene pairs will become 1 as the paralogous gene pairs. The flag `--plotkde` can be added when the kde curve of orthologous *K*<sub>S</sub> is desired. Extra collinear data can be added by the option `-ap`.
+
+```
+(((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
+```
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
+
+As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
+
+If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
+```
+
+Note that we can easily show that *Aquilegia coerulea* has higher substitution rate than *Protea cynaroides* and *Vitis vinifera* by comparing their substitution distance in regard to the same divergence event with outgroup species *Acorus_americanus*, using command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_viz_Compare_rate --spair "Acorus_americanus;Protea_cynaroides" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Vitis_vinifera;Acorus_americanus" --gsmap gene_species.map --plotkde
+```
+
+![](data/Raw_Orthologues_Compare_rate.ksd.svg)
+
+As displayed above, the orthologous *K*<sub>S</sub> values bewteen *Aquilegia coerulea* and *Acorus americanus* has the highest mode, indicatingthe faster substitution rate of *Aquilegia coerulea* compared to *Protea cynaroides* and *Vitis vinifera*.
+
+Note that a necessary gene-species map file is needed for its implementation in `wgd viz`, which should be automately produced by the last `wgd ksd` step. The `gene_species.map` has contents as below in which each line is the joined string of gene name and species name by space.
+
+```
+Aqcoe6G057800.1 Aquilegia_coerulea
+Vvi_VIT_201s0011g01530.1 Vitis_vinifera
+Pcy_Procy01g08510 Protea_cynaroides
+Aam_Acora.04G142900.1 Acorus_americanus
+```
+
+A more complex plot can be made by add the flag `--plotelmm` such that the ELMM mixture modeling of provided paranome *K*<sub>S</sub> can be superimposed, using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm
+```
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Corrected.ksd.svg)
+
+From the mixed *K*<sub>S</sub> plot above, we can see that the optimized lognormal component b with mode 1.2 is younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera* (1.39 and 1.47, respectively).
+
+Besides, we can also add the GMM mixture modeling of anchor *K*<sub>S</sub> values with the flag `--plotapgmm`, using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotapgmmm
+```
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Apgmm_Corrected.ksd.svg)
+
+As manifested above, the anchor *K*<sub>S</sub> component 2 with mode 1.28 is also younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera*. But we need to be of course cautious that such distinction comes with the uncertainties introduced from the applied mixture modeling methodology in terms of for instance different initialization points and the issue of overfitting and the sister speciess adopted in that there might be species with more disparate substitution rates than the one we chose.
+
+Adding both ELMM result for paranome and GMM result for anchor *K*<sub>S</sub> can be achieved just by add the two flags mentioned above, using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm --plotapgmmm
+```
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Apgmm_Corrected.ksd.svg)
+
+An alternative way to calculate the orthologous *K*<sub>S</sub> is to directly use the orthogroups instead of global MRBH family. That way we don't use the pre-inferred paranome *K*<sub>S</sub> but the paralogous gene pairs inside each orthogroup instead. To achieve that, we first need to infer orthogroups using the command below.
+
+```
+wgd dmd Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera --orthoinfer -o wgd_ortho (--onlyortho) 
+```
+
+Users can decide to only conduct the orthogroup analysis while skipping other analysis by adding the flag `--onlyortho`. Next step is the same with global MRBH family except that we don't use the extra pre-inferred paranome *K*<sub>S</sub> anymore. We infer the *K*<sub>S</sub> using the command below. Note that the program `wgd viz` can plot the same just as shown above.
+
+```
+wgd ksd wgd_ortho/Orthogroups.sp.tsv -sp speciestree.nw --reweight -o wgd_ortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
+```
+
+![](data/Aquilegia_coerulea_OrthoKs_Corrected.ksd.svg)
+
+As shown above, the number of both paralogous gene pairs and orthologous gene pairs is different than the one from global MRBH family in that here we plotted all orthologous gene pairs instead of only global MRBH and potentially new paralogous gene pairs might be produced in the orthogroup inference step, together with different recalculated weights.
+
+If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, as we have already shown above, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --gsmap gene_species.map
+```
+
+We can clearly see that *Vitis vinifera* has higher substitution rate than *Protea cynaroides* in that their orthologous *K*<sub>S</sub> peaks with *Aquilegia coerulea*, although representing the same divergence event, differed in substitution distance.
+![](data/Raw_Orthologues.ksd.svg)
+
+After the phylogenetic timing of the Ranunculales WGD, we can further infer its absolute age. First we infer the credible range of anchor pairs by *K*<sub>S</sub> heuristically using the program `wgd peak`.
+
+```
+wgd peak --heuristic wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -ap wgd_syn/iadhore-out/anchorpoints.txt -sm wgd_syn/iadhore-out/segments.txt -le wgd_syn/iadhore-out/list_elements.txt -mp wgd_syn/iadhore-out/multiplicon_pairs.txt -o wgd_peak
+```
+
+![](data/AnchorKs_PeakCI_Aquilegia_coerulea.tsv.ks.tsv_node_weighted.svg)
+
+As shown above, we assumed a lognormal distribution at the peak location detected by the `signal` module of `scipy` library. The 95% confidence level of the lognormal distribution was applied, i.e., 0.68-2.74, in further molecular dating. The file `Aquilegia_coerulea.tsv.ks.tsv_95%CI_AP_for_dating_weighted_format.tsv` is what we need for next step. To build the orthogroups used in phylogenetic dating, we need to select some species and form a starting tree with proper fossil calibrations. We provide one in mcmctree format as below.
+
+```
+17 1
+((((Potamogeton_acutifolius,(Spirodela_intermedia,Amorphophallus_konjac)),(Acanthochlamys_bracteata,(Dioscorea_alata,Dioscorea_rotundata))'>0.5600<1.2863')'>0.8360<1.2863',(Acorus_americanus,Acorus_tatarinowii))'>0.8360<1.2863',((((Tetracentron_sinense,Trochodendron_aralioides),(Buxus_austroyunnanensis,Buxus_sinica))'>1.1080<1.2863',(Nelumbo_nucifera,(Telopea_speciosissima,Protea_cynaroides)))'>1.1080<1.2863',(Aquilegia_coerulea_ap1,Aquilegia_coerulea_ap2))'>1.1080<1.2863')'>1.2720<2.4720';
+```
+
+As presented above, the focus species that is about to be dated needs to be replaced with `(Aquilegia_coerulea_ap1,Aquilegia_coerulea_ap2)`. With this starting tree and predownloaded cds files of all the species, we can build the orthogroup used in the final molecular dating using the command as below.
+
+```
+wgd dmd -f Aquilegia_coerulea -ap wgd_peak/Aquilegia_coerulea.tsv.ks.tsv_95%CI_AP_for_dating_weighted_format.tsv -o wgd_dmd_ortho Potamogeton_acutifolius Spirodela_intermedia Amorphophallus_konjac Acanthochlamys_bracteata Dioscorea_alata Dioscorea_rotundata Acorus_americanus Acorus_tatarinowii Tetracentron_sinense Trochodendron_aralioides Buxus_austroyunnanensis Buxus_sinica Nelumbo_nucifera Telopea_speciosissima Protea_cynaroides Aquilegia_coerulea
+```
+
+The result file `merge_focus_ap.tsv` is what we need for the final step of molecular dating in program `wgd focus`.
+
+```
+wgd focus --protdating --aamodel lg wgd_dmd_ortho/merge_focus_ap.tsv -sp dating_tree.nw -o wgd_dating -d mcmctree -ds 'burnin = 2000' -ds 'sampfreq = 1000' -ds 'nsample = 20000' Potamogeton_acutifolius Spirodela_intermedia Amorphophallus_konjac Acanthochlamys_bracteata Dioscorea_alata Dioscorea_rotundata Acorus_americanus Acorus_tatarinowii Tetracentron_sinense Trochodendron_aralioides Buxus_austroyunnanensis Buxus_sinica Nelumbo_nucifera Telopea_speciosissima Protea_cynaroides Aquilegia_coerulea
+```
+
+Here we only implemented the concatenation analysis using protein sequence by adding the flag `--protdating` and we set the parameter for `mcmctree` via the option `-ds`. Note that other dating program such as `r8s` and `beast` are also available given some mandatory parameters. The final log of the successful run is as below.
+
+```
+16:04:25 INFO     Running mcmctree using Hessian matrix of LG+Gamma  core.py:967
+                  for protein model
+23:49:37 INFO     Posterior mean for the ages of wgd is 1.128945 mcmctree.py:296
+                  billion years from Concatenated peptide
+                  alignment and 95% credibility intervals (CI)
+                  is 1.01224-1.23121 billion years
+         INFO     Total run time: 29175s                              cli.py:241
+         INFO     Done                                                cli.py:242
+```
+
+To visualize the date, we also provided a python script to plot the WGD dates in the `wgd` folder. Users need to extract the raw dates from the `mcmc.txt` for the WGD node first and save it as file `dates.txt` (or whatever preferred name). An example command is as below.
+
+```
+python $PATH/postplot.py postdis dates.txt --percentile 90 --title "WGD date" --hpd -o "Ranunculales_WGD_date.svg"
+```
+
+![](data/Ranunculales_WGD_date.svg)
+
+The posterior mean, median and mode of the Ranunculales WGD age is 112.92, 113.44 and 112.54 mya, with 90% HPD 105.07 - 122.32 mya as manifested above.
+
+## Citation
+ 
+Please cite us at https://doi.org/10.1093/bioinformatics/bty915
+
+```
+Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
+
+Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
+```
+
+For citation of the tools used in wgd, please consult the documentation at
+https://wgdv2.readthedocs.io/en/latest/citation.html.
+
```

### Comparing `wgd-2.0.16/wgd.egg-info/requires.txt` & `wgd-2.0.17/wgd.egg-info/requires.txt`

 * *Files identical despite different names*

