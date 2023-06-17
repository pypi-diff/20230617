# Comparing `tmp/django-passkeys-1.2.2.tar.gz` & `tmp/django-passkeys-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-passkeys-1.2.2.tar", last modified: Sat Jun 17 16:32:04 2023, max compression
+gzip compressed data, was "dist/django-passkeys-1.2.3.tar", last modified: Sat Jun 17 16:35:08 2023, max compression
```

## Comparing `django-passkeys-1.2.2.tar` & `django-passkeys-1.2.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1075 2022-10-28 10:01:16.000000 django-passkeys-1.2.2/LICENSE
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      192 2023-06-17 16:31:58.000000 django-passkeys-1.2.2/MANIFEST.in
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     7165 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5788 2023-06-17 12:31:09.000000 django-passkeys-1.2.2/README.md
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/django_passkeys.egg-info/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     7165 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/django_passkeys.egg-info/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      913 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/django_passkeys.egg-info/SOURCES.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/django_passkeys.egg-info/dependency_links.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2022-10-28 13:54:59.000000 django-passkeys-1.2.2/django_passkeys.egg-info/not-zip-safe
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       47 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/django_passkeys.egg-info/requires.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       17 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/django_passkeys.egg-info/top_level.txt
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/env/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/env/bin/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1199 2022-10-28 10:01:55.000000 django-passkeys-1.2.2/env/bin/activate_this.py
--rwxrwxr-x   0 mohamed   (1000) mohamed   (1000)      153 2022-10-28 10:02:36.000000 django-passkeys-1.2.2/env/bin/django-admin.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/passkeys/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5823 2023-06-17 15:37:35.000000 django-passkeys-1.2.2/passkeys/FIDO2.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       65 2022-10-28 11:16:36.000000 django-passkeys-1.2.2/passkeys/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      790 2023-06-17 11:35:33.000000 django-passkeys-1.2.2/passkeys/backend.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/passkeys/migrations/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1176 2022-10-28 13:18:42.000000 django-passkeys-1.2.2/passkeys/migrations/0001_initial.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2022-10-28 10:29:36.000000 django-passkeys-1.2.2/passkeys/migrations/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      599 2022-12-09 11:07:59.000000 django-passkeys-1.2.2/passkeys/models.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/passkeys/static/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/passkeys/static/passkeys/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/passkeys/static/passkeys/css/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1590 2019-06-20 18:14:15.000000 django-passkeys-1.2.2/passkeys/static/passkeys/css/bootstrap-toggle.min.css
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/passkeys/static/passkeys/imgs/
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     8981 2022-08-24 16:03:28.000000 django-passkeys-1.2.2/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/passkeys/static/passkeys/js/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2684 2022-10-23 19:24:16.000000 django-passkeys-1.2.2/passkeys/static/passkeys/js/base64url.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4129 2019-06-20 18:14:15.000000 django-passkeys-1.2.2/passkeys/static/passkeys/js/bootstrap-toggle.min.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      687 2022-10-23 19:24:16.000000 django-passkeys-1.2.2/passkeys/static/passkeys/js/helpers.js
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/passkeys/templates/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5795 2023-06-17 11:35:33.000000 django-passkeys-1.2.2/passkeys/templates/PassKeys.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      128 2022-10-28 10:53:07.000000 django-passkeys-1.2.2/passkeys/templates/PassKeys_base.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      724 2022-12-09 11:08:08.000000 django-passkeys-1.2.2/passkeys/templates/check_passkeys.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      807 2022-09-09 17:51:05.000000 django-passkeys-1.2.2/passkeys/templates/modal.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2249 2023-06-17 09:46:50.000000 django-passkeys-1.2.2/passkeys/templates/passkeys.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      563 2022-12-09 11:08:08.000000 django-passkeys-1.2.2/passkeys/urls.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      911 2022-12-09 11:08:08.000000 django-passkeys-1.2.2/passkeys/views.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-06-17 16:32:04.000000 django-passkeys-1.2.2/setup.cfg
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1811 2023-06-17 16:31:03.000000 django-passkeys-1.2.2/setup.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1075 2022-10-28 10:01:16.000000 django-passkeys-1.2.3/LICENSE
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      192 2023-06-17 16:31:58.000000 django-passkeys-1.2.3/MANIFEST.in
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     7525 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6148 2023-06-17 16:34:53.000000 django-passkeys-1.2.3/README.md
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/django_passkeys.egg-info/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     7525 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/django_passkeys.egg-info/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      913 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/django_passkeys.egg-info/SOURCES.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/django_passkeys.egg-info/dependency_links.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2022-10-28 13:54:59.000000 django-passkeys-1.2.3/django_passkeys.egg-info/not-zip-safe
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       47 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/django_passkeys.egg-info/requires.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       17 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/django_passkeys.egg-info/top_level.txt
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/env/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/env/bin/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1199 2022-10-28 10:01:55.000000 django-passkeys-1.2.3/env/bin/activate_this.py
+-rwxrwxr-x   0 mohamed   (1000) mohamed   (1000)      153 2022-10-28 10:02:36.000000 django-passkeys-1.2.3/env/bin/django-admin.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/passkeys/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5823 2023-06-17 15:37:35.000000 django-passkeys-1.2.3/passkeys/FIDO2.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       65 2022-10-28 11:16:36.000000 django-passkeys-1.2.3/passkeys/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      790 2023-06-17 11:35:33.000000 django-passkeys-1.2.3/passkeys/backend.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/passkeys/migrations/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1176 2022-10-28 13:18:42.000000 django-passkeys-1.2.3/passkeys/migrations/0001_initial.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2022-10-28 10:29:36.000000 django-passkeys-1.2.3/passkeys/migrations/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      599 2022-12-09 11:07:59.000000 django-passkeys-1.2.3/passkeys/models.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/passkeys/static/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/passkeys/static/passkeys/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/passkeys/static/passkeys/css/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1590 2019-06-20 18:14:15.000000 django-passkeys-1.2.3/passkeys/static/passkeys/css/bootstrap-toggle.min.css
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/passkeys/static/passkeys/imgs/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     8981 2022-08-24 16:03:28.000000 django-passkeys-1.2.3/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/passkeys/static/passkeys/js/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2684 2022-10-23 19:24:16.000000 django-passkeys-1.2.3/passkeys/static/passkeys/js/base64url.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4129 2019-06-20 18:14:15.000000 django-passkeys-1.2.3/passkeys/static/passkeys/js/bootstrap-toggle.min.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      687 2022-10-23 19:24:16.000000 django-passkeys-1.2.3/passkeys/static/passkeys/js/helpers.js
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/passkeys/templates/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5795 2023-06-17 11:35:33.000000 django-passkeys-1.2.3/passkeys/templates/PassKeys.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      128 2022-10-28 10:53:07.000000 django-passkeys-1.2.3/passkeys/templates/PassKeys_base.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      724 2022-12-09 11:08:08.000000 django-passkeys-1.2.3/passkeys/templates/check_passkeys.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      807 2022-09-09 17:51:05.000000 django-passkeys-1.2.3/passkeys/templates/modal.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2249 2023-06-17 09:46:50.000000 django-passkeys-1.2.3/passkeys/templates/passkeys.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      563 2022-12-09 11:08:08.000000 django-passkeys-1.2.3/passkeys/urls.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      911 2022-12-09 11:08:08.000000 django-passkeys-1.2.3/passkeys/views.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/setup.cfg
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1811 2023-06-17 16:35:01.000000 django-passkeys-1.2.3/setup.py
```

### Comparing `django-passkeys-1.2.2/LICENSE` & `django-passkeys-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/PKG-INFO` & `django-passkeys-1.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 616e  : 2.1.Name: djan
 00000020: 676f 2d70 6173 736b 6579 730a 5665 7273  go-passkeys.Vers
-00000030: 696f 6e3a 2031 2e32 2e32 0a53 756d 6d61  ion: 1.2.2.Summa
+00000030: 696f 6e3a 2031 2e32 2e33 0a53 756d 6d61  ion: 1.2.3.Summa
 00000040: 7279 3a20 4120 446a 616e 676f 2041 7574  ry: A Django Aut
 00000050: 6865 6e74 6963 6174 696f 6e20 4261 636b  hentication Back
 00000060: 656e 6420 666f 7220 5061 7373 6b65 7973  end for Passkeys
 00000070: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
 00000080: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
 00000090: 6b61 6c69 6f62 792f 646a 616e 676f 2d70  kalioby/django-p
 000000a0: 6173 736b 6579 730a 446f 776e 6c6f 6164  asskeys.Download
@@ -89,360 +89,383 @@
 00000580: 696f 6e5d 2868 7474 7073 3a2f 2f62 6164  ion](https://bad
 00000590: 6765 2e66 7572 792e 696f 2f70 792f 646a  ge.fury.io/py/dj
 000005a0: 616e 676f 2d70 6173 736b 6579 732e 7376  ango-passkeys.sv
 000005b0: 6729 5d28 6874 7470 733a 2f2f 6261 6467  g)](https://badg
 000005c0: 652e 6675 7279 2e69 6f2f 7079 2f64 6a61  e.fury.io/py/dja
 000005d0: 6e67 6f2d 7061 7373 6b65 7973 290a 5b21  ngo-passkeys).[!
 000005e0: 5b44 6f77 6e6c 6f61 6473 5d28 6874 7470  [Downloads](http
-000005f0: 733a 2f2f 7065 7079 2e74 6563 682f 6261  s://pepy.tech/ba
-00000600: 6467 652f 646a 616e 676f 2d70 6173 736b  dge/django-passk
-00000610: 6579 732f 6d6f 6e74 6829 5d28 6874 7470  eys/month)](http
-00000620: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
-00000630: 6f6a 6563 742f 646a 616e 676f 2d70 6173  oject/django-pas
-00000640: 736b 6579 7329 0a21 5b43 6f76 6572 6167  skeys).![Coverag
-00000650: 655d 2863 6f76 6572 6167 652e 7376 6729  e](coverage.svg)
-00000660: 0a0a 416e 2065 7874 656e 7369 6f6e 2074  ..An extension t
-00000670: 6f20 446a 616e 676f 202a 4d6f 6465 6c42  o Django *ModelB
-00000680: 6163 6b65 6e64 2a20 6261 636b 656e 6420  ackend* backend 
-00000690: 746f 2073 7570 706f 7274 2070 6173 736b  to support passk
-000006a0: 6579 732e 0a0a 5061 7373 6b65 7973 2069  eys...Passkeys i
-000006b0: 7320 616e 2065 7874 656e 7369 6f6e 2074  s an extension t
-000006c0: 6f20 5765 6220 4175 7468 656e 7469 6361  o Web Authentica
-000006d0: 7469 6f6e 2041 5049 2074 6861 7420 7769  tion API that wi
-000006e0: 6c6c 2061 6c6c 6f77 2074 6865 2075 7365  ll allow the use
-000006f0: 7220 746f 206c 6f67 696e 2074 6f20 6120  r to login to a 
-00000700: 7365 7276 6963 6520 7573 696e 6720 616e  service using an
-00000710: 6f74 6865 7220 6465 7669 6365 2e0a 0a54  other device...T
-00000720: 6869 7320 6170 7020 6973 2061 2073 6c69  his app is a sli
-00000730: 6d2d 646f 776e 2076 6572 7369 6f6e 206f  m-down version o
-00000740: 6620 5b64 6a61 6e67 6f2d 6d66 6132 5d28  f [django-mfa2](
-00000750: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000760: 6f6d 2f6d 6b61 6c69 6f62 792f 646a 616e  om/mkalioby/djan
-00000770: 676f 2d6d 6661 3229 0a0a 5061 7373 6b65  go-mfa2)..Passke
-00000780: 7973 2061 7265 206e 6f77 2073 7570 706f  ys are now suppo
-00000790: 7274 6564 206f 6e20 0a2a 2041 7070 6c65  rted on .* Apple
-000007a0: 2045 636f 7379 7374 656d 2028 6950 686f   Ecosystem (iPho
-000007b0: 6e65 2031 362e 302b 2c20 6950 6164 4f53  ne 16.0+, iPadOS
-000007c0: 2031 362e 312c 204d 6163 204f 5320 5820   16.1, Mac OS X 
-000007d0: 5665 6e74 7572 6129 0a2a 2043 6872 6f6d  Ventura).* Chrom
-000007e0: 6975 6d20 6261 7365 6420 6272 6f77 7365  ium based browse
-000007f0: 7273 2028 6f6e 2050 4320 616e 6420 4c61  rs (on PC and La
-00000800: 7074 6f70 2920 616c 6c6f 7773 2070 6963  ptop) allows pic
-00000810: 6b69 6e67 2075 7020 6372 6564 656e 7469  king up credenti
-00000820: 616c 7320 6672 6f6d 2041 6e64 726f 6964  als from Android
-00000830: 2061 6e64 2069 5068 6f6e 652f 6950 6164   and iPhone/iPad
-00000840: 4f53 2e0a 2a20 416e 6472 6f69 6420 4372  OS..* Android Cr
-00000850: 6564 656e 7469 616c 7320 6372 6561 7469  edentials creati
-00000860: 6f6e 2066 6f72 2052 6573 6964 656e 744b  on for ResidentK
-00000870: 6579 7320 6973 2063 7572 7265 6e74 6c79  eys is currently
-00000880: 2069 6e20 6c69 7665 206e 6f77 2e0a 0a4f   in live now...O
-00000890: 6e20 4d61 7920 332c 2032 3032 332c 2047  n May 3, 2023, G
-000008a0: 6f6f 676c 6520 616c 6c6f 7765 6420 7468  oogle allowed th
-000008b0: 6520 7573 6520 6f66 2050 6173 736b 6579  e use of Passkey
-000008c0: 7320 666f 7220 7468 6520 7573 6572 7320  s for the users 
-000008d0: 746f 206c 6f67 696e 2c20 6b69 6c6c 696e  to login, killin
-000008e0: 6720 7468 6520 7061 7373 776f 7264 2066  g the password f
-000008f0: 6f72 2065 6e72 6f6c 6c65 6420 7573 6572  or enrolled user
-00000900: 732e 200a 0a23 2049 6e73 7461 6c6c 6174  s. ..# Installat
-00000910: 696f 6e0a 0a60 7069 7020 696e 7374 616c  ion..`pip instal
-00000920: 6c20 646a 616e 676f 2d70 6173 736b 6579  l django-passkey
-00000930: 7360 0a0a 4375 7272 656e 746c 792c 2069  s`..Currently, i
-00000940: 7420 7375 7070 6f72 7420 446a 616e 676f  t support Django
-00000950: 2032 2e30 2b2c 2050 7974 686f 6e20 332e   2.0+, Python 3.
-00000960: 372b 0a0a 2320 5573 6167 650a 312e 2069  7+..# Usage.1. i
-00000970: 6e20 796f 7572 2073 6574 7469 6e67 732e  n your settings.
-00000980: 7079 2061 6464 2074 6865 2061 7070 6c69  py add the appli
-00000990: 6361 7469 6f6e 2074 6f20 796f 7572 2069  cation to your i
-000009a0: 6e73 7461 6c6c 6564 2061 7070 730a 2020  nstalled apps.  
-000009b0: 2060 6060 7079 7468 6f6e 0a20 2020 494e   ```python.   IN
-000009c0: 5354 414c 4c45 445f 4150 5053 3d28 0a20  STALLED_APPS=(. 
-000009d0: 2020 272e 2e2e 2e2e 2e27 2c0a 2020 2027    '......',.   '
-000009e0: 7061 7373 6b65 7973 272c 0a20 2020 272e  passkeys',.   '.
-000009f0: 2e2e 2e2e 2e27 290a 2020 2060 6060 0a32  .....').   ```.2
-00000a00: 2e20 436f 6c6c 6563 7420 5374 6174 6963  . Collect Static
-00000a10: 2046 696c 6573 0a60 7079 7468 6f6e 206d   Files.`python m
-00000a20: 616e 6167 652e 7079 2063 6f6c 6c65 6374  anage.py collect
-00000a30: 7374 6174 6963 600a 332e 2052 756e 206d  static`.3. Run m
-00000a40: 6967 7261 7465 0a60 7079 7468 6f6e 206d  igrate.`python m
-00000a50: 616e 6167 652e 7079 206d 6967 7261 7465  anage.py migrate
-00000a60: 600a 342e 2041 6464 2074 6865 2066 6f6c  `.4. Add the fol
-00000a70: 6c6f 7769 6e67 2073 6574 7469 6e67 7320  lowing settings 
-00000a80: 746f 2079 6f75 7220 6669 6c65 0a0a 2020  to your file..  
-00000a90: 2060 6060 7079 7468 6f6e 0a20 2020 2041   ```python.    A
-00000aa0: 5554 4845 4e54 4943 4154 494f 4e5f 4241  UTHENTICATION_BA
-00000ab0: 434b 454e 4453 203d 205b 2770 6173 736b  CKENDS = ['passk
-00000ac0: 6579 732e 6261 636b 656e 642e 5061 7373  eys.backend.Pass
-00000ad0: 6b65 794d 6f64 656c 4261 636b 656e 6427  keyModelBackend'
-00000ae0: 5d20 2320 4368 616e 6765 2079 6f75 7220  ] # Change your 
-00000af0: 6175 7468 656e 7469 6361 7469 6f6e 2062  authentication b
-00000b00: 6163 6b65 6e64 0a20 2020 2046 4944 4f5f  ackend.    FIDO_
-00000b10: 5345 5256 4552 5f49 443d 226c 6f63 616c  SERVER_ID="local
-00000b20: 686f 7374 2220 2020 2020 2023 2053 6572  host"      # Ser
-00000b30: 7665 7220 7270 2069 6420 666f 7220 4649  ver rp id for FI
-00000b40: 444f 322c 2069 7420 7468 6520 6675 6c6c  DO2, it the full
-00000b50: 2064 6f6d 6169 6e20 6f66 2079 6f75 7220   domain of your 
-00000b60: 7072 6f6a 6563 740a 2020 2020 4649 444f  project.    FIDO
-00000b70: 5f53 4552 5645 525f 4e41 4d45 3d22 5465  _SERVER_NAME="Te
-00000b80: 7374 4170 7022 0a20 2020 2069 6d70 6f72  stApp".    impor
-00000b90: 7420 7061 7373 6b65 7973 0a20 2020 204b  t passkeys.    K
-00000ba0: 4559 5f41 5454 4143 484d 454e 5420 3d20  EY_ATTACHMENT = 
-00000bb0: 4e6f 6e65 207c 2070 6173 736b 6579 732e  None | passkeys.
-00000bc0: 4174 7461 6368 6d65 6e74 2e43 524f 5353  Attachment.CROSS
-00000bd0: 5f50 4c41 5446 4f52 4d20 7c20 7061 7373  _PLATFORM | pass
-00000be0: 6b65 7973 2e41 7474 6163 686d 656e 742e  keys.Attachment.
-00000bf0: 504c 4154 464f 524d 0a20 2020 6060 600a  PLATFORM.   ```.
-00000c00: 2020 202a 2a4e 6f74 652a 2a3a 2053 7461     **Note**: Sta
-00000c10: 7274 696e 6720 7631 2e31 2c20 6046 4944  rting v1.1, `FID
-00000c20: 4f5f 5345 5256 4552 5f49 4460 2061 6e64  O_SERVER_ID` and
-00000c30: 2f6f 7220 6046 4944 4f5f 5345 5256 4552  /or `FIDO_SERVER
-00000c40: 5f4e 414d 4560 2063 616e 2062 6520 6120  _NAME` can be a 
-00000c50: 6361 6c6c 6162 6c65 2074 6f20 7375 7070  callable to supp
-00000c60: 6f72 7420 6d75 6c74 692d 7465 6e61 6e74  ort multi-tenant
-00000c70: 7320 7765 6220 6170 706c 6963 6174 696f  s web applicatio
-00000c80: 6e73 2c20 7468 6520 6072 6571 7565 7374  ns, the `request
-00000c90: 6020 6973 2070 6173 7365 6420 746f 2074  ` is passed to t
-00000ca0: 6865 2063 616c 6c65 6420 6675 6e63 7469  he called functi
-00000cb0: 6f6e 2e0a 352e 2041 6464 2070 6173 736b  on..5. Add passk
-00000cc0: 6579 7320 746f 2075 726c 732e 7079 0a20  eys to urls.py. 
-00000cd0: 2020 6060 6070 7974 686f 6e20 0a0a 2020    ```python ..  
-00000ce0: 2075 726c 735f 7061 7474 6572 6e73 3d20   urls_patterns= 
-00000cf0: 5b0a 2020 2027 2e2e 2e27 2c0a 2020 2075  [.   '...',.   u
-00000d00: 726c 2872 275e 7061 7373 6b65 7973 2f27  rl(r'^passkeys/'
-00000d10: 2c20 696e 636c 7564 6528 2770 6173 736b  , include('passk
-00000d20: 6579 732e 7572 6c73 2729 292c 0a20 2020  eys.urls')),.   
-00000d30: 272e 2e2e 2e27 2c0a 2020 2020 5d0a 2020  '....',.    ].  
-00000d40: 2020 6060 600a 362e 2054 6f20 6d61 7463    ```.6. To matc
-00000d50: 6820 7468 6520 6c6f 6f6b 2061 6e64 2066  h the look and f
-00000d60: 6565 6c20 6f66 2079 6f75 7220 7072 6f6a  eel of your proj
-00000d70: 6563 742c 2050 6173 736b 6579 7320 696e  ect, Passkeys in
-00000d80: 636c 7564 6573 2060 6261 7365 2e68 746d  cludes `base.htm
-00000d90: 6c60 2062 7574 2069 7420 6e65 6564 7320  l` but it needs 
-00000da0: 626c 6f63 6b73 206e 616d 6564 2060 6865  blocks named `he
-00000db0: 6164 6020 2620 6063 6f6e 7465 6e74 6020  ad` & `content` 
-00000dc0: 746f 2061 6464 6564 2069 7473 2063 6f6e  to added its con
-00000dd0: 7465 6e74 2074 6f20 6974 2e0a 2020 202a  tent to it..   *
-00000de0: 2a4e 6f74 6573 3a2a 2a20 0a20 2020 200a  *Notes:** .    .
-00000df0: 2020 2020 312e 2059 6f75 2063 616e 206f      1. You can o
-00000e00: 7665 7272 6964 6520 6050 6173 734b 6579  verride `PassKey
-00000e10: 735f 6261 7365 2e68 746d 6c60 2077 6869  s_base.html` whi
-00000e20: 6368 2069 7320 7573 6564 2062 7920 6050  ch is used by `P
-00000e30: 6173 736b 6579 732e 6874 6d6c 6020 736f  asskeys.html` so
-00000e40: 2079 6f75 2063 616e 2063 6f6e 7472 6f6c   you can control
-00000e50: 2074 6865 2073 7479 6c69 6e67 2062 6574   the styling bet
-00000e60: 7465 7220 616e 6420 6375 7272 656e 7420  ter and current 
-00000e70: 6050 6173 736b 6579 735f 6261 7365 2e68  `Passkeys_base.h
-00000e80: 746d 6c60 2065 7874 656e 6473 2060 6261  tml` extends `ba
-00000e90: 7365 2e68 746d 6c60 0a20 2020 2031 2e20  se.html`.    1. 
-00000ea0: 4375 7272 656e 746c 792c 2060 5061 7373  Currently, `Pass
-00000eb0: 4b65 7973 5f62 6173 652e 6874 6d6c 6020  Keys_base.html` 
-00000ec0: 6e65 6564 7320 4a51 7565 7279 2061 6e64  needs JQuery and
-00000ed0: 2062 6f6f 7473 7472 6170 2e20 0a0a 372e   bootstrap. ..7.
-00000ee0: 2053 6f6d 6577 6865 7265 2069 6e20 796f   Somewhere in yo
-00000ef0: 7572 2061 7070 2c20 6164 6420 6120 6c69  ur app, add a li
-00000f00: 6e6b 2074 6f20 2770 6173 736b 6579 733a  nk to 'passkeys:
-00000f10: 686f 6d65 270a 2020 2020 6060 603c 6c69  home'.    ```<li
-00000f20: 3e3c 6120 6872 6566 3d22 7b25 2075 726c  ><a href="{% url
-00000f30: 2027 7061 7373 6b65 7973 3a68 6f6d 6527   'passkeys:home'
-00000f40: 2025 7d22 3e50 6173 736b 6579 733c 2f61   %}">Passkeys</a
-00000f50: 3e20 3c2f 6c69 3e60 6060 0a38 2e20 496e  > </li>```.8. In
-00000f60: 2079 6f75 7220 6c6f 6769 6e20 7669 6577   your login view
-00000f70: 2c20 6368 616e 6765 2074 6865 2061 7574  , change the aut
-00000f80: 6865 6e74 6963 6174 6520 6361 6c6c 2074  henticate call t
-00000f90: 6f20 696e 636c 7564 6520 7468 6520 7265  o include the re
-00000fa0: 7175 6573 7420 6173 2066 6f6c 6c6f 7773  quest as follows
-00000fb0: 0a20 2020 6060 6070 7974 686f 6e0a 2020  .   ```python.  
-00000fc0: 2020 7573 6572 3d61 7574 6865 6e74 6963    user=authentic
-00000fd0: 6174 6528 7265 7175 6573 742c 2075 7365  ate(request, use
-00000fe0: 726e 616d 653d 7265 7175 6573 742e 504f  rname=request.PO
-00000ff0: 5354 5b22 7573 6572 6e61 6d65 225d 2c70  ST["username"],p
-00001000: 6173 7377 6f72 643d 7265 7175 6573 742e  assword=request.
-00001010: 504f 5354 5b22 7061 7373 776f 7264 225d  POST["password"]
-00001020: 290a 2020 2020 6060 600a 0a38 2e20 4669  ).    ```..8. Fi
-00001030: 6e61 6c6c 792c 2049 6e20 796f 7572 2060  nally, In your `
-00001040: 6c6f 6769 6e2e 6874 6d6c 600a 2020 202a  login.html`.   *
-00001050: 2047 6976 6520 616e 2069 6420 746f 2079   Give an id to y
-00001060: 6f75 7220 6c6f 6769 6e20 666f 726d 2065  our login form e
-00001070: 2e67 2027 6c6f 6769 6e46 6f72 6d27 2c20  .g 'loginForm', 
-00001080: 7468 6520 6964 2073 686f 756c 6420 6265  the id should be
-00001090: 2070 726f 7669 6465 6420 7768 656e 2063   provided when c
-000010a0: 616c 6c69 6e67 2060 6175 7468 6e60 2066  alling `authn` f
-000010b0: 756e 6374 696f 6e0a 2020 202a 2049 6e73  unction.   * Ins
-000010c0: 6964 6520 7468 6520 666f 726d 2c20 6164  ide the form, ad
-000010d0: 6420 0a20 2020 2020 6060 6068 746d 6c0a  d .     ```html.
-000010e0: 2020 2020 2020 3c69 6e70 7574 2074 7970        <input typ
-000010f0: 653d 2268 6964 6465 6e22 206e 616d 653d  e="hidden" name=
-00001100: 2270 6173 736b 6579 7322 2069 643d 2270  "passkeys" id="p
-00001110: 6173 736b 6579 7322 2f3e 0a20 2020 2020  asskeys"/>.     
-00001120: 203c 6275 7474 6f6e 2063 6c61 7373 3d22   <button class="
-00001130: 6274 6e20 6274 6e2d 626c 6f63 6b20 6274  btn btn-block bt
-00001140: 6e2d 6461 726b 2220 7479 7065 3d22 6275  n-dark" type="bu
-00001150: 7474 6f6e 2220 6f6e 636c 6963 6b3d 2261  tton" onclick="a
-00001160: 7574 686e 2827 6c6f 6769 6e46 6f72 6d27  uthn('loginForm'
-00001170: 2922 3e3c 696d 6720 7372 633d 227b 2520  )"><img src="{% 
-00001180: 7374 6174 6963 2027 7061 7373 6b65 7973  static 'passkeys
-00001190: 2f69 6d67 732f 4649 444f 2d50 6173 736b  /imgs/FIDO-Passk
-000011a0: 6579 5f49 636f 6e2d 5768 6974 652e 706e  ey_Icon-White.pn
-000011b0: 6727 2025 7d22 2073 7479 6c65 3d22 7769  g' %}" style="wi
-000011c0: 6474 683a 2032 3470 7822 3e0a 2020 2020  dth: 24px">.    
-000011d0: 207b 2569 6e63 6c75 6465 2027 7061 7373   {%include 'pass
-000011e0: 6b65 7973 2e6a 7327 2025 7d0a 2020 2020  keys.js' %}.    
-000011f0: 2060 6060 0a46 6f72 2045 7861 6d70 6c65   ```.For Example
-00001200: 2c20 5365 6520 2765 7861 6d70 6c65 2720  , See 'example' 
-00001210: 6170 7020 616e 6420 6c6f 6f6b 2061 7420  app and look at 
-00001220: 4558 414d 504c 452e 6d64 2074 6f20 7365  EXAMPLE.md to se
-00001230: 6520 686f 7720 746f 2073 6574 2069 7420  e how to set it 
-00001240: 7570 2e0a 0a23 2044 6574 6563 7420 6966  up...# Detect if
-00001250: 2075 7365 7220 6973 2075 7369 6e67 2070   user is using p
-00001260: 6173 736b 6579 730a 4f6e 6365 2074 6865  asskeys.Once the
-00001270: 2062 6163 6b65 6e64 2069 7320 7573 6564   backend is used
-00001280: 2c20 7468 6572 6520 7769 6c6c 2062 6520  , there will be 
-00001290: 6120 6070 6173 736b 6579 6020 6b65 7920  a `passkey` key 
-000012a0: 696e 2072 6571 7565 7374 2e73 6573 7369  in request.sessi
-000012b0: 6f6e 2e20 0a49 6620 7468 6520 7573 6572  on. .If the user
-000012c0: 2075 7365 6420 6120 7061 7373 6b65 7920   used a passkey 
-000012d0: 7468 656e 2060 7265 7175 6573 742e 7365  then `request.se
-000012e0: 7373 696f 6e5b 2770 6173 736b 6579 275d  ssion['passkey']
-000012f0: 5b27 7061 7373 6b65 7927 5d60 2077 696c  ['passkey']` wil
-00001300: 6c20 6265 2054 7275 6520 616e 6420 7468  l be True and th
-00001310: 6520 6b65 7920 696e 666f 726d 6174 696f  e key informatio
-00001320: 6e20 7769 6c6c 2062 6520 7468 6572 6520  n will be there 
-00001330: 6c69 6b65 2074 6869 730a 6060 6070 7974  like this.```pyt
-00001340: 686f 6e0a 7b27 7061 7373 6b65 7927 3a20  hon.{'passkey': 
-00001350: 5472 7565 2c20 276e 616d 6527 3a20 2743  True, 'name': 'C
-00001360: 6872 6f6d 6527 2c20 2769 6427 3a20 322c  hrome', 'id': 2,
-00001370: 2027 706c 6174 666f 726d 273a 2027 4368   'platform': 'Ch
-00001380: 726f 6d65 206f 6e20 4170 706c 6527 2c20  rome on Apple', 
-00001390: 2763 726f 7373 5f70 6c61 7466 6f72 6d27  'cross_platform'
-000013a0: 3a20 4661 6c73 657d 0a60 6060 0a60 6372  : False}.```.`cr
-000013b0: 6f73 735f 706c 6174 666f 726d 603a 206d  oss_platform`: m
-000013c0: 6561 6e73 2074 6861 7420 7468 6520 7573  eans that the us
-000013d0: 6572 2075 7365 6420 6120 6b65 7920 6672  er used a key fr
-000013e0: 6f6d 2061 6e6f 7468 6572 2070 6c61 7466  om another platf
-000013f0: 6f72 6d20 736f 2074 6865 7265 2069 7320  orm so there is 
-00001400: 6e6f 206b 6579 206c 6f63 616c 2074 6f20  no key local to 
-00001410: 7468 6520 6465 7669 6365 2075 7365 6420  the device used 
-00001420: 746f 206c 6f67 696e 2065 2e67 2075 7365  to login e.g use
-00001430: 6420 616e 2041 6e64 726f 6964 2070 686f  d an Android pho
-00001440: 6e65 206f 6e20 4d61 6320 4f53 2058 206f  ne on Mac OS X o
-00001450: 7220 6950 6164 2e0a 4966 2074 6865 2075  r iPad..If the u
-00001460: 7365 7220 6469 646e 2774 2075 7365 2061  ser didn't use a
-00001470: 2070 6173 736b 6579 2074 6865 6e20 6974   passkey then it
-00001480: 2077 696c 6c20 6265 2073 6574 2074 6f20   will be set to 
-00001490: 4661 6c73 650a 6060 6070 7974 686f 6e0a  False.```python.
-000014a0: 7b27 7061 7373 6b65 7927 3a46 616c 7365  {'passkey':False
-000014b0: 7d0a 6060 600a 0a0a 2320 4368 6563 6b20  }.```...# Check 
-000014c0: 6966 2074 6865 2075 7365 7220 6361 6e20  if the user can 
-000014d0: 6265 2065 6e72 6f6c 6c65 6420 666f 7220  be enrolled for 
-000014e0: 6120 706c 6174 666f 726d 2061 7574 6865  a platform authe
-000014f0: 6e74 6963 6174 6f72 0a0a 4966 2079 6f75  nticator..If you
-00001500: 2077 616e 7420 746f 2063 6865 636b 2069   want to check i
-00001510: 6620 7468 6520 7573 6572 2063 616e 2062  f the user can b
-00001520: 6520 656e 726f 6c6c 6564 2074 6f20 7573  e enrolled to us
-00001530: 6520 6120 706c 6174 666f 726d 2061 7574  e a platform aut
-00001540: 6865 6e74 6963 6174 6f72 2c20 796f 7520  henticator, you 
-00001550: 6361 6e20 646f 2074 6865 2066 6f6c 6c6f  can do the follo
-00001560: 7769 6e67 2069 6e20 796f 7572 206d 6169  wing in your mai
-00001570: 6e20 7061 6765 2e0a 0a60 6060 6874 6d6c  n page...```html
-00001580: 0a3c 6469 7620 6964 3d22 706b 2220 636c  .<div id="pk" cl
-00001590: 6173 733d 2261 6c65 7274 2061 6c65 7274  ass="alert alert
-000015a0: 2d69 6e66 6f22 2073 7479 6c65 3d22 6469  -info" style="di
-000015b0: 7370 6c61 793a 206e 6f6e 6522 3e59 6f75  splay: none">You
-000015c0: 7220 6465 7669 6365 2073 7570 706f 7274  r device support
-000015d0: 7320 7061 7373 6b65 7973 2c20 3c61 2068  s passkeys, <a h
-000015e0: 7265 663d 227b 2575 726c 2027 7061 7373  ref="{%url 'pass
-000015f0: 6b65 7973 3a65 6e72 6f6c 6c27 257d 223e  keys:enroll'%}">
-00001600: 456e 726f 6c6c 3c2f 613e 203c 2f64 6976  Enroll</a> </div
-00001610: 3e0a 3c73 6372 6970 7420 7479 7065 3d22  >.<script type="
-00001620: 7465 7874 2f6a 6176 6173 6372 6970 7422  text/javascript"
-00001630: 3e0a 6675 6e63 7469 6f6e 2072 6567 6973  >.function regis
-00001640: 7465 725f 706b 2829 0a20 2020 207b 0a20  ter_pk().    {. 
-00001650: 2020 2020 2020 2024 2827 2370 6b27 292e         $('#pk').
-00001660: 7368 6f77 2829 3b0a 2020 2020 7d0a 7b25  show();.    }.{%
-00001670: 2069 6e63 6c75 6465 2027 6368 6563 6b5f   include 'check_
-00001680: 7061 7373 6b65 7973 2e6a 7327 257d 0a24  passkeys.js'%}.$
-00001690: 2864 6f63 756d 656e 7429 2e72 6561 6479  (document).ready
-000016a0: 2863 6865 636b 5f70 6173 736b 6579 2874  (check_passkey(t
-000016b0: 7275 652c 7265 6769 7374 6572 5f70 6b29  rue,register_pk)
-000016c0: 290a 3c2f 7363 7269 7074 3e0a 6060 600a  ).</script>.```.
-000016d0: 6368 6563 6b5f 7061 7373 6b65 7920 6675  check_passkey fu
-000016e0: 6e63 7469 6f6e 2070 6172 616d 7465 7273  nction paramters
-000016f0: 2061 7265 2061 7320 666f 6c6c 6f77 7320   are as follows 
-00001700: 0a2a 2060 706c 6174 666f 726d 5f61 7574  .* `platform_aut
-00001710: 6865 6e74 6963 6174 6f72 603a 2069 6620  henticator`: if 
-00001720: 7468 6520 7365 7276 6963 6520 7265 7175  the service requ
-00001730: 6972 6573 206f 6e6c 7920 6120 706c 6174  ires only a plat
-00001740: 666f 726d 2061 7574 6865 6e74 6963 6174  form authenticat
-00001750: 6f72 2028 652e 6720 546f 7563 6849 442c  or (e.g TouchID,
-00001760: 2057 696e 646f 7773 2048 656c 6c6f 206f   Windows Hello o
-00001770: 7220 416e 6472 6f69 6420 5361 6665 7479  r Android Safety
-00001780: 4e65 7429 0a2a 2060 7375 6363 6573 735f  Net).* `success_
-00001790: 6675 6e63 603a 2066 756e 6374 696f 6e20  func`: function 
-000017a0: 746f 2063 616c 6c20 6966 2061 2070 6c61  to call if a pla
-000017b0: 7466 6f72 6d20 6175 7468 656e 7469 6361  tform authentica
-000017c0: 746f 7220 6973 2066 6f75 6e64 206f 7220  tor is found or 
-000017d0: 6966 2074 6865 2075 7365 7220 6469 646e  if the user didn
-000017e0: 2774 206c 6f67 696e 2062 7920 6120 7061  't login by a pa
-000017f0: 7373 6b65 790a 2a20 6066 6169 6c5f 6675  sskey.* `fail_fu
-00001800: 6e63 603a 2066 756e 6374 696f 6e20 746f  nc`: function to
-00001810: 2063 616c 6c20 6966 206e 6f20 706c 6174   call if no plat
-00001820: 666f 726d 2061 7574 6865 6e74 6963 6174  form authenticat
-00001830: 6f72 2069 7320 666f 756e 6420 286f 7074  or is found (opt
-00001840: 696f 6e61 6c29 2e0a 0a0a 2323 2055 7369  ional)....## Usi
-00001850: 6e67 2043 6f6e 6469 7469 6f6e 616c 2055  ng Conditional U
-00001860: 490a 0a43 6f6e 6469 7469 6f6e 616c 2055  I..Conditional U
-00001870: 4920 6973 2061 2077 6179 2066 6f72 2074  I is a way for t
-00001880: 6865 2062 726f 7773 6572 2074 6f20 7072  he browser to pr
-00001890: 6f6d 7074 2074 6865 2075 7365 7220 746f  ompt the user to
-000018a0: 2075 7365 2074 6865 2070 6173 736b 6579   use the passkey
-000018b0: 2074 6f20 6c6f 6769 6e20 746f 2074 6865   to login to the
-000018c0: 2073 7973 7465 6d20 6173 2073 686f 776e   system as shown
-000018d0: 2069 6e20 0a0a 215b 636f 6e64 6974 696f   in ..![conditio
-000018e0: 6e61 6c55 492e 706e 675d 2869 6d67 7325  nalUI.png](imgs%
-000018f0: 3246 636f 6e64 6974 696f 6e61 6c55 492e  2FconditionalUI.
-00001900: 706e 6729 0a0a 5374 6172 7469 6e67 2076  png)..Starting v
-00001910: 6572 7369 6f6e 2076 312e 322e 2079 6f75  ersion v1.2. you
-00001920: 2063 616e 2075 7365 2043 6f6e 6469 7469   can use Conditi
-00001930: 6f6e 616c 2055 4920 6279 2061 6464 696e  onal UI by addin
-00001940: 6720 7468 6520 666f 6c6c 6f77 696e 6720  g the following 
-00001950: 746f 2079 6f75 7220 6c6f 6769 6e20 7061  to your login pa
-00001960: 6765 0a0a 312e 2041 6464 2060 7765 6261  ge..1. Add `weba
-00001970: 7574 686e 6020 746f 2061 7574 6f63 6f6d  uthn` to autocom
-00001980: 706c 6574 6520 6f66 2074 6865 2075 7365  plete of the use
-00001990: 726e 616d 6520 6669 656c 6420 6173 2073  rname field as s
-000019a0: 686f 776e 2062 656c 6f77 2e0a 6060 6068  hown below..```h
-000019b0: 746d 6c0a 3c69 6e70 7574 206e 616d 653d  tml.<input name=
-000019c0: 2275 7365 726e 616d 6522 2070 6c61 6365  "username" place
-000019d0: 686f 6c64 6572 3d22 7573 6572 6e61 6d65  holder="username
-000019e0: 2220 6175 746f 636f 6d70 6c65 7465 3d22  " autocomplete="
-000019f0: 7573 6572 6e61 6d65 2077 6562 6175 7468  username webauth
-00001a00: 6e22 3e0a 6060 600a 6164 6420 7468 6520  n">.```.add the 
-00001a10: 666f 6c6c 6f77 696e 6720 746f 2074 6865  following to the
-00001a20: 2070 6167 6520 6a73 2e0a 0a60 6060 6a73   page js...```js
-00001a30: 0a77 696e 646f 772e 6f6e 6c6f 6164 203d  .window.onload =
-00001a40: 2063 6865 636b 436f 6e64 6974 696f 6e61   checkConditiona
-00001a50: 6c55 4928 276c 6f67 696e 466f 726d 2729  lUI('loginForm')
-00001a60: 3b0a 6060 600a 7768 6572 6520 606c 6f67  ;.```.where `log
-00001a70: 696e 466f 726d 6020 6973 206e 616d 6520  inForm` is name 
-00001a80: 6f66 2079 6f75 7220 6c6f 6769 6e20 666f  of your login fo
-00001a90: 726d 2e0a 0a23 2320 5365 6375 7269 7479  rm...## Security
-00001aa0: 2063 6f6e 7461 6374 2069 6e66 6f72 6d61   contact informa
-00001ab0: 7469 6f6e 0a0a 546f 2072 6570 6f72 7420  tion..To report 
-00001ac0: 6120 7365 6375 7269 7479 2076 756c 6e65  a security vulne
-00001ad0: 7261 6269 6c69 7479 2c20 706c 6561 7365  rability, please
-00001ae0: 2075 7365 2074 6865 0a5b 5469 6465 6c69   use the.[Tideli
-00001af0: 6674 2073 6563 7572 6974 7920 636f 6e74  ft security cont
-00001b00: 6163 745d 2868 7474 7073 3a2f 2f74 6964  act](https://tid
-00001b10: 656c 6966 742e 636f 6d2f 7365 6375 7269  elift.com/securi
-00001b20: 7479 292e 0a54 6964 656c 6966 7420 7769  ty)..Tidelift wi
-00001b30: 6c6c 2063 6f6f 7264 696e 6174 6520 7468  ll coordinate th
-00001b40: 6520 6669 7820 616e 6420 6469 7363 6c6f  e fix and disclo
-00001b50: 7375 7265 2e0a 0a23 2043 6f6e 7472 6962  sure...# Contrib
-00001b60: 7574 6f72 730a 2a20 5b6d 6168 6d6f 6f64  utors.* [mahmood
-00001b70: 6e61 7372 5d28 6874 7470 733a 2f2f 6769  nasr](https://gi
-00001b80: 7468 7562 2e63 6f6d 2f6d 6168 6d6f 6f64  thub.com/mahmood
-00001b90: 6e61 7372 290a 2a20 5b6a 6163 6f70 7364  nasr).* [jacopsd
-00001ba0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001bb0: 2e63 6f6d 2f6a 6163 6f70 7364 2920 2020  .com/jacopsd)   
-00001bc0: 0a2a 205b 6761 7370 6172 6272 6f67 7565  .* [gasparbrogue
-00001bd0: 6972 615d 2868 7474 7073 3a2f 2f67 6974  ira](https://git
-00001be0: 6875 622e 636f 6d2f 6761 7370 6172 6272  hub.com/gasparbr
-00001bf0: 6f67 7565 6972 6129 0a0a 0a0a 0a         ogueira).....
+000005f0: 733a 2f2f 7374 6174 6963 2e70 6570 792e  s://static.pepy.
+00000600: 7465 6368 2f62 6164 6765 2f64 6a61 6e67  tech/badge/djang
+00000610: 6f2d 7061 7373 6b65 7973 295d 2868 7474  o-passkeys)](htt
+00000620: 7073 3a2f 2f70 6570 792e 7465 6368 2f70  ps://pepy.tech/p
+00000630: 726f 6a65 6374 2f64 6a61 6e67 6f2d 7061  roject/django-pa
+00000640: 7373 6b65 7973 290a 5b21 5b44 6f77 6e6c  sskeys).[![Downl
+00000650: 6f61 6473 202f 204d 6f6e 7468 205d 2868  oads / Month ](h
+00000660: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
+00000670: 2f62 6164 6765 2f64 6a61 6e67 6f2d 7061  /badge/django-pa
+00000680: 7373 6b65 7973 2f6d 6f6e 7468 295d 2868  sskeys/month)](h
+00000690: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
+000006a0: 2f70 726f 6a65 6374 2f64 6a61 6e67 6f2d  /project/django-
+000006b0: 7061 7373 6b65 7973 290a 5b21 5b62 7569  passkeys).[![bui
+000006c0: 6c64 5d28 6874 7470 733a 2f2f 6769 7468  ld](https://gith
+000006d0: 7562 2e63 6f6d 2f6d 6b61 6c69 6f62 792f  ub.com/mkalioby/
+000006e0: 646a 616e 676f 2d70 6173 736b 6579 732f  django-passkeys/
+000006f0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000700: 732f 6261 7369 635f 6368 6563 6b73 2e79  s/basic_checks.y
+00000710: 6d6c 2f62 6164 6765 2e73 7667 295d 2868  ml/badge.svg)](h
+00000720: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000730: 6d2f 6d6b 616c 696f 6279 2f64 6a61 6e67  m/mkalioby/djang
+00000740: 6f2d 7061 7373 6b65 7973 2f61 6374 696f  o-passkeys/actio
+00000750: 6e73 2f77 6f72 6b66 6c6f 7773 2f62 6173  ns/workflows/bas
+00000760: 6963 5f63 6865 636b 732e 796d 6c29 0a21  ic_checks.yml).!
+00000770: 5b43 6f76 6572 6167 655d 2868 7474 7073  [Coverage](https
+00000780: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000790: 7263 6f6e 7465 6e74 2e63 6f6d 2f6d 6b61  rcontent.com/mka
+000007a0: 6c69 6f62 792f 646a 616e 676f 2d70 6173  lioby/django-pas
+000007b0: 736b 6579 732f 6d61 696e 2f63 6f76 6572  skeys/main/cover
+000007c0: 6167 652e 7376 6729 0a0a 416e 2065 7874  age.svg)..An ext
+000007d0: 656e 7369 6f6e 2074 6f20 446a 616e 676f  ension to Django
+000007e0: 202a 4d6f 6465 6c42 6163 6b65 6e64 2a20   *ModelBackend* 
+000007f0: 6261 636b 656e 6420 746f 2073 7570 706f  backend to suppo
+00000800: 7274 2070 6173 736b 6579 732e 0a0a 5061  rt passkeys...Pa
+00000810: 7373 6b65 7973 2069 7320 616e 2065 7874  sskeys is an ext
+00000820: 656e 7369 6f6e 2074 6f20 5765 6220 4175  ension to Web Au
+00000830: 7468 656e 7469 6361 7469 6f6e 2041 5049  thentication API
+00000840: 2074 6861 7420 7769 6c6c 2061 6c6c 6f77   that will allow
+00000850: 2074 6865 2075 7365 7220 746f 206c 6f67   the user to log
+00000860: 696e 2074 6f20 6120 7365 7276 6963 6520  in to a service 
+00000870: 7573 696e 6720 616e 6f74 6865 7220 6465  using another de
+00000880: 7669 6365 2e0a 0a54 6869 7320 6170 7020  vice...This app 
+00000890: 6973 2061 2073 6c69 6d2d 646f 776e 2076  is a slim-down v
+000008a0: 6572 7369 6f6e 206f 6620 5b64 6a61 6e67  ersion of [djang
+000008b0: 6f2d 6d66 6132 5d28 6874 7470 733a 2f2f  o-mfa2](https://
+000008c0: 6769 7468 7562 2e63 6f6d 2f6d 6b61 6c69  github.com/mkali
+000008d0: 6f62 792f 646a 616e 676f 2d6d 6661 3229  oby/django-mfa2)
+000008e0: 0a0a 5061 7373 6b65 7973 2061 7265 206e  ..Passkeys are n
+000008f0: 6f77 2073 7570 706f 7274 6564 206f 6e20  ow supported on 
+00000900: 0a2a 2041 7070 6c65 2045 636f 7379 7374  .* Apple Ecosyst
+00000910: 656d 2028 6950 686f 6e65 2031 362e 302b  em (iPhone 16.0+
+00000920: 2c20 6950 6164 4f53 2031 362e 312c 204d  , iPadOS 16.1, M
+00000930: 6163 204f 5320 5820 5665 6e74 7572 6129  ac OS X Ventura)
+00000940: 0a2a 2043 6872 6f6d 6975 6d20 6261 7365  .* Chromium base
+00000950: 6420 6272 6f77 7365 7273 2028 6f6e 2050  d browsers (on P
+00000960: 4320 616e 6420 4c61 7074 6f70 2920 616c  C and Laptop) al
+00000970: 6c6f 7773 2070 6963 6b69 6e67 2075 7020  lows picking up 
+00000980: 6372 6564 656e 7469 616c 7320 6672 6f6d  credentials from
+00000990: 2041 6e64 726f 6964 2061 6e64 2069 5068   Android and iPh
+000009a0: 6f6e 652f 6950 6164 4f53 2e0a 2a20 416e  one/iPadOS..* An
+000009b0: 6472 6f69 6420 4372 6564 656e 7469 616c  droid Credential
+000009c0: 7320 6372 6561 7469 6f6e 2066 6f72 2052  s creation for R
+000009d0: 6573 6964 656e 744b 6579 7320 6973 2063  esidentKeys is c
+000009e0: 7572 7265 6e74 6c79 2069 6e20 6c69 7665  urrently in live
+000009f0: 206e 6f77 2e0a 0a4f 6e20 4d61 7920 332c   now...On May 3,
+00000a00: 2032 3032 332c 2047 6f6f 676c 6520 616c   2023, Google al
+00000a10: 6c6f 7765 6420 7468 6520 7573 6520 6f66  lowed the use of
+00000a20: 2050 6173 736b 6579 7320 666f 7220 7468   Passkeys for th
+00000a30: 6520 7573 6572 7320 746f 206c 6f67 696e  e users to login
+00000a40: 2c20 6b69 6c6c 696e 6720 7468 6520 7061  , killing the pa
+00000a50: 7373 776f 7264 2066 6f72 2065 6e72 6f6c  ssword for enrol
+00000a60: 6c65 6420 7573 6572 732e 200a 0a23 2049  led users. ..# I
+00000a70: 6e73 7461 6c6c 6174 696f 6e0a 0a60 7069  nstallation..`pi
+00000a80: 7020 696e 7374 616c 6c20 646a 616e 676f  p install django
+00000a90: 2d70 6173 736b 6579 7360 0a0a 4375 7272  -passkeys`..Curr
+00000aa0: 656e 746c 792c 2069 7420 7375 7070 6f72  ently, it suppor
+00000ab0: 7420 446a 616e 676f 2032 2e30 2b2c 2050  t Django 2.0+, P
+00000ac0: 7974 686f 6e20 332e 372b 0a0a 2320 5573  ython 3.7+..# Us
+00000ad0: 6167 650a 312e 2069 6e20 796f 7572 2073  age.1. in your s
+00000ae0: 6574 7469 6e67 732e 7079 2061 6464 2074  ettings.py add t
+00000af0: 6865 2061 7070 6c69 6361 7469 6f6e 2074  he application t
+00000b00: 6f20 796f 7572 2069 6e73 7461 6c6c 6564  o your installed
+00000b10: 2061 7070 730a 2020 2060 6060 7079 7468   apps.   ```pyth
+00000b20: 6f6e 0a20 2020 494e 5354 414c 4c45 445f  on.   INSTALLED_
+00000b30: 4150 5053 3d28 0a20 2020 272e 2e2e 2e2e  APPS=(.   '.....
+00000b40: 2e27 2c0a 2020 2027 7061 7373 6b65 7973  .',.   'passkeys
+00000b50: 272c 0a20 2020 272e 2e2e 2e2e 2e27 290a  ',.   '......').
+00000b60: 2020 2060 6060 0a32 2e20 436f 6c6c 6563     ```.2. Collec
+00000b70: 7420 5374 6174 6963 2046 696c 6573 0a60  t Static Files.`
+00000b80: 7079 7468 6f6e 206d 616e 6167 652e 7079  python manage.py
+00000b90: 2063 6f6c 6c65 6374 7374 6174 6963 600a   collectstatic`.
+00000ba0: 332e 2052 756e 206d 6967 7261 7465 0a60  3. Run migrate.`
+00000bb0: 7079 7468 6f6e 206d 616e 6167 652e 7079  python manage.py
+00000bc0: 206d 6967 7261 7465 600a 342e 2041 6464   migrate`.4. Add
+00000bd0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2073   the following s
+00000be0: 6574 7469 6e67 7320 746f 2079 6f75 7220  ettings to your 
+00000bf0: 6669 6c65 0a0a 2020 2060 6060 7079 7468  file..   ```pyth
+00000c00: 6f6e 0a20 2020 2041 5554 4845 4e54 4943  on.    AUTHENTIC
+00000c10: 4154 494f 4e5f 4241 434b 454e 4453 203d  ATION_BACKENDS =
+00000c20: 205b 2770 6173 736b 6579 732e 6261 636b   ['passkeys.back
+00000c30: 656e 642e 5061 7373 6b65 794d 6f64 656c  end.PasskeyModel
+00000c40: 4261 636b 656e 6427 5d20 2320 4368 616e  Backend'] # Chan
+00000c50: 6765 2079 6f75 7220 6175 7468 656e 7469  ge your authenti
+00000c60: 6361 7469 6f6e 2062 6163 6b65 6e64 0a20  cation backend. 
+00000c70: 2020 2046 4944 4f5f 5345 5256 4552 5f49     FIDO_SERVER_I
+00000c80: 443d 226c 6f63 616c 686f 7374 2220 2020  D="localhost"   
+00000c90: 2020 2023 2053 6572 7665 7220 7270 2069     # Server rp i
+00000ca0: 6420 666f 7220 4649 444f 322c 2069 7420  d for FIDO2, it 
+00000cb0: 7468 6520 6675 6c6c 2064 6f6d 6169 6e20  the full domain 
+00000cc0: 6f66 2079 6f75 7220 7072 6f6a 6563 740a  of your project.
+00000cd0: 2020 2020 4649 444f 5f53 4552 5645 525f      FIDO_SERVER_
+00000ce0: 4e41 4d45 3d22 5465 7374 4170 7022 0a20  NAME="TestApp". 
+00000cf0: 2020 2069 6d70 6f72 7420 7061 7373 6b65     import passke
+00000d00: 7973 0a20 2020 204b 4559 5f41 5454 4143  ys.    KEY_ATTAC
+00000d10: 484d 454e 5420 3d20 4e6f 6e65 207c 2070  HMENT = None | p
+00000d20: 6173 736b 6579 732e 4174 7461 6368 6d65  asskeys.Attachme
+00000d30: 6e74 2e43 524f 5353 5f50 4c41 5446 4f52  nt.CROSS_PLATFOR
+00000d40: 4d20 7c20 7061 7373 6b65 7973 2e41 7474  M | passkeys.Att
+00000d50: 6163 686d 656e 742e 504c 4154 464f 524d  achment.PLATFORM
+00000d60: 0a20 2020 6060 600a 2020 202a 2a4e 6f74  .   ```.   **Not
+00000d70: 652a 2a3a 2053 7461 7274 696e 6720 7631  e**: Starting v1
+00000d80: 2e31 2c20 6046 4944 4f5f 5345 5256 4552  .1, `FIDO_SERVER
+00000d90: 5f49 4460 2061 6e64 2f6f 7220 6046 4944  _ID` and/or `FID
+00000da0: 4f5f 5345 5256 4552 5f4e 414d 4560 2063  O_SERVER_NAME` c
+00000db0: 616e 2062 6520 6120 6361 6c6c 6162 6c65  an be a callable
+00000dc0: 2074 6f20 7375 7070 6f72 7420 6d75 6c74   to support mult
+00000dd0: 692d 7465 6e61 6e74 7320 7765 6220 6170  i-tenants web ap
+00000de0: 706c 6963 6174 696f 6e73 2c20 7468 6520  plications, the 
+00000df0: 6072 6571 7565 7374 6020 6973 2070 6173  `request` is pas
+00000e00: 7365 6420 746f 2074 6865 2063 616c 6c65  sed to the calle
+00000e10: 6420 6675 6e63 7469 6f6e 2e0a 352e 2041  d function..5. A
+00000e20: 6464 2070 6173 736b 6579 7320 746f 2075  dd passkeys to u
+00000e30: 726c 732e 7079 0a20 2020 6060 6070 7974  rls.py.   ```pyt
+00000e40: 686f 6e20 0a0a 2020 2075 726c 735f 7061  hon ..   urls_pa
+00000e50: 7474 6572 6e73 3d20 5b0a 2020 2027 2e2e  tterns= [.   '..
+00000e60: 2e27 2c0a 2020 2075 726c 2872 275e 7061  .',.   url(r'^pa
+00000e70: 7373 6b65 7973 2f27 2c20 696e 636c 7564  sskeys/', includ
+00000e80: 6528 2770 6173 736b 6579 732e 7572 6c73  e('passkeys.urls
+00000e90: 2729 292c 0a20 2020 272e 2e2e 2e27 2c0a  ')),.   '....',.
+00000ea0: 2020 2020 5d0a 2020 2020 6060 600a 362e      ].    ```.6.
+00000eb0: 2054 6f20 6d61 7463 6820 7468 6520 6c6f   To match the lo
+00000ec0: 6f6b 2061 6e64 2066 6565 6c20 6f66 2079  ok and feel of y
+00000ed0: 6f75 7220 7072 6f6a 6563 742c 2050 6173  our project, Pas
+00000ee0: 736b 6579 7320 696e 636c 7564 6573 2060  skeys includes `
+00000ef0: 6261 7365 2e68 746d 6c60 2062 7574 2069  base.html` but i
+00000f00: 7420 6e65 6564 7320 626c 6f63 6b73 206e  t needs blocks n
+00000f10: 616d 6564 2060 6865 6164 6020 2620 6063  amed `head` & `c
+00000f20: 6f6e 7465 6e74 6020 746f 2061 6464 6564  ontent` to added
+00000f30: 2069 7473 2063 6f6e 7465 6e74 2074 6f20   its content to 
+00000f40: 6974 2e0a 2020 202a 2a4e 6f74 6573 3a2a  it..   **Notes:*
+00000f50: 2a20 0a20 2020 200a 2020 2020 312e 2059  * .    .    1. Y
+00000f60: 6f75 2063 616e 206f 7665 7272 6964 6520  ou can override 
+00000f70: 6050 6173 734b 6579 735f 6261 7365 2e68  `PassKeys_base.h
+00000f80: 746d 6c60 2077 6869 6368 2069 7320 7573  tml` which is us
+00000f90: 6564 2062 7920 6050 6173 736b 6579 732e  ed by `Passkeys.
+00000fa0: 6874 6d6c 6020 736f 2079 6f75 2063 616e  html` so you can
+00000fb0: 2063 6f6e 7472 6f6c 2074 6865 2073 7479   control the sty
+00000fc0: 6c69 6e67 2062 6574 7465 7220 616e 6420  ling better and 
+00000fd0: 6375 7272 656e 7420 6050 6173 736b 6579  current `Passkey
+00000fe0: 735f 6261 7365 2e68 746d 6c60 2065 7874  s_base.html` ext
+00000ff0: 656e 6473 2060 6261 7365 2e68 746d 6c60  ends `base.html`
+00001000: 0a20 2020 2031 2e20 4375 7272 656e 746c  .    1. Currentl
+00001010: 792c 2060 5061 7373 4b65 7973 5f62 6173  y, `PassKeys_bas
+00001020: 652e 6874 6d6c 6020 6e65 6564 7320 4a51  e.html` needs JQ
+00001030: 7565 7279 2061 6e64 2062 6f6f 7473 7472  uery and bootstr
+00001040: 6170 2e20 0a0a 372e 2053 6f6d 6577 6865  ap. ..7. Somewhe
+00001050: 7265 2069 6e20 796f 7572 2061 7070 2c20  re in your app, 
+00001060: 6164 6420 6120 6c69 6e6b 2074 6f20 2770  add a link to 'p
+00001070: 6173 736b 6579 733a 686f 6d65 270a 2020  asskeys:home'.  
+00001080: 2020 6060 603c 6c69 3e3c 6120 6872 6566    ```<li><a href
+00001090: 3d22 7b25 2075 726c 2027 7061 7373 6b65  ="{% url 'passke
+000010a0: 7973 3a68 6f6d 6527 2025 7d22 3e50 6173  ys:home' %}">Pas
+000010b0: 736b 6579 733c 2f61 3e20 3c2f 6c69 3e60  skeys</a> </li>`
+000010c0: 6060 0a38 2e20 496e 2079 6f75 7220 6c6f  ``.8. In your lo
+000010d0: 6769 6e20 7669 6577 2c20 6368 616e 6765  gin view, change
+000010e0: 2074 6865 2061 7574 6865 6e74 6963 6174   the authenticat
+000010f0: 6520 6361 6c6c 2074 6f20 696e 636c 7564  e call to includ
+00001100: 6520 7468 6520 7265 7175 6573 7420 6173  e the request as
+00001110: 2066 6f6c 6c6f 7773 0a20 2020 6060 6070   follows.   ```p
+00001120: 7974 686f 6e0a 2020 2020 7573 6572 3d61  ython.    user=a
+00001130: 7574 6865 6e74 6963 6174 6528 7265 7175  uthenticate(requ
+00001140: 6573 742c 2075 7365 726e 616d 653d 7265  est, username=re
+00001150: 7175 6573 742e 504f 5354 5b22 7573 6572  quest.POST["user
+00001160: 6e61 6d65 225d 2c70 6173 7377 6f72 643d  name"],password=
+00001170: 7265 7175 6573 742e 504f 5354 5b22 7061  request.POST["pa
+00001180: 7373 776f 7264 225d 290a 2020 2020 6060  ssword"]).    ``
+00001190: 600a 0a38 2e20 4669 6e61 6c6c 792c 2049  `..8. Finally, I
+000011a0: 6e20 796f 7572 2060 6c6f 6769 6e2e 6874  n your `login.ht
+000011b0: 6d6c 600a 2020 202a 2047 6976 6520 616e  ml`.   * Give an
+000011c0: 2069 6420 746f 2079 6f75 7220 6c6f 6769   id to your logi
+000011d0: 6e20 666f 726d 2065 2e67 2027 6c6f 6769  n form e.g 'logi
+000011e0: 6e46 6f72 6d27 2c20 7468 6520 6964 2073  nForm', the id s
+000011f0: 686f 756c 6420 6265 2070 726f 7669 6465  hould be provide
+00001200: 6420 7768 656e 2063 616c 6c69 6e67 2060  d when calling `
+00001210: 6175 7468 6e60 2066 756e 6374 696f 6e0a  authn` function.
+00001220: 2020 202a 2049 6e73 6964 6520 7468 6520     * Inside the 
+00001230: 666f 726d 2c20 6164 6420 0a20 2020 2020  form, add .     
+00001240: 6060 6068 746d 6c0a 2020 2020 2020 3c69  ```html.      <i
+00001250: 6e70 7574 2074 7970 653d 2268 6964 6465  nput type="hidde
+00001260: 6e22 206e 616d 653d 2270 6173 736b 6579  n" name="passkey
+00001270: 7322 2069 643d 2270 6173 736b 6579 7322  s" id="passkeys"
+00001280: 2f3e 0a20 2020 2020 203c 6275 7474 6f6e  />.      <button
+00001290: 2063 6c61 7373 3d22 6274 6e20 6274 6e2d   class="btn btn-
+000012a0: 626c 6f63 6b20 6274 6e2d 6461 726b 2220  block btn-dark" 
+000012b0: 7479 7065 3d22 6275 7474 6f6e 2220 6f6e  type="button" on
+000012c0: 636c 6963 6b3d 2261 7574 686e 2827 6c6f  click="authn('lo
+000012d0: 6769 6e46 6f72 6d27 2922 3e3c 696d 6720  ginForm')"><img 
+000012e0: 7372 633d 227b 2520 7374 6174 6963 2027  src="{% static '
+000012f0: 7061 7373 6b65 7973 2f69 6d67 732f 4649  passkeys/imgs/FI
+00001300: 444f 2d50 6173 736b 6579 5f49 636f 6e2d  DO-Passkey_Icon-
+00001310: 5768 6974 652e 706e 6727 2025 7d22 2073  White.png' %}" s
+00001320: 7479 6c65 3d22 7769 6474 683a 2032 3470  tyle="width: 24p
+00001330: 7822 3e0a 2020 2020 207b 2569 6e63 6c75  x">.     {%inclu
+00001340: 6465 2027 7061 7373 6b65 7973 2e6a 7327  de 'passkeys.js'
+00001350: 2025 7d0a 2020 2020 2060 6060 0a46 6f72   %}.     ```.For
+00001360: 2045 7861 6d70 6c65 2c20 5365 6520 2765   Example, See 'e
+00001370: 7861 6d70 6c65 2720 6170 7020 616e 6420  xample' app and 
+00001380: 6c6f 6f6b 2061 7420 4558 414d 504c 452e  look at EXAMPLE.
+00001390: 6d64 2074 6f20 7365 6520 686f 7720 746f  md to see how to
+000013a0: 2073 6574 2069 7420 7570 2e0a 0a23 2044   set it up...# D
+000013b0: 6574 6563 7420 6966 2075 7365 7220 6973  etect if user is
+000013c0: 2075 7369 6e67 2070 6173 736b 6579 730a   using passkeys.
+000013d0: 4f6e 6365 2074 6865 2062 6163 6b65 6e64  Once the backend
+000013e0: 2069 7320 7573 6564 2c20 7468 6572 6520   is used, there 
+000013f0: 7769 6c6c 2062 6520 6120 6070 6173 736b  will be a `passk
+00001400: 6579 6020 6b65 7920 696e 2072 6571 7565  ey` key in reque
+00001410: 7374 2e73 6573 7369 6f6e 2e20 0a49 6620  st.session. .If 
+00001420: 7468 6520 7573 6572 2075 7365 6420 6120  the user used a 
+00001430: 7061 7373 6b65 7920 7468 656e 2060 7265  passkey then `re
+00001440: 7175 6573 742e 7365 7373 696f 6e5b 2770  quest.session['p
+00001450: 6173 736b 6579 275d 5b27 7061 7373 6b65  asskey']['passke
+00001460: 7927 5d60 2077 696c 6c20 6265 2054 7275  y']` will be Tru
+00001470: 6520 616e 6420 7468 6520 6b65 7920 696e  e and the key in
+00001480: 666f 726d 6174 696f 6e20 7769 6c6c 2062  formation will b
+00001490: 6520 7468 6572 6520 6c69 6b65 2074 6869  e there like thi
+000014a0: 730a 6060 6070 7974 686f 6e0a 7b27 7061  s.```python.{'pa
+000014b0: 7373 6b65 7927 3a20 5472 7565 2c20 276e  sskey': True, 'n
+000014c0: 616d 6527 3a20 2743 6872 6f6d 6527 2c20  ame': 'Chrome', 
+000014d0: 2769 6427 3a20 322c 2027 706c 6174 666f  'id': 2, 'platfo
+000014e0: 726d 273a 2027 4368 726f 6d65 206f 6e20  rm': 'Chrome on 
+000014f0: 4170 706c 6527 2c20 2763 726f 7373 5f70  Apple', 'cross_p
+00001500: 6c61 7466 6f72 6d27 3a20 4661 6c73 657d  latform': False}
+00001510: 0a60 6060 0a60 6372 6f73 735f 706c 6174  .```.`cross_plat
+00001520: 666f 726d 603a 206d 6561 6e73 2074 6861  form`: means tha
+00001530: 7420 7468 6520 7573 6572 2075 7365 6420  t the user used 
+00001540: 6120 6b65 7920 6672 6f6d 2061 6e6f 7468  a key from anoth
+00001550: 6572 2070 6c61 7466 6f72 6d20 736f 2074  er platform so t
+00001560: 6865 7265 2069 7320 6e6f 206b 6579 206c  here is no key l
+00001570: 6f63 616c 2074 6f20 7468 6520 6465 7669  ocal to the devi
+00001580: 6365 2075 7365 6420 746f 206c 6f67 696e  ce used to login
+00001590: 2065 2e67 2075 7365 6420 616e 2041 6e64   e.g used an And
+000015a0: 726f 6964 2070 686f 6e65 206f 6e20 4d61  roid phone on Ma
+000015b0: 6320 4f53 2058 206f 7220 6950 6164 2e0a  c OS X or iPad..
+000015c0: 4966 2074 6865 2075 7365 7220 6469 646e  If the user didn
+000015d0: 2774 2075 7365 2061 2070 6173 736b 6579  't use a passkey
+000015e0: 2074 6865 6e20 6974 2077 696c 6c20 6265   then it will be
+000015f0: 2073 6574 2074 6f20 4661 6c73 650a 6060   set to False.``
+00001600: 6070 7974 686f 6e0a 7b27 7061 7373 6b65  `python.{'passke
+00001610: 7927 3a46 616c 7365 7d0a 6060 600a 0a0a  y':False}.```...
+00001620: 2320 4368 6563 6b20 6966 2074 6865 2075  # Check if the u
+00001630: 7365 7220 6361 6e20 6265 2065 6e72 6f6c  ser can be enrol
+00001640: 6c65 6420 666f 7220 6120 706c 6174 666f  led for a platfo
+00001650: 726d 2061 7574 6865 6e74 6963 6174 6f72  rm authenticator
+00001660: 0a0a 4966 2079 6f75 2077 616e 7420 746f  ..If you want to
+00001670: 2063 6865 636b 2069 6620 7468 6520 7573   check if the us
+00001680: 6572 2063 616e 2062 6520 656e 726f 6c6c  er can be enroll
+00001690: 6564 2074 6f20 7573 6520 6120 706c 6174  ed to use a plat
+000016a0: 666f 726d 2061 7574 6865 6e74 6963 6174  form authenticat
+000016b0: 6f72 2c20 796f 7520 6361 6e20 646f 2074  or, you can do t
+000016c0: 6865 2066 6f6c 6c6f 7769 6e67 2069 6e20  he following in 
+000016d0: 796f 7572 206d 6169 6e20 7061 6765 2e0a  your main page..
+000016e0: 0a60 6060 6874 6d6c 0a3c 6469 7620 6964  .```html.<div id
+000016f0: 3d22 706b 2220 636c 6173 733d 2261 6c65  ="pk" class="ale
+00001700: 7274 2061 6c65 7274 2d69 6e66 6f22 2073  rt alert-info" s
+00001710: 7479 6c65 3d22 6469 7370 6c61 793a 206e  tyle="display: n
+00001720: 6f6e 6522 3e59 6f75 7220 6465 7669 6365  one">Your device
+00001730: 2073 7570 706f 7274 7320 7061 7373 6b65   supports passke
+00001740: 7973 2c20 3c61 2068 7265 663d 227b 2575  ys, <a href="{%u
+00001750: 726c 2027 7061 7373 6b65 7973 3a65 6e72  rl 'passkeys:enr
+00001760: 6f6c 6c27 257d 223e 456e 726f 6c6c 3c2f  oll'%}">Enroll</
+00001770: 613e 203c 2f64 6976 3e0a 3c73 6372 6970  a> </div>.<scrip
+00001780: 7420 7479 7065 3d22 7465 7874 2f6a 6176  t type="text/jav
+00001790: 6173 6372 6970 7422 3e0a 6675 6e63 7469  ascript">.functi
+000017a0: 6f6e 2072 6567 6973 7465 725f 706b 2829  on register_pk()
+000017b0: 0a20 2020 207b 0a20 2020 2020 2020 2024  .    {.        $
+000017c0: 2827 2370 6b27 292e 7368 6f77 2829 3b0a  ('#pk').show();.
+000017d0: 2020 2020 7d0a 7b25 2069 6e63 6c75 6465      }.{% include
+000017e0: 2027 6368 6563 6b5f 7061 7373 6b65 7973   'check_passkeys
+000017f0: 2e6a 7327 257d 0a24 2864 6f63 756d 656e  .js'%}.$(documen
+00001800: 7429 2e72 6561 6479 2863 6865 636b 5f70  t).ready(check_p
+00001810: 6173 736b 6579 2874 7275 652c 7265 6769  asskey(true,regi
+00001820: 7374 6572 5f70 6b29 290a 3c2f 7363 7269  ster_pk)).</scri
+00001830: 7074 3e0a 6060 600a 6368 6563 6b5f 7061  pt>.```.check_pa
+00001840: 7373 6b65 7920 6675 6e63 7469 6f6e 2070  sskey function p
+00001850: 6172 616d 7465 7273 2061 7265 2061 7320  aramters are as 
+00001860: 666f 6c6c 6f77 7320 0a2a 2060 706c 6174  follows .* `plat
+00001870: 666f 726d 5f61 7574 6865 6e74 6963 6174  form_authenticat
+00001880: 6f72 603a 2069 6620 7468 6520 7365 7276  or`: if the serv
+00001890: 6963 6520 7265 7175 6972 6573 206f 6e6c  ice requires onl
+000018a0: 7920 6120 706c 6174 666f 726d 2061 7574  y a platform aut
+000018b0: 6865 6e74 6963 6174 6f72 2028 652e 6720  henticator (e.g 
+000018c0: 546f 7563 6849 442c 2057 696e 646f 7773  TouchID, Windows
+000018d0: 2048 656c 6c6f 206f 7220 416e 6472 6f69   Hello or Androi
+000018e0: 6420 5361 6665 7479 4e65 7429 0a2a 2060  d SafetyNet).* `
+000018f0: 7375 6363 6573 735f 6675 6e63 603a 2066  success_func`: f
+00001900: 756e 6374 696f 6e20 746f 2063 616c 6c20  unction to call 
+00001910: 6966 2061 2070 6c61 7466 6f72 6d20 6175  if a platform au
+00001920: 7468 656e 7469 6361 746f 7220 6973 2066  thenticator is f
+00001930: 6f75 6e64 206f 7220 6966 2074 6865 2075  ound or if the u
+00001940: 7365 7220 6469 646e 2774 206c 6f67 696e  ser didn't login
+00001950: 2062 7920 6120 7061 7373 6b65 790a 2a20   by a passkey.* 
+00001960: 6066 6169 6c5f 6675 6e63 603a 2066 756e  `fail_func`: fun
+00001970: 6374 696f 6e20 746f 2063 616c 6c20 6966  ction to call if
+00001980: 206e 6f20 706c 6174 666f 726d 2061 7574   no platform aut
+00001990: 6865 6e74 6963 6174 6f72 2069 7320 666f  henticator is fo
+000019a0: 756e 6420 286f 7074 696f 6e61 6c29 2e0a  und (optional)..
+000019b0: 0a0a 2323 2055 7369 6e67 2043 6f6e 6469  ..## Using Condi
+000019c0: 7469 6f6e 616c 2055 490a 0a43 6f6e 6469  tional UI..Condi
+000019d0: 7469 6f6e 616c 2055 4920 6973 2061 2077  tional UI is a w
+000019e0: 6179 2066 6f72 2074 6865 2062 726f 7773  ay for the brows
+000019f0: 6572 2074 6f20 7072 6f6d 7074 2074 6865  er to prompt the
+00001a00: 2075 7365 7220 746f 2075 7365 2074 6865   user to use the
+00001a10: 2070 6173 736b 6579 2074 6f20 6c6f 6769   passkey to logi
+00001a20: 6e20 746f 2074 6865 2073 7973 7465 6d20  n to the system 
+00001a30: 6173 2073 686f 776e 2069 6e20 0a0a 215b  as shown in ..![
+00001a40: 636f 6e64 6974 696f 6e61 6c55 492e 706e  conditionalUI.pn
+00001a50: 675d 2869 6d67 7325 3246 636f 6e64 6974  g](imgs%2Fcondit
+00001a60: 696f 6e61 6c55 492e 706e 6729 0a0a 5374  ionalUI.png)..St
+00001a70: 6172 7469 6e67 2076 6572 7369 6f6e 2076  arting version v
+00001a80: 312e 322e 2079 6f75 2063 616e 2075 7365  1.2. you can use
+00001a90: 2043 6f6e 6469 7469 6f6e 616c 2055 4920   Conditional UI 
+00001aa0: 6279 2061 6464 696e 6720 7468 6520 666f  by adding the fo
+00001ab0: 6c6c 6f77 696e 6720 746f 2079 6f75 7220  llowing to your 
+00001ac0: 6c6f 6769 6e20 7061 6765 0a0a 312e 2041  login page..1. A
+00001ad0: 6464 2060 7765 6261 7574 686e 6020 746f  dd `webauthn` to
+00001ae0: 2061 7574 6f63 6f6d 706c 6574 6520 6f66   autocomplete of
+00001af0: 2074 6865 2075 7365 726e 616d 6520 6669   the username fi
+00001b00: 656c 6420 6173 2073 686f 776e 2062 656c  eld as shown bel
+00001b10: 6f77 2e0a 6060 6068 746d 6c0a 3c69 6e70  ow..```html.<inp
+00001b20: 7574 206e 616d 653d 2275 7365 726e 616d  ut name="usernam
+00001b30: 6522 2070 6c61 6365 686f 6c64 6572 3d22  e" placeholder="
+00001b40: 7573 6572 6e61 6d65 2220 6175 746f 636f  username" autoco
+00001b50: 6d70 6c65 7465 3d22 7573 6572 6e61 6d65  mplete="username
+00001b60: 2077 6562 6175 7468 6e22 3e0a 6060 600a   webauthn">.```.
+00001b70: 6164 6420 7468 6520 666f 6c6c 6f77 696e  add the followin
+00001b80: 6720 746f 2074 6865 2070 6167 6520 6a73  g to the page js
+00001b90: 2e0a 0a60 6060 6a73 0a77 696e 646f 772e  ...```js.window.
+00001ba0: 6f6e 6c6f 6164 203d 2063 6865 636b 436f  onload = checkCo
+00001bb0: 6e64 6974 696f 6e61 6c55 4928 276c 6f67  nditionalUI('log
+00001bc0: 696e 466f 726d 2729 3b0a 6060 600a 7768  inForm');.```.wh
+00001bd0: 6572 6520 606c 6f67 696e 466f 726d 6020  ere `loginForm` 
+00001be0: 6973 206e 616d 6520 6f66 2079 6f75 7220  is name of your 
+00001bf0: 6c6f 6769 6e20 666f 726d 2e0a 0a23 2320  login form...## 
+00001c00: 5365 6375 7269 7479 2063 6f6e 7461 6374  Security contact
+00001c10: 2069 6e66 6f72 6d61 7469 6f6e 0a0a 546f   information..To
+00001c20: 2072 6570 6f72 7420 6120 7365 6375 7269   report a securi
+00001c30: 7479 2076 756c 6e65 7261 6269 6c69 7479  ty vulnerability
+00001c40: 2c20 706c 6561 7365 2075 7365 2074 6865  , please use the
+00001c50: 0a5b 5469 6465 6c69 6674 2073 6563 7572  .[Tidelift secur
+00001c60: 6974 7920 636f 6e74 6163 745d 2868 7474  ity contact](htt
+00001c70: 7073 3a2f 2f74 6964 656c 6966 742e 636f  ps://tidelift.co
+00001c80: 6d2f 7365 6375 7269 7479 292e 0a54 6964  m/security)..Tid
+00001c90: 656c 6966 7420 7769 6c6c 2063 6f6f 7264  elift will coord
+00001ca0: 696e 6174 6520 7468 6520 6669 7820 616e  inate the fix an
+00001cb0: 6420 6469 7363 6c6f 7375 7265 2e0a 0a23  d disclosure...#
+00001cc0: 2043 6f6e 7472 6962 7574 6f72 730a 2a20   Contributors.* 
+00001cd0: 5b6d 6168 6d6f 6f64 6e61 7372 5d28 6874  [mahmoodnasr](ht
+00001ce0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001cf0: 2f6d 6168 6d6f 6f64 6e61 7372 290a 2a20  /mahmoodnasr).* 
+00001d00: 5b6a 6163 6f70 7364 5d28 6874 7470 733a  [jacopsd](https:
+00001d10: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6163  //github.com/jac
+00001d20: 6f70 7364 2920 2020 0a2a 205b 6761 7370  opsd)   .* [gasp
+00001d30: 6172 6272 6f67 7565 6972 615d 2868 7474  arbrogueira](htt
+00001d40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001d50: 6761 7370 6172 6272 6f67 7565 6972 6129  gasparbrogueira)
+00001d60: 0a0a 0a0a 0a                             .....
```

### Comparing `django-passkeys-1.2.2/README.md` & `django-passkeys-1.2.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # django-passkeys
 
 [![PyPI version](https://badge.fury.io/py/django-passkeys.svg)](https://badge.fury.io/py/django-passkeys)
-[![Downloads](https://pepy.tech/badge/django-passkeys/month)](https://pepy.tech/project/django-passkeys)
-![Coverage](coverage.svg)
+[![Downloads](https://static.pepy.tech/badge/django-passkeys)](https://pepy.tech/project/django-passkeys)
+[![Downloads / Month ](https://pepy.tech/badge/django-passkeys/month)](https://pepy.tech/project/django-passkeys)
+[![build](https://github.com/mkalioby/django-passkeys/actions/workflows/basic_checks.yml/badge.svg)](https://github.com/mkalioby/django-passkeys/actions/workflows/basic_checks.yml)
+![Coverage](https://raw.githubusercontent.com/mkalioby/django-passkeys/main/coverage.svg)
 
 An extension to Django *ModelBackend* backend to support passkeys.
 
 Passkeys is an extension to Web Authentication API that will allow the user to login to a service using another device.
 
 This app is a slim-down version of [django-mfa2](https://github.com/mkalioby/django-mfa2)
```

#### html2text {}

```diff
@@ -1,11 +1,16 @@
 # django-passkeys [![PyPI version](https://badge.fury.io/py/django-
 passkeys.svg)](https://badge.fury.io/py/django-passkeys) [![Downloads](https://
-pepy.tech/badge/django-passkeys/month)](https://pepy.tech/project/django-
-passkeys) ![Coverage](coverage.svg) An extension to Django *ModelBackend*
+static.pepy.tech/badge/django-passkeys)](https://pepy.tech/project/django-
+passkeys) [![Downloads / Month ](https://pepy.tech/badge/django-passkeys/
+month)](https://pepy.tech/project/django-passkeys) [![build](https://
+github.com/mkalioby/django-passkeys/actions/workflows/basic_checks.yml/
+badge.svg)](https://github.com/mkalioby/django-passkeys/actions/workflows/
+basic_checks.yml) ![Coverage](https://raw.githubusercontent.com/mkalioby/
+django-passkeys/main/coverage.svg) An extension to Django *ModelBackend*
 backend to support passkeys. Passkeys is an extension to Web Authentication API
 that will allow the user to login to a service using another device. This app
 is a slim-down version of [django-mfa2](https://github.com/mkalioby/django-
 mfa2) Passkeys are now supported on * Apple Ecosystem (iPhone 16.0+, iPadOS
 16.1, Mac OS X Ventura) * Chromium based browsers (on PC and Laptop) allows
 picking up credentials from Android and iPhone/iPadOS. * Android Credentials
 creation for ResidentKeys is currently in live now. On May 3, 2023, Google
```

### Comparing `django-passkeys-1.2.2/django_passkeys.egg-info/PKG-INFO` & `django-passkeys-1.2.3/django_passkeys.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 616e  : 2.1.Name: djan
 00000020: 676f 2d70 6173 736b 6579 730a 5665 7273  go-passkeys.Vers
-00000030: 696f 6e3a 2031 2e32 2e32 0a53 756d 6d61  ion: 1.2.2.Summa
+00000030: 696f 6e3a 2031 2e32 2e33 0a53 756d 6d61  ion: 1.2.3.Summa
 00000040: 7279 3a20 4120 446a 616e 676f 2041 7574  ry: A Django Aut
 00000050: 6865 6e74 6963 6174 696f 6e20 4261 636b  hentication Back
 00000060: 656e 6420 666f 7220 5061 7373 6b65 7973  end for Passkeys
 00000070: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
 00000080: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
 00000090: 6b61 6c69 6f62 792f 646a 616e 676f 2d70  kalioby/django-p
 000000a0: 6173 736b 6579 730a 446f 776e 6c6f 6164  asskeys.Download
@@ -89,360 +89,383 @@
 00000580: 696f 6e5d 2868 7474 7073 3a2f 2f62 6164  ion](https://bad
 00000590: 6765 2e66 7572 792e 696f 2f70 792f 646a  ge.fury.io/py/dj
 000005a0: 616e 676f 2d70 6173 736b 6579 732e 7376  ango-passkeys.sv
 000005b0: 6729 5d28 6874 7470 733a 2f2f 6261 6467  g)](https://badg
 000005c0: 652e 6675 7279 2e69 6f2f 7079 2f64 6a61  e.fury.io/py/dja
 000005d0: 6e67 6f2d 7061 7373 6b65 7973 290a 5b21  ngo-passkeys).[!
 000005e0: 5b44 6f77 6e6c 6f61 6473 5d28 6874 7470  [Downloads](http
-000005f0: 733a 2f2f 7065 7079 2e74 6563 682f 6261  s://pepy.tech/ba
-00000600: 6467 652f 646a 616e 676f 2d70 6173 736b  dge/django-passk
-00000610: 6579 732f 6d6f 6e74 6829 5d28 6874 7470  eys/month)](http
-00000620: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
-00000630: 6f6a 6563 742f 646a 616e 676f 2d70 6173  oject/django-pas
-00000640: 736b 6579 7329 0a21 5b43 6f76 6572 6167  skeys).![Coverag
-00000650: 655d 2863 6f76 6572 6167 652e 7376 6729  e](coverage.svg)
-00000660: 0a0a 416e 2065 7874 656e 7369 6f6e 2074  ..An extension t
-00000670: 6f20 446a 616e 676f 202a 4d6f 6465 6c42  o Django *ModelB
-00000680: 6163 6b65 6e64 2a20 6261 636b 656e 6420  ackend* backend 
-00000690: 746f 2073 7570 706f 7274 2070 6173 736b  to support passk
-000006a0: 6579 732e 0a0a 5061 7373 6b65 7973 2069  eys...Passkeys i
-000006b0: 7320 616e 2065 7874 656e 7369 6f6e 2074  s an extension t
-000006c0: 6f20 5765 6220 4175 7468 656e 7469 6361  o Web Authentica
-000006d0: 7469 6f6e 2041 5049 2074 6861 7420 7769  tion API that wi
-000006e0: 6c6c 2061 6c6c 6f77 2074 6865 2075 7365  ll allow the use
-000006f0: 7220 746f 206c 6f67 696e 2074 6f20 6120  r to login to a 
-00000700: 7365 7276 6963 6520 7573 696e 6720 616e  service using an
-00000710: 6f74 6865 7220 6465 7669 6365 2e0a 0a54  other device...T
-00000720: 6869 7320 6170 7020 6973 2061 2073 6c69  his app is a sli
-00000730: 6d2d 646f 776e 2076 6572 7369 6f6e 206f  m-down version o
-00000740: 6620 5b64 6a61 6e67 6f2d 6d66 6132 5d28  f [django-mfa2](
-00000750: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000760: 6f6d 2f6d 6b61 6c69 6f62 792f 646a 616e  om/mkalioby/djan
-00000770: 676f 2d6d 6661 3229 0a0a 5061 7373 6b65  go-mfa2)..Passke
-00000780: 7973 2061 7265 206e 6f77 2073 7570 706f  ys are now suppo
-00000790: 7274 6564 206f 6e20 0a2a 2041 7070 6c65  rted on .* Apple
-000007a0: 2045 636f 7379 7374 656d 2028 6950 686f   Ecosystem (iPho
-000007b0: 6e65 2031 362e 302b 2c20 6950 6164 4f53  ne 16.0+, iPadOS
-000007c0: 2031 362e 312c 204d 6163 204f 5320 5820   16.1, Mac OS X 
-000007d0: 5665 6e74 7572 6129 0a2a 2043 6872 6f6d  Ventura).* Chrom
-000007e0: 6975 6d20 6261 7365 6420 6272 6f77 7365  ium based browse
-000007f0: 7273 2028 6f6e 2050 4320 616e 6420 4c61  rs (on PC and La
-00000800: 7074 6f70 2920 616c 6c6f 7773 2070 6963  ptop) allows pic
-00000810: 6b69 6e67 2075 7020 6372 6564 656e 7469  king up credenti
-00000820: 616c 7320 6672 6f6d 2041 6e64 726f 6964  als from Android
-00000830: 2061 6e64 2069 5068 6f6e 652f 6950 6164   and iPhone/iPad
-00000840: 4f53 2e0a 2a20 416e 6472 6f69 6420 4372  OS..* Android Cr
-00000850: 6564 656e 7469 616c 7320 6372 6561 7469  edentials creati
-00000860: 6f6e 2066 6f72 2052 6573 6964 656e 744b  on for ResidentK
-00000870: 6579 7320 6973 2063 7572 7265 6e74 6c79  eys is currently
-00000880: 2069 6e20 6c69 7665 206e 6f77 2e0a 0a4f   in live now...O
-00000890: 6e20 4d61 7920 332c 2032 3032 332c 2047  n May 3, 2023, G
-000008a0: 6f6f 676c 6520 616c 6c6f 7765 6420 7468  oogle allowed th
-000008b0: 6520 7573 6520 6f66 2050 6173 736b 6579  e use of Passkey
-000008c0: 7320 666f 7220 7468 6520 7573 6572 7320  s for the users 
-000008d0: 746f 206c 6f67 696e 2c20 6b69 6c6c 696e  to login, killin
-000008e0: 6720 7468 6520 7061 7373 776f 7264 2066  g the password f
-000008f0: 6f72 2065 6e72 6f6c 6c65 6420 7573 6572  or enrolled user
-00000900: 732e 200a 0a23 2049 6e73 7461 6c6c 6174  s. ..# Installat
-00000910: 696f 6e0a 0a60 7069 7020 696e 7374 616c  ion..`pip instal
-00000920: 6c20 646a 616e 676f 2d70 6173 736b 6579  l django-passkey
-00000930: 7360 0a0a 4375 7272 656e 746c 792c 2069  s`..Currently, i
-00000940: 7420 7375 7070 6f72 7420 446a 616e 676f  t support Django
-00000950: 2032 2e30 2b2c 2050 7974 686f 6e20 332e   2.0+, Python 3.
-00000960: 372b 0a0a 2320 5573 6167 650a 312e 2069  7+..# Usage.1. i
-00000970: 6e20 796f 7572 2073 6574 7469 6e67 732e  n your settings.
-00000980: 7079 2061 6464 2074 6865 2061 7070 6c69  py add the appli
-00000990: 6361 7469 6f6e 2074 6f20 796f 7572 2069  cation to your i
-000009a0: 6e73 7461 6c6c 6564 2061 7070 730a 2020  nstalled apps.  
-000009b0: 2060 6060 7079 7468 6f6e 0a20 2020 494e   ```python.   IN
-000009c0: 5354 414c 4c45 445f 4150 5053 3d28 0a20  STALLED_APPS=(. 
-000009d0: 2020 272e 2e2e 2e2e 2e27 2c0a 2020 2027    '......',.   '
-000009e0: 7061 7373 6b65 7973 272c 0a20 2020 272e  passkeys',.   '.
-000009f0: 2e2e 2e2e 2e27 290a 2020 2060 6060 0a32  .....').   ```.2
-00000a00: 2e20 436f 6c6c 6563 7420 5374 6174 6963  . Collect Static
-00000a10: 2046 696c 6573 0a60 7079 7468 6f6e 206d   Files.`python m
-00000a20: 616e 6167 652e 7079 2063 6f6c 6c65 6374  anage.py collect
-00000a30: 7374 6174 6963 600a 332e 2052 756e 206d  static`.3. Run m
-00000a40: 6967 7261 7465 0a60 7079 7468 6f6e 206d  igrate.`python m
-00000a50: 616e 6167 652e 7079 206d 6967 7261 7465  anage.py migrate
-00000a60: 600a 342e 2041 6464 2074 6865 2066 6f6c  `.4. Add the fol
-00000a70: 6c6f 7769 6e67 2073 6574 7469 6e67 7320  lowing settings 
-00000a80: 746f 2079 6f75 7220 6669 6c65 0a0a 2020  to your file..  
-00000a90: 2060 6060 7079 7468 6f6e 0a20 2020 2041   ```python.    A
-00000aa0: 5554 4845 4e54 4943 4154 494f 4e5f 4241  UTHENTICATION_BA
-00000ab0: 434b 454e 4453 203d 205b 2770 6173 736b  CKENDS = ['passk
-00000ac0: 6579 732e 6261 636b 656e 642e 5061 7373  eys.backend.Pass
-00000ad0: 6b65 794d 6f64 656c 4261 636b 656e 6427  keyModelBackend'
-00000ae0: 5d20 2320 4368 616e 6765 2079 6f75 7220  ] # Change your 
-00000af0: 6175 7468 656e 7469 6361 7469 6f6e 2062  authentication b
-00000b00: 6163 6b65 6e64 0a20 2020 2046 4944 4f5f  ackend.    FIDO_
-00000b10: 5345 5256 4552 5f49 443d 226c 6f63 616c  SERVER_ID="local
-00000b20: 686f 7374 2220 2020 2020 2023 2053 6572  host"      # Ser
-00000b30: 7665 7220 7270 2069 6420 666f 7220 4649  ver rp id for FI
-00000b40: 444f 322c 2069 7420 7468 6520 6675 6c6c  DO2, it the full
-00000b50: 2064 6f6d 6169 6e20 6f66 2079 6f75 7220   domain of your 
-00000b60: 7072 6f6a 6563 740a 2020 2020 4649 444f  project.    FIDO
-00000b70: 5f53 4552 5645 525f 4e41 4d45 3d22 5465  _SERVER_NAME="Te
-00000b80: 7374 4170 7022 0a20 2020 2069 6d70 6f72  stApp".    impor
-00000b90: 7420 7061 7373 6b65 7973 0a20 2020 204b  t passkeys.    K
-00000ba0: 4559 5f41 5454 4143 484d 454e 5420 3d20  EY_ATTACHMENT = 
-00000bb0: 4e6f 6e65 207c 2070 6173 736b 6579 732e  None | passkeys.
-00000bc0: 4174 7461 6368 6d65 6e74 2e43 524f 5353  Attachment.CROSS
-00000bd0: 5f50 4c41 5446 4f52 4d20 7c20 7061 7373  _PLATFORM | pass
-00000be0: 6b65 7973 2e41 7474 6163 686d 656e 742e  keys.Attachment.
-00000bf0: 504c 4154 464f 524d 0a20 2020 6060 600a  PLATFORM.   ```.
-00000c00: 2020 202a 2a4e 6f74 652a 2a3a 2053 7461     **Note**: Sta
-00000c10: 7274 696e 6720 7631 2e31 2c20 6046 4944  rting v1.1, `FID
-00000c20: 4f5f 5345 5256 4552 5f49 4460 2061 6e64  O_SERVER_ID` and
-00000c30: 2f6f 7220 6046 4944 4f5f 5345 5256 4552  /or `FIDO_SERVER
-00000c40: 5f4e 414d 4560 2063 616e 2062 6520 6120  _NAME` can be a 
-00000c50: 6361 6c6c 6162 6c65 2074 6f20 7375 7070  callable to supp
-00000c60: 6f72 7420 6d75 6c74 692d 7465 6e61 6e74  ort multi-tenant
-00000c70: 7320 7765 6220 6170 706c 6963 6174 696f  s web applicatio
-00000c80: 6e73 2c20 7468 6520 6072 6571 7565 7374  ns, the `request
-00000c90: 6020 6973 2070 6173 7365 6420 746f 2074  ` is passed to t
-00000ca0: 6865 2063 616c 6c65 6420 6675 6e63 7469  he called functi
-00000cb0: 6f6e 2e0a 352e 2041 6464 2070 6173 736b  on..5. Add passk
-00000cc0: 6579 7320 746f 2075 726c 732e 7079 0a20  eys to urls.py. 
-00000cd0: 2020 6060 6070 7974 686f 6e20 0a0a 2020    ```python ..  
-00000ce0: 2075 726c 735f 7061 7474 6572 6e73 3d20   urls_patterns= 
-00000cf0: 5b0a 2020 2027 2e2e 2e27 2c0a 2020 2075  [.   '...',.   u
-00000d00: 726c 2872 275e 7061 7373 6b65 7973 2f27  rl(r'^passkeys/'
-00000d10: 2c20 696e 636c 7564 6528 2770 6173 736b  , include('passk
-00000d20: 6579 732e 7572 6c73 2729 292c 0a20 2020  eys.urls')),.   
-00000d30: 272e 2e2e 2e27 2c0a 2020 2020 5d0a 2020  '....',.    ].  
-00000d40: 2020 6060 600a 362e 2054 6f20 6d61 7463    ```.6. To matc
-00000d50: 6820 7468 6520 6c6f 6f6b 2061 6e64 2066  h the look and f
-00000d60: 6565 6c20 6f66 2079 6f75 7220 7072 6f6a  eel of your proj
-00000d70: 6563 742c 2050 6173 736b 6579 7320 696e  ect, Passkeys in
-00000d80: 636c 7564 6573 2060 6261 7365 2e68 746d  cludes `base.htm
-00000d90: 6c60 2062 7574 2069 7420 6e65 6564 7320  l` but it needs 
-00000da0: 626c 6f63 6b73 206e 616d 6564 2060 6865  blocks named `he
-00000db0: 6164 6020 2620 6063 6f6e 7465 6e74 6020  ad` & `content` 
-00000dc0: 746f 2061 6464 6564 2069 7473 2063 6f6e  to added its con
-00000dd0: 7465 6e74 2074 6f20 6974 2e0a 2020 202a  tent to it..   *
-00000de0: 2a4e 6f74 6573 3a2a 2a20 0a20 2020 200a  *Notes:** .    .
-00000df0: 2020 2020 312e 2059 6f75 2063 616e 206f      1. You can o
-00000e00: 7665 7272 6964 6520 6050 6173 734b 6579  verride `PassKey
-00000e10: 735f 6261 7365 2e68 746d 6c60 2077 6869  s_base.html` whi
-00000e20: 6368 2069 7320 7573 6564 2062 7920 6050  ch is used by `P
-00000e30: 6173 736b 6579 732e 6874 6d6c 6020 736f  asskeys.html` so
-00000e40: 2079 6f75 2063 616e 2063 6f6e 7472 6f6c   you can control
-00000e50: 2074 6865 2073 7479 6c69 6e67 2062 6574   the styling bet
-00000e60: 7465 7220 616e 6420 6375 7272 656e 7420  ter and current 
-00000e70: 6050 6173 736b 6579 735f 6261 7365 2e68  `Passkeys_base.h
-00000e80: 746d 6c60 2065 7874 656e 6473 2060 6261  tml` extends `ba
-00000e90: 7365 2e68 746d 6c60 0a20 2020 2031 2e20  se.html`.    1. 
-00000ea0: 4375 7272 656e 746c 792c 2060 5061 7373  Currently, `Pass
-00000eb0: 4b65 7973 5f62 6173 652e 6874 6d6c 6020  Keys_base.html` 
-00000ec0: 6e65 6564 7320 4a51 7565 7279 2061 6e64  needs JQuery and
-00000ed0: 2062 6f6f 7473 7472 6170 2e20 0a0a 372e   bootstrap. ..7.
-00000ee0: 2053 6f6d 6577 6865 7265 2069 6e20 796f   Somewhere in yo
-00000ef0: 7572 2061 7070 2c20 6164 6420 6120 6c69  ur app, add a li
-00000f00: 6e6b 2074 6f20 2770 6173 736b 6579 733a  nk to 'passkeys:
-00000f10: 686f 6d65 270a 2020 2020 6060 603c 6c69  home'.    ```<li
-00000f20: 3e3c 6120 6872 6566 3d22 7b25 2075 726c  ><a href="{% url
-00000f30: 2027 7061 7373 6b65 7973 3a68 6f6d 6527   'passkeys:home'
-00000f40: 2025 7d22 3e50 6173 736b 6579 733c 2f61   %}">Passkeys</a
-00000f50: 3e20 3c2f 6c69 3e60 6060 0a38 2e20 496e  > </li>```.8. In
-00000f60: 2079 6f75 7220 6c6f 6769 6e20 7669 6577   your login view
-00000f70: 2c20 6368 616e 6765 2074 6865 2061 7574  , change the aut
-00000f80: 6865 6e74 6963 6174 6520 6361 6c6c 2074  henticate call t
-00000f90: 6f20 696e 636c 7564 6520 7468 6520 7265  o include the re
-00000fa0: 7175 6573 7420 6173 2066 6f6c 6c6f 7773  quest as follows
-00000fb0: 0a20 2020 6060 6070 7974 686f 6e0a 2020  .   ```python.  
-00000fc0: 2020 7573 6572 3d61 7574 6865 6e74 6963    user=authentic
-00000fd0: 6174 6528 7265 7175 6573 742c 2075 7365  ate(request, use
-00000fe0: 726e 616d 653d 7265 7175 6573 742e 504f  rname=request.PO
-00000ff0: 5354 5b22 7573 6572 6e61 6d65 225d 2c70  ST["username"],p
-00001000: 6173 7377 6f72 643d 7265 7175 6573 742e  assword=request.
-00001010: 504f 5354 5b22 7061 7373 776f 7264 225d  POST["password"]
-00001020: 290a 2020 2020 6060 600a 0a38 2e20 4669  ).    ```..8. Fi
-00001030: 6e61 6c6c 792c 2049 6e20 796f 7572 2060  nally, In your `
-00001040: 6c6f 6769 6e2e 6874 6d6c 600a 2020 202a  login.html`.   *
-00001050: 2047 6976 6520 616e 2069 6420 746f 2079   Give an id to y
-00001060: 6f75 7220 6c6f 6769 6e20 666f 726d 2065  our login form e
-00001070: 2e67 2027 6c6f 6769 6e46 6f72 6d27 2c20  .g 'loginForm', 
-00001080: 7468 6520 6964 2073 686f 756c 6420 6265  the id should be
-00001090: 2070 726f 7669 6465 6420 7768 656e 2063   provided when c
-000010a0: 616c 6c69 6e67 2060 6175 7468 6e60 2066  alling `authn` f
-000010b0: 756e 6374 696f 6e0a 2020 202a 2049 6e73  unction.   * Ins
-000010c0: 6964 6520 7468 6520 666f 726d 2c20 6164  ide the form, ad
-000010d0: 6420 0a20 2020 2020 6060 6068 746d 6c0a  d .     ```html.
-000010e0: 2020 2020 2020 3c69 6e70 7574 2074 7970        <input typ
-000010f0: 653d 2268 6964 6465 6e22 206e 616d 653d  e="hidden" name=
-00001100: 2270 6173 736b 6579 7322 2069 643d 2270  "passkeys" id="p
-00001110: 6173 736b 6579 7322 2f3e 0a20 2020 2020  asskeys"/>.     
-00001120: 203c 6275 7474 6f6e 2063 6c61 7373 3d22   <button class="
-00001130: 6274 6e20 6274 6e2d 626c 6f63 6b20 6274  btn btn-block bt
-00001140: 6e2d 6461 726b 2220 7479 7065 3d22 6275  n-dark" type="bu
-00001150: 7474 6f6e 2220 6f6e 636c 6963 6b3d 2261  tton" onclick="a
-00001160: 7574 686e 2827 6c6f 6769 6e46 6f72 6d27  uthn('loginForm'
-00001170: 2922 3e3c 696d 6720 7372 633d 227b 2520  )"><img src="{% 
-00001180: 7374 6174 6963 2027 7061 7373 6b65 7973  static 'passkeys
-00001190: 2f69 6d67 732f 4649 444f 2d50 6173 736b  /imgs/FIDO-Passk
-000011a0: 6579 5f49 636f 6e2d 5768 6974 652e 706e  ey_Icon-White.pn
-000011b0: 6727 2025 7d22 2073 7479 6c65 3d22 7769  g' %}" style="wi
-000011c0: 6474 683a 2032 3470 7822 3e0a 2020 2020  dth: 24px">.    
-000011d0: 207b 2569 6e63 6c75 6465 2027 7061 7373   {%include 'pass
-000011e0: 6b65 7973 2e6a 7327 2025 7d0a 2020 2020  keys.js' %}.    
-000011f0: 2060 6060 0a46 6f72 2045 7861 6d70 6c65   ```.For Example
-00001200: 2c20 5365 6520 2765 7861 6d70 6c65 2720  , See 'example' 
-00001210: 6170 7020 616e 6420 6c6f 6f6b 2061 7420  app and look at 
-00001220: 4558 414d 504c 452e 6d64 2074 6f20 7365  EXAMPLE.md to se
-00001230: 6520 686f 7720 746f 2073 6574 2069 7420  e how to set it 
-00001240: 7570 2e0a 0a23 2044 6574 6563 7420 6966  up...# Detect if
-00001250: 2075 7365 7220 6973 2075 7369 6e67 2070   user is using p
-00001260: 6173 736b 6579 730a 4f6e 6365 2074 6865  asskeys.Once the
-00001270: 2062 6163 6b65 6e64 2069 7320 7573 6564   backend is used
-00001280: 2c20 7468 6572 6520 7769 6c6c 2062 6520  , there will be 
-00001290: 6120 6070 6173 736b 6579 6020 6b65 7920  a `passkey` key 
-000012a0: 696e 2072 6571 7565 7374 2e73 6573 7369  in request.sessi
-000012b0: 6f6e 2e20 0a49 6620 7468 6520 7573 6572  on. .If the user
-000012c0: 2075 7365 6420 6120 7061 7373 6b65 7920   used a passkey 
-000012d0: 7468 656e 2060 7265 7175 6573 742e 7365  then `request.se
-000012e0: 7373 696f 6e5b 2770 6173 736b 6579 275d  ssion['passkey']
-000012f0: 5b27 7061 7373 6b65 7927 5d60 2077 696c  ['passkey']` wil
-00001300: 6c20 6265 2054 7275 6520 616e 6420 7468  l be True and th
-00001310: 6520 6b65 7920 696e 666f 726d 6174 696f  e key informatio
-00001320: 6e20 7769 6c6c 2062 6520 7468 6572 6520  n will be there 
-00001330: 6c69 6b65 2074 6869 730a 6060 6070 7974  like this.```pyt
-00001340: 686f 6e0a 7b27 7061 7373 6b65 7927 3a20  hon.{'passkey': 
-00001350: 5472 7565 2c20 276e 616d 6527 3a20 2743  True, 'name': 'C
-00001360: 6872 6f6d 6527 2c20 2769 6427 3a20 322c  hrome', 'id': 2,
-00001370: 2027 706c 6174 666f 726d 273a 2027 4368   'platform': 'Ch
-00001380: 726f 6d65 206f 6e20 4170 706c 6527 2c20  rome on Apple', 
-00001390: 2763 726f 7373 5f70 6c61 7466 6f72 6d27  'cross_platform'
-000013a0: 3a20 4661 6c73 657d 0a60 6060 0a60 6372  : False}.```.`cr
-000013b0: 6f73 735f 706c 6174 666f 726d 603a 206d  oss_platform`: m
-000013c0: 6561 6e73 2074 6861 7420 7468 6520 7573  eans that the us
-000013d0: 6572 2075 7365 6420 6120 6b65 7920 6672  er used a key fr
-000013e0: 6f6d 2061 6e6f 7468 6572 2070 6c61 7466  om another platf
-000013f0: 6f72 6d20 736f 2074 6865 7265 2069 7320  orm so there is 
-00001400: 6e6f 206b 6579 206c 6f63 616c 2074 6f20  no key local to 
-00001410: 7468 6520 6465 7669 6365 2075 7365 6420  the device used 
-00001420: 746f 206c 6f67 696e 2065 2e67 2075 7365  to login e.g use
-00001430: 6420 616e 2041 6e64 726f 6964 2070 686f  d an Android pho
-00001440: 6e65 206f 6e20 4d61 6320 4f53 2058 206f  ne on Mac OS X o
-00001450: 7220 6950 6164 2e0a 4966 2074 6865 2075  r iPad..If the u
-00001460: 7365 7220 6469 646e 2774 2075 7365 2061  ser didn't use a
-00001470: 2070 6173 736b 6579 2074 6865 6e20 6974   passkey then it
-00001480: 2077 696c 6c20 6265 2073 6574 2074 6f20   will be set to 
-00001490: 4661 6c73 650a 6060 6070 7974 686f 6e0a  False.```python.
-000014a0: 7b27 7061 7373 6b65 7927 3a46 616c 7365  {'passkey':False
-000014b0: 7d0a 6060 600a 0a0a 2320 4368 6563 6b20  }.```...# Check 
-000014c0: 6966 2074 6865 2075 7365 7220 6361 6e20  if the user can 
-000014d0: 6265 2065 6e72 6f6c 6c65 6420 666f 7220  be enrolled for 
-000014e0: 6120 706c 6174 666f 726d 2061 7574 6865  a platform authe
-000014f0: 6e74 6963 6174 6f72 0a0a 4966 2079 6f75  nticator..If you
-00001500: 2077 616e 7420 746f 2063 6865 636b 2069   want to check i
-00001510: 6620 7468 6520 7573 6572 2063 616e 2062  f the user can b
-00001520: 6520 656e 726f 6c6c 6564 2074 6f20 7573  e enrolled to us
-00001530: 6520 6120 706c 6174 666f 726d 2061 7574  e a platform aut
-00001540: 6865 6e74 6963 6174 6f72 2c20 796f 7520  henticator, you 
-00001550: 6361 6e20 646f 2074 6865 2066 6f6c 6c6f  can do the follo
-00001560: 7769 6e67 2069 6e20 796f 7572 206d 6169  wing in your mai
-00001570: 6e20 7061 6765 2e0a 0a60 6060 6874 6d6c  n page...```html
-00001580: 0a3c 6469 7620 6964 3d22 706b 2220 636c  .<div id="pk" cl
-00001590: 6173 733d 2261 6c65 7274 2061 6c65 7274  ass="alert alert
-000015a0: 2d69 6e66 6f22 2073 7479 6c65 3d22 6469  -info" style="di
-000015b0: 7370 6c61 793a 206e 6f6e 6522 3e59 6f75  splay: none">You
-000015c0: 7220 6465 7669 6365 2073 7570 706f 7274  r device support
-000015d0: 7320 7061 7373 6b65 7973 2c20 3c61 2068  s passkeys, <a h
-000015e0: 7265 663d 227b 2575 726c 2027 7061 7373  ref="{%url 'pass
-000015f0: 6b65 7973 3a65 6e72 6f6c 6c27 257d 223e  keys:enroll'%}">
-00001600: 456e 726f 6c6c 3c2f 613e 203c 2f64 6976  Enroll</a> </div
-00001610: 3e0a 3c73 6372 6970 7420 7479 7065 3d22  >.<script type="
-00001620: 7465 7874 2f6a 6176 6173 6372 6970 7422  text/javascript"
-00001630: 3e0a 6675 6e63 7469 6f6e 2072 6567 6973  >.function regis
-00001640: 7465 725f 706b 2829 0a20 2020 207b 0a20  ter_pk().    {. 
-00001650: 2020 2020 2020 2024 2827 2370 6b27 292e         $('#pk').
-00001660: 7368 6f77 2829 3b0a 2020 2020 7d0a 7b25  show();.    }.{%
-00001670: 2069 6e63 6c75 6465 2027 6368 6563 6b5f   include 'check_
-00001680: 7061 7373 6b65 7973 2e6a 7327 257d 0a24  passkeys.js'%}.$
-00001690: 2864 6f63 756d 656e 7429 2e72 6561 6479  (document).ready
-000016a0: 2863 6865 636b 5f70 6173 736b 6579 2874  (check_passkey(t
-000016b0: 7275 652c 7265 6769 7374 6572 5f70 6b29  rue,register_pk)
-000016c0: 290a 3c2f 7363 7269 7074 3e0a 6060 600a  ).</script>.```.
-000016d0: 6368 6563 6b5f 7061 7373 6b65 7920 6675  check_passkey fu
-000016e0: 6e63 7469 6f6e 2070 6172 616d 7465 7273  nction paramters
-000016f0: 2061 7265 2061 7320 666f 6c6c 6f77 7320   are as follows 
-00001700: 0a2a 2060 706c 6174 666f 726d 5f61 7574  .* `platform_aut
-00001710: 6865 6e74 6963 6174 6f72 603a 2069 6620  henticator`: if 
-00001720: 7468 6520 7365 7276 6963 6520 7265 7175  the service requ
-00001730: 6972 6573 206f 6e6c 7920 6120 706c 6174  ires only a plat
-00001740: 666f 726d 2061 7574 6865 6e74 6963 6174  form authenticat
-00001750: 6f72 2028 652e 6720 546f 7563 6849 442c  or (e.g TouchID,
-00001760: 2057 696e 646f 7773 2048 656c 6c6f 206f   Windows Hello o
-00001770: 7220 416e 6472 6f69 6420 5361 6665 7479  r Android Safety
-00001780: 4e65 7429 0a2a 2060 7375 6363 6573 735f  Net).* `success_
-00001790: 6675 6e63 603a 2066 756e 6374 696f 6e20  func`: function 
-000017a0: 746f 2063 616c 6c20 6966 2061 2070 6c61  to call if a pla
-000017b0: 7466 6f72 6d20 6175 7468 656e 7469 6361  tform authentica
-000017c0: 746f 7220 6973 2066 6f75 6e64 206f 7220  tor is found or 
-000017d0: 6966 2074 6865 2075 7365 7220 6469 646e  if the user didn
-000017e0: 2774 206c 6f67 696e 2062 7920 6120 7061  't login by a pa
-000017f0: 7373 6b65 790a 2a20 6066 6169 6c5f 6675  sskey.* `fail_fu
-00001800: 6e63 603a 2066 756e 6374 696f 6e20 746f  nc`: function to
-00001810: 2063 616c 6c20 6966 206e 6f20 706c 6174   call if no plat
-00001820: 666f 726d 2061 7574 6865 6e74 6963 6174  form authenticat
-00001830: 6f72 2069 7320 666f 756e 6420 286f 7074  or is found (opt
-00001840: 696f 6e61 6c29 2e0a 0a0a 2323 2055 7369  ional)....## Usi
-00001850: 6e67 2043 6f6e 6469 7469 6f6e 616c 2055  ng Conditional U
-00001860: 490a 0a43 6f6e 6469 7469 6f6e 616c 2055  I..Conditional U
-00001870: 4920 6973 2061 2077 6179 2066 6f72 2074  I is a way for t
-00001880: 6865 2062 726f 7773 6572 2074 6f20 7072  he browser to pr
-00001890: 6f6d 7074 2074 6865 2075 7365 7220 746f  ompt the user to
-000018a0: 2075 7365 2074 6865 2070 6173 736b 6579   use the passkey
-000018b0: 2074 6f20 6c6f 6769 6e20 746f 2074 6865   to login to the
-000018c0: 2073 7973 7465 6d20 6173 2073 686f 776e   system as shown
-000018d0: 2069 6e20 0a0a 215b 636f 6e64 6974 696f   in ..![conditio
-000018e0: 6e61 6c55 492e 706e 675d 2869 6d67 7325  nalUI.png](imgs%
-000018f0: 3246 636f 6e64 6974 696f 6e61 6c55 492e  2FconditionalUI.
-00001900: 706e 6729 0a0a 5374 6172 7469 6e67 2076  png)..Starting v
-00001910: 6572 7369 6f6e 2076 312e 322e 2079 6f75  ersion v1.2. you
-00001920: 2063 616e 2075 7365 2043 6f6e 6469 7469   can use Conditi
-00001930: 6f6e 616c 2055 4920 6279 2061 6464 696e  onal UI by addin
-00001940: 6720 7468 6520 666f 6c6c 6f77 696e 6720  g the following 
-00001950: 746f 2079 6f75 7220 6c6f 6769 6e20 7061  to your login pa
-00001960: 6765 0a0a 312e 2041 6464 2060 7765 6261  ge..1. Add `weba
-00001970: 7574 686e 6020 746f 2061 7574 6f63 6f6d  uthn` to autocom
-00001980: 706c 6574 6520 6f66 2074 6865 2075 7365  plete of the use
-00001990: 726e 616d 6520 6669 656c 6420 6173 2073  rname field as s
-000019a0: 686f 776e 2062 656c 6f77 2e0a 6060 6068  hown below..```h
-000019b0: 746d 6c0a 3c69 6e70 7574 206e 616d 653d  tml.<input name=
-000019c0: 2275 7365 726e 616d 6522 2070 6c61 6365  "username" place
-000019d0: 686f 6c64 6572 3d22 7573 6572 6e61 6d65  holder="username
-000019e0: 2220 6175 746f 636f 6d70 6c65 7465 3d22  " autocomplete="
-000019f0: 7573 6572 6e61 6d65 2077 6562 6175 7468  username webauth
-00001a00: 6e22 3e0a 6060 600a 6164 6420 7468 6520  n">.```.add the 
-00001a10: 666f 6c6c 6f77 696e 6720 746f 2074 6865  following to the
-00001a20: 2070 6167 6520 6a73 2e0a 0a60 6060 6a73   page js...```js
-00001a30: 0a77 696e 646f 772e 6f6e 6c6f 6164 203d  .window.onload =
-00001a40: 2063 6865 636b 436f 6e64 6974 696f 6e61   checkConditiona
-00001a50: 6c55 4928 276c 6f67 696e 466f 726d 2729  lUI('loginForm')
-00001a60: 3b0a 6060 600a 7768 6572 6520 606c 6f67  ;.```.where `log
-00001a70: 696e 466f 726d 6020 6973 206e 616d 6520  inForm` is name 
-00001a80: 6f66 2079 6f75 7220 6c6f 6769 6e20 666f  of your login fo
-00001a90: 726d 2e0a 0a23 2320 5365 6375 7269 7479  rm...## Security
-00001aa0: 2063 6f6e 7461 6374 2069 6e66 6f72 6d61   contact informa
-00001ab0: 7469 6f6e 0a0a 546f 2072 6570 6f72 7420  tion..To report 
-00001ac0: 6120 7365 6375 7269 7479 2076 756c 6e65  a security vulne
-00001ad0: 7261 6269 6c69 7479 2c20 706c 6561 7365  rability, please
-00001ae0: 2075 7365 2074 6865 0a5b 5469 6465 6c69   use the.[Tideli
-00001af0: 6674 2073 6563 7572 6974 7920 636f 6e74  ft security cont
-00001b00: 6163 745d 2868 7474 7073 3a2f 2f74 6964  act](https://tid
-00001b10: 656c 6966 742e 636f 6d2f 7365 6375 7269  elift.com/securi
-00001b20: 7479 292e 0a54 6964 656c 6966 7420 7769  ty)..Tidelift wi
-00001b30: 6c6c 2063 6f6f 7264 696e 6174 6520 7468  ll coordinate th
-00001b40: 6520 6669 7820 616e 6420 6469 7363 6c6f  e fix and disclo
-00001b50: 7375 7265 2e0a 0a23 2043 6f6e 7472 6962  sure...# Contrib
-00001b60: 7574 6f72 730a 2a20 5b6d 6168 6d6f 6f64  utors.* [mahmood
-00001b70: 6e61 7372 5d28 6874 7470 733a 2f2f 6769  nasr](https://gi
-00001b80: 7468 7562 2e63 6f6d 2f6d 6168 6d6f 6f64  thub.com/mahmood
-00001b90: 6e61 7372 290a 2a20 5b6a 6163 6f70 7364  nasr).* [jacopsd
-00001ba0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001bb0: 2e63 6f6d 2f6a 6163 6f70 7364 2920 2020  .com/jacopsd)   
-00001bc0: 0a2a 205b 6761 7370 6172 6272 6f67 7565  .* [gasparbrogue
-00001bd0: 6972 615d 2868 7474 7073 3a2f 2f67 6974  ira](https://git
-00001be0: 6875 622e 636f 6d2f 6761 7370 6172 6272  hub.com/gasparbr
-00001bf0: 6f67 7565 6972 6129 0a0a 0a0a 0a         ogueira).....
+000005f0: 733a 2f2f 7374 6174 6963 2e70 6570 792e  s://static.pepy.
+00000600: 7465 6368 2f62 6164 6765 2f64 6a61 6e67  tech/badge/djang
+00000610: 6f2d 7061 7373 6b65 7973 295d 2868 7474  o-passkeys)](htt
+00000620: 7073 3a2f 2f70 6570 792e 7465 6368 2f70  ps://pepy.tech/p
+00000630: 726f 6a65 6374 2f64 6a61 6e67 6f2d 7061  roject/django-pa
+00000640: 7373 6b65 7973 290a 5b21 5b44 6f77 6e6c  sskeys).[![Downl
+00000650: 6f61 6473 202f 204d 6f6e 7468 205d 2868  oads / Month ](h
+00000660: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
+00000670: 2f62 6164 6765 2f64 6a61 6e67 6f2d 7061  /badge/django-pa
+00000680: 7373 6b65 7973 2f6d 6f6e 7468 295d 2868  sskeys/month)](h
+00000690: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
+000006a0: 2f70 726f 6a65 6374 2f64 6a61 6e67 6f2d  /project/django-
+000006b0: 7061 7373 6b65 7973 290a 5b21 5b62 7569  passkeys).[![bui
+000006c0: 6c64 5d28 6874 7470 733a 2f2f 6769 7468  ld](https://gith
+000006d0: 7562 2e63 6f6d 2f6d 6b61 6c69 6f62 792f  ub.com/mkalioby/
+000006e0: 646a 616e 676f 2d70 6173 736b 6579 732f  django-passkeys/
+000006f0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000700: 732f 6261 7369 635f 6368 6563 6b73 2e79  s/basic_checks.y
+00000710: 6d6c 2f62 6164 6765 2e73 7667 295d 2868  ml/badge.svg)](h
+00000720: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000730: 6d2f 6d6b 616c 696f 6279 2f64 6a61 6e67  m/mkalioby/djang
+00000740: 6f2d 7061 7373 6b65 7973 2f61 6374 696f  o-passkeys/actio
+00000750: 6e73 2f77 6f72 6b66 6c6f 7773 2f62 6173  ns/workflows/bas
+00000760: 6963 5f63 6865 636b 732e 796d 6c29 0a21  ic_checks.yml).!
+00000770: 5b43 6f76 6572 6167 655d 2868 7474 7073  [Coverage](https
+00000780: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000790: 7263 6f6e 7465 6e74 2e63 6f6d 2f6d 6b61  rcontent.com/mka
+000007a0: 6c69 6f62 792f 646a 616e 676f 2d70 6173  lioby/django-pas
+000007b0: 736b 6579 732f 6d61 696e 2f63 6f76 6572  skeys/main/cover
+000007c0: 6167 652e 7376 6729 0a0a 416e 2065 7874  age.svg)..An ext
+000007d0: 656e 7369 6f6e 2074 6f20 446a 616e 676f  ension to Django
+000007e0: 202a 4d6f 6465 6c42 6163 6b65 6e64 2a20   *ModelBackend* 
+000007f0: 6261 636b 656e 6420 746f 2073 7570 706f  backend to suppo
+00000800: 7274 2070 6173 736b 6579 732e 0a0a 5061  rt passkeys...Pa
+00000810: 7373 6b65 7973 2069 7320 616e 2065 7874  sskeys is an ext
+00000820: 656e 7369 6f6e 2074 6f20 5765 6220 4175  ension to Web Au
+00000830: 7468 656e 7469 6361 7469 6f6e 2041 5049  thentication API
+00000840: 2074 6861 7420 7769 6c6c 2061 6c6c 6f77   that will allow
+00000850: 2074 6865 2075 7365 7220 746f 206c 6f67   the user to log
+00000860: 696e 2074 6f20 6120 7365 7276 6963 6520  in to a service 
+00000870: 7573 696e 6720 616e 6f74 6865 7220 6465  using another de
+00000880: 7669 6365 2e0a 0a54 6869 7320 6170 7020  vice...This app 
+00000890: 6973 2061 2073 6c69 6d2d 646f 776e 2076  is a slim-down v
+000008a0: 6572 7369 6f6e 206f 6620 5b64 6a61 6e67  ersion of [djang
+000008b0: 6f2d 6d66 6132 5d28 6874 7470 733a 2f2f  o-mfa2](https://
+000008c0: 6769 7468 7562 2e63 6f6d 2f6d 6b61 6c69  github.com/mkali
+000008d0: 6f62 792f 646a 616e 676f 2d6d 6661 3229  oby/django-mfa2)
+000008e0: 0a0a 5061 7373 6b65 7973 2061 7265 206e  ..Passkeys are n
+000008f0: 6f77 2073 7570 706f 7274 6564 206f 6e20  ow supported on 
+00000900: 0a2a 2041 7070 6c65 2045 636f 7379 7374  .* Apple Ecosyst
+00000910: 656d 2028 6950 686f 6e65 2031 362e 302b  em (iPhone 16.0+
+00000920: 2c20 6950 6164 4f53 2031 362e 312c 204d  , iPadOS 16.1, M
+00000930: 6163 204f 5320 5820 5665 6e74 7572 6129  ac OS X Ventura)
+00000940: 0a2a 2043 6872 6f6d 6975 6d20 6261 7365  .* Chromium base
+00000950: 6420 6272 6f77 7365 7273 2028 6f6e 2050  d browsers (on P
+00000960: 4320 616e 6420 4c61 7074 6f70 2920 616c  C and Laptop) al
+00000970: 6c6f 7773 2070 6963 6b69 6e67 2075 7020  lows picking up 
+00000980: 6372 6564 656e 7469 616c 7320 6672 6f6d  credentials from
+00000990: 2041 6e64 726f 6964 2061 6e64 2069 5068   Android and iPh
+000009a0: 6f6e 652f 6950 6164 4f53 2e0a 2a20 416e  one/iPadOS..* An
+000009b0: 6472 6f69 6420 4372 6564 656e 7469 616c  droid Credential
+000009c0: 7320 6372 6561 7469 6f6e 2066 6f72 2052  s creation for R
+000009d0: 6573 6964 656e 744b 6579 7320 6973 2063  esidentKeys is c
+000009e0: 7572 7265 6e74 6c79 2069 6e20 6c69 7665  urrently in live
+000009f0: 206e 6f77 2e0a 0a4f 6e20 4d61 7920 332c   now...On May 3,
+00000a00: 2032 3032 332c 2047 6f6f 676c 6520 616c   2023, Google al
+00000a10: 6c6f 7765 6420 7468 6520 7573 6520 6f66  lowed the use of
+00000a20: 2050 6173 736b 6579 7320 666f 7220 7468   Passkeys for th
+00000a30: 6520 7573 6572 7320 746f 206c 6f67 696e  e users to login
+00000a40: 2c20 6b69 6c6c 696e 6720 7468 6520 7061  , killing the pa
+00000a50: 7373 776f 7264 2066 6f72 2065 6e72 6f6c  ssword for enrol
+00000a60: 6c65 6420 7573 6572 732e 200a 0a23 2049  led users. ..# I
+00000a70: 6e73 7461 6c6c 6174 696f 6e0a 0a60 7069  nstallation..`pi
+00000a80: 7020 696e 7374 616c 6c20 646a 616e 676f  p install django
+00000a90: 2d70 6173 736b 6579 7360 0a0a 4375 7272  -passkeys`..Curr
+00000aa0: 656e 746c 792c 2069 7420 7375 7070 6f72  ently, it suppor
+00000ab0: 7420 446a 616e 676f 2032 2e30 2b2c 2050  t Django 2.0+, P
+00000ac0: 7974 686f 6e20 332e 372b 0a0a 2320 5573  ython 3.7+..# Us
+00000ad0: 6167 650a 312e 2069 6e20 796f 7572 2073  age.1. in your s
+00000ae0: 6574 7469 6e67 732e 7079 2061 6464 2074  ettings.py add t
+00000af0: 6865 2061 7070 6c69 6361 7469 6f6e 2074  he application t
+00000b00: 6f20 796f 7572 2069 6e73 7461 6c6c 6564  o your installed
+00000b10: 2061 7070 730a 2020 2060 6060 7079 7468   apps.   ```pyth
+00000b20: 6f6e 0a20 2020 494e 5354 414c 4c45 445f  on.   INSTALLED_
+00000b30: 4150 5053 3d28 0a20 2020 272e 2e2e 2e2e  APPS=(.   '.....
+00000b40: 2e27 2c0a 2020 2027 7061 7373 6b65 7973  .',.   'passkeys
+00000b50: 272c 0a20 2020 272e 2e2e 2e2e 2e27 290a  ',.   '......').
+00000b60: 2020 2060 6060 0a32 2e20 436f 6c6c 6563     ```.2. Collec
+00000b70: 7420 5374 6174 6963 2046 696c 6573 0a60  t Static Files.`
+00000b80: 7079 7468 6f6e 206d 616e 6167 652e 7079  python manage.py
+00000b90: 2063 6f6c 6c65 6374 7374 6174 6963 600a   collectstatic`.
+00000ba0: 332e 2052 756e 206d 6967 7261 7465 0a60  3. Run migrate.`
+00000bb0: 7079 7468 6f6e 206d 616e 6167 652e 7079  python manage.py
+00000bc0: 206d 6967 7261 7465 600a 342e 2041 6464   migrate`.4. Add
+00000bd0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2073   the following s
+00000be0: 6574 7469 6e67 7320 746f 2079 6f75 7220  ettings to your 
+00000bf0: 6669 6c65 0a0a 2020 2060 6060 7079 7468  file..   ```pyth
+00000c00: 6f6e 0a20 2020 2041 5554 4845 4e54 4943  on.    AUTHENTIC
+00000c10: 4154 494f 4e5f 4241 434b 454e 4453 203d  ATION_BACKENDS =
+00000c20: 205b 2770 6173 736b 6579 732e 6261 636b   ['passkeys.back
+00000c30: 656e 642e 5061 7373 6b65 794d 6f64 656c  end.PasskeyModel
+00000c40: 4261 636b 656e 6427 5d20 2320 4368 616e  Backend'] # Chan
+00000c50: 6765 2079 6f75 7220 6175 7468 656e 7469  ge your authenti
+00000c60: 6361 7469 6f6e 2062 6163 6b65 6e64 0a20  cation backend. 
+00000c70: 2020 2046 4944 4f5f 5345 5256 4552 5f49     FIDO_SERVER_I
+00000c80: 443d 226c 6f63 616c 686f 7374 2220 2020  D="localhost"   
+00000c90: 2020 2023 2053 6572 7665 7220 7270 2069     # Server rp i
+00000ca0: 6420 666f 7220 4649 444f 322c 2069 7420  d for FIDO2, it 
+00000cb0: 7468 6520 6675 6c6c 2064 6f6d 6169 6e20  the full domain 
+00000cc0: 6f66 2079 6f75 7220 7072 6f6a 6563 740a  of your project.
+00000cd0: 2020 2020 4649 444f 5f53 4552 5645 525f      FIDO_SERVER_
+00000ce0: 4e41 4d45 3d22 5465 7374 4170 7022 0a20  NAME="TestApp". 
+00000cf0: 2020 2069 6d70 6f72 7420 7061 7373 6b65     import passke
+00000d00: 7973 0a20 2020 204b 4559 5f41 5454 4143  ys.    KEY_ATTAC
+00000d10: 484d 454e 5420 3d20 4e6f 6e65 207c 2070  HMENT = None | p
+00000d20: 6173 736b 6579 732e 4174 7461 6368 6d65  asskeys.Attachme
+00000d30: 6e74 2e43 524f 5353 5f50 4c41 5446 4f52  nt.CROSS_PLATFOR
+00000d40: 4d20 7c20 7061 7373 6b65 7973 2e41 7474  M | passkeys.Att
+00000d50: 6163 686d 656e 742e 504c 4154 464f 524d  achment.PLATFORM
+00000d60: 0a20 2020 6060 600a 2020 202a 2a4e 6f74  .   ```.   **Not
+00000d70: 652a 2a3a 2053 7461 7274 696e 6720 7631  e**: Starting v1
+00000d80: 2e31 2c20 6046 4944 4f5f 5345 5256 4552  .1, `FIDO_SERVER
+00000d90: 5f49 4460 2061 6e64 2f6f 7220 6046 4944  _ID` and/or `FID
+00000da0: 4f5f 5345 5256 4552 5f4e 414d 4560 2063  O_SERVER_NAME` c
+00000db0: 616e 2062 6520 6120 6361 6c6c 6162 6c65  an be a callable
+00000dc0: 2074 6f20 7375 7070 6f72 7420 6d75 6c74   to support mult
+00000dd0: 692d 7465 6e61 6e74 7320 7765 6220 6170  i-tenants web ap
+00000de0: 706c 6963 6174 696f 6e73 2c20 7468 6520  plications, the 
+00000df0: 6072 6571 7565 7374 6020 6973 2070 6173  `request` is pas
+00000e00: 7365 6420 746f 2074 6865 2063 616c 6c65  sed to the calle
+00000e10: 6420 6675 6e63 7469 6f6e 2e0a 352e 2041  d function..5. A
+00000e20: 6464 2070 6173 736b 6579 7320 746f 2075  dd passkeys to u
+00000e30: 726c 732e 7079 0a20 2020 6060 6070 7974  rls.py.   ```pyt
+00000e40: 686f 6e20 0a0a 2020 2075 726c 735f 7061  hon ..   urls_pa
+00000e50: 7474 6572 6e73 3d20 5b0a 2020 2027 2e2e  tterns= [.   '..
+00000e60: 2e27 2c0a 2020 2075 726c 2872 275e 7061  .',.   url(r'^pa
+00000e70: 7373 6b65 7973 2f27 2c20 696e 636c 7564  sskeys/', includ
+00000e80: 6528 2770 6173 736b 6579 732e 7572 6c73  e('passkeys.urls
+00000e90: 2729 292c 0a20 2020 272e 2e2e 2e27 2c0a  ')),.   '....',.
+00000ea0: 2020 2020 5d0a 2020 2020 6060 600a 362e      ].    ```.6.
+00000eb0: 2054 6f20 6d61 7463 6820 7468 6520 6c6f   To match the lo
+00000ec0: 6f6b 2061 6e64 2066 6565 6c20 6f66 2079  ok and feel of y
+00000ed0: 6f75 7220 7072 6f6a 6563 742c 2050 6173  our project, Pas
+00000ee0: 736b 6579 7320 696e 636c 7564 6573 2060  skeys includes `
+00000ef0: 6261 7365 2e68 746d 6c60 2062 7574 2069  base.html` but i
+00000f00: 7420 6e65 6564 7320 626c 6f63 6b73 206e  t needs blocks n
+00000f10: 616d 6564 2060 6865 6164 6020 2620 6063  amed `head` & `c
+00000f20: 6f6e 7465 6e74 6020 746f 2061 6464 6564  ontent` to added
+00000f30: 2069 7473 2063 6f6e 7465 6e74 2074 6f20   its content to 
+00000f40: 6974 2e0a 2020 202a 2a4e 6f74 6573 3a2a  it..   **Notes:*
+00000f50: 2a20 0a20 2020 200a 2020 2020 312e 2059  * .    .    1. Y
+00000f60: 6f75 2063 616e 206f 7665 7272 6964 6520  ou can override 
+00000f70: 6050 6173 734b 6579 735f 6261 7365 2e68  `PassKeys_base.h
+00000f80: 746d 6c60 2077 6869 6368 2069 7320 7573  tml` which is us
+00000f90: 6564 2062 7920 6050 6173 736b 6579 732e  ed by `Passkeys.
+00000fa0: 6874 6d6c 6020 736f 2079 6f75 2063 616e  html` so you can
+00000fb0: 2063 6f6e 7472 6f6c 2074 6865 2073 7479   control the sty
+00000fc0: 6c69 6e67 2062 6574 7465 7220 616e 6420  ling better and 
+00000fd0: 6375 7272 656e 7420 6050 6173 736b 6579  current `Passkey
+00000fe0: 735f 6261 7365 2e68 746d 6c60 2065 7874  s_base.html` ext
+00000ff0: 656e 6473 2060 6261 7365 2e68 746d 6c60  ends `base.html`
+00001000: 0a20 2020 2031 2e20 4375 7272 656e 746c  .    1. Currentl
+00001010: 792c 2060 5061 7373 4b65 7973 5f62 6173  y, `PassKeys_bas
+00001020: 652e 6874 6d6c 6020 6e65 6564 7320 4a51  e.html` needs JQ
+00001030: 7565 7279 2061 6e64 2062 6f6f 7473 7472  uery and bootstr
+00001040: 6170 2e20 0a0a 372e 2053 6f6d 6577 6865  ap. ..7. Somewhe
+00001050: 7265 2069 6e20 796f 7572 2061 7070 2c20  re in your app, 
+00001060: 6164 6420 6120 6c69 6e6b 2074 6f20 2770  add a link to 'p
+00001070: 6173 736b 6579 733a 686f 6d65 270a 2020  asskeys:home'.  
+00001080: 2020 6060 603c 6c69 3e3c 6120 6872 6566    ```<li><a href
+00001090: 3d22 7b25 2075 726c 2027 7061 7373 6b65  ="{% url 'passke
+000010a0: 7973 3a68 6f6d 6527 2025 7d22 3e50 6173  ys:home' %}">Pas
+000010b0: 736b 6579 733c 2f61 3e20 3c2f 6c69 3e60  skeys</a> </li>`
+000010c0: 6060 0a38 2e20 496e 2079 6f75 7220 6c6f  ``.8. In your lo
+000010d0: 6769 6e20 7669 6577 2c20 6368 616e 6765  gin view, change
+000010e0: 2074 6865 2061 7574 6865 6e74 6963 6174   the authenticat
+000010f0: 6520 6361 6c6c 2074 6f20 696e 636c 7564  e call to includ
+00001100: 6520 7468 6520 7265 7175 6573 7420 6173  e the request as
+00001110: 2066 6f6c 6c6f 7773 0a20 2020 6060 6070   follows.   ```p
+00001120: 7974 686f 6e0a 2020 2020 7573 6572 3d61  ython.    user=a
+00001130: 7574 6865 6e74 6963 6174 6528 7265 7175  uthenticate(requ
+00001140: 6573 742c 2075 7365 726e 616d 653d 7265  est, username=re
+00001150: 7175 6573 742e 504f 5354 5b22 7573 6572  quest.POST["user
+00001160: 6e61 6d65 225d 2c70 6173 7377 6f72 643d  name"],password=
+00001170: 7265 7175 6573 742e 504f 5354 5b22 7061  request.POST["pa
+00001180: 7373 776f 7264 225d 290a 2020 2020 6060  ssword"]).    ``
+00001190: 600a 0a38 2e20 4669 6e61 6c6c 792c 2049  `..8. Finally, I
+000011a0: 6e20 796f 7572 2060 6c6f 6769 6e2e 6874  n your `login.ht
+000011b0: 6d6c 600a 2020 202a 2047 6976 6520 616e  ml`.   * Give an
+000011c0: 2069 6420 746f 2079 6f75 7220 6c6f 6769   id to your logi
+000011d0: 6e20 666f 726d 2065 2e67 2027 6c6f 6769  n form e.g 'logi
+000011e0: 6e46 6f72 6d27 2c20 7468 6520 6964 2073  nForm', the id s
+000011f0: 686f 756c 6420 6265 2070 726f 7669 6465  hould be provide
+00001200: 6420 7768 656e 2063 616c 6c69 6e67 2060  d when calling `
+00001210: 6175 7468 6e60 2066 756e 6374 696f 6e0a  authn` function.
+00001220: 2020 202a 2049 6e73 6964 6520 7468 6520     * Inside the 
+00001230: 666f 726d 2c20 6164 6420 0a20 2020 2020  form, add .     
+00001240: 6060 6068 746d 6c0a 2020 2020 2020 3c69  ```html.      <i
+00001250: 6e70 7574 2074 7970 653d 2268 6964 6465  nput type="hidde
+00001260: 6e22 206e 616d 653d 2270 6173 736b 6579  n" name="passkey
+00001270: 7322 2069 643d 2270 6173 736b 6579 7322  s" id="passkeys"
+00001280: 2f3e 0a20 2020 2020 203c 6275 7474 6f6e  />.      <button
+00001290: 2063 6c61 7373 3d22 6274 6e20 6274 6e2d   class="btn btn-
+000012a0: 626c 6f63 6b20 6274 6e2d 6461 726b 2220  block btn-dark" 
+000012b0: 7479 7065 3d22 6275 7474 6f6e 2220 6f6e  type="button" on
+000012c0: 636c 6963 6b3d 2261 7574 686e 2827 6c6f  click="authn('lo
+000012d0: 6769 6e46 6f72 6d27 2922 3e3c 696d 6720  ginForm')"><img 
+000012e0: 7372 633d 227b 2520 7374 6174 6963 2027  src="{% static '
+000012f0: 7061 7373 6b65 7973 2f69 6d67 732f 4649  passkeys/imgs/FI
+00001300: 444f 2d50 6173 736b 6579 5f49 636f 6e2d  DO-Passkey_Icon-
+00001310: 5768 6974 652e 706e 6727 2025 7d22 2073  White.png' %}" s
+00001320: 7479 6c65 3d22 7769 6474 683a 2032 3470  tyle="width: 24p
+00001330: 7822 3e0a 2020 2020 207b 2569 6e63 6c75  x">.     {%inclu
+00001340: 6465 2027 7061 7373 6b65 7973 2e6a 7327  de 'passkeys.js'
+00001350: 2025 7d0a 2020 2020 2060 6060 0a46 6f72   %}.     ```.For
+00001360: 2045 7861 6d70 6c65 2c20 5365 6520 2765   Example, See 'e
+00001370: 7861 6d70 6c65 2720 6170 7020 616e 6420  xample' app and 
+00001380: 6c6f 6f6b 2061 7420 4558 414d 504c 452e  look at EXAMPLE.
+00001390: 6d64 2074 6f20 7365 6520 686f 7720 746f  md to see how to
+000013a0: 2073 6574 2069 7420 7570 2e0a 0a23 2044   set it up...# D
+000013b0: 6574 6563 7420 6966 2075 7365 7220 6973  etect if user is
+000013c0: 2075 7369 6e67 2070 6173 736b 6579 730a   using passkeys.
+000013d0: 4f6e 6365 2074 6865 2062 6163 6b65 6e64  Once the backend
+000013e0: 2069 7320 7573 6564 2c20 7468 6572 6520   is used, there 
+000013f0: 7769 6c6c 2062 6520 6120 6070 6173 736b  will be a `passk
+00001400: 6579 6020 6b65 7920 696e 2072 6571 7565  ey` key in reque
+00001410: 7374 2e73 6573 7369 6f6e 2e20 0a49 6620  st.session. .If 
+00001420: 7468 6520 7573 6572 2075 7365 6420 6120  the user used a 
+00001430: 7061 7373 6b65 7920 7468 656e 2060 7265  passkey then `re
+00001440: 7175 6573 742e 7365 7373 696f 6e5b 2770  quest.session['p
+00001450: 6173 736b 6579 275d 5b27 7061 7373 6b65  asskey']['passke
+00001460: 7927 5d60 2077 696c 6c20 6265 2054 7275  y']` will be Tru
+00001470: 6520 616e 6420 7468 6520 6b65 7920 696e  e and the key in
+00001480: 666f 726d 6174 696f 6e20 7769 6c6c 2062  formation will b
+00001490: 6520 7468 6572 6520 6c69 6b65 2074 6869  e there like thi
+000014a0: 730a 6060 6070 7974 686f 6e0a 7b27 7061  s.```python.{'pa
+000014b0: 7373 6b65 7927 3a20 5472 7565 2c20 276e  sskey': True, 'n
+000014c0: 616d 6527 3a20 2743 6872 6f6d 6527 2c20  ame': 'Chrome', 
+000014d0: 2769 6427 3a20 322c 2027 706c 6174 666f  'id': 2, 'platfo
+000014e0: 726d 273a 2027 4368 726f 6d65 206f 6e20  rm': 'Chrome on 
+000014f0: 4170 706c 6527 2c20 2763 726f 7373 5f70  Apple', 'cross_p
+00001500: 6c61 7466 6f72 6d27 3a20 4661 6c73 657d  latform': False}
+00001510: 0a60 6060 0a60 6372 6f73 735f 706c 6174  .```.`cross_plat
+00001520: 666f 726d 603a 206d 6561 6e73 2074 6861  form`: means tha
+00001530: 7420 7468 6520 7573 6572 2075 7365 6420  t the user used 
+00001540: 6120 6b65 7920 6672 6f6d 2061 6e6f 7468  a key from anoth
+00001550: 6572 2070 6c61 7466 6f72 6d20 736f 2074  er platform so t
+00001560: 6865 7265 2069 7320 6e6f 206b 6579 206c  here is no key l
+00001570: 6f63 616c 2074 6f20 7468 6520 6465 7669  ocal to the devi
+00001580: 6365 2075 7365 6420 746f 206c 6f67 696e  ce used to login
+00001590: 2065 2e67 2075 7365 6420 616e 2041 6e64   e.g used an And
+000015a0: 726f 6964 2070 686f 6e65 206f 6e20 4d61  roid phone on Ma
+000015b0: 6320 4f53 2058 206f 7220 6950 6164 2e0a  c OS X or iPad..
+000015c0: 4966 2074 6865 2075 7365 7220 6469 646e  If the user didn
+000015d0: 2774 2075 7365 2061 2070 6173 736b 6579  't use a passkey
+000015e0: 2074 6865 6e20 6974 2077 696c 6c20 6265   then it will be
+000015f0: 2073 6574 2074 6f20 4661 6c73 650a 6060   set to False.``
+00001600: 6070 7974 686f 6e0a 7b27 7061 7373 6b65  `python.{'passke
+00001610: 7927 3a46 616c 7365 7d0a 6060 600a 0a0a  y':False}.```...
+00001620: 2320 4368 6563 6b20 6966 2074 6865 2075  # Check if the u
+00001630: 7365 7220 6361 6e20 6265 2065 6e72 6f6c  ser can be enrol
+00001640: 6c65 6420 666f 7220 6120 706c 6174 666f  led for a platfo
+00001650: 726d 2061 7574 6865 6e74 6963 6174 6f72  rm authenticator
+00001660: 0a0a 4966 2079 6f75 2077 616e 7420 746f  ..If you want to
+00001670: 2063 6865 636b 2069 6620 7468 6520 7573   check if the us
+00001680: 6572 2063 616e 2062 6520 656e 726f 6c6c  er can be enroll
+00001690: 6564 2074 6f20 7573 6520 6120 706c 6174  ed to use a plat
+000016a0: 666f 726d 2061 7574 6865 6e74 6963 6174  form authenticat
+000016b0: 6f72 2c20 796f 7520 6361 6e20 646f 2074  or, you can do t
+000016c0: 6865 2066 6f6c 6c6f 7769 6e67 2069 6e20  he following in 
+000016d0: 796f 7572 206d 6169 6e20 7061 6765 2e0a  your main page..
+000016e0: 0a60 6060 6874 6d6c 0a3c 6469 7620 6964  .```html.<div id
+000016f0: 3d22 706b 2220 636c 6173 733d 2261 6c65  ="pk" class="ale
+00001700: 7274 2061 6c65 7274 2d69 6e66 6f22 2073  rt alert-info" s
+00001710: 7479 6c65 3d22 6469 7370 6c61 793a 206e  tyle="display: n
+00001720: 6f6e 6522 3e59 6f75 7220 6465 7669 6365  one">Your device
+00001730: 2073 7570 706f 7274 7320 7061 7373 6b65   supports passke
+00001740: 7973 2c20 3c61 2068 7265 663d 227b 2575  ys, <a href="{%u
+00001750: 726c 2027 7061 7373 6b65 7973 3a65 6e72  rl 'passkeys:enr
+00001760: 6f6c 6c27 257d 223e 456e 726f 6c6c 3c2f  oll'%}">Enroll</
+00001770: 613e 203c 2f64 6976 3e0a 3c73 6372 6970  a> </div>.<scrip
+00001780: 7420 7479 7065 3d22 7465 7874 2f6a 6176  t type="text/jav
+00001790: 6173 6372 6970 7422 3e0a 6675 6e63 7469  ascript">.functi
+000017a0: 6f6e 2072 6567 6973 7465 725f 706b 2829  on register_pk()
+000017b0: 0a20 2020 207b 0a20 2020 2020 2020 2024  .    {.        $
+000017c0: 2827 2370 6b27 292e 7368 6f77 2829 3b0a  ('#pk').show();.
+000017d0: 2020 2020 7d0a 7b25 2069 6e63 6c75 6465      }.{% include
+000017e0: 2027 6368 6563 6b5f 7061 7373 6b65 7973   'check_passkeys
+000017f0: 2e6a 7327 257d 0a24 2864 6f63 756d 656e  .js'%}.$(documen
+00001800: 7429 2e72 6561 6479 2863 6865 636b 5f70  t).ready(check_p
+00001810: 6173 736b 6579 2874 7275 652c 7265 6769  asskey(true,regi
+00001820: 7374 6572 5f70 6b29 290a 3c2f 7363 7269  ster_pk)).</scri
+00001830: 7074 3e0a 6060 600a 6368 6563 6b5f 7061  pt>.```.check_pa
+00001840: 7373 6b65 7920 6675 6e63 7469 6f6e 2070  sskey function p
+00001850: 6172 616d 7465 7273 2061 7265 2061 7320  aramters are as 
+00001860: 666f 6c6c 6f77 7320 0a2a 2060 706c 6174  follows .* `plat
+00001870: 666f 726d 5f61 7574 6865 6e74 6963 6174  form_authenticat
+00001880: 6f72 603a 2069 6620 7468 6520 7365 7276  or`: if the serv
+00001890: 6963 6520 7265 7175 6972 6573 206f 6e6c  ice requires onl
+000018a0: 7920 6120 706c 6174 666f 726d 2061 7574  y a platform aut
+000018b0: 6865 6e74 6963 6174 6f72 2028 652e 6720  henticator (e.g 
+000018c0: 546f 7563 6849 442c 2057 696e 646f 7773  TouchID, Windows
+000018d0: 2048 656c 6c6f 206f 7220 416e 6472 6f69   Hello or Androi
+000018e0: 6420 5361 6665 7479 4e65 7429 0a2a 2060  d SafetyNet).* `
+000018f0: 7375 6363 6573 735f 6675 6e63 603a 2066  success_func`: f
+00001900: 756e 6374 696f 6e20 746f 2063 616c 6c20  unction to call 
+00001910: 6966 2061 2070 6c61 7466 6f72 6d20 6175  if a platform au
+00001920: 7468 656e 7469 6361 746f 7220 6973 2066  thenticator is f
+00001930: 6f75 6e64 206f 7220 6966 2074 6865 2075  ound or if the u
+00001940: 7365 7220 6469 646e 2774 206c 6f67 696e  ser didn't login
+00001950: 2062 7920 6120 7061 7373 6b65 790a 2a20   by a passkey.* 
+00001960: 6066 6169 6c5f 6675 6e63 603a 2066 756e  `fail_func`: fun
+00001970: 6374 696f 6e20 746f 2063 616c 6c20 6966  ction to call if
+00001980: 206e 6f20 706c 6174 666f 726d 2061 7574   no platform aut
+00001990: 6865 6e74 6963 6174 6f72 2069 7320 666f  henticator is fo
+000019a0: 756e 6420 286f 7074 696f 6e61 6c29 2e0a  und (optional)..
+000019b0: 0a0a 2323 2055 7369 6e67 2043 6f6e 6469  ..## Using Condi
+000019c0: 7469 6f6e 616c 2055 490a 0a43 6f6e 6469  tional UI..Condi
+000019d0: 7469 6f6e 616c 2055 4920 6973 2061 2077  tional UI is a w
+000019e0: 6179 2066 6f72 2074 6865 2062 726f 7773  ay for the brows
+000019f0: 6572 2074 6f20 7072 6f6d 7074 2074 6865  er to prompt the
+00001a00: 2075 7365 7220 746f 2075 7365 2074 6865   user to use the
+00001a10: 2070 6173 736b 6579 2074 6f20 6c6f 6769   passkey to logi
+00001a20: 6e20 746f 2074 6865 2073 7973 7465 6d20  n to the system 
+00001a30: 6173 2073 686f 776e 2069 6e20 0a0a 215b  as shown in ..![
+00001a40: 636f 6e64 6974 696f 6e61 6c55 492e 706e  conditionalUI.pn
+00001a50: 675d 2869 6d67 7325 3246 636f 6e64 6974  g](imgs%2Fcondit
+00001a60: 696f 6e61 6c55 492e 706e 6729 0a0a 5374  ionalUI.png)..St
+00001a70: 6172 7469 6e67 2076 6572 7369 6f6e 2076  arting version v
+00001a80: 312e 322e 2079 6f75 2063 616e 2075 7365  1.2. you can use
+00001a90: 2043 6f6e 6469 7469 6f6e 616c 2055 4920   Conditional UI 
+00001aa0: 6279 2061 6464 696e 6720 7468 6520 666f  by adding the fo
+00001ab0: 6c6c 6f77 696e 6720 746f 2079 6f75 7220  llowing to your 
+00001ac0: 6c6f 6769 6e20 7061 6765 0a0a 312e 2041  login page..1. A
+00001ad0: 6464 2060 7765 6261 7574 686e 6020 746f  dd `webauthn` to
+00001ae0: 2061 7574 6f63 6f6d 706c 6574 6520 6f66   autocomplete of
+00001af0: 2074 6865 2075 7365 726e 616d 6520 6669   the username fi
+00001b00: 656c 6420 6173 2073 686f 776e 2062 656c  eld as shown bel
+00001b10: 6f77 2e0a 6060 6068 746d 6c0a 3c69 6e70  ow..```html.<inp
+00001b20: 7574 206e 616d 653d 2275 7365 726e 616d  ut name="usernam
+00001b30: 6522 2070 6c61 6365 686f 6c64 6572 3d22  e" placeholder="
+00001b40: 7573 6572 6e61 6d65 2220 6175 746f 636f  username" autoco
+00001b50: 6d70 6c65 7465 3d22 7573 6572 6e61 6d65  mplete="username
+00001b60: 2077 6562 6175 7468 6e22 3e0a 6060 600a   webauthn">.```.
+00001b70: 6164 6420 7468 6520 666f 6c6c 6f77 696e  add the followin
+00001b80: 6720 746f 2074 6865 2070 6167 6520 6a73  g to the page js
+00001b90: 2e0a 0a60 6060 6a73 0a77 696e 646f 772e  ...```js.window.
+00001ba0: 6f6e 6c6f 6164 203d 2063 6865 636b 436f  onload = checkCo
+00001bb0: 6e64 6974 696f 6e61 6c55 4928 276c 6f67  nditionalUI('log
+00001bc0: 696e 466f 726d 2729 3b0a 6060 600a 7768  inForm');.```.wh
+00001bd0: 6572 6520 606c 6f67 696e 466f 726d 6020  ere `loginForm` 
+00001be0: 6973 206e 616d 6520 6f66 2079 6f75 7220  is name of your 
+00001bf0: 6c6f 6769 6e20 666f 726d 2e0a 0a23 2320  login form...## 
+00001c00: 5365 6375 7269 7479 2063 6f6e 7461 6374  Security contact
+00001c10: 2069 6e66 6f72 6d61 7469 6f6e 0a0a 546f   information..To
+00001c20: 2072 6570 6f72 7420 6120 7365 6375 7269   report a securi
+00001c30: 7479 2076 756c 6e65 7261 6269 6c69 7479  ty vulnerability
+00001c40: 2c20 706c 6561 7365 2075 7365 2074 6865  , please use the
+00001c50: 0a5b 5469 6465 6c69 6674 2073 6563 7572  .[Tidelift secur
+00001c60: 6974 7920 636f 6e74 6163 745d 2868 7474  ity contact](htt
+00001c70: 7073 3a2f 2f74 6964 656c 6966 742e 636f  ps://tidelift.co
+00001c80: 6d2f 7365 6375 7269 7479 292e 0a54 6964  m/security)..Tid
+00001c90: 656c 6966 7420 7769 6c6c 2063 6f6f 7264  elift will coord
+00001ca0: 696e 6174 6520 7468 6520 6669 7820 616e  inate the fix an
+00001cb0: 6420 6469 7363 6c6f 7375 7265 2e0a 0a23  d disclosure...#
+00001cc0: 2043 6f6e 7472 6962 7574 6f72 730a 2a20   Contributors.* 
+00001cd0: 5b6d 6168 6d6f 6f64 6e61 7372 5d28 6874  [mahmoodnasr](ht
+00001ce0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001cf0: 2f6d 6168 6d6f 6f64 6e61 7372 290a 2a20  /mahmoodnasr).* 
+00001d00: 5b6a 6163 6f70 7364 5d28 6874 7470 733a  [jacopsd](https:
+00001d10: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6163  //github.com/jac
+00001d20: 6f70 7364 2920 2020 0a2a 205b 6761 7370  opsd)   .* [gasp
+00001d30: 6172 6272 6f67 7565 6972 615d 2868 7474  arbrogueira](htt
+00001d40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001d50: 6761 7370 6172 6272 6f67 7565 6972 6129  gasparbrogueira)
+00001d60: 0a0a 0a0a 0a                             .....
```

### Comparing `django-passkeys-1.2.2/django_passkeys.egg-info/SOURCES.txt` & `django-passkeys-1.2.3/django_passkeys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/env/bin/activate_this.py` & `django-passkeys-1.2.3/env/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/passkeys/FIDO2.py` & `django-passkeys-1.2.3/passkeys/FIDO2.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/passkeys/backend.py` & `django-passkeys-1.2.3/passkeys/backend.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/passkeys/migrations/0001_initial.py` & `django-passkeys-1.2.3/passkeys/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/passkeys/models.py` & `django-passkeys-1.2.3/passkeys/models.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/passkeys/static/passkeys/css/bootstrap-toggle.min.css` & `django-passkeys-1.2.3/passkeys/static/passkeys/css/bootstrap-toggle.min.css`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png` & `django-passkeys-1.2.3/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/passkeys/static/passkeys/js/base64url.js` & `django-passkeys-1.2.3/passkeys/static/passkeys/js/base64url.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/passkeys/static/passkeys/js/bootstrap-toggle.min.js` & `django-passkeys-1.2.3/passkeys/static/passkeys/js/bootstrap-toggle.min.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/passkeys/static/passkeys/js/helpers.js` & `django-passkeys-1.2.3/passkeys/static/passkeys/js/helpers.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/passkeys/templates/PassKeys.html` & `django-passkeys-1.2.3/passkeys/templates/PassKeys.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/passkeys/templates/check_passkeys.js` & `django-passkeys-1.2.3/passkeys/templates/check_passkeys.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/passkeys/templates/modal.html` & `django-passkeys-1.2.3/passkeys/templates/modal.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/passkeys/templates/passkeys.js` & `django-passkeys-1.2.3/passkeys/templates/passkeys.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/passkeys/urls.py` & `django-passkeys-1.2.3/passkeys/urls.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/passkeys/views.py` & `django-passkeys-1.2.3/passkeys/views.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.2/setup.py` & `django-passkeys-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='django-passkeys',
-    version='1.2.2',
+    version='1.2.3',
     description='A Django Authentication Backend for Passkeys',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='Mohamed El-Kalioby',
     author_email = 'mkalioby@mkalioby.com',
     url = 'https://github.com/mkalioby/django-passkeys',
     download_url='https://github.com/mkalioby/django-passkeys',
```

