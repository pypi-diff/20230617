# Comparing `tmp/lief-0.8.3.post3.zip` & `tmp/lief-0.9.0.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,343 +1,336 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                      5682 (0000000000001632h)
-  Actual end-cent-dir record offset:          5660 (000000000000161Ch)
-  Expected end-cent-dir record offset:        5660 (000000000000161Ch)
+  Zip archive file size:                      5699 (0000000000001643h)
+  Actual end-cent-dir record offset:          5677 (000000000000162Dh)
+  Expected end-cent-dir record offset:        5677 (000000000000162Dh)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
   central directory contains 11 entries.
-  The central directory is 855 (0000000000000357h) bytes long,
+  The central directory is 819 (0000000000000333h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 4805 (00000000000012C5h).
+  is 4858 (00000000000012FAh).
 
 
 Central directory entry #1:
 ---------------------------
 
-  lief-0.8.3/MANIFEST.in
+  lief-0.9.0/setup.py
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2017 Oct 29 17:37:38
-  32-bit CRC value (hex):                         c8ffc06a
-  compressed size:                                28 bytes
-  uncompressed size:                              26 bytes
-  length of filename:                             22 characters
+  file last modified on (DOS date/time):          2018 Jun 10 16:34:46
+  32-bit CRC value (hex):                         2fc5017e
+  compressed size:                                2165 bytes
+  uncompressed size:                              9315 bytes
+  length of filename:                             19 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  lief-0.8.3/PKG-INFO
+  lief-0.9.0/setup.cfg
 
-  offset of local header from start of archive:   80
-                                                  (0000000000000050h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   2214
+                                                  (00000000000008A6h) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2017 Oct 29 18:07:02
-  32-bit CRC value (hex):                         a80859be
-  compressed size:                                481 bytes
-  uncompressed size:                              1084 bytes
-  length of filename:                             19 characters
+  file last modified on (DOS date/time):          2018 Jun 10 16:38:36
+  32-bit CRC value (hex):                         6da1bd14
+  compressed size:                                471 bytes
+  uncompressed size:                              899 bytes
+  length of filename:                             20 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  lief-0.8.3/README
+  lief-0.9.0/README
 
-  offset of local header from start of archive:   610
-                                                  (0000000000000262h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   2735
+                                                  (0000000000000AAFh) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2017 Oct 29 17:37:38
-  32-bit CRC value (hex):                         34359ace
-  compressed size:                                303 bytes
-  uncompressed size:                              529 bytes
+  file last modified on (DOS date/time):          2018 Jun 10 16:34:46
+  32-bit CRC value (hex):                         03642846
+  compressed size:                                296 bytes
+  uncompressed size:                              514 bytes
   length of filename:                             17 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  lief-0.8.3/lief.egg-info/PKG-INFO
+  lief-0.9.0/MANIFEST.in
 
-  offset of local header from start of archive:   960
-                                                  (00000000000003C0h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   3078
+                                                  (0000000000000C06h) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2017 Oct 29 18:07:02
-  32-bit CRC value (hex):                         a80859be
-  compressed size:                                481 bytes
-  uncompressed size:                              1084 bytes
-  length of filename:                             33 characters
+  file last modified on (DOS date/time):          2018 Jun 10 16:34:46
+  32-bit CRC value (hex):                         b99f0fbd
+  compressed size:                                27 bytes
+  uncompressed size:                              25 bytes
+  length of filename:                             22 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
-  lief-0.8.3/lief.egg-info/SOURCES.txt
+  lief-0.9.0/PKG-INFO
 
-  offset of local header from start of archive:   1504
-                                                  (00000000000005E0h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   3157
+                                                  (0000000000000C55h) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2017 Oct 29 18:07:02
-  32-bit CRC value (hex):                         7cef749c
-  compressed size:                                121 bytes
-  uncompressed size:                              193 bytes
-  length of filename:                             36 characters
+  file last modified on (DOS date/time):          2018 Jun 10 16:38:36
+  32-bit CRC value (hex):                         c601fb45
+  compressed size:                                457 bytes
+  uncompressed size:                              1023 bytes
+  length of filename:                             19 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #6:
 ---------------------------
 
-  lief-0.8.3/lief.egg-info/dependency_links.txt
+  lief-0.9.0/lief.egg-info/top_level.txt
 
-  offset of local header from start of archive:   1691
-                                                  (000000000000069Bh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   3663
+                                                  (0000000000000E4Fh) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2017 Oct 29 18:07:02
-  32-bit CRC value (hex):                         32d70693
-  compressed size:                                3 bytes
-  uncompressed size:                              1 bytes
-  length of filename:                             45 characters
+  file last modified on (DOS date/time):          2018 Jun 10 16:38:36
+  32-bit CRC value (hex):                         edc46012
+  compressed size:                                11 bytes
+  uncompressed size:                              13 bytes
+  length of filename:                             38 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #7:
 ---------------------------
 
-  lief-0.8.3/lief.egg-info/not-zip-safe
+  lief-0.9.0/lief.egg-info/not-zip-safe
 
-  offset of local header from start of archive:   1769
-                                                  (00000000000006E9h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   3742
+                                                  (0000000000000E9Eh) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2017 Oct 29 18:07:00
-  32-bit CRC value (hex):                         14a285ac
-  compressed size:                                4 bytes
-  uncompressed size:                              2 bytes
+  file last modified on (DOS date/time):          2018 Jun 10 16:38:34
+  32-bit CRC value (hex):                         32d70693
+  compressed size:                                3 bytes
+  uncompressed size:                              1 bytes
   length of filename:                             37 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #8:
 ---------------------------
 
-  lief-0.8.3/lief.egg-info/top_level.txt
+  lief-0.9.0/lief.egg-info/PKG-INFO
 
-  offset of local header from start of archive:   1840
-                                                  (0000000000000730h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   3812
+                                                  (0000000000000EE4h) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2017 Oct 29 18:07:02
-  32-bit CRC value (hex):                         edc46012
-  compressed size:                                11 bytes
-  uncompressed size:                              13 bytes
-  length of filename:                             38 characters
+  file last modified on (DOS date/time):          2018 Jun 10 16:38:36
+  32-bit CRC value (hex):                         c601fb45
+  compressed size:                                457 bytes
+  uncompressed size:                              1023 bytes
+  length of filename:                             33 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #9:
 ---------------------------
 
-  lief-0.8.3/lief/__init__.py
+  lief-0.9.0/lief.egg-info/dependency_links.txt
 
-  offset of local header from start of archive:   1919
-                                                  (000000000000077Fh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   4332
+                                                  (00000000000010ECh) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2017 Oct 29 17:37:38
-  32-bit CRC value (hex):                         84eb79c9
-  compressed size:                                150 bytes
-  uncompressed size:                              349 bytes
-  length of filename:                             27 characters
+  file last modified on (DOS date/time):          2018 Jun 10 16:38:36
+  32-bit CRC value (hex):                         32d70693
+  compressed size:                                3 bytes
+  uncompressed size:                              1 bytes
+  length of filename:                             45 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #10:
 ---------------------------
 
-  lief-0.8.3/setup.cfg
+  lief-0.9.0/lief.egg-info/SOURCES.txt
 
-  offset of local header from start of archive:   2126
-                                                  (000000000000084Eh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   4410
+                                                  (000000000000113Ah) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2017 Oct 29 18:07:02
-  32-bit CRC value (hex):                         914a1a74
-  compressed size:                                479 bytes
-  uncompressed size:                              932 bytes
-  length of filename:                             20 characters
+  file last modified on (DOS date/time):          2018 Jun 10 16:38:36
+  32-bit CRC value (hex):                         7cef749c
+  compressed size:                                121 bytes
+  uncompressed size:                              193 bytes
+  length of filename:                             36 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #11:
 ---------------------------
 
-  lief-0.8.3/setup.py
+  lief-0.9.0/lief/__init__.py
 
-  offset of local header from start of archive:   2655
-                                                  (0000000000000A5Fh) bytes
+  offset of local header from start of archive:   4597
+                                                  (00000000000011F5h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   6.3
-  minimum file system compatibility required:     Unix
+  version of encoding software:                   2.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2017 Nov 21 16:56:02
-  32-bit CRC value (hex):                         c0234e57
-  compressed size:                                2101 bytes
-  uncompressed size:                              9441 bytes
-  length of filename:                             19 characters
-  length of extra field:                          36 bytes
+  file last modified on (DOS date/time):          2018 Jun 10 16:34:46
+  32-bit CRC value (hex):                         6aaa0cf1
+  compressed size:                                204 bytes
+  uncompressed size:                              715 bytes
+  length of filename:                             27 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (20 hex):                arc 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
-    20 are:   00 00 00 00 01 00 18 00 80 be 59 3a e1 62 d3 01 80 be 59 3a.
-
-  There is a local extra field with ID 0x5855 (old Info-ZIP Unix/OS2/NT) and
-  8 data bytes (GMT modification/access times only).
+  Unix file attributes (100664 octal):            -rw-rw-r--
+  MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
```

## zipnote {}

```diff
@@ -1,34 +1,34 @@
-Filename: lief-0.8.3/MANIFEST.in
+Filename: lief-0.9.0/setup.py
 Comment: 
 
-Filename: lief-0.8.3/PKG-INFO
+Filename: lief-0.9.0/setup.cfg
 Comment: 
 
-Filename: lief-0.8.3/README
+Filename: lief-0.9.0/README
 Comment: 
 
-Filename: lief-0.8.3/lief.egg-info/PKG-INFO
+Filename: lief-0.9.0/MANIFEST.in
 Comment: 
 
-Filename: lief-0.8.3/lief.egg-info/SOURCES.txt
+Filename: lief-0.9.0/PKG-INFO
 Comment: 
 
-Filename: lief-0.8.3/lief.egg-info/dependency_links.txt
+Filename: lief-0.9.0/lief.egg-info/top_level.txt
 Comment: 
 
-Filename: lief-0.8.3/lief.egg-info/not-zip-safe
+Filename: lief-0.9.0/lief.egg-info/not-zip-safe
 Comment: 
 
-Filename: lief-0.8.3/lief.egg-info/top_level.txt
+Filename: lief-0.9.0/lief.egg-info/PKG-INFO
 Comment: 
 
-Filename: lief-0.8.3/lief/__init__.py
+Filename: lief-0.9.0/lief.egg-info/dependency_links.txt
 Comment: 
 
-Filename: lief-0.8.3/setup.cfg
+Filename: lief-0.9.0/lief.egg-info/SOURCES.txt
 Comment: 
 
-Filename: lief-0.8.3/setup.py
+Filename: lief-0.9.0/lief/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `lief-0.8.3/PKG-INFO` & `lief-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-Metadata-Version: 1.1
-Name: lief
-Version: 0.8.3
-Summary: LIEF is a library to instrument executable formats
-Home-page: https://lief.quarkslab.com
-Author: Romain Thomas
-Author-email: rthomas@quarkslab.com
-License: Apache 2.0
-Description-Content-Type: UNKNOWN
-Description: UNKNOWN
-Keywords: parser,elf,pe,macho
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Security
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Software Development :: Build Tools
+Metadata-Version: 1.1
+Name: lief
+Version: 0.9.0
+Summary: LIEF is a library to instrument executable formats
+Home-page: https://lief.quarkslab.com
+Author: Romain Thomas
+Author-email: rthomas@quarkslab.com
+License: Apache 2.0
+Description: UNKNOWN
+Keywords: parser,elf,pe,macho
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Security
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development :: Build Tools
```

## Comparing `lief-0.8.3/README` & `lief-0.9.0/README`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-LIEF - Python API
------------------
-
-The purpose of this project is to provide a cross platform library which can parse, modify and abstract ELF, PE and MachO formats.
-
-Main features:
-
-  * Parsing: LIEF can parse ELF, PE, MachO and provides an user-friendly API to access to format internals.
-  * Modify: LIEF enables to modify some parts of these formats
-  * Abstract: Three formats have common features like sections, symbols, entry point... LIEF factors them.
-  * API: LIEF can be used in C, C++ and Python
-
-
-
-
+LIEF - Python API
+-----------------
+
+The purpose of this project is to provide a cross platform library which can parse, modify and abstract ELF, PE and MachO formats.
+
+Main features:
+
+  * Parsing: LIEF can parse ELF, PE, MachO and provides an user-friendly API to access to format internals.
+  * Modify: LIEF enables to modify some parts of these formats
+  * Abstract: Three formats have common features like sections, symbols, entry point... LIEF factors them.
+  * API: LIEF can be used in C, C++ and Python
+
+
+
+
```

## Comparing `lief-0.8.3/lief.egg-info/PKG-INFO` & `lief-0.9.0/lief.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-Metadata-Version: 1.1
-Name: lief
-Version: 0.8.3
-Summary: LIEF is a library to instrument executable formats
-Home-page: https://lief.quarkslab.com
-Author: Romain Thomas
-Author-email: rthomas@quarkslab.com
-License: Apache 2.0
-Description-Content-Type: UNKNOWN
-Description: UNKNOWN
-Keywords: parser,elf,pe,macho
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Security
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Software Development :: Build Tools
+Metadata-Version: 1.1
+Name: lief
+Version: 0.9.0
+Summary: LIEF is a library to instrument executable formats
+Home-page: https://lief.quarkslab.com
+Author: Romain Thomas
+Author-email: rthomas@quarkslab.com
+License: Apache 2.0
+Description: UNKNOWN
+Keywords: parser,elf,pe,macho
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Security
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development :: Build Tools
```

## Comparing `lief-0.8.3/setup.cfg` & `lief-0.9.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,57 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 206c 6965 660d 0a64 6573 6372 6970   = lief..descrip
-00000020: 7469 6f6e 203d 204c 4945 4620 6973 2061  tion = LIEF is a
-00000030: 206c 6962 7261 7279 2074 6f20 696e 7374   library to inst
-00000040: 7275 6d65 6e74 2065 7865 6375 7461 626c  rument executabl
-00000050: 6520 666f 726d 6174 730d 0a61 7574 686f  e formats..autho
-00000060: 7220 3d20 526f 6d61 696e 2054 686f 6d61  r = Romain Thoma
-00000070: 730d 0a61 7574 686f 725f 656d 6169 6c20  s..author_email 
-00000080: 3d20 7274 686f 6d61 7340 7175 6172 6b73  = rthomas@quarks
-00000090: 6c61 622e 636f 6d0d 0a75 726c 203d 2068  lab.com..url = h
-000000a0: 7474 7073 3a2f 2f6c 6965 662e 7175 6172  ttps://lief.quar
-000000b0: 6b73 6c61 622e 636f 6d0d 0a6c 6963 656e  kslab.com..licen
-000000c0: 7365 203d 2041 7061 6368 6520 322e 300d  se = Apache 2.0.
-000000d0: 0a6b 6579 776f 7264 7320 3d20 7061 7273  .keywords = pars
-000000e0: 6572 2c20 656c 662c 2070 652c 206d 6163  er, elf, pe, mac
-000000f0: 686f 0d0a 636c 6173 7369 6669 6572 7320  ho..classifiers 
-00000100: 3d20 0d0a 094c 6963 656e 7365 203a 3a20  = ...License :: 
-00000110: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-00000120: 4170 6163 6865 2053 6f66 7477 6172 6520  Apache Software 
-00000130: 4c69 6365 6e73 650d 0a09 4465 7665 6c6f  License...Develo
-00000140: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
-00000150: 3420 2d20 4265 7461 0d0a 0945 6e76 6972  4 - Beta...Envir
-00000160: 6f6e 6d65 6e74 203a 3a20 436f 6e73 6f6c  onment :: Consol
-00000170: 650d 0a09 496e 7465 6e64 6564 2041 7564  e...Intended Aud
-00000180: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
-00000190: 6572 730d 0a09 496e 7465 6e64 6564 2041  ers...Intended A
-000001a0: 7564 6965 6e63 6520 3a3a 2053 6369 656e  udience :: Scien
-000001b0: 6365 2f52 6573 6561 7263 680d 0a09 4f70  ce/Research...Op
-000001c0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-000001d0: 3a20 4d61 634f 5320 3a3a 204d 6163 4f53  : MacOS :: MacOS
-000001e0: 2058 0d0a 094f 7065 7261 7469 6e67 2053   X...Operating S
-000001f0: 7973 7465 6d20 3a3a 2050 4f53 4958 203a  ystem :: POSIX :
-00000200: 3a20 4c69 6e75 780d 0a09 4f70 6572 6174  : Linux...Operat
-00000210: 696e 6720 5379 7374 656d 203a 3a20 4d69  ing System :: Mi
-00000220: 6372 6f73 6f66 7420 3a3a 2057 696e 646f  crosoft :: Windo
-00000230: 7773 0d0a 0950 726f 6772 616d 6d69 6e67  ws...Programming
-00000240: 204c 616e 6775 6167 6520 3a3a 2043 2b2b   Language :: C++
-00000250: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000260: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000270: 6e20 3a3a 2032 0d0a 0950 726f 6772 616d  n :: 2...Program
-00000280: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000290: 2050 7974 686f 6e20 3a3a 2033 0d0a 0954   Python :: 3...T
-000002a0: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
-000002b0: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
-000002c0: 4c69 6272 6172 6965 730d 0a09 546f 7069  Libraries...Topi
-000002d0: 6320 3a3a 2053 6563 7572 6974 790d 0a09  c :: Security...
-000002e0: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
-000002f0: 6669 632f 456e 6769 6e65 6572 696e 6720  fic/Engineering 
-00000300: 3a3a 2049 6e66 6f72 6d61 7469 6f6e 2041  :: Information A
-00000310: 6e61 6c79 7369 730d 0a09 546f 7069 6320  nalysis...Topic 
-00000320: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-00000330: 6c6f 706d 656e 7420 3a3a 2042 7569 6c64  lopment :: Build
-00000340: 2054 6f6f 6c73 0d0a 0d0a 5b6f 7074 696f   Tools....[optio
-00000350: 6e73 5d0d 0a7a 6970 5f73 6166 6520 3d20  ns]..zip_safe = 
-00000360: 4661 6c73 650d 0a70 6163 6b61 6765 7320  False..packages 
-00000370: 3d20 6c69 6566 0d0a 0d0a 5b65 6767 5f69  = lief....[egg_i
-00000380: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-00000390: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-000003a0: 0d0a 0d0a                                ....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6c69 6566 0a64 6573 6372 6970 7469  = lief.descripti
+00000020: 6f6e 203d 204c 4945 4620 6973 2061 206c  on = LIEF is a l
+00000030: 6962 7261 7279 2074 6f20 696e 7374 7275  ibrary to instru
+00000040: 6d65 6e74 2065 7865 6375 7461 626c 6520  ment executable 
+00000050: 666f 726d 6174 730a 6175 7468 6f72 203d  formats.author =
+00000060: 2052 6f6d 6169 6e20 5468 6f6d 6173 0a61   Romain Thomas.a
+00000070: 7574 686f 725f 656d 6169 6c20 3d20 7274  uthor_email = rt
+00000080: 686f 6d61 7340 7175 6172 6b73 6c61 622e  homas@quarkslab.
+00000090: 636f 6d0a 7572 6c20 3d20 6874 7470 733a  com.url = https:
+000000a0: 2f2f 6c69 6566 2e71 7561 726b 736c 6162  //lief.quarkslab
+000000b0: 2e63 6f6d 0a6c 6963 656e 7365 203d 2041  .com.license = A
+000000c0: 7061 6368 6520 322e 300a 6b65 7977 6f72  pache 2.0.keywor
+000000d0: 6473 203d 2070 6172 7365 722c 2065 6c66  ds = parser, elf
+000000e0: 2c20 7065 2c20 6d61 6368 6f0a 636c 6173  , pe, macho.clas
+000000f0: 7369 6669 6572 7320 3d20 0a09 4c69 6365  sifiers = ..Lice
+00000100: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000110: 7665 6420 3a3a 2041 7061 6368 6520 536f  ved :: Apache So
+00000120: 6674 7761 7265 204c 6963 656e 7365 0a09  ftware License..
+00000130: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
+00000140: 7573 203a 3a20 3420 2d20 4265 7461 0a09  us :: 4 - Beta..
+00000150: 456e 7669 726f 6e6d 656e 7420 3a3a 2043  Environment :: C
+00000160: 6f6e 736f 6c65 0a09 496e 7465 6e64 6564  onsole..Intended
+00000170: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
+00000180: 656c 6f70 6572 730a 0949 6e74 656e 6465  elopers..Intende
+00000190: 6420 4175 6469 656e 6365 203a 3a20 5363  d Audience :: Sc
+000001a0: 6965 6e63 652f 5265 7365 6172 6368 0a09  ience/Research..
+000001b0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+000001c0: 203a 3a20 4d61 634f 5320 3a3a 204d 6163   :: MacOS :: Mac
+000001d0: 4f53 2058 0a09 4f70 6572 6174 696e 6720  OS X..Operating 
+000001e0: 5379 7374 656d 203a 3a20 504f 5349 5820  System :: POSIX 
+000001f0: 3a3a 204c 696e 7578 0a09 4f70 6572 6174  :: Linux..Operat
+00000200: 696e 6720 5379 7374 656d 203a 3a20 4d69  ing System :: Mi
+00000210: 6372 6f73 6f66 7420 3a3a 2057 696e 646f  crosoft :: Windo
+00000220: 7773 0a09 5072 6f67 7261 6d6d 696e 6720  ws..Programming 
+00000230: 4c61 6e67 7561 6765 203a 3a20 432b 2b0a  Language :: C++.
+00000240: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000250: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000260: 3a3a 2032 0a09 5072 6f67 7261 6d6d 696e  :: 2..Programmin
+00000270: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000280: 7468 6f6e 203a 3a20 330a 0954 6f70 6963  thon :: 3..Topic
+00000290: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
+000002a0: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
+000002b0: 6172 6965 730a 0954 6f70 6963 203a 3a20  aries..Topic :: 
+000002c0: 5365 6375 7269 7479 0a09 546f 7069 6320  Security..Topic 
+000002d0: 3a3a 2053 6369 656e 7469 6669 632f 456e  :: Scientific/En
+000002e0: 6769 6e65 6572 696e 6720 3a3a 2049 6e66  gineering :: Inf
+000002f0: 6f72 6d61 7469 6f6e 2041 6e61 6c79 7369  ormation Analysi
+00000300: 730a 0954 6f70 6963 203a 3a20 536f 6674  s..Topic :: Soft
+00000310: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
+00000320: 203a 3a20 4275 696c 6420 546f 6f6c 730a   :: Build Tools.
+00000330: 0a5b 6f70 7469 6f6e 735d 0a7a 6970 5f73  .[options].zip_s
+00000340: 6166 6520 3d20 4661 6c73 650a 7061 636b  afe = False.pack
+00000350: 6167 6573 203d 206c 6965 660a 0a5b 6567  ages = lief..[eg
+00000360: 675f 696e 666f 5d0a 7461 675f 6275 696c  g_info].tag_buil
+00000370: 6420 3d20 0a74 6167 5f64 6174 6520 3d20  d = .tag_date = 
+00000380: 300a 0a                                  0..
```

## Comparing `lief-0.8.3/setup.py` & `lief-0.9.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,283 +1,287 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-MIN_SETUPTOOLS_VERSION = "31.0.0"
-import setuptools
-from distutils.version import LooseVersion
-assert (LooseVersion(setuptools.__version__) >= LooseVersion(MIN_SETUPTOOLS_VERSION)), "LIEF requires a setuptools version '{}' or higher".format(MIN_SETUPTOOLS_VERSION)
-
-from setuptools import setup
-from setuptools.command.build_ext import build_ext
-from distutils.dir_util import remove_tree, mkpath
-from setuptools.command.bdist_egg import bdist_egg
-from setuptools.command.bdist_egg import log as bdist_egg_log
-
-from setuptools.command.sdist import sdist
-from setuptools.command.sdist import log as sdist_log
-
-from setuptools.extension import Extension
-
-import re
-import os
-import platform
-import shutil
-import sys
-import struct
-import zipfile
-
-try:
-    from urllib.request import urlopen, Request
-except:
-    from urllib2 import urlopen, Request
-
-
-try:
-    from io import BytesIO
-except:
-    try:
-        from cStringIO import StringIO as BytesIO
-    except:
-        from StringIO import StringIO as BytesIO
-
-package_dir       = os.path.dirname(os.path.realpath(__file__))
-pkg_info          = os.path.join(package_dir, "PKG-INFO")
-in_source_package = os.path.isfile(pkg_info) # (e.g. pip)
-
-is_branch = False
-
-libpylief = {
-        'Windows': "_pylief.pyd",
-        'Darwin': "_pylief.so",
-        'Linux': "_pylief.so",
-        }
-version_re = r"Version:\s+(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)\.?(.*)"
-if in_source_package:
-    with open(pkg_info, "r") as f:
-        major, minor, patch, branch = re.findall(version_re, f.read(), re.MULTILINE)[0]
-        lief_version = "{:d}.{:d}.{:d}".format(int(major), int(minor), int(patch))
-        is_branch = len(branch.strip()) > 0
-else:
-    lief_version = "0.8.3"
-
-package_description = open(os.path.join(package_dir, "README")).read()
-
-
-def get_lief_platform_name():
-    system = platform.system()
-    arch   = struct.calcsize('P') * 8
-
-    if system == 'Windows':
-        return "windows_x64" if arch == 64 else "windows_x32"
-    elif system == 'Darwin':
-        return "osx" if arch == 64 else "osx_x32"
-    elif system == 'Linux':
-        return "linux" if arch == 64 else "linux_x32"
-
-
-class lief_sdist(sdist):
-
-    user_options = sdist.user_options + [
-            ('dev', None, "Add a dev marker")
-            ]
-
-    def initialize_options(self):
-        sdist.initialize_options(self)
-        self.dev = 0
-
-    def run(self):
-        if self.dev:
-            suffix = '.dev-{:s}'.format("18d5b75")
-            self.distribution.metadata.version += suffix
-        sdist.run(self)
-
-    def make_distribution(self):
-        sdist.make_distribution(self)
-        base_dir = self.distribution.get_fullname()
-        base_name = os.path.join(self.dist_dir, base_dir)
-        for fmt in self.formats:
-            if fmt == 'gztar':
-                fmt = 'tar.gz'
-
-            if fmt == 'bztar':
-                fmt = 'tar.bz2'
-
-            if fmt == 'ztar':
-                fmt = 'tar.Z'
-
-            new_name = "py{name}-{version}.{ext}".format(
-                        name=self.distribution.get_name(),
-                        version=lief_version,
-                        ext=fmt)
-
-            if self.dev:
-                new_name = "py{name}-{version}.dev.{ext}".format(
-                        name=self.distribution.get_name(),
-                        version=lief_version,
-                        ext=fmt)
-            new_name = os.path.join(self.dist_dir, new_name)
-            shutil.move(base_name + "." + fmt, new_name)
-
-
-
-
-class lief_bdist_egg(bdist_egg):
-    def initialize_options(self):
-        bdist_egg.initialize_options(self)
-
-        if not in_source_package:
-            self.plat_name = get_lief_platform_name()
-
-
-    def run(self):
-        if in_source_package:
-            self._build_from_source_package()
-        else:
-            bdist_egg.run(self)
-
-    def _build_from_source_package(self):
-        python_version       = sys.version_info
-        python_major_version = python_version[0]
-        os_version           = get_lief_platform_name()
-
-        url_branch_fmt  = "https://github.com/lief-project/packages/raw/lief-{branch}-latest/lief-{version}-py{pyversion}-{platform}.{ext}"
-        url_release_fmt = "https://github.com/lief-project/LIEF/releases/download/{version}/lief-{version}-py{pyversion}-{platform}.{ext}"
-        url_userpath    = "~/lief-{version}-py{pyversion}-{platform}.{ext}"
-
-        url = ""
-        if is_branch:
-            url = url_branch_fmt.format(
-                    branch='master',
-                    platform=os_version,
-                    version=lief_version,
-                    pyversion="{}.{}".format(python_version[0], python_version[1]),
-                    ext="egg")
-        else:
-            url = url_release_fmt.format(
-                    platform=os_version,
-                    version=lief_version,
-                    pyversion="{}.{}".format(python_version[0], python_version[1]),
-                    ext="egg")
-
-        bdist_egg_log.info("Url: {}".format(url))
-        egg_data = None
-        network_error = None
-        try:
-            egg_data = urlopen(url).read()
-        except Exception as e:
-            network_error = e
-
-
-        if network_error is not None:
-            bdist_egg_log.warn(network_error)
-            url = url_userpath.format(
-                    platform=os_version,
-                    version=lief_version,
-                    pyversion="{}.{}".format(python_version[0], python_version[1]),
-                    ext="egg")
-            url = os.path.expanduser(url)
-            if os.path.isfile(url):
-                with open(url, 'rb') as f:
-                    egg_data = f.read()
-            else:
-                raise Exception("Unable to find {}".format(url))
-
-
-        egg_file = BytesIO(egg_data)
-
-        mkpath(os.path.dirname(self.egg_output))
-
-        bdist_egg_log.info("Output: {}".format(self.egg_output))
-        with open(self.egg_output, 'wb') as f:
-            f.write(egg_file.getvalue())
-
-        getattr(self.distribution, 'dist_files', []).append(
-        ('bdist_egg', "{}.{}".format(python_version[0], python_version[1]), self.egg_output))
-
-
-
-class lief_build_ext(build_ext):
-
-
-    def build_extension(self, ext):
-        self.target = self.get_ext_fullpath(ext.name)
-        target_dir  = os.path.dirname(self.target)
-
-        try:
-            os.makedirs(target_dir)
-        except:
-            pass
-
-        if in_source_package:
-            self._install_from_source_package()
-        else:
-            shutil.copyfile(libpylief[platform.system()], self.target)
-
-
-    def _install_from_source_package(self):
-        python_version       = sys.version_info
-        python_major_version = python_version[0]
-        os_version           = get_lief_platform_name()
-        target_extension     = os.path.splitext(self.target)[1]
-
-        url_branch_fmt  = "https://github.com/lief-project/packages/raw/lief-{branch}-latest/lief-{version}-py{pyversion}-{platform}.{ext}"
-        url_release_fmt = "https://github.com/lief-project/LIEF/releases/download/{version}/lief-{version}-py{pyversion}-{platform}.{ext}"
-        url_userpath    = "~/lief-{version}-py{pyversion}-{platform}.{ext}"
-
-        url = ""
-        if is_branch:
-            url = url_branch_fmt.format(
-                    branch='master',
-                    platform=os_version,
-                    version=lief_version,
-                    pyversion="{}.{}".format(python_version[0], python_version[1]),
-                    ext="egg")
-        else:
-            url = url_release_fmt.format(
-                    platform=os_version,
-                    version=lief_version,
-                    pyversion="{}.{}".format(python_version[0], python_version[1]),
-                    ext="egg")
-
-        bdist_egg_log.info("Url: {}".format(url))
-        egg_data = None
-        network_error = None
-        try:
-            egg_data = urlopen(url).read()
-        except Exception as e:
-            network_error = e
-
-        if network_error is not None:
-            bdist_egg_log.warn(network_error)
-            url = url_userpath.format(
-                    platform=os_version,
-                    version=lief_version,
-                    pyversion="{}.{}".format(python_version[0], python_version[1]),
-                    ext="egg")
-            url = os.path.expanduser(url)
-            if os.path.isfile(url):
-                with open(url, 'rb') as f:
-                    egg_data = f.read()
-            else:
-                raise Exception("Unable to find {}".format(url))
-
-
-
-
-
-        egg_file = BytesIO(egg_data)
-
-        egg_zip = zipfile.ZipFile(egg_file)
-        extension_member = [info for info in egg_zip.infolist() if info.filename.endswith(target_extension)][0]
-        extension_data = egg_zip.read(extension_member)
-        with open(self.target, 'wb') as f:
-            f.write(extension_data)
-
-setup(
-    version              = lief_version,
-    ext_modules          = [Extension('_pylief', [])],
-    cmdclass={
-        'build_ext': lief_build_ext,
-        'bdist_egg': lief_bdist_egg,
-        'sdist':     lief_sdist
-    },
-)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+MIN_SETUPTOOLS_VERSION = "31.0.0"
+import setuptools
+from distutils.version import LooseVersion
+assert (LooseVersion(setuptools.__version__) >= LooseVersion(MIN_SETUPTOOLS_VERSION)), "LIEF requires a setuptools version '{}' or higher (pip install setuptools --upgrade)".format(MIN_SETUPTOOLS_VERSION)
+
+from setuptools import setup
+from setuptools.command.build_ext import build_ext
+from distutils.dir_util import remove_tree, mkpath
+from setuptools.command.bdist_egg import bdist_egg
+from setuptools.command.bdist_egg import log as bdist_egg_log
+
+from setuptools.command.sdist import sdist
+from setuptools.command.sdist import log as sdist_log
+
+from setuptools.extension import Extension
+
+import re
+import os
+import platform
+import shutil
+import sys
+import struct
+import zipfile
+
+try:
+    from urllib.request import urlopen, Request
+except:
+    from urllib2 import urlopen, Request
+
+
+try:
+    from io import BytesIO
+except:
+    try:
+        from cStringIO import StringIO as BytesIO
+    except:
+        from StringIO import StringIO as BytesIO
+
+package_dir       = os.path.dirname(os.path.realpath(__file__))
+pkg_info          = os.path.join(package_dir, "PKG-INFO")
+in_source_package = os.path.isfile(pkg_info) # (e.g. pip)
+
+is_branch = False
+
+libpylief = {
+        'Windows': "_pylief.pyd",
+        'Darwin': "_pylief.so",
+        'Linux': "_pylief.so",
+        'FreeBSD': "_pylief.so",
+        }
+version_re = r"Version:\s+(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)\.?(.*)"
+if in_source_package:
+    with open(pkg_info, "r") as f:
+        major, minor, patch, branch = re.findall(version_re, f.read(), re.MULTILINE)[0]
+        lief_version = "{:d}.{:d}.{:d}".format(int(major), int(minor), int(patch))
+        is_branch = len(branch.strip()) > 0
+else:
+    lief_version = "0.9.0"
+
+package_description = open(os.path.join(package_dir, "README")).read()
+
+
+def get_lief_platform_name():
+    system = platform.system()
+    arch   = struct.calcsize('P') * 8
+
+    if system == 'Windows':
+        return "windows_x64" if arch == 64 else "windows_x32"
+    elif system == 'Darwin':
+        return "osx" if arch == 64 else "osx_x32"
+    elif system == 'Linux':
+        return "linux" if arch == 64 else "linux_x32"
+    elif system == 'FreeBSD':
+        return "freebsd" if arch == 64 else "freebsd_x32"
+
+
+
+class lief_sdist(sdist):
+
+    user_options = sdist.user_options + [
+            ('dev', None, "Add a dev marker")
+            ]
+
+    def initialize_options(self):
+        sdist.initialize_options(self)
+        self.dev = 0
+
+    def run(self):
+        if self.dev:
+            suffix = '.dev-{:s}'.format("a448c5e")
+            self.distribution.metadata.version += suffix
+        sdist.run(self)
+
+    def make_distribution(self):
+        sdist.make_distribution(self)
+        base_dir = self.distribution.get_fullname()
+        base_name = os.path.join(self.dist_dir, base_dir)
+        for fmt in self.formats:
+            if fmt == 'gztar':
+                fmt = 'tar.gz'
+
+            if fmt == 'bztar':
+                fmt = 'tar.bz2'
+
+            if fmt == 'ztar':
+                fmt = 'tar.Z'
+
+            new_name = "py{name}-{version}.{ext}".format(
+                        name=self.distribution.get_name(),
+                        version=lief_version,
+                        ext=fmt)
+
+            if self.dev:
+                new_name = "py{name}-{version}.dev.{ext}".format(
+                        name=self.distribution.get_name(),
+                        version=lief_version,
+                        ext=fmt)
+            new_name = os.path.join(self.dist_dir, new_name)
+            shutil.move(base_name + "." + fmt, new_name)
+
+
+
+
+class lief_bdist_egg(bdist_egg):
+    def initialize_options(self):
+        bdist_egg.initialize_options(self)
+
+        if not in_source_package:
+            self.plat_name = get_lief_platform_name()
+
+
+    def run(self):
+        if in_source_package:
+            self._build_from_source_package()
+        else:
+            bdist_egg.run(self)
+
+    def _build_from_source_package(self):
+        python_version       = sys.version_info
+        python_major_version = python_version[0]
+        os_version           = get_lief_platform_name()
+
+        url_branch_fmt  = "https://github.com/lief-project/packages/raw/lief-{branch}-latest/lief-{version}-py{pyversion}-{platform}.{ext}"
+        url_release_fmt = "https://github.com/lief-project/LIEF/releases/download/{version}/lief-{version}-py{pyversion}-{platform}.{ext}"
+        url_userpath    = "~/lief-{version}-py{pyversion}-{platform}.{ext}"
+
+        url = ""
+        if is_branch:
+            url = url_branch_fmt.format(
+                    branch='master',
+                    platform=os_version,
+                    version=lief_version,
+                    pyversion="{}.{}".format(python_version[0], python_version[1]),
+                    ext="egg")
+        else:
+            url = url_release_fmt.format(
+                    platform=os_version,
+                    version=lief_version,
+                    pyversion="{}.{}".format(python_version[0], python_version[1]),
+                    ext="egg")
+
+        bdist_egg_log.info("Url: {}".format(url))
+        egg_data = None
+        network_error = None
+        try:
+            egg_data = urlopen(url).read()
+        except Exception as e:
+            network_error = e
+
+
+        if network_error is not None:
+            bdist_egg_log.warn(network_error)
+            url = url_userpath.format(
+                    platform=os_version,
+                    version=lief_version,
+                    pyversion="{}.{}".format(python_version[0], python_version[1]),
+                    ext="egg")
+            url = os.path.expanduser(url)
+            if os.path.isfile(url):
+                with open(url, 'rb') as f:
+                    egg_data = f.read()
+            else:
+                raise Exception("Unable to find {}".format(url))
+
+
+        egg_file = BytesIO(egg_data)
+
+        mkpath(os.path.dirname(self.egg_output))
+
+        bdist_egg_log.info("Output: {}".format(self.egg_output))
+        with open(self.egg_output, 'wb') as f:
+            f.write(egg_file.getvalue())
+
+        getattr(self.distribution, 'dist_files', []).append(
+        ('bdist_egg', "{}.{}".format(python_version[0], python_version[1]), self.egg_output))
+
+
+
+class lief_build_ext(build_ext):
+
+
+    def build_extension(self, ext):
+        self.target = self.get_ext_fullpath(ext.name)
+        target_dir  = os.path.dirname(self.target)
+
+        try:
+            os.makedirs(target_dir)
+        except:
+            pass
+
+        if in_source_package:
+            self._install_from_source_package()
+        else:
+            shutil.copyfile(libpylief[platform.system()], self.target)
+
+
+    def _install_from_source_package(self):
+        python_version       = sys.version_info
+        python_major_version = python_version[0]
+        os_version           = get_lief_platform_name()
+        target_extension     = os.path.splitext(self.target)[1]
+
+        url_branch_fmt  = "https://github.com/lief-project/packages/raw/lief-{branch}-latest/lief-{version}-py{pyversion}-{platform}.{ext}"
+        url_release_fmt = "https://github.com/lief-project/LIEF/releases/download/{version}/lief-{version}-py{pyversion}-{platform}.{ext}"
+        url_userpath    = "~/lief-{version}-py{pyversion}-{platform}.{ext}"
+
+        url = ""
+        if is_branch:
+            url = url_branch_fmt.format(
+                    branch='master',
+                    platform=os_version,
+                    version=lief_version,
+                    pyversion="{}.{}".format(python_version[0], python_version[1]),
+                    ext="egg")
+        else:
+            url = url_release_fmt.format(
+                    platform=os_version,
+                    version=lief_version,
+                    pyversion="{}.{}".format(python_version[0], python_version[1]),
+                    ext="egg")
+
+        bdist_egg_log.info("Url: {}".format(url))
+        egg_data = None
+        network_error = None
+        try:
+            egg_data = urlopen(url).read()
+        except Exception as e:
+            network_error = e
+
+        if network_error is not None:
+            bdist_egg_log.warn(network_error)
+            url = url_userpath.format(
+                    platform=os_version,
+                    version=lief_version,
+                    pyversion="{}.{}".format(python_version[0], python_version[1]),
+                    ext="egg")
+            url = os.path.expanduser(url)
+            if os.path.isfile(url):
+                with open(url, 'rb') as f:
+                    egg_data = f.read()
+            else:
+                raise Exception("Unable to find {}".format(url))
+
+
+
+
+
+        egg_file = BytesIO(egg_data)
+
+        egg_zip = zipfile.ZipFile(egg_file)
+        extension_member = [info for info in egg_zip.infolist() if info.filename.endswith(target_extension)][0]
+        extension_data = egg_zip.read(extension_member)
+        with open(self.target, 'wb') as f:
+            f.write(extension_data)
+
+setup(
+    version              = lief_version,
+    ext_modules          = [Extension('_pylief', [])],
+    cmdclass={
+        'build_ext': lief_build_ext,
+        'bdist_egg': lief_bdist_egg,
+        'sdist':     lief_sdist
+    },
+)
```

