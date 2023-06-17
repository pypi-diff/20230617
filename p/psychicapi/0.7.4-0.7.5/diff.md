# Comparing `tmp/psychicapi-0.7.4.tar.gz` & `tmp/psychicapi-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/psychicapi-0.7.4.tar", last modified: Mon Jun 12 17:06:53 2023, max compression
+gzip compressed data, was "dist/psychicapi-0.7.5.tar", last modified: Sat Jun 17 07:29:42 2023, max compression
```

## Comparing `psychicapi-0.7.4.tar` & `psychicapi-0.7.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-12 17:06:53.000000 psychicapi-0.7.4/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4225 2023-06-12 17:06:53.000000 psychicapi-0.7.4/PKG-INFO
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-12 17:06:53.000000 psychicapi-0.7.4/psychicapi/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       65 2023-06-12 16:34:35.000000 psychicapi-0.7.4/psychicapi/__init__.py
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     6162 2023-06-12 16:52:37.000000 psychicapi-0.7.4/psychicapi/psychic.py
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     3276 2023-06-12 17:05:18.000000 psychicapi-0.7.4/README.md
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      648 2023-06-12 17:06:50.000000 psychicapi-0.7.4/setup.py
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-12 17:06:53.000000 psychicapi-0.7.4/psychicapi.egg-info/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4225 2023-06-12 17:06:53.000000 psychicapi-0.7.4/psychicapi.egg-info/PKG-INFO
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-06-12 17:06:53.000000 psychicapi-0.7.4/psychicapi.egg-info/SOURCES.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-06-12 17:06:53.000000 psychicapi-0.7.4/psychicapi.egg-info/requires.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-06-12 17:06:53.000000 psychicapi-0.7.4/psychicapi.egg-info/top_level.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-06-12 17:06:53.000000 psychicapi-0.7.4/psychicapi.egg-info/dependency_links.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-06-12 17:06:53.000000 psychicapi-0.7.4/setup.cfg
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-17 07:29:42.000000 psychicapi-0.7.5/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4412 2023-06-17 07:29:42.000000 psychicapi-0.7.5/PKG-INFO
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-17 07:29:42.000000 psychicapi-0.7.5/psychicapi/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       65 2023-06-12 16:34:35.000000 psychicapi-0.7.5/psychicapi/__init__.py
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     6477 2023-06-16 23:11:57.000000 psychicapi-0.7.5/psychicapi/psychic.py
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     3399 2023-06-12 19:04:35.000000 psychicapi-0.7.5/README.md
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      648 2023-06-16 23:25:17.000000 psychicapi-0.7.5/setup.py
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-17 07:29:42.000000 psychicapi-0.7.5/psychicapi.egg-info/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4412 2023-06-17 07:29:42.000000 psychicapi-0.7.5/psychicapi.egg-info/PKG-INFO
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-06-17 07:29:42.000000 psychicapi-0.7.5/psychicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-06-17 07:29:42.000000 psychicapi-0.7.5/psychicapi.egg-info/requires.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-06-17 07:29:42.000000 psychicapi-0.7.5/psychicapi.egg-info/top_level.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-06-17 07:29:42.000000 psychicapi-0.7.5/psychicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-06-17 07:29:42.000000 psychicapi-0.7.5/setup.cfg
```

### Comparing `psychicapi-0.7.4/PKG-INFO` & `psychicapi-0.7.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.7.4
+Version: 0.7.5
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Home-page: UNKNOWN
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 License: UNKNOWN
 Description: # Psychic
         
@@ -38,17 +38,17 @@
         
         ### Retrieve documents from a connection
         
         ```
         docs = psychic.get_documents(account_id="account_id")
         ```
         
-        ### Advanced Filtering
+        ## Advanced Filtering
         
-        #### Filtering by section(s)
+        ### Filtering by section(s)
         
         Most file storage, CRM and helpdesk apps have documents organized in sections. Confluence calls them spaces, Zendesk calls them  sections, Google Drive calls them folders. Psychic allows you to define filters based on these sections using the `SectionFilter` class. You can define and query sections as follows:
         
         ```
         from psychicapi import Psychic, ConnectorId, Section, SectionFilter
         
         client = Psychic("YOUR-SECRET-KEY")
@@ -68,21 +68,29 @@
         # add the section filter to the connection
         client.add_section_filter(connector_id=ConnectorId.notion, account_id="test", section_filter=filter)
         
         # get documents from the sections in the filter
         client.get_documents(account_id="test", connector_id=ConnectorId.notion, section_filter_id="index1")
         ```
         
-        #### Filtering by uri
+        ### Filtering by uri
         
         Every document returned by Psychic has a uri. If you want to query a document by uri instead of retrieving all documents in a connection, you can use the optional `uris` parameter in `get_documents`
         
         
         ```
         client.get_documents(
             account_id="test", 
             connector_id=ConnectorId.notion, 
             uris=["https://docs.google.com/document/d/document-id-1/edit?usp=drivesdk", "https://drive.google.com/file/d/document-id-2/view?usp=drivesdk"]
         )
         ```
+        ## Local development
+        
+        To run the python package locally, use the following command:
+        
+        ```
+        pip install -e /path/to/package
+        ```
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `psychicapi-0.7.4/psychicapi/psychic.py` & `psychicapi-0.7.5/psychicapi/psychic.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,29 @@
 class ConnectorId(Enum):
     notion = "notion"
     confluence = "confluence"
     zendesk = "zendesk"
     gdrive = "gdrive"
     slack = "slack"
 
+class SectionType(str, Enum):
+    folder = "folder"
+    document = "document"
+
 class Section:
     id: str
     name: str
+    type: SectionType
+    children: Optional[List["Section"]] = None
 
-    def __init__(self, id: str, name: str) -> None:
+    def __init__(self, id: str, name: str, type: SectionType, children: Optional[List["Section"]] = None) -> None:
         self.id = id
         self.name = name
+        self.type = type
+        self.children = children
 
 class SectionFilter:
     id: str
     sections: List[Section]
 
     def __init__(self, id: str, sections: List[Section]) -> None:
         self.id = id
@@ -121,15 +129,16 @@
             "connector_id": connector_id.value,
             "account_id": account_id,
             "section_filter": {
                 "id": section_filter.id,
                 "sections": [
                     {
                         "id": section.id,
-                        "name": section.name
+                        "name": section.name,
+                        "type": section.type
                     }
                     for section in section_filter.sections
                 ]
             }    
         }
         response = requests.post(
             self.api_url + "add-section-filter",
```

### Comparing `psychicapi-0.7.4/README.md` & `psychicapi-0.7.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 
 ### Retrieve documents from a connection
 
 ```
 docs = psychic.get_documents(account_id="account_id")
 ```
 
-### Advanced Filtering
+## Advanced Filtering
 
-#### Filtering by section(s)
+### Filtering by section(s)
 
 Most file storage, CRM and helpdesk apps have documents organized in sections. Confluence calls them spaces, Zendesk calls them  sections, Google Drive calls them folders. Psychic allows you to define filters based on these sections using the `SectionFilter` class. You can define and query sections as follows:
 
 ```
 from psychicapi import Psychic, ConnectorId, Section, SectionFilter
 
 client = Psychic("YOUR-SECRET-KEY")
@@ -60,19 +60,26 @@
 # add the section filter to the connection
 client.add_section_filter(connector_id=ConnectorId.notion, account_id="test", section_filter=filter)
 
 # get documents from the sections in the filter
 client.get_documents(account_id="test", connector_id=ConnectorId.notion, section_filter_id="index1")
 ```
 
-#### Filtering by uri
+### Filtering by uri
 
 Every document returned by Psychic has a uri. If you want to query a document by uri instead of retrieving all documents in a connection, you can use the optional `uris` parameter in `get_documents`
 
 
 ```
 client.get_documents(
     account_id="test", 
     connector_id=ConnectorId.notion, 
     uris=["https://docs.google.com/document/d/document-id-1/edit?usp=drivesdk", "https://drive.google.com/file/d/document-id-2/view?usp=drivesdk"]
 )
-```
+```
+## Local development
+
+To run the python package locally, use the following command:
+
+```
+pip install -e /path/to/package
+```
```

### Comparing `psychicapi-0.7.4/setup.py` & `psychicapi-0.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='psychicapi',
-    version='0.7.4',
+    version='0.7.5',
     description='Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayan Bandyopadhyay',
     author_email='ayan@psychic.dev',
     packages=['psychicapi'],
     install_requires=[
```

### Comparing `psychicapi-0.7.4/psychicapi.egg-info/PKG-INFO` & `psychicapi-0.7.5/psychicapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.7.4
+Version: 0.7.5
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Home-page: UNKNOWN
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 License: UNKNOWN
 Description: # Psychic
         
@@ -38,17 +38,17 @@
         
         ### Retrieve documents from a connection
         
         ```
         docs = psychic.get_documents(account_id="account_id")
         ```
         
-        ### Advanced Filtering
+        ## Advanced Filtering
         
-        #### Filtering by section(s)
+        ### Filtering by section(s)
         
         Most file storage, CRM and helpdesk apps have documents organized in sections. Confluence calls them spaces, Zendesk calls them  sections, Google Drive calls them folders. Psychic allows you to define filters based on these sections using the `SectionFilter` class. You can define and query sections as follows:
         
         ```
         from psychicapi import Psychic, ConnectorId, Section, SectionFilter
         
         client = Psychic("YOUR-SECRET-KEY")
@@ -68,21 +68,29 @@
         # add the section filter to the connection
         client.add_section_filter(connector_id=ConnectorId.notion, account_id="test", section_filter=filter)
         
         # get documents from the sections in the filter
         client.get_documents(account_id="test", connector_id=ConnectorId.notion, section_filter_id="index1")
         ```
         
-        #### Filtering by uri
+        ### Filtering by uri
         
         Every document returned by Psychic has a uri. If you want to query a document by uri instead of retrieving all documents in a connection, you can use the optional `uris` parameter in `get_documents`
         
         
         ```
         client.get_documents(
             account_id="test", 
             connector_id=ConnectorId.notion, 
             uris=["https://docs.google.com/document/d/document-id-1/edit?usp=drivesdk", "https://drive.google.com/file/d/document-id-2/view?usp=drivesdk"]
         )
         ```
+        ## Local development
+        
+        To run the python package locally, use the following command:
+        
+        ```
+        pip install -e /path/to/package
+        ```
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

