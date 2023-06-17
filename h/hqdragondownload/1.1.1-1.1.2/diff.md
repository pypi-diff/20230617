# Comparing `tmp/hqdragondownload-1.1.1.tar.gz` & `tmp/hqdragondownload-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hqdragondownload-1.1.1.tar", last modified: Mon Apr 17 20:05:23 2023, max compression
+gzip compressed data, was "hqdragondownload-1.1.2.tar", last modified: Sat Jun 17 20:51:01 2023, max compression
```

## Comparing `hqdragondownload-1.1.1.tar` & `hqdragondownload-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 20:05:23.161341 hqdragondownload-1.1.1/
--rw-rw-rw-   0        0        0     1114 2022-04-21 03:01:14.000000 hqdragondownload-1.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      786 2023-04-17 20:05:23.162338 hqdragondownload-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      899 2022-04-21 03:01:14.000000 hqdragondownload-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 20:05:23.124356 hqdragondownload-1.1.1/hqdragon/
--rw-rw-rw-   0        0        0       97 2023-04-17 20:05:03.000000 hqdragondownload-1.1.1/hqdragon/__init__.py
--rw-rw-rw-   0        0        0     6502 2023-04-16 09:56:44.000000 hqdragondownload-1.1.1/hqdragon/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 20:05:23.159334 hqdragondownload-1.1.1/hqdragondownload.egg-info/
--rw-rw-rw-   0        0        0      786 2023-04-17 20:05:21.000000 hqdragondownload-1.1.1/hqdragondownload.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-04-17 20:05:21.000000 hqdragondownload-1.1.1/hqdragondownload.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 20:05:21.000000 hqdragondownload-1.1.1/hqdragondownload.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-17 20:05:21.000000 hqdragondownload-1.1.1/hqdragondownload.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 20:05:21.000000 hqdragondownload-1.1.1/hqdragondownload.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      114 2023-04-17 20:05:23.170345 hqdragondownload-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1015 2023-04-17 20:04:48.000000 hqdragondownload-1.1.1/setup.py
+drwxrwxr-x   0 mrpowerup  (1000) mrpowerup  (1000)        0 2023-06-17 20:51:01.164342 hqdragondownload-1.1.2/
+-rw-rw-r--   0 mrpowerup  (1000) mrpowerup  (1000)     1094 2023-03-23 18:57:41.000000 hqdragondownload-1.1.2/LICENSE.txt
+-rw-rw-r--   0 mrpowerup  (1000) mrpowerup  (1000)      826 2023-06-17 20:51:01.164342 hqdragondownload-1.1.2/PKG-INFO
+-rw-rw-r--   0 mrpowerup  (1000) mrpowerup  (1000)      983 2023-06-17 20:22:05.000000 hqdragondownload-1.1.2/README.md
+drwxrwxr-x   0 mrpowerup  (1000) mrpowerup  (1000)        0 2023-06-17 20:51:01.160342 hqdragondownload-1.1.2/hqdragon/
+-rw-rw-r--   0 mrpowerup  (1000) mrpowerup  (1000)       95 2023-06-17 20:29:04.000000 hqdragondownload-1.1.2/hqdragon/__init__.py
+-rw-rw-r--   0 mrpowerup  (1000) mrpowerup  (1000)     8239 2023-06-17 20:37:24.000000 hqdragondownload-1.1.2/hqdragon/__main__.py
+drwxrwxr-x   0 mrpowerup  (1000) mrpowerup  (1000)        0 2023-06-17 20:51:01.164342 hqdragondownload-1.1.2/hqdragondownload.egg-info/
+-rw-rw-r--   0 mrpowerup  (1000) mrpowerup  (1000)      826 2023-06-17 20:51:01.000000 hqdragondownload-1.1.2/hqdragondownload.egg-info/PKG-INFO
+-rw-rw-r--   0 mrpowerup  (1000) mrpowerup  (1000)      281 2023-06-17 20:51:01.000000 hqdragondownload-1.1.2/hqdragondownload.egg-info/SOURCES.txt
+-rw-rw-r--   0 mrpowerup  (1000) mrpowerup  (1000)        1 2023-06-17 20:51:01.000000 hqdragondownload-1.1.2/hqdragondownload.egg-info/dependency_links.txt
+-rw-rw-r--   0 mrpowerup  (1000) mrpowerup  (1000)       41 2023-06-17 20:51:01.000000 hqdragondownload-1.1.2/hqdragondownload.egg-info/requires.txt
+-rw-rw-r--   0 mrpowerup  (1000) mrpowerup  (1000)        9 2023-06-17 20:51:01.000000 hqdragondownload-1.1.2/hqdragondownload.egg-info/top_level.txt
+-rw-rw-r--   0 mrpowerup  (1000) mrpowerup  (1000)      106 2023-06-17 20:51:01.164342 hqdragondownload-1.1.2/setup.cfg
+-rw-rw-r--   0 mrpowerup  (1000) mrpowerup  (1000)     1051 2023-06-17 20:38:55.000000 hqdragondownload-1.1.2/setup.py
```

### Comparing `hqdragondownload-1.1.1/LICENSE.txt` & `hqdragondownload-1.1.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2018 MrPowerUp - www.github.com/MrPowerUp82
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+MIT License
+
+Copyright (c) 2018 MrPowerUp - www.github.com/MrPowerUp82
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
```

### Comparing `hqdragondownload-1.1.1/README.md` & `hqdragondownload-1.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,37 @@
-# HQDragonDownload
-  CLI para baixar hq's no https://hqdragon.com/ (em PDF)
-## Exemplos:
-  ```console
-  python .\main.py --search "superman" --option 1 --no-pdf True
-  ```
-  ```console
-  python .\main.py --search "superman" --option 1 --cap 2 --output "superman"
-  ```
-  ```console
-  python .\main.py --search "superman" --option 1 --cap 1,2 --no-pdf True
-  ```
-  ```console
-  python .\main.py --url "https://hqdragon.com/hq/nju4mq/6581-a-morte-do-superman" --cap 2 --output "superman"
-  ```
-  ```console
-  python .\main.py -h
-  ```
-
-## Argumentos
-| Argumento | Descrição |
-| - | - |
-| -h, --help | Mostra a mensagem de ajuda. | 
-| --url | Define a URL da HQ. |
-| --search | Realiza pesquisa. | 
-| --output | Nome de saida do pdf. (no directory) |
-| --option | Opção de escolha da pesquisa. |
-| --no-pdf | Salva apenas as imagens.  |
+# HQDragonDownload
+  CLI para baixar hq's no https://hqdragon.com/ (em PDF)
+## Exemplos:
+  ```console
+  python .\main.py --search "superman" --option 1 --no-pdf True
+  ```
+  ```console
+  python .\main.py --search "superman" --option 1 --cap 2 --output "superman"
+  ```
+  ```console
+  python .\main.py --search "superman" --option 1 --cap 1,2 --no-pdf True
+  ```
+  ```console
+  python .\main.py --url "https://hqdragon.com/hq/nju4mq/6581-a-morte-do-superman" --cap 2 --output "superman"
+  ```
+  ```console
+  python .\main.py -h
+  ```
+
+## Lib:
+  ```console
+  python3 -m pip install hqdragondownload 
+  ```
+  ```console
+  python3 -m hqdragon
+  ```
+
+## Argumentos
+| Argumento | Descrição |
+| - | - |
+| -h, --help | Mostra a mensagem de ajuda. | 
+| --url | Define a URL da HQ. |
+| --search | Realiza pesquisa. | 
+| --output | Nome de saida do pdf. (no directory) |
+| --option | Opção de escolha da pesquisa. |
+| --no-pdf | Salva apenas as imagens.  |
 | --cap | Define os capitulos. ||
```

