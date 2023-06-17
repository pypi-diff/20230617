# Comparing `tmp/FinGen-0.3.tar.gz` & `tmp/FinGen-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinGen-0.3.tar", last modified: Sat Jun 17 03:58:14 2023, max compression
+gzip compressed data, was "FinGen-0.3.1.tar", last modified: Sat Jun 17 04:08:53 2023, max compression
```

## Comparing `FinGen-0.3.tar` & `FinGen-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 03:58:14.138520 FinGen-0.3/
-drwxrwxrwx   0        0        0        0 2023-06-17 03:58:14.122953 FinGen-0.3/FinGen/
--rw-rw-rw-   0        0        0     4914 2023-06-17 03:56:41.000000 FinGen-0.3/FinGen/FindingsGenerator.py
--rw-rw-rw-   0        0        0     1440 2023-02-01 01:25:37.000000 FinGen-0.3/FinGen/Loader.py
--rw-rw-rw-   0        0        0        0 2023-02-01 01:30:43.000000 FinGen-0.3/FinGen/__init__.py
--rw-rw-rw-   0        0        0      196 2023-03-07 02:15:39.000000 FinGen-0.3/FinGen/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 03:58:14.137516 FinGen-0.3/FinGen.egg-info/
--rw-rw-rw-   0        0        0      595 2023-06-17 03:58:13.000000 FinGen-0.3/FinGen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-06-17 03:58:13.000000 FinGen-0.3/FinGen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 03:58:13.000000 FinGen-0.3/FinGen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-17 03:58:13.000000 FinGen-0.3/FinGen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-17 03:58:13.000000 FinGen-0.3/FinGen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2023-02-01 01:18:31.000000 FinGen-0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      595 2023-06-17 03:58:14.138520 FinGen-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-06-17 03:58:14.139517 FinGen-0.3/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-06-17 03:57:43.000000 FinGen-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 04:08:53.348039 FinGen-0.3.1/
+drwxrwxrwx   0        0        0        0 2023-06-17 04:08:53.338014 FinGen-0.3.1/FinGen/
+-rw-rw-rw-   0        0        0     5492 2023-06-17 04:04:35.000000 FinGen-0.3.1/FinGen/FindingsGenerator.py
+-rw-rw-rw-   0        0        0     1440 2023-02-01 01:25:37.000000 FinGen-0.3.1/FinGen/Loader.py
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:30:43.000000 FinGen-0.3.1/FinGen/__init__.py
+-rw-rw-rw-   0        0        0      196 2023-03-07 02:15:39.000000 FinGen-0.3.1/FinGen/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 04:08:53.348039 FinGen-0.3.1/FinGen.egg-info/
+-rw-rw-rw-   0        0        0      597 2023-06-17 04:08:53.000000 FinGen-0.3.1/FinGen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-17 04:08:53.000000 FinGen-0.3.1/FinGen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 04:08:53.000000 FinGen-0.3.1/FinGen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-17 04:08:53.000000 FinGen-0.3.1/FinGen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-17 04:08:53.000000 FinGen-0.3.1/FinGen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2023-02-01 01:18:31.000000 FinGen-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      597 2023-06-17 04:08:53.348039 FinGen-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-06-17 04:08:53.356064 FinGen-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      716 2023-06-17 04:05:58.000000 FinGen-0.3.1/setup.py
```

### Comparing `FinGen-0.3/FinGen/FindingsGenerator.py` & `FinGen-0.3.1/FinGen/FindingsGenerator.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,17 @@
             loader = Loader("Thinking...", "Thinking... Done!").start()
             prompt = (
                 # Preamble
                 "Write a finding for \"" + title + "\".\n"
 
                 # Description Spec
                 "The description section should contain enough detail to understand the finding and the risk posed to the business.\n"
+                
+                # implication spec
+                "The implication should contain a paragraph outlining the implication of not implementing the finding and how it may impact an organisation"
 
                 # Remediation Spec
                 "The remediation should contain a paragraph outlining how to remediate the finding."
 
                 # Risk Rating Spec
                 "The risk rating is based on the likelihood and impact of exploitation following on the OWASP Risk Rating Methodology." 
             )
@@ -77,28 +80,32 @@
                                     "type": "string",
                                     "description": "Description of the finding"
                                 },
                                 "remediation": {
                                     "type": "string",
                                     "description": "How to fix the finding"
                                 },
+                                "implication": {
+                                    "type": "string",
+                                    "description": "The business implication if the finding isn't fixed"
+                                },
                                 "overall_risk": {
                                     "type": "string",
                                     "enum": ["Informational", "Low", "Medium", "High", "Critical"]
                                 },
                                 "impact": {
                                     "type": "string",
                                     "enum": ["Insignificant", "Minor", "Moderate", "Major", "Very High"]
                                 },
                                 "likelihood": {
                                     "type": "string",
                                     "enum": ["Rare", "Unlikely", "Possible", "Likely", "Almost Certain"]
                                 }
                             },
-                            "required": ["title", "description", "remediation", "overall_risk", "impact", "likelihood"]
+                            "required": ["title", "description", "remediation", "implication", "overall_risk", "impact", "likelihood"]
                         }
                     }
                 ],
                 function_call={"name": "generate_finding"}
             )
             output = json.loads(response.choices[0]["message"]["function_call"]["arguments"])
             loader.stop()
@@ -107,14 +114,17 @@
             print(output["title"])
 
             print("\n----- Description -----")
             print(output["description"])
 
             print("\n----- Remediation -----")
             print(output["remediation"])
+            
+            print("\n----- Implication -----")
+            print(output["implication"])
 
             print("\n----- Risk Rating -----")
             print(output["overall_risk"])
 
             print("\n----- Impact -----")
             print(output["impact"])
```

### Comparing `FinGen-0.3/FinGen/Loader.py` & `FinGen-0.3.1/FinGen/Loader.py`

 * *Files identical despite different names*

### Comparing `FinGen-0.3/FinGen.egg-info/PKG-INFO` & `FinGen-0.3.1/FinGen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinGen
-Version: 0.3
+Version: 0.3.1
 Summary: A penetration testing findings generator using ChatGPT.
 Home-page: https://github.com/Stratus-Security/FinGen
 Author: Stratus Security
 Author-email: contact@stratussecurity.com
 License: GPLv3
 Keywords: ChatGPT,Pentesting,Penetration Testing,Findings Generator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `FinGen-0.3/LICENSE.txt` & `FinGen-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FinGen-0.3/PKG-INFO` & `FinGen-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinGen
-Version: 0.3
+Version: 0.3.1
 Summary: A penetration testing findings generator using ChatGPT.
 Home-page: https://github.com/Stratus-Security/FinGen
 Author: Stratus Security
 Author-email: contact@stratussecurity.com
 License: GPLv3
 Keywords: ChatGPT,Pentesting,Penetration Testing,Findings Generator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `FinGen-0.3/setup.py` & `FinGen-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'FinGen',
   packages = ['FinGen'],
-  version = '0.3',
+  version = '0.3.1',
   license='GPLv3',
   description = 'A penetration testing findings generator using ChatGPT.',
   author = 'Stratus Security',
   author_email = 'contact@stratussecurity.com',
   url = 'https://github.com/Stratus-Security/FinGen',
   keywords = ['ChatGPT', 'Pentesting', 'Penetration Testing', 'Findings Generator'],
   install_requires=[
```

