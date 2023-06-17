# Comparing `tmp/PyQt6_QScintilla-2.14.0.tar.gz` & `tmp/PyQt6_QScintilla-2.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQt6_QScintilla-2.14.0.tar", last modified: Thu Apr 27 16:09:49 2023, max compression
+gzip compressed data, was "PyQt6_QScintilla-2.14.1.tar", last modified: Wed Jun  7 15:38:43 2023, max compression
```

## Comparing `PyQt6_QScintilla-2.14.0.tar` & `PyQt6_QScintilla-2.14.1.tar`

### file list

```diff
@@ -1,451 +1,451 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.664997 PyQt6_QScintilla-2.14.0/
--rw-r--r--   0 phil       (501) staff       (20)   243812 2023-04-27 16:09:48.659561 PyQt6_QScintilla-2.14.0/ChangeLog
--rw-r--r--   0 phil       (501) staff       (20)    35147 2023-04-27 16:09:47.663220 PyQt6_QScintilla-2.14.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)    28049 2023-04-27 15:54:13.221252 PyQt6_QScintilla-2.14.0/NEWS
--rw-r--r--   0 phil       (501) staff       (20)     1911 2023-04-27 16:09:49.665136 PyQt6_QScintilla-2.14.0/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1564 2023-04-27 16:09:48.942340 PyQt6_QScintilla-2.14.0/README
--rw-r--r--   0 phil       (501) staff       (20)     7485 2023-04-27 16:09:48.985963 PyQt6_QScintilla-2.14.0/project.py
--rw-r--r--   0 phil       (501) staff       (20)      553 2023-04-27 16:09:48.941855 PyQt6_QScintilla-2.14.0/pyproject.toml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.608302 PyQt6_QScintilla-2.14.0/qsci/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.608352 PyQt6_QScintilla-2.14.0/qsci/api/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.614210 PyQt6_QScintilla-2.14.0/qsci/api/python/
--rw-r--r--   0 phil       (501) staff       (20)   172772 2023-04-27 15:54:13.263872 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-2.4.api
--rw-r--r--   0 phil       (501) staff       (20)   199839 2023-04-27 15:54:13.263463 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-2.5.api
--rw-r--r--   0 phil       (501) staff       (20)   191764 2023-04-27 15:54:13.259922 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-2.6.api
--rw-r--r--   0 phil       (501) staff       (20)   192152 2023-04-27 15:54:13.262933 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-2.7.api
--rw-r--r--   0 phil       (501) staff       (20)   175453 2023-04-27 15:54:13.262669 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.1.api
--rw-r--r--   0 phil       (501) staff       (20)   233448 2023-04-27 15:54:13.263802 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.10.api
--rw-r--r--   0 phil       (501) staff       (20)   243538 2023-04-27 15:54:13.263478 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.11.api
--rw-r--r--   0 phil       (501) staff       (20)   156049 2023-04-27 15:54:13.263519 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.2.api
--rw-r--r--   0 phil       (501) staff       (20)   254493 2023-04-27 15:54:13.278213 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.3.api
--rw-r--r--   0 phil       (501) staff       (20)   246543 2023-04-27 15:54:13.263311 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.4.api
--rw-r--r--   0 phil       (501) staff       (20)   238049 2023-04-27 15:54:13.275161 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.5.api
--rw-r--r--   0 phil       (501) staff       (20)   234256 2023-04-27 15:54:13.269879 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.6.api
--rw-r--r--   0 phil       (501) staff       (20)   233756 2023-04-27 15:54:13.269916 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.7.api
--rw-r--r--   0 phil       (501) staff       (20)   235810 2023-04-27 15:54:13.269971 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.8.api
--rw-r--r--   0 phil       (501) staff       (20)   227832 2023-04-27 15:54:13.266211 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.9.api
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.562578 PyQt6_QScintilla-2.14.0/scintilla/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.552287 PyQt6_QScintilla-2.14.0/scintilla/include/
--rw-r--r--   0 phil       (501) staff       (20)     4124 2023-04-27 15:54:13.238178 PyQt6_QScintilla-2.14.0/scintilla/include/ILexer.h
--rw-r--r--   0 phil       (501) staff       (20)      607 2023-04-27 15:54:13.236543 PyQt6_QScintilla-2.14.0/scintilla/include/ILoader.h
--rw-r--r--   0 phil       (501) staff       (20)      854 2023-04-27 15:54:13.218300 PyQt6_QScintilla-2.14.0/scintilla/include/License.txt
--rw-r--r--   0 phil       (501) staff       (20)    15732 2023-04-27 15:54:13.238441 PyQt6_QScintilla-2.14.0/scintilla/include/Platform.h
--rw-r--r--   0 phil       (501) staff       (20)    52975 2023-04-27 15:54:13.255597 PyQt6_QScintilla-2.14.0/scintilla/include/SciLexer.h
--rw-r--r--   0 phil       (501) staff       (20)      822 2023-04-27 15:54:13.237904 PyQt6_QScintilla-2.14.0/scintilla/include/Sci_Position.h
--rw-r--r--   0 phil       (501) staff       (20)    39252 2023-04-27 15:54:13.251609 PyQt6_QScintilla-2.14.0/scintilla/include/Scintilla.h
--rw-r--r--   0 phil       (501) staff       (20)   151936 2023-04-27 15:54:13.246147 PyQt6_QScintilla-2.14.0/scintilla/include/Scintilla.iface
--rw-r--r--   0 phil       (501) staff       (20)     2646 2023-04-27 15:54:13.242743 PyQt6_QScintilla-2.14.0/scintilla/include/ScintillaWidget.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.548966 PyQt6_QScintilla-2.14.0/scintilla/lexers/
--rw-r--r--   0 phil       (501) staff       (20)    12485 2023-04-27 15:54:13.242410 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexA68k.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7680 2023-04-27 15:54:13.239503 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAPDL.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7365 2023-04-27 15:54:13.239854 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexASY.cpp
--rw-r--r--   0 phil       (501) staff       (20)    29486 2023-04-27 15:54:13.241423 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAU3.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6762 2023-04-27 15:54:13.239403 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAVE.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8571 2023-04-27 15:54:13.237915 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAVS.cpp
--rw-r--r--   0 phil       (501) staff       (20)    19666 2023-04-27 15:54:13.240012 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAbaqus.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11716 2023-04-27 15:54:13.256846 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAda.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13719 2023-04-27 15:54:13.239256 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAsm.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5275 2023-04-27 15:54:13.252788 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAsn1.cpp
--rw-r--r--   0 phil       (501) staff       (20)    30635 2023-04-27 15:54:13.247915 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBaan.cpp
--rw-r--r--   0 phil       (501) staff       (20)    27588 2023-04-27 15:54:13.244645 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBash.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16591 2023-04-27 15:54:13.243983 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBasic.cpp
--rw-r--r--   0 phil       (501) staff       (20)    17352 2023-04-27 15:54:13.240788 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBatch.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8737 2023-04-27 15:54:13.241023 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBibTeX.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6474 2023-04-27 15:54:13.242658 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBullant.cpp
--rw-r--r--   0 phil       (501) staff       (20)    22108 2023-04-27 15:54:13.240934 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCLW.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12466 2023-04-27 15:54:13.239317 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCOBOL.cpp
--rw-r--r--   0 phil       (501) staff       (20)    58102 2023-04-27 15:54:13.243039 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCPP.cpp
--rw-r--r--   0 phil       (501) staff       (20)    18495 2023-04-27 15:54:13.257892 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCSS.cpp
--rw-r--r--   0 phil       (501) staff       (20)    14510 2023-04-27 15:54:13.240688 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCaml.cpp
--rw-r--r--   0 phil       (501) staff       (20)    15711 2023-04-27 15:54:13.254063 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCmake.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16780 2023-04-27 15:54:13.249365 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCoffeeScript.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5705 2023-04-27 15:54:13.245799 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexConf.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7221 2023-04-27 15:54:13.245325 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCrontab.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6336 2023-04-27 15:54:13.241978 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCsound.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16777 2023-04-27 15:54:13.242696 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexD.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9146 2023-04-27 15:54:13.244061 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexDMAP.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8358 2023-04-27 15:54:13.242147 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexDMIS.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6360 2023-04-27 15:54:13.240565 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexDiff.cpp
--rw-r--r--   0 phil       (501) staff       (20)    15652 2023-04-27 15:54:13.244655 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexECL.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9531 2023-04-27 15:54:13.259121 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexEDIFACT.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8188 2023-04-27 15:54:13.242100 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexEScript.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7601 2023-04-27 15:54:13.255433 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexEiffel.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16475 2023-04-27 15:54:13.250724 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexErlang.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13292 2023-04-27 15:54:13.247434 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexErrorList.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12296 2023-04-27 15:54:13.246526 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexFlagship.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5318 2023-04-27 15:54:13.243277 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexForth.cpp
--rw-r--r--   0 phil       (501) staff       (20)    24685 2023-04-27 15:54:13.244503 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexFortran.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6977 2023-04-27 15:54:13.245578 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexGAP.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8904 2023-04-27 15:54:13.243539 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexGui4Cli.cpp
--rw-r--r--   0 phil       (501) staff       (20)    81836 2023-04-27 15:54:13.243810 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexHTML.cpp
--rw-r--r--   0 phil       (501) staff       (20)    36346 2023-04-27 15:54:13.247195 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexHaskell.cpp
--rw-r--r--   0 phil       (501) staff       (20)    29024 2023-04-27 15:54:13.261376 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexHex.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2500 2023-04-27 15:54:13.243561 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexIndent.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8369 2023-04-27 15:54:13.256471 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexInno.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13704 2023-04-27 15:54:13.252060 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexJSON.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16299 2023-04-27 15:54:13.248659 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexKVIrc.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3747 2023-04-27 15:54:13.247771 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexKix.cpp
--rw-r--r--   0 phil       (501) staff       (20)    28943 2023-04-27 15:54:13.245085 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLPeg.cpp
--rw-r--r--   0 phil       (501) staff       (20)    15494 2023-04-27 15:54:13.245963 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLaTeX.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8300 2023-04-27 15:54:13.247012 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLisp.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6042 2023-04-27 15:54:13.245231 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLout.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16099 2023-04-27 15:54:13.245523 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLua.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5444 2023-04-27 15:54:13.248148 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMMIXAL.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5257 2023-04-27 15:54:13.263030 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMPT.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11271 2023-04-27 15:54:13.244978 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMSSQL.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13633 2023-04-27 15:54:13.257633 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMagik.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4391 2023-04-27 15:54:13.253264 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMake.cpp
--rw-r--r--   0 phil       (501) staff       (20)    15564 2023-04-27 15:54:13.250039 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMarkdown.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12124 2023-04-27 15:54:13.248924 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMatlab.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4997 2023-04-27 15:54:13.246245 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMaxima.cpp
--rw-r--r--   0 phil       (501) staff       (20)    10974 2023-04-27 15:54:13.247301 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMetapost.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16541 2023-04-27 15:54:13.248209 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexModula.cpp
--rw-r--r--   0 phil       (501) staff       (20)    18626 2023-04-27 15:54:13.247013 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMySQL.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13810 2023-04-27 15:54:13.247177 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexNimrod.cpp
--rw-r--r--   0 phil       (501) staff       (20)    18818 2023-04-27 15:54:13.249687 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexNsis.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1098 2023-04-27 15:54:13.264094 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexNull.cpp
--rw-r--r--   0 phil       (501) staff       (20)    19685 2023-04-27 15:54:13.246945 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexOScript.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9768 2023-04-27 15:54:13.258854 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexOpal.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12578 2023-04-27 15:54:13.254552 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPB.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5609 2023-04-27 15:54:13.251164 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPLM.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6620 2023-04-27 15:54:13.250194 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPO.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9536 2023-04-27 15:54:13.247546 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPOV.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12511 2023-04-27 15:54:13.248420 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPS.cpp
--rw-r--r--   0 phil       (501) staff       (20)    20877 2023-04-27 15:54:13.250007 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPascal.cpp
--rw-r--r--   0 phil       (501) staff       (20)    57970 2023-04-27 15:54:13.249765 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPerl.cpp
--rw-r--r--   0 phil       (501) staff       (20)    20435 2023-04-27 15:54:13.248844 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPowerPro.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7966 2023-04-27 15:54:13.250838 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPowerShell.cpp
--rw-r--r--   0 phil       (501) staff       (20)    20629 2023-04-27 15:54:13.265287 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexProgress.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5518 2023-04-27 15:54:13.248474 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexProps.cpp
--rw-r--r--   0 phil       (501) staff       (20)    32996 2023-04-27 15:54:13.261171 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPython.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6264 2023-04-27 15:54:13.255686 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexR.cpp
--rw-r--r--   0 phil       (501) staff       (20)    10729 2023-04-27 15:54:13.252533 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexRebol.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11302 2023-04-27 15:54:13.251447 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexRegistry.cpp
--rw-r--r--   0 phil       (501) staff       (20)    70986 2023-04-27 15:54:13.250491 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexRuby.cpp
--rw-r--r--   0 phil       (501) staff       (20)    24817 2023-04-27 15:54:13.250393 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexRust.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7803 2023-04-27 15:54:13.251042 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSAS.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5888 2023-04-27 15:54:13.250975 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSML.cpp
--rw-r--r--   0 phil       (501) staff       (20)    31189 2023-04-27 15:54:13.250716 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSQL.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11010 2023-04-27 15:54:13.251902 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSTTXT.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11945 2023-04-27 15:54:13.266468 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexScriptol.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8980 2023-04-27 15:54:13.249848 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSmalltalk.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4744 2023-04-27 15:54:13.262753 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSorcus.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9048 2023-04-27 15:54:13.256744 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSpecman.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6085 2023-04-27 15:54:13.253750 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSpice.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7292 2023-04-27 15:54:13.252647 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexStata.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11159 2023-04-27 15:54:13.251662 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTACL.cpp
--rw-r--r--   0 phil       (501) staff       (20)    37477 2023-04-27 15:54:13.253259 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTADS3.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11157 2023-04-27 15:54:13.252245 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTAL.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11073 2023-04-27 15:54:13.252466 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTCL.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16671 2023-04-27 15:54:13.253061 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTCMD.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13999 2023-04-27 15:54:13.253314 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTeX.cpp
--rw-r--r--   0 phil       (501) staff       (20)    17089 2023-04-27 15:54:13.267696 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTxt2tags.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9851 2023-04-27 15:54:13.251294 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexVB.cpp
--rw-r--r--   0 phil       (501) staff       (20)    20499 2023-04-27 15:54:13.264173 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexVHDL.cpp
--rw-r--r--   0 phil       (501) staff       (20)    35586 2023-04-27 15:54:13.258343 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexVerilog.cpp
--rw-r--r--   0 phil       (501) staff       (20)    17725 2023-04-27 15:54:13.255315 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexVisualProlog.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12465 2023-04-27 15:54:13.253919 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexYAML.cpp
--rw-r--r--   0 phil       (501) staff       (20)      854 2023-04-27 15:54:13.218300 PyQt6_QScintilla-2.14.0/scintilla/lexers/License.txt
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.562198 PyQt6_QScintilla-2.14.0/scintilla/lexlib/
--rw-r--r--   0 phil       (501) staff       (20)     2177 2023-04-27 15:54:13.252824 PyQt6_QScintilla-2.14.0/scintilla/lexlib/Accessor.cpp
--rw-r--r--   0 phil       (501) staff       (20)      829 2023-04-27 15:54:13.254318 PyQt6_QScintilla-2.14.0/scintilla/lexlib/Accessor.h
--rw-r--r--   0 phil       (501) staff       (20)    37773 2023-04-27 15:54:13.254459 PyQt6_QScintilla-2.14.0/scintilla/lexlib/CharacterCategory.cpp
--rw-r--r--   0 phil       (501) staff       (20)      850 2023-04-27 15:54:13.253830 PyQt6_QScintilla-2.14.0/scintilla/lexlib/CharacterCategory.h
--rw-r--r--   0 phil       (501) staff       (20)     1077 2023-04-27 15:54:13.254103 PyQt6_QScintilla-2.14.0/scintilla/lexlib/CharacterSet.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4516 2023-04-27 15:54:13.254516 PyQt6_QScintilla-2.14.0/scintilla/lexlib/CharacterSet.h
--rw-r--r--   0 phil       (501) staff       (20)     2820 2023-04-27 15:54:13.268772 PyQt6_QScintilla-2.14.0/scintilla/lexlib/DefaultLexer.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2336 2023-04-27 15:54:13.252761 PyQt6_QScintilla-2.14.0/scintilla/lexlib/DefaultLexer.h
--rw-r--r--   0 phil       (501) staff       (20)     5532 2023-04-27 15:54:13.265663 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexAccessor.h
--rw-r--r--   0 phil       (501) staff       (20)     3161 2023-04-27 15:54:13.259515 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerBase.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2261 2023-04-27 15:54:13.256387 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerBase.h
--rw-r--r--   0 phil       (501) staff       (20)     3025 2023-04-27 15:54:13.255020 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerModule.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2498 2023-04-27 15:54:13.253738 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerModule.h
--rw-r--r--   0 phil       (501) staff       (20)     1963 2023-04-27 15:54:13.255371 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerNoExceptions.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1135 2023-04-27 15:54:13.255610 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerNoExceptions.h
--rw-r--r--   0 phil       (501) staff       (20)     1494 2023-04-27 15:54:13.254952 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerSimple.cpp
--rw-r--r--   0 phil       (501) staff       (20)      809 2023-04-27 15:54:13.254939 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerSimple.h
--rw-r--r--   0 phil       (501) staff       (20)      854 2023-04-27 15:54:13.218300 PyQt6_QScintilla-2.14.0/scintilla/lexlib/License.txt
--rw-r--r--   0 phil       (501) staff       (20)     3453 2023-04-27 15:54:13.255662 PyQt6_QScintilla-2.14.0/scintilla/lexlib/OptionSet.h
--rw-r--r--   0 phil       (501) staff       (20)     4334 2023-04-27 15:54:13.270663 PyQt6_QScintilla-2.14.0/scintilla/lexlib/PropSetSimple.cpp
--rw-r--r--   0 phil       (501) staff       (20)      725 2023-04-27 15:54:13.253632 PyQt6_QScintilla-2.14.0/scintilla/lexlib/PropSetSimple.h
--rw-r--r--   0 phil       (501) staff       (20)     3003 2023-04-27 15:54:13.266862 PyQt6_QScintilla-2.14.0/scintilla/lexlib/SparseState.h
--rw-r--r--   0 phil       (501) staff       (20)      853 2023-04-27 15:54:13.260592 PyQt6_QScintilla-2.14.0/scintilla/lexlib/StringCopy.h
--rw-r--r--   0 phil       (501) staff       (20)     1550 2023-04-27 15:54:13.257279 PyQt6_QScintilla-2.14.0/scintilla/lexlib/StyleContext.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6026 2023-04-27 15:54:13.256286 PyQt6_QScintilla-2.14.0/scintilla/lexlib/StyleContext.h
--rw-r--r--   0 phil       (501) staff       (20)     4592 2023-04-27 15:54:13.254766 PyQt6_QScintilla-2.14.0/scintilla/lexlib/SubStyles.h
--rw-r--r--   0 phil       (501) staff       (20)     6887 2023-04-27 15:54:13.256610 PyQt6_QScintilla-2.14.0/scintilla/lexlib/WordList.cpp
--rw-r--r--   0 phil       (501) staff       (20)      965 2023-04-27 15:54:13.256426 PyQt6_QScintilla-2.14.0/scintilla/lexlib/WordList.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.586403 PyQt6_QScintilla-2.14.0/scintilla/src/
--rw-r--r--   0 phil       (501) staff       (20)     7326 2023-04-27 15:54:13.286351 PyQt6_QScintilla-2.14.0/scintilla/src/AutoComplete.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2786 2023-04-27 15:54:13.290783 PyQt6_QScintilla-2.14.0/scintilla/src/AutoComplete.h
--rw-r--r--   0 phil       (501) staff       (20)    11394 2023-04-27 15:54:13.284049 PyQt6_QScintilla-2.14.0/scintilla/src/CallTip.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2821 2023-04-27 15:54:13.287896 PyQt6_QScintilla-2.14.0/scintilla/src/CallTip.h
--rw-r--r--   0 phil       (501) staff       (20)    25198 2023-04-27 15:54:13.281777 PyQt6_QScintilla-2.14.0/scintilla/src/CaseConvert.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1601 2023-04-27 15:54:13.284193 PyQt6_QScintilla-2.14.0/scintilla/src/CaseConvert.h
--rw-r--r--   0 phil       (501) staff       (20)     1711 2023-04-27 15:54:13.288850 PyQt6_QScintilla-2.14.0/scintilla/src/CaseFolder.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1010 2023-04-27 15:54:13.291137 PyQt6_QScintilla-2.14.0/scintilla/src/CaseFolder.h
--rw-r--r--   0 phil       (501) staff       (20)     4777 2023-04-27 15:54:13.299833 PyQt6_QScintilla-2.14.0/scintilla/src/Catalogue.cpp
--rw-r--r--   0 phil       (501) staff       (20)      623 2023-04-27 15:54:13.294417 PyQt6_QScintilla-2.14.0/scintilla/src/Catalogue.h
--rw-r--r--   0 phil       (501) staff       (20)    36730 2023-04-27 15:54:13.294797 PyQt6_QScintilla-2.14.0/scintilla/src/CellBuffer.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7215 2023-04-27 15:54:13.291463 PyQt6_QScintilla-2.14.0/scintilla/src/CellBuffer.h
--rw-r--r--   0 phil       (501) staff       (20)     1588 2023-04-27 15:54:13.287277 PyQt6_QScintilla-2.14.0/scintilla/src/CharClassify.cpp
--rw-r--r--   0 phil       (501) staff       (20)      930 2023-04-27 15:54:13.291716 PyQt6_QScintilla-2.14.0/scintilla/src/CharClassify.h
--rw-r--r--   0 phil       (501) staff       (20)    11872 2023-04-27 15:54:13.286254 PyQt6_QScintilla-2.14.0/scintilla/src/ContractionState.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1694 2023-04-27 15:54:13.289026 PyQt6_QScintilla-2.14.0/scintilla/src/ContractionState.h
--rw-r--r--   0 phil       (501) staff       (20)     1107 2023-04-27 15:54:13.282737 PyQt6_QScintilla-2.14.0/scintilla/src/DBCS.cpp
--rw-r--r--   0 phil       (501) staff       (20)      397 2023-04-27 15:54:13.285971 PyQt6_QScintilla-2.14.0/scintilla/src/DBCS.h
--rw-r--r--   0 phil       (501) staff       (20)     9522 2023-04-27 15:54:13.289880 PyQt6_QScintilla-2.14.0/scintilla/src/Decoration.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2072 2023-04-27 15:54:13.292044 PyQt6_QScintilla-2.14.0/scintilla/src/Decoration.h
--rw-r--r--   0 phil       (501) staff       (20)    98470 2023-04-27 15:54:13.303656 PyQt6_QScintilla-2.14.0/scintilla/src/Document.cpp
--rw-r--r--   0 phil       (501) staff       (20)    21627 2023-04-27 15:54:13.296216 PyQt6_QScintilla-2.14.0/scintilla/src/Document.h
--rw-r--r--   0 phil       (501) staff       (20)     1867 2023-04-27 15:54:13.296191 PyQt6_QScintilla-2.14.0/scintilla/src/EditModel.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1486 2023-04-27 15:54:13.292670 PyQt6_QScintilla-2.14.0/scintilla/src/EditModel.h
--rw-r--r--   0 phil       (501) staff       (20)   101652 2023-04-27 15:54:13.290169 PyQt6_QScintilla-2.14.0/scintilla/src/EditView.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7923 2023-04-27 15:54:13.292887 PyQt6_QScintilla-2.14.0/scintilla/src/EditView.h
--rw-r--r--   0 phil       (501) staff       (20)   248617 2023-04-27 15:54:13.296479 PyQt6_QScintilla-2.14.0/scintilla/src/Editor.cpp
--rw-r--r--   0 phil       (501) staff       (20)    23032 2023-04-27 15:54:13.290857 PyQt6_QScintilla-2.14.0/scintilla/src/Editor.h
--rw-r--r--   0 phil       (501) staff       (20)      970 2023-04-27 15:54:13.283574 PyQt6_QScintilla-2.14.0/scintilla/src/ElapsedPeriod.h
--rw-r--r--   0 phil       (501) staff       (20)     3570 2023-04-27 15:54:13.287221 PyQt6_QScintilla-2.14.0/scintilla/src/ExternalLexer.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2094 2023-04-27 15:54:13.290982 PyQt6_QScintilla-2.14.0/scintilla/src/ExternalLexer.h
--rw-r--r--   0 phil       (501) staff       (20)      813 2023-04-27 15:54:13.293071 PyQt6_QScintilla-2.14.0/scintilla/src/FontQuality.h
--rw-r--r--   0 phil       (501) staff       (20)     7835 2023-04-27 15:54:13.305306 PyQt6_QScintilla-2.14.0/scintilla/src/Indicator.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1674 2023-04-27 15:54:13.297523 PyQt6_QScintilla-2.14.0/scintilla/src/Indicator.h
--rw-r--r--   0 phil       (501) staff       (20)      735 2023-04-27 15:54:13.297276 PyQt6_QScintilla-2.14.0/scintilla/src/IntegerRectangle.h
--rw-r--r--   0 phil       (501) staff       (20)     5434 2023-04-27 15:54:13.293661 PyQt6_QScintilla-2.14.0/scintilla/src/KeyMap.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1331 2023-04-27 15:54:13.291212 PyQt6_QScintilla-2.14.0/scintilla/src/KeyMap.h
--rw-r--r--   0 phil       (501) staff       (20)      854 2023-04-27 15:54:13.218300 PyQt6_QScintilla-2.14.0/scintilla/src/License.txt
--rw-r--r--   0 phil       (501) staff       (20)    15402 2023-04-27 15:54:13.294466 PyQt6_QScintilla-2.14.0/scintilla/src/LineMarker.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1510 2023-04-27 15:54:13.299705 PyQt6_QScintilla-2.14.0/scintilla/src/LineMarker.h
--rw-r--r--   0 phil       (501) staff       (20)    16819 2023-04-27 15:54:13.292530 PyQt6_QScintilla-2.14.0/scintilla/src/MarginView.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1576 2023-04-27 15:54:13.284513 PyQt6_QScintilla-2.14.0/scintilla/src/MarginView.h
--rw-r--r--   0 phil       (501) staff       (20)     5803 2023-04-27 15:54:13.288173 PyQt6_QScintilla-2.14.0/scintilla/src/Partitioning.h
--rw-r--r--   0 phil       (501) staff       (20)    12933 2023-04-27 15:54:13.292625 PyQt6_QScintilla-2.14.0/scintilla/src/PerLine.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5100 2023-04-27 15:54:13.294183 PyQt6_QScintilla-2.14.0/scintilla/src/PerLine.h
--rw-r--r--   0 phil       (501) staff       (20)      827 2023-04-27 15:54:13.306439 PyQt6_QScintilla-2.14.0/scintilla/src/Position.h
--rw-r--r--   0 phil       (501) staff       (20)    20501 2023-04-27 15:54:13.300405 PyQt6_QScintilla-2.14.0/scintilla/src/PositionCache.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7771 2023-04-27 15:54:13.300098 PyQt6_QScintilla-2.14.0/scintilla/src/PositionCache.h
--rw-r--r--   0 phil       (501) staff       (20)    26564 2023-04-27 15:54:13.295605 PyQt6_QScintilla-2.14.0/scintilla/src/RESearch.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1744 2023-04-27 15:54:13.292693 PyQt6_QScintilla-2.14.0/scintilla/src/RESearch.h
--rw-r--r--   0 phil       (501) staff       (20)     9604 2023-04-27 15:54:13.295932 PyQt6_QScintilla-2.14.0/scintilla/src/RunStyles.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2148 2023-04-27 15:54:13.300899 PyQt6_QScintilla-2.14.0/scintilla/src/RunStyles.h
--rw-r--r--   0 phil       (501) staff       (20)      305 2023-04-27 15:54:13.293599 PyQt6_QScintilla-2.14.0/scintilla/src/SciTE.properties
--rw-r--r--   0 phil       (501) staff       (20)    30781 2023-04-27 15:54:13.286747 PyQt6_QScintilla-2.14.0/scintilla/src/ScintillaBase.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3124 2023-04-27 15:54:13.289188 PyQt6_QScintilla-2.14.0/scintilla/src/ScintillaBase.h
--rw-r--r--   0 phil       (501) staff       (20)    10711 2023-04-27 15:54:13.294313 PyQt6_QScintilla-2.14.0/scintilla/src/Selection.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5757 2023-04-27 15:54:13.295658 PyQt6_QScintilla-2.14.0/scintilla/src/Selection.h
--rw-r--r--   0 phil       (501) staff       (20)     5323 2023-04-27 15:54:13.307420 PyQt6_QScintilla-2.14.0/scintilla/src/SparseVector.h
--rw-r--r--   0 phil       (501) staff       (20)    10129 2023-04-27 15:54:13.301804 PyQt6_QScintilla-2.14.0/scintilla/src/SplitVector.h
--rw-r--r--   0 phil       (501) staff       (20)     4388 2023-04-27 15:54:13.301084 PyQt6_QScintilla-2.14.0/scintilla/src/Style.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2412 2023-04-27 15:54:13.296808 PyQt6_QScintilla-2.14.0/scintilla/src/Style.h
--rw-r--r--   0 phil       (501) staff       (20)    10279 2023-04-27 15:54:13.294066 PyQt6_QScintilla-2.14.0/scintilla/src/UniConversion.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2825 2023-04-27 15:54:13.297512 PyQt6_QScintilla-2.14.0/scintilla/src/UniConversion.h
--rw-r--r--   0 phil       (501) staff       (20)      820 2023-04-27 15:54:13.301907 PyQt6_QScintilla-2.14.0/scintilla/src/UniqueString.h
--rw-r--r--   0 phil       (501) staff       (20)    19320 2023-04-27 15:54:13.295349 PyQt6_QScintilla-2.14.0/scintilla/src/ViewStyle.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6791 2023-04-27 15:54:13.287998 PyQt6_QScintilla-2.14.0/scintilla/src/ViewStyle.h
--rw-r--r--   0 phil       (501) staff       (20)    10701 2023-04-27 15:54:13.290545 PyQt6_QScintilla-2.14.0/scintilla/src/XPM.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3597 2023-04-27 15:54:13.295701 PyQt6_QScintilla-2.14.0/scintilla/src/XPM.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.607818 PyQt6_QScintilla-2.14.0/sip/
--rw-r--r--   0 phil       (501) staff       (20)     1525 2023-04-27 16:09:48.974880 PyQt6_QScintilla-2.14.0/sip/qsciabstractapis.sip
--rw-r--r--   0 phil       (501) staff       (20)     2048 2023-04-27 16:09:48.967333 PyQt6_QScintilla-2.14.0/sip/qsciapis.sip
--rw-r--r--   0 phil       (501) staff       (20)     3643 2023-04-27 16:09:48.975800 PyQt6_QScintilla-2.14.0/sip/qscicommand.sip
--rw-r--r--   0 phil       (501) staff       (20)     1463 2023-04-27 16:09:48.965856 PyQt6_QScintilla-2.14.0/sip/qscicommandset.sip
--rw-r--r--   0 phil       (501) staff       (20)     1085 2023-04-27 16:09:48.980998 PyQt6_QScintilla-2.14.0/sip/qscidocument.sip
--rw-r--r--   0 phil       (501) staff       (20)     3663 2023-04-27 16:09:48.973005 PyQt6_QScintilla-2.14.0/sip/qscilexer.sip
--rw-r--r--   0 phil       (501) staff       (20)     2286 2023-04-27 16:09:48.959830 PyQt6_QScintilla-2.14.0/sip/qscilexerasm.sip
--rw-r--r--   0 phil       (501) staff       (20)     2089 2023-04-27 16:09:48.969112 PyQt6_QScintilla-2.14.0/sip/qscilexeravs.sip
--rw-r--r--   0 phil       (501) staff       (20)     2194 2023-04-27 16:09:48.983574 PyQt6_QScintilla-2.14.0/sip/qscilexerbash.sip
--rw-r--r--   0 phil       (501) staff       (20)     1712 2023-04-27 16:09:48.944691 PyQt6_QScintilla-2.14.0/sip/qscilexerbatch.sip
--rw-r--r--   0 phil       (501) staff       (20)     2000 2023-04-27 16:09:48.974554 PyQt6_QScintilla-2.14.0/sip/qscilexercmake.sip
--rw-r--r--   0 phil       (501) staff       (20)     2854 2023-04-27 16:09:48.966904 PyQt6_QScintilla-2.14.0/sip/qscilexercoffeescript.sip
--rw-r--r--   0 phil       (501) staff       (20)     4497 2023-04-27 16:09:48.960731 PyQt6_QScintilla-2.14.0/sip/qscilexercpp.sip
--rw-r--r--   0 phil       (501) staff       (20)     1448 2023-04-27 16:09:48.984206 PyQt6_QScintilla-2.14.0/sip/qscilexercsharp.sip
--rw-r--r--   0 phil       (501) staff       (20)     2568 2023-04-27 16:09:48.976395 PyQt6_QScintilla-2.14.0/sip/qscilexercss.sip
--rw-r--r--   0 phil       (501) staff       (20)     1460 2023-04-27 16:09:48.963633 PyQt6_QScintilla-2.14.0/sip/qscilexercustom.sip
--rw-r--r--   0 phil       (501) staff       (20)     2660 2023-04-27 16:09:48.967929 PyQt6_QScintilla-2.14.0/sip/qscilexerd.sip
--rw-r--r--   0 phil       (501) staff       (20)     1614 2023-04-27 16:09:48.973702 PyQt6_QScintilla-2.14.0/sip/qscilexerdiff.sip
--rw-r--r--   0 phil       (501) staff       (20)     1547 2023-04-27 16:09:48.976771 PyQt6_QScintilla-2.14.0/sip/qscilexeredifact.sip
--rw-r--r--   0 phil       (501) staff       (20)     1251 2023-04-27 16:09:48.961355 PyQt6_QScintilla-2.14.0/sip/qscilexerfortran.sip
--rw-r--r--   0 phil       (501) staff       (20)     2096 2023-04-27 16:09:48.982992 PyQt6_QScintilla-2.14.0/sip/qscilexerfortran77.sip
--rw-r--r--   0 phil       (501) staff       (20)     1692 2023-04-27 16:09:48.966278 PyQt6_QScintilla-2.14.0/sip/qscilexerhex.sip
--rw-r--r--   0 phil       (501) staff       (20)     5292 2023-04-27 16:09:48.947204 PyQt6_QScintilla-2.14.0/sip/qscilexerhtml.sip
--rw-r--r--   0 phil       (501) staff       (20)     1303 2023-04-27 16:09:48.946041 PyQt6_QScintilla-2.14.0/sip/qscilexeridl.sip
--rw-r--r--   0 phil       (501) staff       (20)     1271 2023-04-27 16:09:48.961653 PyQt6_QScintilla-2.14.0/sip/qscilexerintelhex.sip
--rw-r--r--   0 phil       (501) staff       (20)     1226 2023-04-27 16:09:48.983876 PyQt6_QScintilla-2.14.0/sip/qscilexerjava.sip
--rw-r--r--   0 phil       (501) staff       (20)     1476 2023-04-27 16:09:48.961064 PyQt6_QScintilla-2.14.0/sip/qscilexerjavascript.sip
--rw-r--r--   0 phil       (501) staff       (20)     2161 2023-04-27 16:09:48.970175 PyQt6_QScintilla-2.14.0/sip/qscilexerjson.sip
--rw-r--r--   0 phil       (501) staff       (20)     2316 2023-04-27 16:09:48.947761 PyQt6_QScintilla-2.14.0/sip/qscilexerlua.sip
--rw-r--r--   0 phil       (501) staff       (20)     1630 2023-04-27 16:09:48.958857 PyQt6_QScintilla-2.14.0/sip/qscilexermakefile.sip
--rw-r--r--   0 phil       (501) staff       (20)     1903 2023-04-27 16:09:48.981759 PyQt6_QScintilla-2.14.0/sip/qscilexermarkdown.sip
--rw-r--r--   0 phil       (501) staff       (20)     1216 2023-04-27 16:09:48.968599 PyQt6_QScintilla-2.14.0/sip/qscilexermasm.sip
--rw-r--r--   0 phil       (501) staff       (20)     1588 2023-04-27 16:09:48.943235 PyQt6_QScintilla-2.14.0/sip/qscilexermatlab.sip
--rw-r--r--   0 phil       (501) staff       (20)     1216 2023-04-27 16:09:48.981296 PyQt6_QScintilla-2.14.0/sip/qscilexernasm.sip
--rw-r--r--   0 phil       (501) staff       (20)     1274 2023-04-27 16:09:48.972389 PyQt6_QScintilla-2.14.0/sip/qscilexeroctave.sip
--rw-r--r--   0 phil       (501) staff       (20)     2574 2023-04-27 16:09:48.945723 PyQt6_QScintilla-2.14.0/sip/qscilexerpascal.sip
--rw-r--r--   0 phil       (501) staff       (20)     3226 2023-04-27 16:09:48.972086 PyQt6_QScintilla-2.14.0/sip/qscilexerperl.sip
--rw-r--r--   0 phil       (501) staff       (20)     2023 2023-04-27 16:09:48.964117 PyQt6_QScintilla-2.14.0/sip/qscilexerpo.sip
--rw-r--r--   0 phil       (501) staff       (20)     2322 2023-04-27 16:09:48.958000 PyQt6_QScintilla-2.14.0/sip/qscilexerpostscript.sip
--rw-r--r--   0 phil       (501) staff       (20)     2335 2023-04-27 16:09:48.971355 PyQt6_QScintilla-2.14.0/sip/qscilexerpov.sip
--rw-r--r--   0 phil       (501) staff       (20)     1964 2023-04-27 16:09:48.958460 PyQt6_QScintilla-2.14.0/sip/qscilexerproperties.sip
--rw-r--r--   0 phil       (501) staff       (20)     3334 2023-04-27 16:09:48.962350 PyQt6_QScintilla-2.14.0/sip/qscilexerpython.sip
--rw-r--r--   0 phil       (501) staff       (20)     2660 2023-04-27 16:09:48.970798 PyQt6_QScintilla-2.14.0/sip/qscilexerruby.sip
--rw-r--r--   0 phil       (501) staff       (20)     1590 2023-04-27 16:09:48.982494 PyQt6_QScintilla-2.14.0/sip/qscilexerspice.sip
--rw-r--r--   0 phil       (501) staff       (20)     2764 2023-04-27 16:09:48.964750 PyQt6_QScintilla-2.14.0/sip/qscilexersql.sip
--rw-r--r--   0 phil       (501) staff       (20)     1243 2023-04-27 16:09:48.984508 PyQt6_QScintilla-2.14.0/sip/qscilexersrec.sip
--rw-r--r--   0 phil       (501) staff       (20)     2195 2023-04-27 16:09:48.965515 PyQt6_QScintilla-2.14.0/sip/qscilexertcl.sip
--rw-r--r--   0 phil       (501) staff       (20)     1257 2023-04-27 16:09:48.943594 PyQt6_QScintilla-2.14.0/sip/qscilexertekhex.sip
--rw-r--r--   0 phil       (501) staff       (20)     1935 2023-04-27 16:09:48.959317 PyQt6_QScintilla-2.14.0/sip/qscilexertex.sip
--rw-r--r--   0 phil       (501) staff       (20)     3027 2023-04-27 16:09:48.963305 PyQt6_QScintilla-2.14.0/sip/qscilexerverilog.sip
--rw-r--r--   0 phil       (501) staff       (20)     2409 2023-04-27 16:09:48.969670 PyQt6_QScintilla-2.14.0/sip/qscilexervhdl.sip
--rw-r--r--   0 phil       (501) staff       (20)     1665 2023-04-27 16:09:48.968298 PyQt6_QScintilla-2.14.0/sip/qscilexerxml.sip
--rw-r--r--   0 phil       (501) staff       (20)     1950 2023-04-27 16:09:48.945157 PyQt6_QScintilla-2.14.0/sip/qscilexeryaml.sip
--rw-r--r--   0 phil       (501) staff       (20)     1381 2023-04-27 16:09:48.982095 PyQt6_QScintilla-2.14.0/sip/qscimacro.sip
--rw-r--r--   0 phil       (501) staff       (20)     1027 2023-04-27 16:09:48.962584 PyQt6_QScintilla-2.14.0/sip/qscimod5.sip
--rw-r--r--   0 phil       (501) staff       (20)     1027 2023-04-27 16:09:48.964979 PyQt6_QScintilla-2.14.0/sip/qscimod6.sip
--rw-r--r--   0 phil       (501) staff       (20)     3603 2023-04-27 16:09:48.944269 PyQt6_QScintilla-2.14.0/sip/qscimodcommon.sip
--rw-r--r--   0 phil       (501) staff       (20)     1656 2023-04-27 16:09:48.974063 PyQt6_QScintilla-2.14.0/sip/qsciprinter.sip
--rw-r--r--   0 phil       (501) staff       (20)    18318 2023-04-27 16:09:48.980172 PyQt6_QScintilla-2.14.0/sip/qsciscintilla.sip
--rw-r--r--   0 phil       (501) staff       (20)    44084 2023-04-27 16:09:48.957408 PyQt6_QScintilla-2.14.0/sip/qsciscintillabase.sip
--rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-27 16:09:48.980715 PyQt6_QScintilla-2.14.0/sip/qscistyle.sip
--rw-r--r--   0 phil       (501) staff       (20)     1169 2023-04-27 16:09:48.973292 PyQt6_QScintilla-2.14.0/sip/qscistyledtext.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.643552 PyQt6_QScintilla-2.14.0/src/
--rw-r--r--   0 phil       (501) staff       (20)     9963 2023-04-27 16:09:48.742697 PyQt6_QScintilla-2.14.0/src/InputMethod.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7215 2023-04-27 16:09:48.680251 PyQt6_QScintilla-2.14.0/src/ListBoxQt.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2639 2023-04-27 16:09:48.840247 PyQt6_QScintilla-2.14.0/src/ListBoxQt.h
--rw-r--r--   0 phil       (501) staff       (20)     2863 2023-04-27 16:09:48.808678 PyQt6_QScintilla-2.14.0/src/MacPasteboardMime.cpp
--rw-r--r--   0 phil       (501) staff       (20)    23192 2023-04-27 16:09:48.846629 PyQt6_QScintilla-2.14.0/src/PlatQt.cpp
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.664736 PyQt6_QScintilla-2.14.0/src/Qsci/
--rw-r--r--   0 phil       (501) staff       (20)     3627 2023-04-27 16:09:48.908858 PyQt6_QScintilla-2.14.0/src/Qsci/qsciabstractapis.h
--rw-r--r--   0 phil       (501) staff       (20)     8302 2023-04-27 16:09:48.744123 PyQt6_QScintilla-2.14.0/src/Qsci/qsciapis.h
--rw-r--r--   0 phil       (501) staff       (20)    14883 2023-04-27 16:09:48.748310 PyQt6_QScintilla-2.14.0/src/Qsci/qscicommand.h
--rw-r--r--   0 phil       (501) staff       (20)     2811 2023-04-27 16:09:48.922221 PyQt6_QScintilla-2.14.0/src/Qsci/qscicommandset.h
--rw-r--r--   0 phil       (501) staff       (20)     1901 2023-04-27 16:09:48.710894 PyQt6_QScintilla-2.14.0/src/Qsci/qscidocument.h
--rw-r--r--   0 phil       (501) staff       (20)     1715 2023-04-27 16:09:48.890407 PyQt6_QScintilla-2.14.0/src/Qsci/qsciglobal.h
--rw-r--r--   0 phil       (501) staff       (20)    13290 2023-04-27 16:09:48.727875 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexer.h
--rw-r--r--   0 phil       (501) staff       (20)     6123 2023-04-27 16:09:48.754058 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerasm.h
--rw-r--r--   0 phil       (501) staff       (20)     5290 2023-04-27 16:09:48.892386 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeravs.h
--rw-r--r--   0 phil       (501) staff       (20)     4875 2023-04-27 16:09:48.687619 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerbash.h
--rw-r--r--   0 phil       (501) staff       (20)     3432 2023-04-27 16:09:48.812588 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerbatch.h
--rw-r--r--   0 phil       (501) staff       (20)     4744 2023-04-27 16:09:48.694534 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercmake.h
--rw-r--r--   0 phil       (501) staff       (20)     8627 2023-04-27 16:09:48.810364 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercoffeescript.h
--rw-r--r--   0 phil       (501) staff       (20)    13427 2023-04-27 16:09:48.750961 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercpp.h
--rw-r--r--   0 phil       (501) staff       (20)     2586 2023-04-27 16:09:48.720724 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercsharp.h
--rw-r--r--   0 phil       (501) staff       (20)     7687 2023-04-27 16:09:48.939775 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercss.h
--rw-r--r--   0 phil       (501) staff       (20)     3655 2023-04-27 16:09:48.710421 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercustom.h
--rw-r--r--   0 phil       (501) staff       (20)     7509 2023-04-27 16:09:48.930437 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerd.h
--rw-r--r--   0 phil       (501) staff       (20)     3001 2023-04-27 16:09:48.725566 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerdiff.h
--rw-r--r--   0 phil       (501) staff       (20)     2846 2023-04-27 16:09:48.740068 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeredifact.h
--rw-r--r--   0 phil       (501) staff       (20)     1968 2023-04-27 16:09:48.940246 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerfortran.h
--rw-r--r--   0 phil       (501) staff       (20)     5055 2023-04-27 16:09:48.762214 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerfortran77.h
--rw-r--r--   0 phil       (501) staff       (20)     3360 2023-04-27 16:09:48.891243 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerhex.h
--rw-r--r--   0 phil       (501) staff       (20)    14535 2023-04-27 16:09:48.807867 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerhtml.h
--rw-r--r--   0 phil       (501) staff       (20)     2158 2023-04-27 16:09:48.734476 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeridl.h
--rw-r--r--   0 phil       (501) staff       (20)     2014 2023-04-27 16:09:48.728471 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerintelhex.h
--rw-r--r--   0 phil       (501) staff       (20)     1791 2023-04-27 16:09:48.917596 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerjava.h
--rw-r--r--   0 phil       (501) staff       (20)     2711 2023-04-27 16:09:48.928381 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerjavascript.h
--rw-r--r--   0 phil       (501) staff       (20)     5543 2023-04-27 16:09:48.730669 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerjson.h
--rw-r--r--   0 phil       (501) staff       (20)     6049 2023-04-27 16:09:48.937158 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerlua.h
--rw-r--r--   0 phil       (501) staff       (20)     3127 2023-04-27 16:09:48.813323 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexermakefile.h
--rw-r--r--   0 phil       (501) staff       (20)     4181 2023-04-27 16:09:48.729469 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexermarkdown.h
--rw-r--r--   0 phil       (501) staff       (20)     1696 2023-04-27 16:09:48.724823 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexermasm.h
--rw-r--r--   0 phil       (501) staff       (20)     3031 2023-04-27 16:09:48.839671 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexermatlab.h
--rw-r--r--   0 phil       (501) staff       (20)     1696 2023-04-27 16:09:48.892836 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexernasm.h
--rw-r--r--   0 phil       (501) staff       (20)     1957 2023-04-27 16:09:48.781796 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeroctave.h
--rw-r--r--   0 phil       (501) staff       (20)     7197 2023-04-27 16:09:48.927776 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpascal.h
--rw-r--r--   0 phil       (501) staff       (20)     8811 2023-04-27 16:09:48.784814 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerperl.h
--rw-r--r--   0 phil       (501) staff       (20)     4776 2023-04-27 16:09:48.921569 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpo.h
--rw-r--r--   0 phil       (501) staff       (20)     5883 2023-04-27 16:09:48.758076 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpostscript.h
--rw-r--r--   0 phil       (501) staff       (20)     6188 2023-04-27 16:09:48.677956 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpov.h
--rw-r--r--   0 phil       (501) staff       (20)     4714 2023-04-27 16:09:48.802461 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerproperties.h
--rw-r--r--   0 phil       (501) staff       (20)    10679 2023-04-27 16:09:48.906499 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpython.h
--rw-r--r--   0 phil       (501) staff       (20)     6813 2023-04-27 16:09:48.794779 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerruby.h
--rw-r--r--   0 phil       (501) staff       (20)     3059 2023-04-27 16:09:48.740813 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerspice.h
--rw-r--r--   0 phil       (501) staff       (20)     8893 2023-04-27 16:09:48.789876 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexersql.h
--rw-r--r--   0 phil       (501) staff       (20)     1957 2023-04-27 16:09:48.733961 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexersrec.h
--rw-r--r--   0 phil       (501) staff       (20)     5523 2023-04-27 16:09:48.707696 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexertcl.h
--rw-r--r--   0 phil       (501) staff       (20)     1992 2023-04-27 16:09:48.930913 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexertekhex.h
--rw-r--r--   0 phil       (501) staff       (20)     5076 2023-04-27 16:09:48.756289 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexertex.h
--rw-r--r--   0 phil       (501) staff       (20)     8086 2023-04-27 16:09:48.676613 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerverilog.h
--rw-r--r--   0 phil       (501) staff       (20)     6446 2023-04-27 16:09:48.811795 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexervhdl.h
--rw-r--r--   0 phil       (501) staff       (20)     3458 2023-04-27 16:09:48.889956 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerxml.h
--rw-r--r--   0 phil       (501) staff       (20)     4424 2023-04-27 16:09:48.689510 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeryaml.h
--rw-r--r--   0 phil       (501) staff       (20)     2786 2023-04-27 16:09:48.838141 PyQt6_QScintilla-2.14.0/src/Qsci/qscimacro.h
--rw-r--r--   0 phil       (501) staff       (20)     4423 2023-04-27 16:09:48.814604 PyQt6_QScintilla-2.14.0/src/Qsci/qsciprinter.h
--rw-r--r--   0 phil       (501) staff       (20)    86594 2023-04-27 16:09:48.674896 PyQt6_QScintilla-2.14.0/src/Qsci/qsciscintilla.h
--rw-r--r--   0 phil       (501) staff       (20)    89964 2023-04-27 16:09:48.837397 PyQt6_QScintilla-2.14.0/src/Qsci/qsciscintillabase.h
--rw-r--r--   0 phil       (501) staff       (20)     6226 2023-04-27 16:09:48.897008 PyQt6_QScintilla-2.14.0/src/Qsci/qscistyle.h
--rw-r--r--   0 phil       (501) staff       (20)     1898 2023-04-27 16:09:48.917148 PyQt6_QScintilla-2.14.0/src/Qsci/qscistyledtext.h
--rw-r--r--   0 phil       (501) staff       (20)    21851 2023-04-27 16:09:48.885387 PyQt6_QScintilla-2.14.0/src/SciAccessibility.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4457 2023-04-27 16:09:48.688490 PyQt6_QScintilla-2.14.0/src/SciAccessibility.h
--rw-r--r--   0 phil       (501) staff       (20)     4754 2023-04-27 16:09:48.908201 PyQt6_QScintilla-2.14.0/src/SciClasses.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2740 2023-04-27 16:09:48.904397 PyQt6_QScintilla-2.14.0/src/SciClasses.h
--rw-r--r--   0 phil       (501) staff       (20)    19373 2023-04-27 16:09:48.903648 PyQt6_QScintilla-2.14.0/src/ScintillaQt.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4225 2023-04-27 16:09:48.765916 PyQt6_QScintilla-2.14.0/src/ScintillaQt.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.642716 PyQt6_QScintilla-2.14.0/src/features/
--rw-r--r--   0 phil       (501) staff       (20)      534 2023-04-27 16:09:48.752675 PyQt6_QScintilla-2.14.0/src/features/qscintilla2.prf
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.643155 PyQt6_QScintilla-2.14.0/src/features_staticlib/
--rw-r--r--   0 phil       (501) staff       (20)      507 2023-04-27 16:09:48.909333 PyQt6_QScintilla-2.14.0/src/features_staticlib/qscintilla2.prf
--rw-r--r--   0 phil       (501) staff       (20)     1423 2023-04-27 16:09:48.906974 PyQt6_QScintilla-2.14.0/src/qsciabstractapis.cpp
--rw-r--r--   0 phil       (501) staff       (20)    24667 2023-04-27 16:09:48.703639 PyQt6_QScintilla-2.14.0/src/qsciapis.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3394 2023-04-27 16:09:48.850463 PyQt6_QScintilla-2.14.0/src/qscicommand.cpp
--rw-r--r--   0 phil       (501) staff       (20)    27482 2023-04-27 16:09:48.686351 PyQt6_QScintilla-2.14.0/src/qscicommandset.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3793 2023-04-27 16:09:48.880447 PyQt6_QScintilla-2.14.0/src/qscidocument.cpp
--rw-r--r--   0 phil       (501) staff       (20)    17245 2023-04-27 16:09:48.935842 PyQt6_QScintilla-2.14.0/src/qscilexer.cpp
--rw-r--r--   0 phil       (501) staff       (20)    23577 2023-04-27 16:09:48.798328 PyQt6_QScintilla-2.14.0/src/qscilexerasm.cpp
--rw-r--r--   0 phil       (501) staff       (20)    14533 2023-04-27 16:09:48.706333 PyQt6_QScintilla-2.14.0/src/qscilexeravs.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8166 2023-04-27 16:09:48.804610 PyQt6_QScintilla-2.14.0/src/qscilexerbash.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4490 2023-04-27 16:09:48.761107 PyQt6_QScintilla-2.14.0/src/qscilexerbatch.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8247 2023-04-27 16:09:48.898948 PyQt6_QScintilla-2.14.0/src/qscilexercmake.cpp
--rw-r--r--   0 phil       (501) staff       (20)    10030 2023-04-27 16:09:48.692369 PyQt6_QScintilla-2.14.0/src/qscilexercoffeescript.cpp
--rw-r--r--   0 phil       (501) staff       (20)    20137 2023-04-27 16:09:48.739306 PyQt6_QScintilla-2.14.0/src/qscilexercpp.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3237 2023-04-27 16:09:48.838945 PyQt6_QScintilla-2.14.0/src/qscilexercsharp.cpp
--rw-r--r--   0 phil       (501) staff       (20)    10573 2023-04-27 16:09:48.849444 PyQt6_QScintilla-2.14.0/src/qscilexercss.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2683 2023-04-27 16:09:48.715596 PyQt6_QScintilla-2.14.0/src/qscilexercustom.cpp
--rw-r--r--   0 phil       (501) staff       (20)    10175 2023-04-27 16:09:48.697359 PyQt6_QScintilla-2.14.0/src/qscilexerd.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3146 2023-04-27 16:09:48.938131 PyQt6_QScintilla-2.14.0/src/qscilexerdiff.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2815 2023-04-27 16:09:48.878232 PyQt6_QScintilla-2.14.0/src/qscilexeredifact.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4910 2023-04-27 16:09:48.745753 PyQt6_QScintilla-2.14.0/src/qscilexerfortran.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7062 2023-04-27 16:09:48.800214 PyQt6_QScintilla-2.14.0/src/qscilexerfortran77.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3604 2023-04-27 16:09:48.693457 PyQt6_QScintilla-2.14.0/src/qscilexerhex.cpp
--rw-r--r--   0 phil       (501) staff       (20)    30776 2023-04-27 16:09:48.778974 PyQt6_QScintilla-2.14.0/src/qscilexerhtml.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3629 2023-04-27 16:09:48.771886 PyQt6_QScintilla-2.14.0/src/qscilexeridl.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1542 2023-04-27 16:09:48.711359 PyQt6_QScintilla-2.14.0/src/qscilexerintelhex.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1776 2023-04-27 16:09:48.813773 PyQt6_QScintilla-2.14.0/src/qscilexerjava.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3207 2023-04-27 16:09:48.744981 PyQt6_QScintilla-2.14.0/src/qscilexerjavascript.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6285 2023-04-27 16:09:48.911265 PyQt6_QScintilla-2.14.0/src/qscilexerjson.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8617 2023-04-27 16:09:48.781297 PyQt6_QScintilla-2.14.0/src/qscilexerlua.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3418 2023-04-27 16:09:48.782843 PyQt6_QScintilla-2.14.0/src/qscilexermakefile.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6253 2023-04-27 16:09:48.887234 PyQt6_QScintilla-2.14.0/src/qscilexermarkdown.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1269 2023-04-27 16:09:48.709700 PyQt6_QScintilla-2.14.0/src/qscilexermasm.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3405 2023-04-27 16:09:48.755210 PyQt6_QScintilla-2.14.0/src/qscilexermatlab.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1268 2023-04-27 16:09:48.880865 PyQt6_QScintilla-2.14.0/src/qscilexernasm.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1970 2023-04-27 16:09:48.928904 PyQt6_QScintilla-2.14.0/src/qscilexeroctave.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9835 2023-04-27 16:09:48.764873 PyQt6_QScintilla-2.14.0/src/qscilexerpascal.cpp
--rw-r--r--   0 phil       (501) staff       (20)    15626 2023-04-27 16:09:48.926257 PyQt6_QScintilla-2.14.0/src/qscilexerperl.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4596 2023-04-27 16:09:48.720128 PyQt6_QScintilla-2.14.0/src/qscilexerpo.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13559 2023-04-27 16:09:48.788011 PyQt6_QScintilla-2.14.0/src/qscilexerpostscript.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12918 2023-04-27 16:09:48.920444 PyQt6_QScintilla-2.14.0/src/qscilexerpov.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4689 2023-04-27 16:09:48.791260 PyQt6_QScintilla-2.14.0/src/qscilexerproperties.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11799 2023-04-27 16:09:48.718691 PyQt6_QScintilla-2.14.0/src/qscilexerpython.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9035 2023-04-27 16:09:48.916627 PyQt6_QScintilla-2.14.0/src/qscilexerruby.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5256 2023-04-27 16:09:48.801461 PyQt6_QScintilla-2.14.0/src/qscilexerspice.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13713 2023-04-27 16:09:48.724342 PyQt6_QScintilla-2.14.0/src/qscilexersql.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1549 2023-04-27 16:09:48.840728 PyQt6_QScintilla-2.14.0/src/qscilexersrec.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13475 2023-04-27 16:09:48.733407 PyQt6_QScintilla-2.14.0/src/qscilexertcl.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1603 2023-04-27 16:09:48.756764 PyQt6_QScintilla-2.14.0/src/qscilexertekhex.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9867 2023-04-27 16:09:48.793221 PyQt6_QScintilla-2.14.0/src/qscilexertex.cpp
--rw-r--r--   0 phil       (501) staff       (20)    15610 2023-04-27 16:09:48.714834 PyQt6_QScintilla-2.14.0/src/qscilexerverilog.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9890 2023-04-27 16:09:48.913854 PyQt6_QScintilla-2.14.0/src/qscilexervhdl.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5283 2023-04-27 16:09:48.709286 PyQt6_QScintilla-2.14.0/src/qscilexerxml.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5531 2023-04-27 16:09:48.759750 PyQt6_QScintilla-2.14.0/src/qscilexeryaml.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7469 2023-04-27 16:09:48.889189 PyQt6_QScintilla-2.14.0/src/qscimacro.cpp
--rw-r--r--   0 phil       (501) staff       (20)    14299 2023-04-27 16:09:48.895625 PyQt6_QScintilla-2.14.0/src/qscintilla.pro
--rw-r--r--   0 phil       (501) staff       (20)    44424 2023-04-27 15:54:13.281422 PyQt6_QScintilla-2.14.0/src/qscintilla_cs.qm
--rw-r--r--   0 phil       (501) staff       (20)    82744 2023-04-27 15:54:13.293213 PyQt6_QScintilla-2.14.0/src/qscintilla_de.qm
--rw-r--r--   0 phil       (501) staff       (20)    81850 2023-04-27 15:54:13.290333 PyQt6_QScintilla-2.14.0/src/qscintilla_es.qm
--rw-r--r--   0 phil       (501) staff       (20)    53842 2023-04-27 15:54:13.284613 PyQt6_QScintilla-2.14.0/src/qscintilla_fr.qm
--rw-r--r--   0 phil       (501) staff       (20)    49459 2023-04-27 15:54:13.281912 PyQt6_QScintilla-2.14.0/src/qscintilla_pt_br.qm
--rw-r--r--   0 phil       (501) staff       (20)     5046 2023-04-27 16:09:48.941504 PyQt6_QScintilla-2.14.0/src/qsciprinter.cpp
--rw-r--r--   0 phil       (501) staff       (20)   113218 2023-04-27 16:09:48.877355 PyQt6_QScintilla-2.14.0/src/qsciscintilla.cpp
--rw-r--r--   0 phil       (501) staff       (20)    21783 2023-04-27 16:09:48.771123 PyQt6_QScintilla-2.14.0/src/qsciscintillabase.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5035 2023-04-27 16:09:48.879430 PyQt6_QScintilla-2.14.0/src/qscistyle.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1620 2023-04-27 16:09:48.931347 PyQt6_QScintilla-2.14.0/src/qscistyledtext.cpp
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-07 15:38:43.118007 PyQt6_QScintilla-2.14.1/
+-rw-r--r--   0 phil       (501) staff       (20)   244561 2023-06-07 15:38:41.870093 PyQt6_QScintilla-2.14.1/ChangeLog
+-rw-r--r--   0 phil       (501) staff       (20)    35147 2023-06-07 15:38:40.593378 PyQt6_QScintilla-2.14.1/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)    28087 2023-06-07 15:18:09.134637 PyQt6_QScintilla-2.14.1/NEWS
+-rw-r--r--   0 phil       (501) staff       (20)     1911 2023-06-07 15:38:43.118181 PyQt6_QScintilla-2.14.1/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1564 2023-06-07 15:38:42.198386 PyQt6_QScintilla-2.14.1/README
+-rw-r--r--   0 phil       (501) staff       (20)     7485 2023-06-07 15:38:42.251251 PyQt6_QScintilla-2.14.1/project.py
+-rw-r--r--   0 phil       (501) staff       (20)      553 2023-06-07 15:38:42.197784 PyQt6_QScintilla-2.14.1/pyproject.toml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-07 15:38:43.039175 PyQt6_QScintilla-2.14.1/qsci/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-07 15:38:43.039240 PyQt6_QScintilla-2.14.1/qsci/api/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-07 15:38:43.050953 PyQt6_QScintilla-2.14.1/qsci/api/python/
+-rw-r--r--   0 phil       (501) staff       (20)   172772 2023-06-07 15:18:08.596559 PyQt6_QScintilla-2.14.1/qsci/api/python/Python-2.4.api
+-rw-r--r--   0 phil       (501) staff       (20)   199839 2023-06-07 15:18:08.592867 PyQt6_QScintilla-2.14.1/qsci/api/python/Python-2.5.api
+-rw-r--r--   0 phil       (501) staff       (20)   191764 2023-06-07 15:18:08.592176 PyQt6_QScintilla-2.14.1/qsci/api/python/Python-2.6.api
+-rw-r--r--   0 phil       (501) staff       (20)   192152 2023-06-07 15:18:08.597754 PyQt6_QScintilla-2.14.1/qsci/api/python/Python-2.7.api
+-rw-r--r--   0 phil       (501) staff       (20)   175453 2023-06-07 15:18:08.592006 PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.1.api
+-rw-r--r--   0 phil       (501) staff       (20)   233448 2023-06-07 15:18:08.595663 PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.10.api
+-rw-r--r--   0 phil       (501) staff       (20)   243538 2023-06-07 15:18:08.597455 PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.11.api
+-rw-r--r--   0 phil       (501) staff       (20)   156049 2023-06-07 15:18:08.594592 PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.2.api
+-rw-r--r--   0 phil       (501) staff       (20)   254493 2023-06-07 15:18:08.615083 PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.3.api
+-rw-r--r--   0 phil       (501) staff       (20)   246543 2023-06-07 15:18:08.594572 PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.4.api
+-rw-r--r--   0 phil       (501) staff       (20)   238049 2023-06-07 15:18:08.606426 PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.5.api
+-rw-r--r--   0 phil       (501) staff       (20)   234256 2023-06-07 15:18:08.605402 PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.6.api
+-rw-r--r--   0 phil       (501) staff       (20)   233756 2023-06-07 15:18:08.605969 PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.7.api
+-rw-r--r--   0 phil       (501) staff       (20)   235810 2023-06-07 15:18:08.603693 PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.8.api
+-rw-r--r--   0 phil       (501) staff       (20)   227832 2023-06-07 15:18:08.601714 PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.9.api
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-07 15:38:42.978881 PyQt6_QScintilla-2.14.1/scintilla/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-07 15:38:42.965174 PyQt6_QScintilla-2.14.1/scintilla/include/
+-rw-r--r--   0 phil       (501) staff       (20)     4124 2023-06-07 15:18:08.561772 PyQt6_QScintilla-2.14.1/scintilla/include/ILexer.h
+-rw-r--r--   0 phil       (501) staff       (20)      607 2023-06-07 15:18:08.560010 PyQt6_QScintilla-2.14.1/scintilla/include/ILoader.h
+-rw-r--r--   0 phil       (501) staff       (20)      854 2023-06-07 15:18:08.537125 PyQt6_QScintilla-2.14.1/scintilla/include/License.txt
+-rw-r--r--   0 phil       (501) staff       (20)    15732 2023-06-07 15:18:08.560583 PyQt6_QScintilla-2.14.1/scintilla/include/Platform.h
+-rw-r--r--   0 phil       (501) staff       (20)    52975 2023-06-07 15:18:08.583935 PyQt6_QScintilla-2.14.1/scintilla/include/SciLexer.h
+-rw-r--r--   0 phil       (501) staff       (20)      822 2023-06-07 15:18:08.560406 PyQt6_QScintilla-2.14.1/scintilla/include/Sci_Position.h
+-rw-r--r--   0 phil       (501) staff       (20)    39252 2023-06-07 15:18:08.574409 PyQt6_QScintilla-2.14.1/scintilla/include/Scintilla.h
+-rw-r--r--   0 phil       (501) staff       (20)   151936 2023-06-07 15:18:08.569869 PyQt6_QScintilla-2.14.1/scintilla/include/Scintilla.iface
+-rw-r--r--   0 phil       (501) staff       (20)     2646 2023-06-07 15:18:08.568245 PyQt6_QScintilla-2.14.1/scintilla/include/ScintillaWidget.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-07 15:38:42.960718 PyQt6_QScintilla-2.14.1/scintilla/lexers/
+-rw-r--r--   0 phil       (501) staff       (20)    12485 2023-06-07 15:18:08.563714 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexA68k.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7680 2023-06-07 15:18:08.562240 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexAPDL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7365 2023-06-07 15:18:08.570214 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexASY.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    29486 2023-06-07 15:18:08.563380 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexAU3.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6762 2023-06-07 15:18:08.563457 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexAVE.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8571 2023-06-07 15:18:08.561476 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexAVS.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    19666 2023-06-07 15:18:08.562688 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexAbaqus.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11716 2023-06-07 15:18:08.585322 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexAda.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13719 2023-06-07 15:18:08.562556 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexAsm.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5275 2023-06-07 15:18:08.575760 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexAsn1.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    30635 2023-06-07 15:18:08.572815 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexBaan.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    27588 2023-06-07 15:18:08.571178 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexBash.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    16591 2023-06-07 15:18:08.566607 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexBasic.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    17352 2023-06-07 15:18:08.564336 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexBatch.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8737 2023-06-07 15:18:08.572035 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexBibTeX.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6474 2023-06-07 15:18:08.564958 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexBullant.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    22108 2023-06-07 15:18:08.565813 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCLW.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12466 2023-06-07 15:18:08.563852 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCOBOL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    58102 2023-06-07 15:18:08.566909 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCPP.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    18495 2023-06-07 15:18:08.587175 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCSS.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    14510 2023-06-07 15:18:08.564265 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCaml.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    15711 2023-06-07 15:18:08.577508 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCmake.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    16780 2023-06-07 15:18:08.574911 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCoffeeScript.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5705 2023-06-07 15:18:08.572731 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexConf.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7221 2023-06-07 15:18:08.568455 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCrontab.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6336 2023-06-07 15:18:08.566439 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCsound.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    16777 2023-06-07 15:18:08.573750 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexD.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9146 2023-06-07 15:18:08.566943 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexDMAP.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8358 2023-06-07 15:18:08.567518 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexDMIS.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6360 2023-06-07 15:18:08.565694 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexDiff.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    15652 2023-06-07 15:18:08.569117 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexECL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9531 2023-06-07 15:18:08.588818 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexEDIFACT.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8188 2023-06-07 15:18:08.566713 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexEScript.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7601 2023-06-07 15:18:08.579100 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexEiffel.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    16475 2023-06-07 15:18:08.577030 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexErlang.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13292 2023-06-07 15:18:08.574484 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexErrorList.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12296 2023-06-07 15:18:08.570707 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexFlagship.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5318 2023-06-07 15:18:08.567917 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexForth.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    24685 2023-06-07 15:18:08.575633 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexFortran.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6977 2023-06-07 15:18:08.568838 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexGAP.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8904 2023-06-07 15:18:08.569273 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexGui4Cli.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    81836 2023-06-07 15:18:08.570340 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexHTML.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    36346 2023-06-07 15:18:08.571806 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexHaskell.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    29024 2023-06-07 15:18:08.591783 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexHex.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2500 2023-06-07 15:18:08.568359 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexIndent.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8369 2023-06-07 15:18:08.580863 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexInno.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13704 2023-06-07 15:18:08.578920 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexJSON.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    16299 2023-06-07 15:18:08.576194 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexKVIrc.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3747 2023-06-07 15:18:08.572407 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexKix.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    28943 2023-06-07 15:18:08.570931 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexLPeg.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    15494 2023-06-07 15:18:08.577338 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexLaTeX.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8300 2023-06-07 15:18:08.571175 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexLisp.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6042 2023-06-07 15:18:08.571378 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexLout.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    16099 2023-06-07 15:18:08.572611 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexLua.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5444 2023-06-07 15:18:08.573547 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMMIXAL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5257 2023-06-07 15:18:08.595288 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMPT.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11271 2023-06-07 15:18:08.570689 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMSSQL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13633 2023-06-07 15:18:08.582592 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMagik.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4391 2023-06-07 15:18:08.580537 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMake.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    15564 2023-06-07 15:18:08.577962 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMarkdown.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12124 2023-06-07 15:18:08.574104 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMatlab.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4997 2023-06-07 15:18:08.572416 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMaxima.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    10974 2023-06-07 15:18:08.578997 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMetapost.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    16541 2023-06-07 15:18:08.573111 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexModula.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    18626 2023-06-07 15:18:08.573405 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMySQL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13810 2023-06-07 15:18:08.574642 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexNimrod.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    18818 2023-06-07 15:18:08.575428 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexNsis.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1098 2023-06-07 15:18:08.596698 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexNull.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    19685 2023-06-07 15:18:08.573297 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexOScript.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9768 2023-06-07 15:18:08.584475 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexOpal.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12578 2023-06-07 15:18:08.582462 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPB.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5609 2023-06-07 15:18:08.579685 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPLM.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6620 2023-06-07 15:18:08.575575 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPO.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9536 2023-06-07 15:18:08.573846 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPOV.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12511 2023-06-07 15:18:08.581189 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPS.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    20877 2023-06-07 15:18:08.575251 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPascal.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    57970 2023-06-07 15:18:08.576541 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPerl.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    20435 2023-06-07 15:18:08.576747 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPowerPro.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7966 2023-06-07 15:18:08.577123 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPowerShell.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    20629 2023-06-07 15:18:08.598484 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexProgress.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5518 2023-06-07 15:18:08.574772 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexProps.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    32996 2023-06-07 15:18:08.586759 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPython.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6264 2023-06-07 15:18:08.583966 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexR.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    10729 2023-06-07 15:18:08.581525 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexRebol.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11302 2023-06-07 15:18:08.577632 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexRegistry.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    70986 2023-06-07 15:18:08.577888 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexRuby.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    24817 2023-06-07 15:18:08.583545 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexRust.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7803 2023-06-07 15:18:08.576738 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexSAS.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5888 2023-06-07 15:18:08.578171 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexSML.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    31189 2023-06-07 15:18:08.580370 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexSQL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11010 2023-06-07 15:18:08.578671 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexSTTXT.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11945 2023-06-07 15:18:08.600006 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexScriptol.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8980 2023-06-07 15:18:08.576376 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexSmalltalk.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4744 2023-06-07 15:18:08.588623 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexSorcus.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9048 2023-06-07 15:18:08.585173 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexSpecman.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6085 2023-06-07 15:18:08.582979 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexSpice.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7292 2023-06-07 15:18:08.579246 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexStata.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11159 2023-06-07 15:18:08.579469 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexTACL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    37477 2023-06-07 15:18:08.585844 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexTADS3.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11157 2023-06-07 15:18:08.578382 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexTAL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11073 2023-06-07 15:18:08.579910 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexTCL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    16671 2023-06-07 15:18:08.582550 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexTCMD.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13999 2023-06-07 15:18:08.580476 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexTeX.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    17089 2023-06-07 15:18:08.602112 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexTxt2tags.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9851 2023-06-07 15:18:08.577960 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexVB.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    20499 2023-06-07 15:18:08.590995 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexVHDL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    35586 2023-06-07 15:18:08.588125 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexVerilog.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    17725 2023-06-07 15:18:08.584932 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexVisualProlog.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12465 2023-06-07 15:18:08.581436 PyQt6_QScintilla-2.14.1/scintilla/lexers/LexYAML.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      854 2023-06-07 15:18:08.537125 PyQt6_QScintilla-2.14.1/scintilla/lexers/License.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-07 15:38:42.978354 PyQt6_QScintilla-2.14.1/scintilla/lexlib/
+-rw-r--r--   0 phil       (501) staff       (20)     2177 2023-06-07 15:18:08.581129 PyQt6_QScintilla-2.14.1/scintilla/lexlib/Accessor.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      829 2023-06-07 15:18:08.587168 PyQt6_QScintilla-2.14.1/scintilla/lexlib/Accessor.h
+-rw-r--r--   0 phil       (501) staff       (20)    37773 2023-06-07 15:18:08.581424 PyQt6_QScintilla-2.14.1/scintilla/lexlib/CharacterCategory.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      850 2023-06-07 15:18:08.581783 PyQt6_QScintilla-2.14.1/scintilla/lexlib/CharacterCategory.h
+-rw-r--r--   0 phil       (501) staff       (20)     1077 2023-06-07 15:18:08.584398 PyQt6_QScintilla-2.14.1/scintilla/lexlib/CharacterSet.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4516 2023-06-07 15:18:08.582361 PyQt6_QScintilla-2.14.1/scintilla/lexlib/CharacterSet.h
+-rw-r--r--   0 phil       (501) staff       (20)     2820 2023-06-07 15:18:08.604100 PyQt6_QScintilla-2.14.1/scintilla/lexlib/DefaultLexer.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2336 2023-06-07 15:18:08.579644 PyQt6_QScintilla-2.14.1/scintilla/lexlib/DefaultLexer.h
+-rw-r--r--   0 phil       (501) staff       (20)     5532 2023-06-07 15:18:08.592822 PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexAccessor.h
+-rw-r--r--   0 phil       (501) staff       (20)     3161 2023-06-07 15:18:08.589439 PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexerBase.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2261 2023-06-07 15:18:08.586141 PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexerBase.h
+-rw-r--r--   0 phil       (501) staff       (20)     3025 2023-06-07 15:18:08.582767 PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexerModule.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2498 2023-06-07 15:18:08.582310 PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexerModule.h
+-rw-r--r--   0 phil       (501) staff       (20)     1963 2023-06-07 15:18:08.588285 PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexerNoExceptions.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1135 2023-06-07 15:18:08.583186 PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexerNoExceptions.h
+-rw-r--r--   0 phil       (501) staff       (20)     1494 2023-06-07 15:18:08.582959 PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexerSimple.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      809 2023-06-07 15:18:08.585434 PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexerSimple.h
+-rw-r--r--   0 phil       (501) staff       (20)      854 2023-06-07 15:18:08.537125 PyQt6_QScintilla-2.14.1/scintilla/lexlib/License.txt
+-rw-r--r--   0 phil       (501) staff       (20)     3453 2023-06-07 15:18:08.583657 PyQt6_QScintilla-2.14.1/scintilla/lexlib/OptionSet.h
+-rw-r--r--   0 phil       (501) staff       (20)     4334 2023-06-07 15:18:08.605780 PyQt6_QScintilla-2.14.1/scintilla/lexlib/PropSetSimple.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      725 2023-06-07 15:18:08.581419 PyQt6_QScintilla-2.14.1/scintilla/lexlib/PropSetSimple.h
+-rw-r--r--   0 phil       (501) staff       (20)     3003 2023-06-07 15:18:08.596247 PyQt6_QScintilla-2.14.1/scintilla/lexlib/SparseState.h
+-rw-r--r--   0 phil       (501) staff       (20)      853 2023-06-07 15:18:08.590671 PyQt6_QScintilla-2.14.1/scintilla/lexlib/StringCopy.h
+-rw-r--r--   0 phil       (501) staff       (20)     1550 2023-06-07 15:18:08.587258 PyQt6_QScintilla-2.14.1/scintilla/lexlib/StyleContext.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6026 2023-06-07 15:18:08.584217 PyQt6_QScintilla-2.14.1/scintilla/lexlib/StyleContext.h
+-rw-r--r--   0 phil       (501) staff       (20)     4592 2023-06-07 15:18:08.583535 PyQt6_QScintilla-2.14.1/scintilla/lexlib/SubStyles.h
+-rw-r--r--   0 phil       (501) staff       (20)     6887 2023-06-07 15:18:08.590010 PyQt6_QScintilla-2.14.1/scintilla/lexlib/WordList.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      965 2023-06-07 15:18:08.584423 PyQt6_QScintilla-2.14.1/scintilla/lexlib/WordList.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-07 15:38:43.010019 PyQt6_QScintilla-2.14.1/scintilla/src/
+-rw-r--r--   0 phil       (501) staff       (20)     7326 2023-06-07 15:18:08.628836 PyQt6_QScintilla-2.14.1/scintilla/src/AutoComplete.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2786 2023-06-07 15:18:08.633219 PyQt6_QScintilla-2.14.1/scintilla/src/AutoComplete.h
+-rw-r--r--   0 phil       (501) staff       (20)    11394 2023-06-07 15:18:08.627098 PyQt6_QScintilla-2.14.1/scintilla/src/CallTip.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2821 2023-06-07 15:18:08.631086 PyQt6_QScintilla-2.14.1/scintilla/src/CallTip.h
+-rw-r--r--   0 phil       (501) staff       (20)    25198 2023-06-07 15:18:08.619867 PyQt6_QScintilla-2.14.1/scintilla/src/CaseConvert.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1601 2023-06-07 15:18:08.621066 PyQt6_QScintilla-2.14.1/scintilla/src/CaseConvert.h
+-rw-r--r--   0 phil       (501) staff       (20)     1711 2023-06-07 15:18:08.631510 PyQt6_QScintilla-2.14.1/scintilla/src/CaseFolder.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1010 2023-06-07 15:18:08.631319 PyQt6_QScintilla-2.14.1/scintilla/src/CaseFolder.h
+-rw-r--r--   0 phil       (501) staff       (20)     4777 2023-06-07 15:18:08.641646 PyQt6_QScintilla-2.14.1/scintilla/src/Catalogue.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      623 2023-06-07 15:18:08.636673 PyQt6_QScintilla-2.14.1/scintilla/src/Catalogue.h
+-rw-r--r--   0 phil       (501) staff       (20)    36730 2023-06-07 15:18:08.635800 PyQt6_QScintilla-2.14.1/scintilla/src/CellBuffer.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7215 2023-06-07 15:18:08.636158 PyQt6_QScintilla-2.14.1/scintilla/src/CellBuffer.h
+-rw-r--r--   0 phil       (501) staff       (20)     1588 2023-06-07 15:18:08.630387 PyQt6_QScintilla-2.14.1/scintilla/src/CharClassify.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      930 2023-06-07 15:18:08.634510 PyQt6_QScintilla-2.14.1/scintilla/src/CharClassify.h
+-rw-r--r--   0 phil       (501) staff       (20)    11872 2023-06-07 15:18:08.629495 PyQt6_QScintilla-2.14.1/scintilla/src/ContractionState.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1694 2023-06-07 15:18:08.632352 PyQt6_QScintilla-2.14.1/scintilla/src/ContractionState.h
+-rw-r--r--   0 phil       (501) staff       (20)     1107 2023-06-07 15:18:08.621220 PyQt6_QScintilla-2.14.1/scintilla/src/DBCS.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      397 2023-06-07 15:18:08.621896 PyQt6_QScintilla-2.14.1/scintilla/src/DBCS.h
+-rw-r--r--   0 phil       (501) staff       (20)     9522 2023-06-07 15:18:08.632892 PyQt6_QScintilla-2.14.1/scintilla/src/Decoration.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2072 2023-06-07 15:18:08.632510 PyQt6_QScintilla-2.14.1/scintilla/src/Decoration.h
+-rw-r--r--   0 phil       (501) staff       (20)    98470 2023-06-07 15:18:08.646029 PyQt6_QScintilla-2.14.1/scintilla/src/Document.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    21627 2023-06-07 15:18:08.638842 PyQt6_QScintilla-2.14.1/scintilla/src/Document.h
+-rw-r--r--   0 phil       (501) staff       (20)     1867 2023-06-07 15:18:08.637012 PyQt6_QScintilla-2.14.1/scintilla/src/EditModel.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1486 2023-06-07 15:18:08.637361 PyQt6_QScintilla-2.14.1/scintilla/src/EditModel.h
+-rw-r--r--   0 phil       (501) staff       (20)   101652 2023-06-07 15:18:08.634858 PyQt6_QScintilla-2.14.1/scintilla/src/EditView.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7923 2023-06-07 15:18:08.635911 PyQt6_QScintilla-2.14.1/scintilla/src/EditView.h
+-rw-r--r--   0 phil       (501) staff       (20)   248617 2023-06-07 15:18:08.640807 PyQt6_QScintilla-2.14.1/scintilla/src/Editor.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    23032 2023-06-07 15:18:08.634711 PyQt6_QScintilla-2.14.1/scintilla/src/Editor.h
+-rw-r--r--   0 phil       (501) staff       (20)      970 2023-06-07 15:18:08.622433 PyQt6_QScintilla-2.14.1/scintilla/src/ElapsedPeriod.h
+-rw-r--r--   0 phil       (501) staff       (20)     3570 2023-06-07 15:18:08.623453 PyQt6_QScintilla-2.14.1/scintilla/src/ExternalLexer.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2094 2023-06-07 15:18:08.634264 PyQt6_QScintilla-2.14.1/scintilla/src/ExternalLexer.h
+-rw-r--r--   0 phil       (501) staff       (20)      813 2023-06-07 15:18:08.633893 PyQt6_QScintilla-2.14.1/scintilla/src/FontQuality.h
+-rw-r--r--   0 phil       (501) staff       (20)     7835 2023-06-07 15:18:08.647676 PyQt6_QScintilla-2.14.1/scintilla/src/Indicator.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1674 2023-06-07 15:18:08.640176 PyQt6_QScintilla-2.14.1/scintilla/src/Indicator.h
+-rw-r--r--   0 phil       (501) staff       (20)      735 2023-06-07 15:18:08.638645 PyQt6_QScintilla-2.14.1/scintilla/src/IntegerRectangle.h
+-rw-r--r--   0 phil       (501) staff       (20)     5434 2023-06-07 15:18:08.639271 PyQt6_QScintilla-2.14.1/scintilla/src/KeyMap.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1331 2023-06-07 15:18:08.636468 PyQt6_QScintilla-2.14.1/scintilla/src/KeyMap.h
+-rw-r--r--   0 phil       (501) staff       (20)      854 2023-06-07 15:18:08.537125 PyQt6_QScintilla-2.14.1/scintilla/src/License.txt
+-rw-r--r--   0 phil       (501) staff       (20)    15402 2023-06-07 15:18:08.638299 PyQt6_QScintilla-2.14.1/scintilla/src/LineMarker.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1510 2023-06-07 15:18:08.642221 PyQt6_QScintilla-2.14.1/scintilla/src/LineMarker.h
+-rw-r--r--   0 phil       (501) staff       (20)    16819 2023-06-07 15:18:08.636656 PyQt6_QScintilla-2.14.1/scintilla/src/MarginView.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1576 2023-06-07 15:18:08.623607 PyQt6_QScintilla-2.14.1/scintilla/src/MarginView.h
+-rw-r--r--   0 phil       (501) staff       (20)     5803 2023-06-07 15:18:08.625248 PyQt6_QScintilla-2.14.1/scintilla/src/Partitioning.h
+-rw-r--r--   0 phil       (501) staff       (20)    12933 2023-06-07 15:18:08.635928 PyQt6_QScintilla-2.14.1/scintilla/src/PerLine.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5100 2023-06-07 15:18:08.635318 PyQt6_QScintilla-2.14.1/scintilla/src/PerLine.h
+-rw-r--r--   0 phil       (501) staff       (20)      827 2023-06-07 15:18:08.649522 PyQt6_QScintilla-2.14.1/scintilla/src/Position.h
+-rw-r--r--   0 phil       (501) staff       (20)    20501 2023-06-07 15:18:08.642306 PyQt6_QScintilla-2.14.1/scintilla/src/PositionCache.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7771 2023-06-07 15:18:08.640113 PyQt6_QScintilla-2.14.1/scintilla/src/PositionCache.h
+-rw-r--r--   0 phil       (501) staff       (20)    26564 2023-06-07 15:18:08.641164 PyQt6_QScintilla-2.14.1/scintilla/src/RESearch.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1744 2023-06-07 15:18:08.637746 PyQt6_QScintilla-2.14.1/scintilla/src/RESearch.h
+-rw-r--r--   0 phil       (501) staff       (20)     9604 2023-06-07 15:18:08.640562 PyQt6_QScintilla-2.14.1/scintilla/src/RunStyles.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2148 2023-06-07 15:18:08.643427 PyQt6_QScintilla-2.14.1/scintilla/src/RunStyles.h
+-rw-r--r--   0 phil       (501) staff       (20)      305 2023-06-07 15:18:08.638076 PyQt6_QScintilla-2.14.1/scintilla/src/SciTE.properties
+-rw-r--r--   0 phil       (501) staff       (20)    30781 2023-06-07 15:18:08.626227 PyQt6_QScintilla-2.14.1/scintilla/src/ScintillaBase.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3124 2023-06-07 15:18:08.626630 PyQt6_QScintilla-2.14.1/scintilla/src/ScintillaBase.h
+-rw-r--r--   0 phil       (501) staff       (20)    10711 2023-06-07 15:18:08.638083 PyQt6_QScintilla-2.14.1/scintilla/src/Selection.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5757 2023-06-07 15:18:08.636689 PyQt6_QScintilla-2.14.1/scintilla/src/Selection.h
+-rw-r--r--   0 phil       (501) staff       (20)     5323 2023-06-07 15:18:08.650804 PyQt6_QScintilla-2.14.1/scintilla/src/SparseVector.h
+-rw-r--r--   0 phil       (501) staff       (20)    10129 2023-06-07 15:18:08.643806 PyQt6_QScintilla-2.14.1/scintilla/src/SplitVector.h
+-rw-r--r--   0 phil       (501) staff       (20)     4388 2023-06-07 15:18:08.641580 PyQt6_QScintilla-2.14.1/scintilla/src/Style.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2412 2023-06-07 15:18:08.642416 PyQt6_QScintilla-2.14.1/scintilla/src/Style.h
+-rw-r--r--   0 phil       (501) staff       (20)    10279 2023-06-07 15:18:08.639895 PyQt6_QScintilla-2.14.1/scintilla/src/UniConversion.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2825 2023-06-07 15:18:08.641865 PyQt6_QScintilla-2.14.1/scintilla/src/UniConversion.h
+-rw-r--r--   0 phil       (501) staff       (20)      820 2023-06-07 15:18:08.644594 PyQt6_QScintilla-2.14.1/scintilla/src/UniqueString.h
+-rw-r--r--   0 phil       (501) staff       (20)    19320 2023-06-07 15:18:08.640515 PyQt6_QScintilla-2.14.1/scintilla/src/ViewStyle.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6791 2023-06-07 15:18:08.628260 PyQt6_QScintilla-2.14.1/scintilla/src/ViewStyle.h
+-rw-r--r--   0 phil       (501) staff       (20)    10701 2023-06-07 15:18:08.628973 PyQt6_QScintilla-2.14.1/scintilla/src/XPM.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3597 2023-06-07 15:18:08.639611 PyQt6_QScintilla-2.14.1/scintilla/src/XPM.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-07 15:38:43.038515 PyQt6_QScintilla-2.14.1/sip/
+-rw-r--r--   0 phil       (501) staff       (20)     1525 2023-06-07 15:38:42.237861 PyQt6_QScintilla-2.14.1/sip/qsciabstractapis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2048 2023-06-07 15:38:42.228420 PyQt6_QScintilla-2.14.1/sip/qsciapis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3643 2023-06-07 15:38:42.238950 PyQt6_QScintilla-2.14.1/sip/qscicommand.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1463 2023-06-07 15:38:42.226481 PyQt6_QScintilla-2.14.1/sip/qscicommandset.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1085 2023-06-07 15:38:42.245154 PyQt6_QScintilla-2.14.1/sip/qscidocument.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3663 2023-06-07 15:38:42.235478 PyQt6_QScintilla-2.14.1/sip/qscilexer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2286 2023-06-07 15:38:42.219050 PyQt6_QScintilla-2.14.1/sip/qscilexerasm.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2089 2023-06-07 15:38:42.230630 PyQt6_QScintilla-2.14.1/sip/qscilexeravs.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2194 2023-06-07 15:38:42.248322 PyQt6_QScintilla-2.14.1/sip/qscilexerbash.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1712 2023-06-07 15:38:42.201227 PyQt6_QScintilla-2.14.1/sip/qscilexerbatch.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2000 2023-06-07 15:38:42.237431 PyQt6_QScintilla-2.14.1/sip/qscilexercmake.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2854 2023-06-07 15:38:42.227872 PyQt6_QScintilla-2.14.1/sip/qscilexercoffeescript.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4497 2023-06-07 15:38:42.220135 PyQt6_QScintilla-2.14.1/sip/qscilexercpp.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1448 2023-06-07 15:38:42.249142 PyQt6_QScintilla-2.14.1/sip/qscilexercsharp.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2568 2023-06-07 15:38:42.239679 PyQt6_QScintilla-2.14.1/sip/qscilexercss.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1460 2023-06-07 15:38:42.223738 PyQt6_QScintilla-2.14.1/sip/qscilexercustom.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2660 2023-06-07 15:38:42.229145 PyQt6_QScintilla-2.14.1/sip/qscilexerd.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1614 2023-06-07 15:38:42.236348 PyQt6_QScintilla-2.14.1/sip/qscilexerdiff.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1547 2023-06-07 15:38:42.240168 PyQt6_QScintilla-2.14.1/sip/qscilexeredifact.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1251 2023-06-07 15:38:42.220934 PyQt6_QScintilla-2.14.1/sip/qscilexerfortran.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2096 2023-06-07 15:38:42.247679 PyQt6_QScintilla-2.14.1/sip/qscilexerfortran77.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1692 2023-06-07 15:38:42.227075 PyQt6_QScintilla-2.14.1/sip/qscilexerhex.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5292 2023-06-07 15:38:42.204237 PyQt6_QScintilla-2.14.1/sip/qscilexerhtml.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1303 2023-06-07 15:38:42.202886 PyQt6_QScintilla-2.14.1/sip/qscilexeridl.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1271 2023-06-07 15:38:42.221329 PyQt6_QScintilla-2.14.1/sip/qscilexerintelhex.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1226 2023-06-07 15:38:42.248716 PyQt6_QScintilla-2.14.1/sip/qscilexerjava.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1476 2023-06-07 15:38:42.220560 PyQt6_QScintilla-2.14.1/sip/qscilexerjavascript.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2161 2023-06-07 15:38:42.231921 PyQt6_QScintilla-2.14.1/sip/qscilexerjson.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2316 2023-06-07 15:38:42.204908 PyQt6_QScintilla-2.14.1/sip/qscilexerlua.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1630 2023-06-07 15:38:42.217842 PyQt6_QScintilla-2.14.1/sip/qscilexermakefile.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1903 2023-06-07 15:38:42.246134 PyQt6_QScintilla-2.14.1/sip/qscilexermarkdown.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1216 2023-06-07 15:38:42.229993 PyQt6_QScintilla-2.14.1/sip/qscilexermasm.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1588 2023-06-07 15:38:42.199505 PyQt6_QScintilla-2.14.1/sip/qscilexermatlab.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1216 2023-06-07 15:38:42.245543 PyQt6_QScintilla-2.14.1/sip/qscilexernasm.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1274 2023-06-07 15:38:42.234729 PyQt6_QScintilla-2.14.1/sip/qscilexeroctave.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2574 2023-06-07 15:38:42.202497 PyQt6_QScintilla-2.14.1/sip/qscilexerpascal.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3226 2023-06-07 15:38:42.234330 PyQt6_QScintilla-2.14.1/sip/qscilexerperl.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2023 2023-06-07 15:38:42.224329 PyQt6_QScintilla-2.14.1/sip/qscilexerpo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2322 2023-06-07 15:38:42.216791 PyQt6_QScintilla-2.14.1/sip/qscilexerpostscript.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2335 2023-06-07 15:38:42.233435 PyQt6_QScintilla-2.14.1/sip/qscilexerpov.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1964 2023-06-07 15:38:42.217355 PyQt6_QScintilla-2.14.1/sip/qscilexerproperties.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3334 2023-06-07 15:38:42.222168 PyQt6_QScintilla-2.14.1/sip/qscilexerpython.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2660 2023-06-07 15:38:42.232745 PyQt6_QScintilla-2.14.1/sip/qscilexerruby.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1590 2023-06-07 15:38:42.247061 PyQt6_QScintilla-2.14.1/sip/qscilexerspice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2764 2023-06-07 15:38:42.225100 PyQt6_QScintilla-2.14.1/sip/qscilexersql.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1243 2023-06-07 15:38:42.249530 PyQt6_QScintilla-2.14.1/sip/qscilexersrec.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2195 2023-06-07 15:38:42.226047 PyQt6_QScintilla-2.14.1/sip/qscilexertcl.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1257 2023-06-07 15:38:42.199907 PyQt6_QScintilla-2.14.1/sip/qscilexertekhex.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1935 2023-06-07 15:38:42.218404 PyQt6_QScintilla-2.14.1/sip/qscilexertex.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3027 2023-06-07 15:38:42.223326 PyQt6_QScintilla-2.14.1/sip/qscilexerverilog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2409 2023-06-07 15:38:42.231315 PyQt6_QScintilla-2.14.1/sip/qscilexervhdl.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1665 2023-06-07 15:38:42.229618 PyQt6_QScintilla-2.14.1/sip/qscilexerxml.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1950 2023-06-07 15:38:42.201805 PyQt6_QScintilla-2.14.1/sip/qscilexeryaml.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1381 2023-06-07 15:38:42.246564 PyQt6_QScintilla-2.14.1/sip/qscimacro.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1027 2023-06-07 15:38:42.222475 PyQt6_QScintilla-2.14.1/sip/qscimod5.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1027 2023-06-07 15:38:42.225399 PyQt6_QScintilla-2.14.1/sip/qscimod6.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3603 2023-06-07 15:38:42.200712 PyQt6_QScintilla-2.14.1/sip/qscimodcommon.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1656 2023-06-07 15:38:42.236826 PyQt6_QScintilla-2.14.1/sip/qsciprinter.sip
+-rw-r--r--   0 phil       (501) staff       (20)    18318 2023-06-07 15:38:42.244148 PyQt6_QScintilla-2.14.1/sip/qsciscintilla.sip
+-rw-r--r--   0 phil       (501) staff       (20)    44084 2023-06-07 15:38:42.216041 PyQt6_QScintilla-2.14.1/sip/qsciscintillabase.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1939 2023-06-07 15:38:42.244803 PyQt6_QScintilla-2.14.1/sip/qscistyle.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1169 2023-06-07 15:38:42.235845 PyQt6_QScintilla-2.14.1/sip/qscistyledtext.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-07 15:38:43.089461 PyQt6_QScintilla-2.14.1/src/
+-rw-r--r--   0 phil       (501) staff       (20)     9725 2023-06-07 15:38:41.965262 PyQt6_QScintilla-2.14.1/src/InputMethod.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7215 2023-06-07 15:38:41.893577 PyQt6_QScintilla-2.14.1/src/ListBoxQt.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2639 2023-06-07 15:38:42.079515 PyQt6_QScintilla-2.14.1/src/ListBoxQt.h
+-rw-r--r--   0 phil       (501) staff       (20)     2863 2023-06-07 15:38:42.042157 PyQt6_QScintilla-2.14.1/src/MacPasteboardMime.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    23192 2023-06-07 15:38:42.086926 PyQt6_QScintilla-2.14.1/src/PlatQt.cpp
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-07 15:38:43.117645 PyQt6_QScintilla-2.14.1/src/Qsci/
+-rw-r--r--   0 phil       (501) staff       (20)     3627 2023-06-07 15:38:42.159143 PyQt6_QScintilla-2.14.1/src/Qsci/qsciabstractapis.h
+-rw-r--r--   0 phil       (501) staff       (20)     8302 2023-06-07 15:38:41.966898 PyQt6_QScintilla-2.14.1/src/Qsci/qsciapis.h
+-rw-r--r--   0 phil       (501) staff       (20)    14883 2023-06-07 15:38:41.971764 PyQt6_QScintilla-2.14.1/src/Qsci/qscicommand.h
+-rw-r--r--   0 phil       (501) staff       (20)     2811 2023-06-07 15:38:42.174832 PyQt6_QScintilla-2.14.1/src/Qsci/qscicommandset.h
+-rw-r--r--   0 phil       (501) staff       (20)     1901 2023-06-07 15:38:41.928331 PyQt6_QScintilla-2.14.1/src/Qsci/qscidocument.h
+-rw-r--r--   0 phil       (501) staff       (20)     1715 2023-06-07 15:38:42.137571 PyQt6_QScintilla-2.14.1/src/Qsci/qsciglobal.h
+-rw-r--r--   0 phil       (501) staff       (20)    13290 2023-06-07 15:38:41.948161 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexer.h
+-rw-r--r--   0 phil       (501) staff       (20)     6123 2023-06-07 15:38:41.978294 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerasm.h
+-rw-r--r--   0 phil       (501) staff       (20)     5290 2023-06-07 15:38:42.139921 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexeravs.h
+-rw-r--r--   0 phil       (501) staff       (20)     4875 2023-06-07 15:38:41.901883 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerbash.h
+-rw-r--r--   0 phil       (501) staff       (20)     3432 2023-06-07 15:38:42.046852 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerbatch.h
+-rw-r--r--   0 phil       (501) staff       (20)     4744 2023-06-07 15:38:41.909815 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexercmake.h
+-rw-r--r--   0 phil       (501) staff       (20)     8627 2023-06-07 15:38:42.044143 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexercoffeescript.h
+-rw-r--r--   0 phil       (501) staff       (20)    13427 2023-06-07 15:38:41.974704 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexercpp.h
+-rw-r--r--   0 phil       (501) staff       (20)     2586 2023-06-07 15:38:41.939790 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexercsharp.h
+-rw-r--r--   0 phil       (501) staff       (20)     7687 2023-06-07 15:38:42.195257 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexercss.h
+-rw-r--r--   0 phil       (501) staff       (20)     3655 2023-06-07 15:38:41.927737 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexercustom.h
+-rw-r--r--   0 phil       (501) staff       (20)     7509 2023-06-07 15:38:42.184378 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerd.h
+-rw-r--r--   0 phil       (501) staff       (20)     3001 2023-06-07 15:38:41.945558 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerdiff.h
+-rw-r--r--   0 phil       (501) staff       (20)     2846 2023-06-07 15:38:41.962226 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexeredifact.h
+-rw-r--r--   0 phil       (501) staff       (20)     1968 2023-06-07 15:38:42.195855 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerfortran.h
+-rw-r--r--   0 phil       (501) staff       (20)     5055 2023-06-07 15:38:41.987857 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerfortran77.h
+-rw-r--r--   0 phil       (501) staff       (20)     3360 2023-06-07 15:38:42.138567 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerhex.h
+-rw-r--r--   0 phil       (501) staff       (20)    14535 2023-06-07 15:38:42.041172 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerhtml.h
+-rw-r--r--   0 phil       (501) staff       (20)     2158 2023-06-07 15:38:41.955766 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexeridl.h
+-rw-r--r--   0 phil       (501) staff       (20)     2014 2023-06-07 15:38:41.948791 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerintelhex.h
+-rw-r--r--   0 phil       (501) staff       (20)     1791 2023-06-07 15:38:42.169387 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerjava.h
+-rw-r--r--   0 phil       (501) staff       (20)     2711 2023-06-07 15:38:42.181928 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerjavascript.h
+-rw-r--r--   0 phil       (501) staff       (20)     5543 2023-06-07 15:38:41.951385 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerjson.h
+-rw-r--r--   0 phil       (501) staff       (20)     6049 2023-06-07 15:38:42.192249 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerlua.h
+-rw-r--r--   0 phil       (501) staff       (20)     3127 2023-06-07 15:38:42.047749 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexermakefile.h
+-rw-r--r--   0 phil       (501) staff       (20)     4181 2023-06-07 15:38:41.949965 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexermarkdown.h
+-rw-r--r--   0 phil       (501) staff       (20)     1696 2023-06-07 15:38:41.944637 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexermasm.h
+-rw-r--r--   0 phil       (501) staff       (20)     3031 2023-06-07 15:38:42.078801 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexermatlab.h
+-rw-r--r--   0 phil       (501) staff       (20)     1696 2023-06-07 15:38:42.140475 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexernasm.h
+-rw-r--r--   0 phil       (501) staff       (20)     1957 2023-06-07 15:38:42.010573 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexeroctave.h
+-rw-r--r--   0 phil       (501) staff       (20)     7197 2023-06-07 15:38:42.181184 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerpascal.h
+-rw-r--r--   0 phil       (501) staff       (20)     8811 2023-06-07 15:38:42.014117 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerperl.h
+-rw-r--r--   0 phil       (501) staff       (20)     4776 2023-06-07 15:38:42.174051 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerpo.h
+-rw-r--r--   0 phil       (501) staff       (20)     5883 2023-06-07 15:38:41.982984 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerpostscript.h
+-rw-r--r--   0 phil       (501) staff       (20)     6188 2023-06-07 15:38:41.890977 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerpov.h
+-rw-r--r--   0 phil       (501) staff       (20)     4714 2023-06-07 15:38:42.034852 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerproperties.h
+-rw-r--r--   0 phil       (501) staff       (20)    10679 2023-06-07 15:38:42.156367 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerpython.h
+-rw-r--r--   0 phil       (501) staff       (20)     6813 2023-06-07 15:38:42.025697 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerruby.h
+-rw-r--r--   0 phil       (501) staff       (20)     3059 2023-06-07 15:38:41.963116 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerspice.h
+-rw-r--r--   0 phil       (501) staff       (20)     8893 2023-06-07 15:38:42.020022 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexersql.h
+-rw-r--r--   0 phil       (501) staff       (20)     1957 2023-06-07 15:38:41.955159 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexersrec.h
+-rw-r--r--   0 phil       (501) staff       (20)     5523 2023-06-07 15:38:41.924531 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexertcl.h
+-rw-r--r--   0 phil       (501) staff       (20)     1992 2023-06-07 15:38:42.184960 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexertekhex.h
+-rw-r--r--   0 phil       (501) staff       (20)     5076 2023-06-07 15:38:41.980848 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexertex.h
+-rw-r--r--   0 phil       (501) staff       (20)     8086 2023-06-07 15:38:41.889416 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerverilog.h
+-rw-r--r--   0 phil       (501) staff       (20)     6446 2023-06-07 15:38:42.045873 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexervhdl.h
+-rw-r--r--   0 phil       (501) staff       (20)     3458 2023-06-07 15:38:42.136996 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerxml.h
+-rw-r--r--   0 phil       (501) staff       (20)     4424 2023-06-07 15:38:41.904069 PyQt6_QScintilla-2.14.1/src/Qsci/qscilexeryaml.h
+-rw-r--r--   0 phil       (501) staff       (20)     2786 2023-06-07 15:38:42.076857 PyQt6_QScintilla-2.14.1/src/Qsci/qscimacro.h
+-rw-r--r--   0 phil       (501) staff       (20)     4423 2023-06-07 15:38:42.049360 PyQt6_QScintilla-2.14.1/src/Qsci/qsciprinter.h
+-rw-r--r--   0 phil       (501) staff       (20)    86594 2023-06-07 15:38:41.887387 PyQt6_QScintilla-2.14.1/src/Qsci/qsciscintilla.h
+-rw-r--r--   0 phil       (501) staff       (20)    89964 2023-06-07 15:38:42.075732 PyQt6_QScintilla-2.14.1/src/Qsci/qsciscintillabase.h
+-rw-r--r--   0 phil       (501) staff       (20)     6226 2023-06-07 15:38:42.145348 PyQt6_QScintilla-2.14.1/src/Qsci/qscistyle.h
+-rw-r--r--   0 phil       (501) staff       (20)     1898 2023-06-07 15:38:42.168819 PyQt6_QScintilla-2.14.1/src/Qsci/qscistyledtext.h
+-rw-r--r--   0 phil       (501) staff       (20)    21851 2023-06-07 15:38:42.131566 PyQt6_QScintilla-2.14.1/src/SciAccessibility.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4457 2023-06-07 15:38:41.902891 PyQt6_QScintilla-2.14.1/src/SciAccessibility.h
+-rw-r--r--   0 phil       (501) staff       (20)     4754 2023-06-07 15:38:42.158351 PyQt6_QScintilla-2.14.1/src/SciClasses.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2740 2023-06-07 15:38:42.153916 PyQt6_QScintilla-2.14.1/src/SciClasses.h
+-rw-r--r--   0 phil       (501) staff       (20)    19373 2023-06-07 15:38:42.152960 PyQt6_QScintilla-2.14.1/src/ScintillaQt.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4225 2023-06-07 15:38:41.992118 PyQt6_QScintilla-2.14.1/src/ScintillaQt.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-07 15:38:43.088360 PyQt6_QScintilla-2.14.1/src/features/
+-rw-r--r--   0 phil       (501) staff       (20)      534 2023-06-07 15:38:41.976687 PyQt6_QScintilla-2.14.1/src/features/qscintilla2.prf
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-07 15:38:43.088948 PyQt6_QScintilla-2.14.1/src/features_staticlib/
+-rw-r--r--   0 phil       (501) staff       (20)      507 2023-06-07 15:38:42.159725 PyQt6_QScintilla-2.14.1/src/features_staticlib/qscintilla2.prf
+-rw-r--r--   0 phil       (501) staff       (20)     1423 2023-06-07 15:38:42.156912 PyQt6_QScintilla-2.14.1/src/qsciabstractapis.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    24667 2023-06-07 15:38:41.919930 PyQt6_QScintilla-2.14.1/src/qsciapis.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3394 2023-06-07 15:38:42.091352 PyQt6_QScintilla-2.14.1/src/qscicommand.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    27482 2023-06-07 15:38:41.900424 PyQt6_QScintilla-2.14.1/src/qscicommandset.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3793 2023-06-07 15:38:42.125843 PyQt6_QScintilla-2.14.1/src/qscidocument.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    17245 2023-06-07 15:38:42.190685 PyQt6_QScintilla-2.14.1/src/qscilexer.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    23577 2023-06-07 15:38:42.029803 PyQt6_QScintilla-2.14.1/src/qscilexerasm.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    14533 2023-06-07 15:38:41.923036 PyQt6_QScintilla-2.14.1/src/qscilexeravs.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8166 2023-06-07 15:38:42.037387 PyQt6_QScintilla-2.14.1/src/qscilexerbash.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4490 2023-06-07 15:38:41.986547 PyQt6_QScintilla-2.14.1/src/qscilexerbatch.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8247 2023-06-07 15:38:42.147605 PyQt6_QScintilla-2.14.1/src/qscilexercmake.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    10030 2023-06-07 15:38:41.907332 PyQt6_QScintilla-2.14.1/src/qscilexercoffeescript.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    20137 2023-06-07 15:38:41.961331 PyQt6_QScintilla-2.14.1/src/qscilexercpp.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3237 2023-06-07 15:38:42.077906 PyQt6_QScintilla-2.14.1/src/qscilexercsharp.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    10573 2023-06-07 15:38:42.090187 PyQt6_QScintilla-2.14.1/src/qscilexercss.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2683 2023-06-07 15:38:41.933838 PyQt6_QScintilla-2.14.1/src/qscilexercustom.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    10175 2023-06-07 15:38:41.913055 PyQt6_QScintilla-2.14.1/src/qscilexerd.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3146 2023-06-07 15:38:42.193389 PyQt6_QScintilla-2.14.1/src/qscilexerdiff.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2815 2023-06-07 15:38:42.123209 PyQt6_QScintilla-2.14.1/src/qscilexeredifact.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4910 2023-06-07 15:38:41.968803 PyQt6_QScintilla-2.14.1/src/qscilexerfortran.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7062 2023-06-07 15:38:42.032021 PyQt6_QScintilla-2.14.1/src/qscilexerfortran77.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3604 2023-06-07 15:38:41.908567 PyQt6_QScintilla-2.14.1/src/qscilexerhex.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    30776 2023-06-07 15:38:42.007234 PyQt6_QScintilla-2.14.1/src/qscilexerhtml.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3629 2023-06-07 15:38:41.999072 PyQt6_QScintilla-2.14.1/src/qscilexeridl.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1542 2023-06-07 15:38:41.928915 PyQt6_QScintilla-2.14.1/src/qscilexerintelhex.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1776 2023-06-07 15:38:42.048358 PyQt6_QScintilla-2.14.1/src/qscilexerjava.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3207 2023-06-07 15:38:41.967885 PyQt6_QScintilla-2.14.1/src/qscilexerjavascript.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6285 2023-06-07 15:38:42.161975 PyQt6_QScintilla-2.14.1/src/qscilexerjson.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8617 2023-06-07 15:38:42.009982 PyQt6_QScintilla-2.14.1/src/qscilexerlua.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3418 2023-06-07 15:38:42.011810 PyQt6_QScintilla-2.14.1/src/qscilexermakefile.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6253 2023-06-07 15:38:42.133787 PyQt6_QScintilla-2.14.1/src/qscilexermarkdown.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1269 2023-06-07 15:38:41.926871 PyQt6_QScintilla-2.14.1/src/qscilexermasm.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3405 2023-06-07 15:38:41.979559 PyQt6_QScintilla-2.14.1/src/qscilexermatlab.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1268 2023-06-07 15:38:42.126360 PyQt6_QScintilla-2.14.1/src/qscilexernasm.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1970 2023-06-07 15:38:42.182562 PyQt6_QScintilla-2.14.1/src/qscilexeroctave.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9835 2023-06-07 15:38:41.990915 PyQt6_QScintilla-2.14.1/src/qscilexerpascal.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    15626 2023-06-07 15:38:42.179428 PyQt6_QScintilla-2.14.1/src/qscilexerperl.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4596 2023-06-07 15:38:41.939073 PyQt6_QScintilla-2.14.1/src/qscilexerpo.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13559 2023-06-07 15:38:42.017859 PyQt6_QScintilla-2.14.1/src/qscilexerpostscript.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12918 2023-06-07 15:38:42.172738 PyQt6_QScintilla-2.14.1/src/qscilexerpov.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4689 2023-06-07 15:38:42.021648 PyQt6_QScintilla-2.14.1/src/qscilexerproperties.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11799 2023-06-07 15:38:41.937400 PyQt6_QScintilla-2.14.1/src/qscilexerpython.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9035 2023-06-07 15:38:42.168198 PyQt6_QScintilla-2.14.1/src/qscilexerruby.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5256 2023-06-07 15:38:42.033578 PyQt6_QScintilla-2.14.1/src/qscilexerspice.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13713 2023-06-07 15:38:41.944003 PyQt6_QScintilla-2.14.1/src/qscilexersql.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1549 2023-06-07 15:38:42.080121 PyQt6_QScintilla-2.14.1/src/qscilexersrec.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13475 2023-06-07 15:38:41.954538 PyQt6_QScintilla-2.14.1/src/qscilexertcl.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1603 2023-06-07 15:38:41.981434 PyQt6_QScintilla-2.14.1/src/qscilexertekhex.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9867 2023-06-07 15:38:42.023912 PyQt6_QScintilla-2.14.1/src/qscilexertex.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    15610 2023-06-07 15:38:41.932946 PyQt6_QScintilla-2.14.1/src/qscilexerverilog.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9890 2023-06-07 15:38:42.164992 PyQt6_QScintilla-2.14.1/src/qscilexervhdl.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5283 2023-06-07 15:38:41.926375 PyQt6_QScintilla-2.14.1/src/qscilexerxml.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5531 2023-06-07 15:38:41.984954 PyQt6_QScintilla-2.14.1/src/qscilexeryaml.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7469 2023-06-07 15:38:42.136087 PyQt6_QScintilla-2.14.1/src/qscimacro.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    14299 2023-06-07 15:38:42.143714 PyQt6_QScintilla-2.14.1/src/qscintilla.pro
+-rw-r--r--   0 phil       (501) staff       (20)    44424 2023-06-07 15:18:08.620586 PyQt6_QScintilla-2.14.1/src/qscintilla_cs.qm
+-rw-r--r--   0 phil       (501) staff       (20)    82744 2023-06-07 15:18:08.635322 PyQt6_QScintilla-2.14.1/src/qscintilla_de.qm
+-rw-r--r--   0 phil       (501) staff       (20)    81850 2023-06-07 15:18:08.630276 PyQt6_QScintilla-2.14.1/src/qscintilla_es.qm
+-rw-r--r--   0 phil       (501) staff       (20)    53842 2023-06-07 15:18:08.625200 PyQt6_QScintilla-2.14.1/src/qscintilla_fr.qm
+-rw-r--r--   0 phil       (501) staff       (20)    49459 2023-06-07 15:18:08.622511 PyQt6_QScintilla-2.14.1/src/qscintilla_pt_br.qm
+-rw-r--r--   0 phil       (501) staff       (20)     5046 2023-06-07 15:38:42.197340 PyQt6_QScintilla-2.14.1/src/qsciprinter.cpp
+-rw-r--r--   0 phil       (501) staff       (20)   113218 2023-06-07 15:38:42.122065 PyQt6_QScintilla-2.14.1/src/qsciscintilla.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    21783 2023-06-07 15:38:41.998123 PyQt6_QScintilla-2.14.1/src/qsciscintillabase.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5035 2023-06-07 15:38:42.124633 PyQt6_QScintilla-2.14.1/src/qscistyle.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1620 2023-06-07 15:38:42.185511 PyQt6_QScintilla-2.14.1/src/qscistyledtext.cpp
```

### Comparing `PyQt6_QScintilla-2.14.0/ChangeLog` & `PyQt6_QScintilla-2.14.1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+2023-06-07  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, Python/project.py:
+	Rolled back the explicit setting of the minimum GLIBC version now
+	that we have changed the build platform.
+	[4ea73206e689] [2.14.1] <2.14-maint>
+
+2023-05-22  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, qt/InputMethod.cpp, qt/qscintilla.pro:
+	Fixed a pointer truncation in the handling of input method queries.
+	[e3a47ebe8c93] <2.14-maint>
+
+2023-05-14  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, Python/project.py:
+	Fixed the manylinux wheel tag when building on Ubuntu 22.04.
+	[77c97572f18c] <2.14-maint>
+
+2023-04-27  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* .hgtags:
+	Added tag 2.14.0 for changeset b748338e45bb
+	[670c1fb1beeb]
+
 2023-04-24  Phil Thompson  <phil@riverbankcomputing.com>
 
 	* NEWS, qt/qsciscintilla.cpp:
 	Fixed a regression in QSciScintilla::text().
 	[b748338e45bb] [2.14.0]
 
 2023-04-20  Phil Thompson  <phil@riverbankcomputing.com>
```

### Comparing `PyQt6_QScintilla-2.14.0/LICENSE` & `PyQt6_QScintilla-2.14.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/NEWS` & `PyQt6_QScintilla-2.14.1/NEWS`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+v2.14.1 7th June 2023
+  - Bug fixes.
+
 v2.14.0 24th April 2023
   - Added the QsciLexerAsm, QsciLexerMASM and QsciLexerNASM classes.
   - Added the QsciLexerHex, QsciLexerIntelHex, QsciLexerSRec and
     QsciLexerTekHex classes.
   - Bug fixes.
 
 v2.13.4 6th December 2022
```

### Comparing `PyQt6_QScintilla-2.14.0/PKG-INFO` & `PyQt6_QScintilla-2.14.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-QScintilla
-Version: 2.14.0
+Version: 2.14.1
 Requires-Python: >=3.7
 Summary: Python bindings for the QScintilla programmers editor widget
 Home-Page: https://www.riverbankcomputing.com/software/qscintilla/
 Author: Riverbank Computing Limited
 Author-Email: info@riverbankcomputing.com
 License: GPL v3
 Requires-Dist: PyQt6 (>=6.0.3)
```

### Comparing `PyQt6_QScintilla-2.14.0/README` & `PyQt6_QScintilla-2.14.1/README`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/project.py` & `PyQt6_QScintilla-2.14.1/project.py`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/pyproject.toml` & `PyQt6_QScintilla-2.14.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["sip >=6.0.2, <7", "PyQt-builder >=1.6, <2"]
 build-backend = "sipbuild.api"
 
 # Specify the PEP 566 metadata for the project.
 [tool.sip.metadata]
 name = "PyQt6-QScintilla"
-version = "2.14.0"
+version = "2.14.1"
 summary = "Python bindings for the QScintilla programmers editor widget"
 home-page = "https://www.riverbankcomputing.com/software/qscintilla/"
 author = "Riverbank Computing Limited"
 author-email = "info@riverbankcomputing.com"
 license = "GPL v3"
 description-file = "README"
 requires-dist = "PyQt6 (>=6.0.3)"
```

### Comparing `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-2.4.api` & `PyQt6_QScintilla-2.14.1/qsci/api/python/Python-2.4.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-2.5.api` & `PyQt6_QScintilla-2.14.1/qsci/api/python/Python-2.5.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-2.6.api` & `PyQt6_QScintilla-2.14.1/qsci/api/python/Python-2.6.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-2.7.api` & `PyQt6_QScintilla-2.14.1/qsci/api/python/Python-2.7.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.1.api` & `PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.1.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.10.api` & `PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.10.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.11.api` & `PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.11.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.2.api` & `PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.2.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.3.api` & `PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.3.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.4.api` & `PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.4.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.5.api` & `PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.5.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.6.api` & `PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.6.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.7.api` & `PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.7.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.8.api` & `PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.8.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.9.api` & `PyQt6_QScintilla-2.14.1/qsci/api/python/Python-3.9.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/include/ILexer.h` & `PyQt6_QScintilla-2.14.1/scintilla/include/ILexer.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/include/ILoader.h` & `PyQt6_QScintilla-2.14.1/scintilla/include/ILoader.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/include/License.txt` & `PyQt6_QScintilla-2.14.1/scintilla/include/License.txt`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/include/Platform.h` & `PyQt6_QScintilla-2.14.1/scintilla/include/Platform.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/include/SciLexer.h` & `PyQt6_QScintilla-2.14.1/scintilla/include/SciLexer.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/include/Sci_Position.h` & `PyQt6_QScintilla-2.14.1/scintilla/include/Sci_Position.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/include/Scintilla.h` & `PyQt6_QScintilla-2.14.1/scintilla/include/Scintilla.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/include/Scintilla.iface` & `PyQt6_QScintilla-2.14.1/scintilla/include/Scintilla.iface`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/include/ScintillaWidget.h` & `PyQt6_QScintilla-2.14.1/scintilla/include/ScintillaWidget.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexA68k.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexA68k.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAPDL.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexAPDL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexASY.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexASY.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAU3.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexAU3.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAVE.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexAVE.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAVS.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexAVS.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAbaqus.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexAbaqus.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAda.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexAda.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAsm.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexAsm.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAsn1.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexAsn1.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBaan.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexBaan.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBash.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexBash.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBasic.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexBasic.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBatch.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexBatch.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBibTeX.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexBibTeX.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBullant.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexBullant.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCLW.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCLW.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCOBOL.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCOBOL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCPP.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCPP.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCSS.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCSS.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCaml.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCaml.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCmake.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCmake.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCoffeeScript.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCoffeeScript.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexConf.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexConf.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCrontab.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCrontab.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCsound.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexCsound.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexD.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexD.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexDMAP.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexDMAP.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexDMIS.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexDMIS.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexDiff.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexDiff.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexECL.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexECL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexEDIFACT.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexEDIFACT.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexEScript.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexEScript.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexEiffel.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexEiffel.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexErlang.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexErlang.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexErrorList.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexErrorList.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexFlagship.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexFlagship.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexForth.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexForth.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexFortran.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexFortran.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexGAP.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexGAP.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexGui4Cli.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexGui4Cli.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexHTML.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexHTML.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexHaskell.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexHaskell.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexHex.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexHex.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexIndent.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexIndent.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexInno.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexInno.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexJSON.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexJSON.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexKVIrc.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexKVIrc.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexKix.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexKix.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLPeg.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexLPeg.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLaTeX.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexLaTeX.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLisp.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexLisp.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLout.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexLout.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLua.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexLua.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMMIXAL.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMMIXAL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMPT.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMPT.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMSSQL.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMSSQL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMagik.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMagik.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMake.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMake.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMarkdown.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMarkdown.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMatlab.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMatlab.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMaxima.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMaxima.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMetapost.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMetapost.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexModula.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexModula.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMySQL.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexMySQL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexNimrod.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexNimrod.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexNsis.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexNsis.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexNull.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexNull.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexOScript.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexOScript.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexOpal.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexOpal.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPB.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPB.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPLM.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPLM.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPO.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPO.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPOV.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPOV.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPS.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPS.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPascal.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPascal.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPerl.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPerl.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPowerPro.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPowerPro.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPowerShell.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPowerShell.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexProgress.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexProgress.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexProps.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexProps.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPython.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexPython.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexR.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexR.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexRebol.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexRebol.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexRegistry.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexRegistry.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexRuby.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexRuby.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexRust.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexRust.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSAS.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexSAS.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSML.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexSML.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSQL.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexSQL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSTTXT.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexSTTXT.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexScriptol.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexScriptol.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSmalltalk.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexSmalltalk.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSorcus.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexSorcus.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSpecman.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexSpecman.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSpice.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexSpice.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexStata.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexStata.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTACL.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexTACL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTADS3.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexTADS3.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTAL.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexTAL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTCL.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexTCL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTCMD.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexTCMD.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTeX.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexTeX.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTxt2tags.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexTxt2tags.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexVB.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexVB.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexVHDL.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexVHDL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexVerilog.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexVerilog.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexVisualProlog.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexVisualProlog.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexYAML.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/LexYAML.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexers/License.txt` & `PyQt6_QScintilla-2.14.1/scintilla/lexers/License.txt`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/Accessor.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/Accessor.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/Accessor.h` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/Accessor.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/CharacterCategory.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/CharacterCategory.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/CharacterCategory.h` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/CharacterCategory.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/CharacterSet.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/CharacterSet.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/CharacterSet.h` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/CharacterSet.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/DefaultLexer.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/DefaultLexer.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/DefaultLexer.h` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/DefaultLexer.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexAccessor.h` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexAccessor.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerBase.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexerBase.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerBase.h` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexerBase.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerModule.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexerModule.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerModule.h` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexerModule.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerNoExceptions.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexerNoExceptions.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerNoExceptions.h` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexerNoExceptions.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerSimple.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexerSimple.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerSimple.h` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/LexerSimple.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/License.txt` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/License.txt`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/OptionSet.h` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/OptionSet.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/PropSetSimple.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/PropSetSimple.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/PropSetSimple.h` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/PropSetSimple.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/SparseState.h` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/SparseState.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/StringCopy.h` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/StringCopy.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/StyleContext.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/StyleContext.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/StyleContext.h` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/StyleContext.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/SubStyles.h` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/SubStyles.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/WordList.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/WordList.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/lexlib/WordList.h` & `PyQt6_QScintilla-2.14.1/scintilla/lexlib/WordList.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/AutoComplete.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/AutoComplete.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/AutoComplete.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/AutoComplete.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/CallTip.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/CallTip.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/CallTip.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/CallTip.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/CaseConvert.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/CaseConvert.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/CaseConvert.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/CaseConvert.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/CaseFolder.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/CaseFolder.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/CaseFolder.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/CaseFolder.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/Catalogue.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/Catalogue.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/Catalogue.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/Catalogue.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/CellBuffer.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/CellBuffer.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/CellBuffer.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/CellBuffer.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/CharClassify.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/CharClassify.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/CharClassify.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/CharClassify.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/ContractionState.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/ContractionState.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/ContractionState.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/ContractionState.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/DBCS.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/DBCS.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/Decoration.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/Decoration.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/Decoration.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/Decoration.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/Document.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/Document.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/Document.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/Document.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/EditModel.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/EditModel.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/EditModel.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/EditModel.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/EditView.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/EditView.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/EditView.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/EditView.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/Editor.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/Editor.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/Editor.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/Editor.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/ElapsedPeriod.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/ElapsedPeriod.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/ExternalLexer.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/ExternalLexer.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/ExternalLexer.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/ExternalLexer.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/FontQuality.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/FontQuality.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/Indicator.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/Indicator.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/Indicator.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/Indicator.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/IntegerRectangle.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/IntegerRectangle.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/KeyMap.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/KeyMap.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/KeyMap.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/KeyMap.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/License.txt` & `PyQt6_QScintilla-2.14.1/scintilla/src/License.txt`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/LineMarker.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/LineMarker.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/LineMarker.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/LineMarker.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/MarginView.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/MarginView.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/MarginView.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/MarginView.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/Partitioning.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/Partitioning.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/PerLine.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/PerLine.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/PerLine.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/PerLine.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/Position.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/Position.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/PositionCache.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/PositionCache.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/PositionCache.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/PositionCache.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/RESearch.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/RESearch.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/RESearch.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/RESearch.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/RunStyles.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/RunStyles.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/RunStyles.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/RunStyles.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/ScintillaBase.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/ScintillaBase.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/ScintillaBase.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/ScintillaBase.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/Selection.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/Selection.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/Selection.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/Selection.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/SparseVector.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/SparseVector.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/SplitVector.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/SplitVector.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/Style.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/Style.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/Style.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/Style.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/UniConversion.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/UniConversion.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/UniConversion.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/UniConversion.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/UniqueString.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/UniqueString.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/ViewStyle.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/ViewStyle.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/ViewStyle.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/ViewStyle.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/XPM.cpp` & `PyQt6_QScintilla-2.14.1/scintilla/src/XPM.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/scintilla/src/XPM.h` & `PyQt6_QScintilla-2.14.1/scintilla/src/XPM.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qsciabstractapis.sip` & `PyQt6_QScintilla-2.14.1/sip/qsciabstractapis.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qsciapis.sip` & `PyQt6_QScintilla-2.14.1/sip/qsciapis.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscicommand.sip` & `PyQt6_QScintilla-2.14.1/sip/qscicommand.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscicommandset.sip` & `PyQt6_QScintilla-2.14.1/sip/qscicommandset.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscidocument.sip` & `PyQt6_QScintilla-2.14.1/sip/qscidocument.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexer.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerasm.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerasm.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexeravs.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexeravs.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerbash.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerbash.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerbatch.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerbatch.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexercmake.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexercmake.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexercoffeescript.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexercoffeescript.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexercpp.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexercpp.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexercsharp.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexercsharp.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexercss.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexercss.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexercustom.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexercustom.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerd.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerd.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerdiff.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerdiff.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexeredifact.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexeredifact.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerfortran.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerfortran.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerfortran77.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerfortran77.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerhex.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerhex.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerhtml.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerhtml.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexeridl.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexeridl.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerintelhex.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerintelhex.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerjava.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerjava.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerjavascript.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerjavascript.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerjson.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerjson.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerlua.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerlua.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexermakefile.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexermakefile.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexermarkdown.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexermarkdown.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexermasm.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexermasm.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexermatlab.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexermatlab.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexernasm.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexernasm.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexeroctave.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexeroctave.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerpascal.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerpascal.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerperl.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerperl.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerpo.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerpo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerpostscript.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerpostscript.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerpov.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerpov.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerproperties.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerproperties.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerpython.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerpython.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerruby.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerruby.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerspice.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerspice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexersql.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexersql.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexersrec.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexersrec.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexertcl.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexertcl.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexertekhex.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexertekhex.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexertex.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexertex.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerverilog.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerverilog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexervhdl.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexervhdl.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexerxml.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexerxml.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscilexeryaml.sip` & `PyQt6_QScintilla-2.14.1/sip/qscilexeryaml.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscimacro.sip` & `PyQt6_QScintilla-2.14.1/sip/qscimacro.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscimod5.sip` & `PyQt6_QScintilla-2.14.1/sip/qscimod5.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscimod6.sip` & `PyQt6_QScintilla-2.14.1/sip/qscimod6.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscimodcommon.sip` & `PyQt6_QScintilla-2.14.1/sip/qscimodcommon.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qsciprinter.sip` & `PyQt6_QScintilla-2.14.1/sip/qsciprinter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qsciscintilla.sip` & `PyQt6_QScintilla-2.14.1/sip/qsciscintilla.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qsciscintillabase.sip` & `PyQt6_QScintilla-2.14.1/sip/qsciscintillabase.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscistyle.sip` & `PyQt6_QScintilla-2.14.1/sip/qscistyle.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/sip/qscistyledtext.sip` & `PyQt6_QScintilla-2.14.1/sip/qscistyledtext.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/InputMethod.cpp` & `PyQt6_QScintilla-2.14.1/src/InputMethod.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -250,23 +250,15 @@
 
         case Qt::ImSurroundingText:
         {
             int paraStart = sci->pdoc->ParaUp(pos);
             int paraEnd = sci->pdoc->ParaDown(pos);
             QVarLengthArray<char,1024> buffer(paraEnd - paraStart + 1);
 
-            Sci_CharacterRange charRange;
-            charRange.cpMin = paraStart;
-            charRange.cpMax = paraEnd;
-
-            Sci_TextRange textRange;
-            textRange.chrg = charRange;
-            textRange.lpstrText = buffer.data();
-
-            SendScintilla(SCI_GETTEXTRANGE, 0, (sptr_t)&textRange);
+            SendScintilla(SCI_GETTEXTRANGE, paraStart, paraEnd, buffer.data());
 
             return bytesAsText(buffer.constData(), buffer.size());
         }
 
         case Qt::ImCurrentSelection:
         {
             QVarLengthArray<char,1024> buffer(SendScintilla(SCI_GETSELTEXT) + 1);
```

### Comparing `PyQt6_QScintilla-2.14.0/src/ListBoxQt.cpp` & `PyQt6_QScintilla-2.14.1/src/ListBoxQt.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/ListBoxQt.h` & `PyQt6_QScintilla-2.14.1/src/ListBoxQt.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/MacPasteboardMime.cpp` & `PyQt6_QScintilla-2.14.1/src/MacPasteboardMime.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/PlatQt.cpp` & `PyQt6_QScintilla-2.14.1/src/PlatQt.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qsciabstractapis.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qsciabstractapis.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qsciapis.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qsciapis.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscicommand.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscicommand.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscicommandset.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscicommandset.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscidocument.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscidocument.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qsciglobal.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qsciglobal.h`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 #ifndef QSCIGLOBAL_H
 #define QSCIGLOBAL_H
 
 #include <qglobal.h>
 
 
-#define QSCINTILLA_VERSION      0x020e00
-#define QSCINTILLA_VERSION_STR  "2.14.0"
+#define QSCINTILLA_VERSION      0x020e01
+#define QSCINTILLA_VERSION_STR  "2.14.1"
 
 
 // We only support Qt v5.11 and later.
 #if QT_VERSION < 0x050b00
 #error "Qt v5.11.0 or later is required"
 #endif
```

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexer.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexer.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerasm.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerasm.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeravs.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexeravs.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerbash.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerbash.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerbatch.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerbatch.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercmake.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexercmake.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercoffeescript.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexercoffeescript.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercpp.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexercpp.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercsharp.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexercsharp.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercss.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexercss.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercustom.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexercustom.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerd.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerd.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerdiff.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerdiff.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeredifact.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexeredifact.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerfortran.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerfortran.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerfortran77.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerfortran77.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerhex.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerhex.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerhtml.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerhtml.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeridl.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexeridl.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerintelhex.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerintelhex.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerjava.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerjava.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerjavascript.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerjavascript.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerjson.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerjson.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerlua.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerlua.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexermakefile.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexermakefile.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexermarkdown.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexermarkdown.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexermasm.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexermasm.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexermatlab.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexermatlab.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexernasm.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexernasm.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeroctave.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexeroctave.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpascal.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerpascal.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerperl.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerperl.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpo.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerpo.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpostscript.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerpostscript.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpov.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerpov.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerproperties.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerproperties.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpython.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerpython.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerruby.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerruby.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerspice.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerspice.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexersql.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexersql.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexersrec.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexersrec.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexertcl.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexertcl.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexertekhex.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexertekhex.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexertex.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexertex.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerverilog.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerverilog.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexervhdl.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexervhdl.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerxml.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexerxml.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeryaml.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscilexeryaml.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscimacro.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscimacro.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qsciprinter.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qsciprinter.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qsciscintilla.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qsciscintilla.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qsciscintillabase.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qsciscintillabase.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscistyle.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscistyle.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/Qsci/qscistyledtext.h` & `PyQt6_QScintilla-2.14.1/src/Qsci/qscistyledtext.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/SciAccessibility.cpp` & `PyQt6_QScintilla-2.14.1/src/SciAccessibility.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/SciAccessibility.h` & `PyQt6_QScintilla-2.14.1/src/SciAccessibility.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/SciClasses.cpp` & `PyQt6_QScintilla-2.14.1/src/SciClasses.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/SciClasses.h` & `PyQt6_QScintilla-2.14.1/src/SciClasses.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/ScintillaQt.cpp` & `PyQt6_QScintilla-2.14.1/src/ScintillaQt.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/ScintillaQt.h` & `PyQt6_QScintilla-2.14.1/src/ScintillaQt.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/features/qscintilla2.prf` & `PyQt6_QScintilla-2.14.1/src/features/qscintilla2.prf`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qsciabstractapis.cpp` & `PyQt6_QScintilla-2.14.1/src/qsciabstractapis.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qsciapis.cpp` & `PyQt6_QScintilla-2.14.1/src/qsciapis.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscicommand.cpp` & `PyQt6_QScintilla-2.14.1/src/qscicommand.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscicommandset.cpp` & `PyQt6_QScintilla-2.14.1/src/qscicommandset.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscidocument.cpp` & `PyQt6_QScintilla-2.14.1/src/qscidocument.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexer.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexer.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerasm.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerasm.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexeravs.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexeravs.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerbash.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerbash.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerbatch.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerbatch.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexercmake.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexercmake.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexercoffeescript.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexercoffeescript.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexercpp.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexercpp.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexercsharp.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexercsharp.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexercss.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexercss.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexercustom.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexercustom.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerd.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerd.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerdiff.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerdiff.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexeredifact.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexeredifact.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerfortran.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerfortran.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerfortran77.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerfortran77.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerhex.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerhex.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerhtml.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerhtml.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexeridl.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexeridl.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerintelhex.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerintelhex.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerjava.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerjava.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerjavascript.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerjavascript.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerjson.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerjson.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerlua.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerlua.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexermakefile.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexermakefile.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexermarkdown.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexermarkdown.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexermasm.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexermasm.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexermatlab.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexermatlab.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexernasm.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexernasm.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexeroctave.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexeroctave.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerpascal.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerpascal.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerperl.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerperl.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerpo.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerpo.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerpostscript.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerpostscript.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerpov.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerpov.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerproperties.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerproperties.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerpython.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerpython.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerruby.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerruby.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerspice.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerspice.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexersql.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexersql.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexersrec.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexersrec.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexertcl.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexertcl.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexertekhex.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexertekhex.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexertex.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexertex.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerverilog.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerverilog.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexervhdl.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexervhdl.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexerxml.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexerxml.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscilexeryaml.cpp` & `PyQt6_QScintilla-2.14.1/src/qscilexeryaml.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscimacro.cpp` & `PyQt6_QScintilla-2.14.1/src/qscimacro.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscintilla.pro` & `PyQt6_QScintilla-2.14.1/src/qscintilla.pro`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # then you may purchase a commercial license.  For more information contact
 # info@riverbankcomputing.com.
 # 
 # This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 # WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-!win32:VERSION = 15.2.0
+!win32:VERSION = 15.2.1
 
 TEMPLATE = lib
 CONFIG += qt warn_off thread exceptions hide_symbols
 
 CONFIG(debug, debug|release) {
     mac: {
         TARGET = qscintilla2_qt$${QT_MAJOR_VERSION}_debug
```

### Comparing `PyQt6_QScintilla-2.14.0/src/qscintilla_cs.qm` & `PyQt6_QScintilla-2.14.1/src/qscintilla_cs.qm`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscintilla_de.qm` & `PyQt6_QScintilla-2.14.1/src/qscintilla_de.qm`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscintilla_es.qm` & `PyQt6_QScintilla-2.14.1/src/qscintilla_es.qm`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscintilla_fr.qm` & `PyQt6_QScintilla-2.14.1/src/qscintilla_fr.qm`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscintilla_pt_br.qm` & `PyQt6_QScintilla-2.14.1/src/qscintilla_pt_br.qm`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qsciprinter.cpp` & `PyQt6_QScintilla-2.14.1/src/qsciprinter.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qsciscintilla.cpp` & `PyQt6_QScintilla-2.14.1/src/qsciscintilla.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qsciscintillabase.cpp` & `PyQt6_QScintilla-2.14.1/src/qsciscintillabase.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscistyle.cpp` & `PyQt6_QScintilla-2.14.1/src/qscistyle.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.14.0/src/qscistyledtext.cpp` & `PyQt6_QScintilla-2.14.1/src/qscistyledtext.cpp`

 * *Files identical despite different names*

