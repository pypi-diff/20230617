# Comparing `tmp/naludaq_rs-0.1.8-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/naludaq_rs-0.1.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 9101952 bytes, number of entries: 6
--rw-r--r--  4.6 unx     2899 b- defN 23-Apr-28 20:51 naludaq_rs-0.1.8.dist-info/METADATA
--rw-r--r--  4.6 unx      136 b- defN 23-Apr-28 20:51 naludaq_rs-0.1.8.dist-info/WHEEL
--rw-r--r--  4.6 unx     7652 b- defN 23-Apr-28 20:51 naludaq_rs-0.1.8.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      123 b- defN 23-Apr-28 20:51 naludaq_rs/__init__.py
--rwxr-xr-x  4.6 unx 28000432 b- defN 23-Apr-28 20:51 naludaq_rs/naludaq_rs.pypy39-pp73-x86_64-linux-gnu.so
--rw-r--r--  4.6 unx      513 b- defN 23-Apr-28 20:51 naludaq_rs-0.1.8.dist-info/RECORD
-6 files, 28011755 bytes uncompressed, 9101028 bytes compressed:  67.5%
+Zip file size: 6015966 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     2975 b- defN 23-Jun-17 02:01 naludaq_rs-0.1.9.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jun-17 02:01 naludaq_rs-0.1.9.dist-info/WHEEL
+-rw-r--r--  4.6 unx     7817 b- defN 23-Jun-17 02:01 naludaq_rs-0.1.9.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      123 b- defN 23-Jun-17 02:01 naludaq_rs/__init__.py
+-rwxr-xr-x  4.6 unx 18182656 b- defN 23-Jun-17 02:01 naludaq_rs/naludaq_rs.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      499 b- defN 23-Jun-17 02:01 naludaq_rs-0.1.9.dist-info/RECORD
+6 files, 18194164 bytes uncompressed, 6015068 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: naludaq_rs-0.1.8.dist-info/METADATA
+Filename: naludaq_rs-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: naludaq_rs-0.1.8.dist-info/WHEEL
+Filename: naludaq_rs-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: naludaq_rs-0.1.8.dist-info/license_files/LICENSE
+Filename: naludaq_rs-0.1.9.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: naludaq_rs/__init__.py
 Comment: 
 
-Filename: naludaq_rs/naludaq_rs.pypy39-pp73-x86_64-linux-gnu.so
+Filename: naludaq_rs/naludaq_rs.cp39-win_amd64.pyd
 Comment: 
 
-Filename: naludaq_rs-0.1.8.dist-info/RECORD
+Filename: naludaq_rs-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `naludaq_rs-0.1.8.dist-info/METADATA` & `naludaq_rs-0.1.9.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,105 +1,105 @@
 Metadata-Version: 2.1
 Name: naludaq_rs
-Version: 0.1.8
+Version: 0.1.9
 License-File: LICENSE
 Summary: Rust backend for NaluDAQ
 Author: Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Marcus Luck <marcus@naluscientific.com>
 Author-email: Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Marcus Luck <marcus@naluscientific.com>
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
-# NaluDAQ_rs
-
-Rust backend for NaluDaq.
-
-
-## Setup
-
-Make sure the [Rust toolchain](https://rustup.rs/) is installed.
-
-Clone the repository to a suitable location:
-```sh
-$ git clone http://gitlab.naluscientific.com/nalusoft/prototypes/naludaq_rs.git
-```
-
-Done!
-
-## Building the backend for python
-
-```sh
-pip install maturin
-maturin build
-```
-
-## Building the Backend
-
-The backend is easy to build:
-
-```sh
-$ cd naludaq_rs
-$ cargo build --release
-```
-
-Developers may ommit the `--release` flag for unoptimized builds.
-
-
-### Building for RPI4
-Building using docker:
-
-```sh
-docker build . -t cc/rpi4
-```
-to make the container, the build the app with:
-```sh
-docker run --rm -v ${pwd}:/app cc/rpi4
-```
-
-## Running the Backend
-To run the backend, run the following command:
-
-```sh
-$ cargo run  --release -- [<ROOT>] [--addr <ADDR>] [-d | --debug]  [--api]
-```
-
-Where the arguments are as follows:
-- `<ROOT>` is the root directory to run the server in. By default, it is the current working directory of the terminal it was run from.
-- `--addr <ADDR>` is the address to bind the server to in the format `IP:PORT`. If unspecified, the server is bound to an open port on the loopback address.
-- `-d | --debug` shows additional debug messages.
-- `--api` will open the Swagger UI in the system browser.
-
-## Documentation
-The documentation can be built using the following command:
-```sh
-$ cargo doc --document-private-items --no-deps
-```
-
-
-## The API
-NaluDAQ_rs is controlled through its [REST API](https://www.redhat.com/en/topics/api/what-is-a-rest-api) over
-[HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview). This allows it to be controlled from any
-machine connected to a network.
-
-The backend can be controlled on the fly via Swagger. Use the `--api` flag when starting the backend to display the Swagger UI.
-
-Alternatively, the (non-interactive) Swagger UI may be viewed without the backend by running the
-following command:
-
-```sh
-$ cargo run --bin api -- [--output OUTPUT_FILE]
-```
-
-If the `--output` argument is provided, the OpenAPI JSON data describing
-the API is written to the file and the program will immediately exit.
-
-
-## Developers
-
-### Profiling
-Use the build profile called `release-with-debug for building release mode with debug symbols.
-
-```sh
-$ cargo build --profile release-with-debug
-```
-
-On Windows machines with Intel processors you can use [Intel VTune](https://www.intel.com/content/www/us/en/developer/tools/oneapi/vtune-profiler.html#gs.q7qmtk)
-to profile the backend.
+# NaluDAQ_rs
+
+Rust backend for NaluDaq.
+
+
+## Setup
+
+Make sure the [Rust toolchain](https://rustup.rs/) is installed.
+
+Clone the repository to a suitable location:
+```sh
+$ git clone https://github.com/NaluScientific/naludaq_rs.git
+```
+
+Done!
+
+## Building the backend for python
+
+```sh
+pip install maturin
+maturin build
+```
+
+## Building the Backend
+
+The backend is easy to build:
+
+```sh
+$ cd naludaq_rs
+$ cargo build --release
+```
+
+Developers may ommit the `--release` flag for unoptimized builds.
+
+
+### Building for RPI4
+Building using docker:
+
+```sh
+docker build . -t cc/rpi4
+```
+to make the container, the build the app with:
+```sh
+docker run --rm -v ${pwd}:/app cc/rpi4
+```
+
+## Running the Backend
+To run the backend, run the following command:
+
+```sh
+$ cargo run  --release -- [<ROOT>] [--addr <ADDR>] [-d | --debug]  [--api]
+```
+
+Where the arguments are as follows:
+- `<ROOT>` is the root directory to run the server in. By default, it is the current working directory of the terminal it was run from.
+- `--addr <ADDR>` is the address to bind the server to in the format `IP:PORT`. If unspecified, the server is bound to an open port on the loopback address.
+- `-d | --debug` shows additional debug messages.
+- `--api` will open the Swagger UI in the system browser.
+
+## Documentation
+The documentation can be built using the following command:
+```sh
+$ cargo doc --document-private-items --no-deps
+```
+
+
+## The API
+NaluDAQ_rs is controlled through its [REST API](https://www.redhat.com/en/topics/api/what-is-a-rest-api) over
+[HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview). This allows it to be controlled from any
+machine connected to a network.
+
+The backend can be controlled on the fly via Swagger. Use the `--api` flag when starting the backend to display the Swagger UI.
+
+Alternatively, the (non-interactive) Swagger UI may be viewed without the backend by running the
+following command:
+
+```sh
+$ cargo run --bin api -- [--output OUTPUT_FILE]
+```
+
+If the `--output` argument is provided, the OpenAPI JSON data describing
+the API is written to the file and the program will immediately exit.
+
+
+## Developers
+
+### Profiling
+Use the build profile called `release-with-debug for building release mode with debug symbols.
+
+```sh
+$ cargo build --profile release-with-debug
+```
+
+On Windows machines with Intel processors you can use [Intel VTune](https://www.intel.com/content/www/us/en/developer/tools/oneapi/vtune-profiler.html#gs.q7qmtk)
+to profile the backend.
```

## Comparing `naludaq_rs-0.1.8.dist-info/license_files/LICENSE` & `naludaq_rs-0.1.9.dist-info/license_files/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-                   GNU LESSER GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-
-  This version of the GNU Lesser General Public License incorporates
-the terms and conditions of version 3 of the GNU General Public
-License, supplemented by the additional permissions listed below.
-
-  0. Additional Definitions.
-
-  As used herein, "this License" refers to version 3 of the GNU Lesser
-General Public License, and the "GNU GPL" refers to version 3 of the GNU
-General Public License.
-
-  "The Library" refers to a covered work governed by this License,
-other than an Application or a Combined Work as defined below.
-
-  An "Application" is any work that makes use of an interface provided
-by the Library, but which is not otherwise based on the Library.
-Defining a subclass of a class defined by the Library is deemed a mode
-of using an interface provided by the Library.
-
-  A "Combined Work" is a work produced by combining or linking an
-Application with the Library.  The particular version of the Library
-with which the Combined Work was made is also called the "Linked
-Version".
-
-  The "Minimal Corresponding Source" for a Combined Work means the
-Corresponding Source for the Combined Work, excluding any source code
-for portions of the Combined Work that, considered in isolation, are
-based on the Application, and not on the Linked Version.
-
-  The "Corresponding Application Code" for a Combined Work means the
-object code and/or source code for the Application, including any data
-and utility programs needed for reproducing the Combined Work from the
-Application, but excluding the System Libraries of the Combined Work.
-
-  1. Exception to Section 3 of the GNU GPL.
-
-  You may convey a covered work under sections 3 and 4 of this License
-without being bound by section 3 of the GNU GPL.
-
-  2. Conveying Modified Versions.
-
-  If you modify a copy of the Library, and, in your modifications, a
-facility refers to a function or data to be supplied by an Application
-that uses the facility (other than as an argument passed when the
-facility is invoked), then you may convey a copy of the modified
-version:
-
-   a) under this License, provided that you make a good faith effort to
-   ensure that, in the event an Application does not supply the
-   function or data, the facility still operates, and performs
-   whatever part of its purpose remains meaningful, or
-
-   b) under the GNU GPL, with none of the additional permissions of
-   this License applicable to that copy.
-
-  3. Object Code Incorporating Material from Library Header Files.
-
-  The object code form of an Application may incorporate material from
-a header file that is part of the Library.  You may convey such object
-code under terms of your choice, provided that, if the incorporated
-material is not limited to numerical parameters, data structure
-layouts and accessors, or small macros, inline functions and templates
-(ten or fewer lines in length), you do both of the following:
-
-   a) Give prominent notice with each copy of the object code that the
-   Library is used in it and that the Library and its use are
-   covered by this License.
-
-   b) Accompany the object code with a copy of the GNU GPL and this license
-   document.
-
-  4. Combined Works.
-
-  You may convey a Combined Work under terms of your choice that,
-taken together, effectively do not restrict modification of the
-portions of the Library contained in the Combined Work and reverse
-engineering for debugging such modifications, if you also do each of
-the following:
-
-   a) Give prominent notice with each copy of the Combined Work that
-   the Library is used in it and that the Library and its use are
-   covered by this License.
-
-   b) Accompany the Combined Work with a copy of the GNU GPL and this license
-   document.
-
-   c) For a Combined Work that displays copyright notices during
-   execution, include the copyright notice for the Library among
-   these notices, as well as a reference directing the user to the
-   copies of the GNU GPL and this license document.
-
-   d) Do one of the following:
-
-       0) Convey the Minimal Corresponding Source under the terms of this
-       License, and the Corresponding Application Code in a form
-       suitable for, and under terms that permit, the user to
-       recombine or relink the Application with a modified version of
-       the Linked Version to produce a modified Combined Work, in the
-       manner specified by section 6 of the GNU GPL for conveying
-       Corresponding Source.
-
-       1) Use a suitable shared library mechanism for linking with the
-       Library.  A suitable mechanism is one that (a) uses at run time
-       a copy of the Library already present on the user's computer
-       system, and (b) will operate properly with a modified version
-       of the Library that is interface-compatible with the Linked
-       Version.
-
-   e) Provide Installation Information, but only if you would otherwise
-   be required to provide such information under section 6 of the
-   GNU GPL, and only to the extent that such information is
-   necessary to install and execute a modified version of the
-   Combined Work produced by recombining or relinking the
-   Application with a modified version of the Linked Version. (If
-   you use option 4d0, the Installation Information must accompany
-   the Minimal Corresponding Source and Corresponding Application
-   Code. If you use option 4d1, you must provide the Installation
-   Information in the manner specified by section 6 of the GNU GPL
-   for conveying Corresponding Source.)
-
-  5. Combined Libraries.
-
-  You may place library facilities that are a work based on the
-Library side by side in a single library together with other library
-facilities that are not Applications and are not covered by this
-License, and convey such a combined library under terms of your
-choice, if you do both of the following:
-
-   a) Accompany the combined library with a copy of the same work based
-   on the Library, uncombined with any other library facilities,
-   conveyed under the terms of this License.
-
-   b) Give prominent notice with the combined library that part of it
-   is a work based on the Library, and explaining where to find the
-   accompanying uncombined form of the same work.
-
-  6. Revised Versions of the GNU Lesser General Public License.
-
-  The Free Software Foundation may publish revised and/or new versions
-of the GNU Lesser General Public License from time to time. Such new
-versions will be similar in spirit to the present version, but may
-differ in detail to address new problems or concerns.
-
-  Each version is given a distinguishing version number. If the
-Library as you received it specifies that a certain numbered version
-of the GNU Lesser General Public License "or any later version"
-applies to it, you have the option of following the terms and
-conditions either of that published version or of any later version
-published by the Free Software Foundation. If the Library as you
-received it does not specify a version number of the GNU Lesser
-General Public License, you may choose any version of the GNU Lesser
-General Public License ever published by the Free Software Foundation.
-
-  If the Library as you received it specifies that a proxy can decide
-whether future versions of the GNU Lesser General Public License shall
-apply, that proxy's public statement of acceptance of any version is
-permanent authorization for you to choose that version for the
-Library.
+                   GNU LESSER GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+
+  This version of the GNU Lesser General Public License incorporates
+the terms and conditions of version 3 of the GNU General Public
+License, supplemented by the additional permissions listed below.
+
+  0. Additional Definitions.
+
+  As used herein, "this License" refers to version 3 of the GNU Lesser
+General Public License, and the "GNU GPL" refers to version 3 of the GNU
+General Public License.
+
+  "The Library" refers to a covered work governed by this License,
+other than an Application or a Combined Work as defined below.
+
+  An "Application" is any work that makes use of an interface provided
+by the Library, but which is not otherwise based on the Library.
+Defining a subclass of a class defined by the Library is deemed a mode
+of using an interface provided by the Library.
+
+  A "Combined Work" is a work produced by combining or linking an
+Application with the Library.  The particular version of the Library
+with which the Combined Work was made is also called the "Linked
+Version".
+
+  The "Minimal Corresponding Source" for a Combined Work means the
+Corresponding Source for the Combined Work, excluding any source code
+for portions of the Combined Work that, considered in isolation, are
+based on the Application, and not on the Linked Version.
+
+  The "Corresponding Application Code" for a Combined Work means the
+object code and/or source code for the Application, including any data
+and utility programs needed for reproducing the Combined Work from the
+Application, but excluding the System Libraries of the Combined Work.
+
+  1. Exception to Section 3 of the GNU GPL.
+
+  You may convey a covered work under sections 3 and 4 of this License
+without being bound by section 3 of the GNU GPL.
+
+  2. Conveying Modified Versions.
+
+  If you modify a copy of the Library, and, in your modifications, a
+facility refers to a function or data to be supplied by an Application
+that uses the facility (other than as an argument passed when the
+facility is invoked), then you may convey a copy of the modified
+version:
+
+   a) under this License, provided that you make a good faith effort to
+   ensure that, in the event an Application does not supply the
+   function or data, the facility still operates, and performs
+   whatever part of its purpose remains meaningful, or
+
+   b) under the GNU GPL, with none of the additional permissions of
+   this License applicable to that copy.
+
+  3. Object Code Incorporating Material from Library Header Files.
+
+  The object code form of an Application may incorporate material from
+a header file that is part of the Library.  You may convey such object
+code under terms of your choice, provided that, if the incorporated
+material is not limited to numerical parameters, data structure
+layouts and accessors, or small macros, inline functions and templates
+(ten or fewer lines in length), you do both of the following:
+
+   a) Give prominent notice with each copy of the object code that the
+   Library is used in it and that the Library and its use are
+   covered by this License.
+
+   b) Accompany the object code with a copy of the GNU GPL and this license
+   document.
+
+  4. Combined Works.
+
+  You may convey a Combined Work under terms of your choice that,
+taken together, effectively do not restrict modification of the
+portions of the Library contained in the Combined Work and reverse
+engineering for debugging such modifications, if you also do each of
+the following:
+
+   a) Give prominent notice with each copy of the Combined Work that
+   the Library is used in it and that the Library and its use are
+   covered by this License.
+
+   b) Accompany the Combined Work with a copy of the GNU GPL and this license
+   document.
+
+   c) For a Combined Work that displays copyright notices during
+   execution, include the copyright notice for the Library among
+   these notices, as well as a reference directing the user to the
+   copies of the GNU GPL and this license document.
+
+   d) Do one of the following:
+
+       0) Convey the Minimal Corresponding Source under the terms of this
+       License, and the Corresponding Application Code in a form
+       suitable for, and under terms that permit, the user to
+       recombine or relink the Application with a modified version of
+       the Linked Version to produce a modified Combined Work, in the
+       manner specified by section 6 of the GNU GPL for conveying
+       Corresponding Source.
+
+       1) Use a suitable shared library mechanism for linking with the
+       Library.  A suitable mechanism is one that (a) uses at run time
+       a copy of the Library already present on the user's computer
+       system, and (b) will operate properly with a modified version
+       of the Library that is interface-compatible with the Linked
+       Version.
+
+   e) Provide Installation Information, but only if you would otherwise
+   be required to provide such information under section 6 of the
+   GNU GPL, and only to the extent that such information is
+   necessary to install and execute a modified version of the
+   Combined Work produced by recombining or relinking the
+   Application with a modified version of the Linked Version. (If
+   you use option 4d0, the Installation Information must accompany
+   the Minimal Corresponding Source and Corresponding Application
+   Code. If you use option 4d1, you must provide the Installation
+   Information in the manner specified by section 6 of the GNU GPL
+   for conveying Corresponding Source.)
+
+  5. Combined Libraries.
+
+  You may place library facilities that are a work based on the
+Library side by side in a single library together with other library
+facilities that are not Applications and are not covered by this
+License, and convey such a combined library under terms of your
+choice, if you do both of the following:
+
+   a) Accompany the combined library with a copy of the same work based
+   on the Library, uncombined with any other library facilities,
+   conveyed under the terms of this License.
+
+   b) Give prominent notice with the combined library that part of it
+   is a work based on the Library, and explaining where to find the
+   accompanying uncombined form of the same work.
+
+  6. Revised Versions of the GNU Lesser General Public License.
+
+  The Free Software Foundation may publish revised and/or new versions
+of the GNU Lesser General Public License from time to time. Such new
+versions will be similar in spirit to the present version, but may
+differ in detail to address new problems or concerns.
+
+  Each version is given a distinguishing version number. If the
+Library as you received it specifies that a certain numbered version
+of the GNU Lesser General Public License "or any later version"
+applies to it, you have the option of following the terms and
+conditions either of that published version or of any later version
+published by the Free Software Foundation. If the Library as you
+received it does not specify a version number of the GNU Lesser
+General Public License, you may choose any version of the GNU Lesser
+General Public License ever published by the Free Software Foundation.
+
+  If the Library as you received it specifies that a proxy can decide
+whether future versions of the GNU Lesser General Public License shall
+apply, that proxy's public statement of acceptance of any version is
+permanent authorization for you to choose that version for the
+Library.
```

