# Comparing `tmp/delta-sharing-0.6.7.tar.gz` & `tmp/delta-sharing-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/delta-sharing-0.6.7.tar", last modified: Fri Jun  2 19:25:01 2023, max compression
+gzip compressed data, was "delta-sharing-0.7.0.tar", last modified: Thu Jun 15 23:02:17 2023, max compression
```

## Comparing `delta-sharing-0.6.7.tar` & `delta-sharing-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-06-02 19:25:01.000000 delta-sharing-0.6.7/
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2257 2023-06-02 19:25:01.000000 delta-sharing-0.6.7/PKG-INFO
--rw-r--r--   0 lin.zhou   (502) staff       (20)     1201 2023-05-12 09:10:25.000000 delta-sharing-0.6.7/README.md
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-06-02 19:25:01.000000 delta-sharing-0.6.7/delta_sharing/
--rw-r--r--   0 lin.zhou   (502) staff       (20)     1099 2023-05-12 09:10:25.000000 delta-sharing-0.6.7/delta_sharing/__init__.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)      855 2023-05-12 09:10:25.000000 delta-sharing-0.6.7/delta_sharing/_yarl_patch.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)     5066 2023-05-12 09:10:25.000000 delta-sharing-0.6.7/delta_sharing/converter.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)    11137 2023-05-12 09:10:25.000000 delta-sharing-0.6.7/delta_sharing/delta_sharing.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)     7819 2023-05-12 09:10:25.000000 delta-sharing-0.6.7/delta_sharing/protocol.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)     7712 2023-05-12 09:10:25.000000 delta-sharing-0.6.7/delta_sharing/reader.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)    14850 2023-05-12 09:10:25.000000 delta-sharing-0.6.7/delta_sharing/rest_client.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)      626 2023-06-02 19:22:46.000000 delta-sharing-0.6.7/delta_sharing/version.py
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-06-02 19:25:01.000000 delta-sharing-0.6.7/delta_sharing.egg-info/
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2257 2023-06-02 19:25:01.000000 delta-sharing-0.6.7/delta_sharing.egg-info/PKG-INFO
--rw-r--r--   0 lin.zhou   (502) staff       (20)      419 2023-06-02 19:25:01.000000 delta-sharing-0.6.7/delta_sharing.egg-info/SOURCES.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)        1 2023-06-02 19:25:01.000000 delta-sharing-0.6.7/delta_sharing.egg-info/dependency_links.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)      167 2023-06-02 19:25:01.000000 delta-sharing-0.6.7/delta_sharing.egg-info/requires.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)       14 2023-06-02 19:25:01.000000 delta-sharing-0.6.7/delta_sharing.egg-info/top_level.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)       38 2023-06-02 19:25:01.000000 delta-sharing-0.6.7/setup.cfg
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2600 2023-05-12 09:10:25.000000 delta-sharing-0.6.7/setup.py
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-06-15 23:02:17.380104 delta-sharing-0.7.0/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      534 2023-06-14 21:43:09.000000 delta-sharing-0.7.0/NOTICE.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2302 2023-06-15 23:02:17.379963 delta-sharing-0.7.0/PKG-INFO
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     1201 2023-06-14 21:43:09.000000 delta-sharing-0.7.0/README.md
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-06-15 23:02:17.377466 delta-sharing-0.7.0/delta_sharing/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     1274 2023-06-14 21:43:09.000000 delta-sharing-0.7.0/delta_sharing/__init__.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      855 2023-06-14 21:43:09.000000 delta-sharing-0.7.0/delta_sharing/_yarl_patch.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     5066 2023-06-14 21:43:09.000000 delta-sharing-0.7.0/delta_sharing/converter.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)    12923 2023-06-14 21:43:09.000000 delta-sharing-0.7.0/delta_sharing/delta_sharing.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)    10304 2023-06-14 21:43:09.000000 delta-sharing-0.7.0/delta_sharing/protocol.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     7912 2023-06-14 21:43:09.000000 delta-sharing-0.7.0/delta_sharing/reader.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)    16644 2023-06-14 21:43:09.000000 delta-sharing-0.7.0/delta_sharing/rest_client.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      626 2023-06-15 23:01:24.000000 delta-sharing-0.7.0/delta_sharing/version.py
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-06-15 23:02:17.379709 delta-sharing-0.7.0/delta_sharing.egg-info/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2302 2023-06-15 23:02:17.000000 delta-sharing-0.7.0/delta_sharing.egg-info/PKG-INFO
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      430 2023-06-15 23:02:17.000000 delta-sharing-0.7.0/delta_sharing.egg-info/SOURCES.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)        1 2023-06-15 23:02:17.000000 delta-sharing-0.7.0/delta_sharing.egg-info/dependency_links.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      167 2023-06-15 23:02:17.000000 delta-sharing-0.7.0/delta_sharing.egg-info/requires.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)       14 2023-06-15 23:02:17.000000 delta-sharing-0.7.0/delta_sharing.egg-info/top_level.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)       38 2023-06-15 23:02:17.380143 delta-sharing-0.7.0/setup.cfg
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2600 2023-06-14 21:43:09.000000 delta-sharing-0.7.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `delta-sharing-0.6.7/PKG-INFO` & `delta-sharing-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: delta-sharing
-Version: 0.6.7
+Version: 0.7.0
 Summary: Python Connector for Delta Sharing
 Home-page: https://github.com/delta-io/delta-sharing/
 Author: The Delta Lake Project Authors
 Author-email: delta-users@googlegroups.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/delta-io/delta-sharing
 Project-URL: Documentation, https://github.com/delta-io/delta-sharing
 Project-URL: Issues, https://github.com/delta-io/delta-sharing/issues
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -20,14 +21,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: s3
 Provides-Extra: abfs
 Provides-Extra: adl
 Provides-Extra: gcs
 Provides-Extra: gs
+License-File: NOTICE.txt
 
 # Delta Sharing
 
 [Delta Sharing](https://delta.io/sharing) is an open protocol for secure real-time exchange of large datasets, which enables secure data sharing across different computing platforms. It lets organizations share access to existing [Delta Lake](https://delta.io) and [Apache Parquet](https://parquet.apache.org) tables with other organizations, who can then directly read the table in Pandas, Apache Spark, or any other software that implements the open protocol.
 
 This is the Python client library for Delta Sharing, which lets you load shared tables as [pandas](https://pandas.pydata.org/) DataFrames or as [Apache Spark](http://spark.apache.org/) DataFrames if running in PySpark with the [Apache Spark Connector library](https://github.com/delta-io/delta-sharing#set-up-apache-spark).
 
@@ -35,7 +37,9 @@
 
 1. Install using `pip install delta-sharing`.
 2. To use the Python Connector, see [the project docs](https://github.com/delta-io/delta-sharing) for details.
 
 ## Documentation
 
 This README only contains basic information about the Delta Sharing Python Connector. Please read [the project documentation](https://github.com/delta-io/delta-sharing) for full usage details.
+
+
```

### Comparing `delta-sharing-0.6.7/README.md` & `delta-sharing-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.7/delta_sharing/__init__.py` & `delta-sharing-0.7.0/delta_sharing/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,23 +11,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from delta_sharing.delta_sharing import SharingClient, load_as_pandas, load_as_spark
+from delta_sharing.delta_sharing import get_table_metadata, get_table_protocol, get_table_version
 from delta_sharing.delta_sharing import load_table_changes_as_pandas, load_table_changes_as_spark
 from delta_sharing.protocol import Share, Schema, Table
 from delta_sharing.version import __version__
 
 
 __all__ = [
     "SharingClient",
     "Share",
     "Schema",
     "Table",
+    "get_table_metadata",
+    "get_table_protocol",
+    "get_table_version",
     "load_as_pandas",
     "load_as_spark",
     "load_table_changes_as_pandas",
     "load_table_changes_as_spark",
     "__version__",
 ]
```

### Comparing `delta-sharing-0.6.7/delta_sharing/_yarl_patch.py` & `delta-sharing-0.7.0/delta_sharing/_yarl_patch.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.7/delta_sharing/converter.py` & `delta-sharing-0.7.0/delta_sharing/converter.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.7/delta_sharing/delta_sharing.py` & `delta-sharing-0.7.0/delta_sharing/delta_sharing.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 from itertools import chain
 from typing import BinaryIO, List, Optional, Sequence, TextIO, Tuple, Union
 from pathlib import Path
 
 import pandas as pd
 
-from delta_sharing.protocol import CdfOptions
+from delta_sharing.protocol import CdfOptions, Protocol, Metadata
 
 try:
     from pyspark.sql import DataFrame as PySparkDataFrame
 except ImportError:
     pass
 
 from delta_sharing.protocol import DeltaSharingProfile, Schema, Share, Table
@@ -47,14 +47,61 @@
         raise ValueError(f"Invalid 'url': {url}")
     share, schema, table = fragments
     if len(profile) == 0 or len(share) == 0 or len(schema) == 0 or len(table) == 0:
         raise ValueError(f"Invalid 'url': {url}")
     return (profile, share, schema, table)
 
 
+def get_table_version(
+    url: str,
+    starting_timestamp: Optional[str] = None
+) -> int:
+    """
+    Get the shared table version using the given url.
+
+    :param url: a url under the format "<profile>#<share>.<schema>.<table>"
+    :param starting_timestamp: a string in the format of YYYY-MM-DDThh:mm:ssZ. Get the version at or
+      after the given timestamp. The latest table version will be returned if this is not specified.
+    """
+    profile_json, share, schema, table = _parse_url(url)
+    profile = DeltaSharingProfile.read_from_file(profile_json)
+    rest_client = DataSharingRestClient(profile)
+    response = rest_client.query_table_version(
+        Table(name=table, share=share, schema=schema),
+        starting_timestamp
+    )
+    return response.delta_table_version
+
+
+def get_table_protocol(url: str) -> Protocol:
+    """
+    Get the shared table protocol using the given url.
+
+    :param url: a url under the format "<profile>#<share>.<schema>.<table>"
+    """
+    profile_json, share, schema, table = _parse_url(url)
+    profile = DeltaSharingProfile.read_from_file(profile_json)
+    rest_client = DataSharingRestClient(profile)
+    response = rest_client.query_table_metadata(Table(name=table, share=share, schema=schema))
+    return response.protocol
+
+
+def get_table_metadata(url: str) -> Metadata:
+    """
+    Get the shared table metadata using the given url.
+
+    :param url: a url under the format "<profile>#<share>.<schema>.<table>"
+    """
+    profile_json, share, schema, table = _parse_url(url)
+    profile = DeltaSharingProfile.read_from_file(profile_json)
+    rest_client = DataSharingRestClient(profile)
+    response = rest_client.query_table_metadata(Table(name=table, share=share, schema=schema))
+    return response.metadata
+
+
 def load_as_pandas(
     url: str,
     limit: Optional[int] = None,
     version: Optional[int] = None,
     timestamp: Optional[str] = None
 ) -> pd.DataFrame:
     """
```

### Comparing `delta-sharing-0.6.7/delta_sharing/protocol.py` & `delta-sharing-0.7.0/delta_sharing/protocol.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,20 +19,26 @@
 from typing import ClassVar, Dict, IO, Optional, Sequence, Union
 
 import fsspec
 
 
 @dataclass(frozen=True)
 class DeltaSharingProfile:
-    CURRENT: ClassVar[int] = 1
+    CURRENT: ClassVar[int] = 2
 
     share_credentials_version: int
     endpoint: str
-    bearer_token: str
+    bearer_token: Optional[str] = None
     expiration_time: Optional[str] = None
+    type: Optional[str] = None
+    token_endpoint: Optional[str] = None
+    client_id: Optional[str] = None
+    client_secret: Optional[str] = None
+    username: Optional[str] = None
+    password: Optional[str] = None
 
     def __post_init__(self):
         if self.share_credentials_version > DeltaSharingProfile.CURRENT:
             raise ValueError(
                 "'shareCredentialsVersion' in the profile is "
                 f"{self.share_credentials_version} which is too new. "
                 f"The current release supports version {DeltaSharingProfile.CURRENT} and below. "
@@ -52,24 +58,68 @@
         finally:
             infile.close()
 
     @staticmethod
     def from_json(json) -> "DeltaSharingProfile":
         if isinstance(json, (str, bytes, bytearray)):
             json = loads(json)
+
+        share_credentials_version = int(json["shareCredentialsVersion"])
         endpoint = json["endpoint"]
-        if endpoint.endswith("/"):
+        if endpoint is not None and endpoint.endswith("/"):
             endpoint = endpoint[:-1]
-        expiration_time = json.get("expirationTime")
-        return DeltaSharingProfile(
-            share_credentials_version=int(json["shareCredentialsVersion"]),
-            endpoint=endpoint,
-            bearer_token=json["bearerToken"],
-            expiration_time=expiration_time,
-        )
+
+        if share_credentials_version == 1:
+            return DeltaSharingProfile(
+                share_credentials_version=share_credentials_version,
+                endpoint=endpoint,
+                bearer_token=json["bearerToken"],
+                expiration_time=json.get("expirationTime"),
+            )
+        elif share_credentials_version == 2:
+            type = json["type"]
+            if type == "persistent_oauth2.0":
+                token_endpoint = json["tokenEndpoint"]
+                if token_endpoint is not None and token_endpoint.endswith("/"):
+                    token_endpoint = token_endpoint[:-1]
+                return DeltaSharingProfile(
+                    share_credentials_version=share_credentials_version,
+                    type=type,
+                    endpoint=endpoint,
+                    token_endpoint=token_endpoint,
+                    client_id=json["clientId"],
+                    client_secret=json["clientSecret"],
+                )
+            elif type == "bearer_token":
+                return DeltaSharingProfile(
+                    share_credentials_version=share_credentials_version,
+                    type=type,
+                    endpoint=endpoint,
+                    bearer_token=json["bearerToken"],
+                    expiration_time=json.get("expirationTime")
+                )
+            elif type == "basic":
+                return DeltaSharingProfile(
+                    share_credentials_version=share_credentials_version,
+                    type=type,
+                    endpoint=endpoint,
+                    username=json["username"],
+                    password=json["password"],
+                )
+            else:
+                raise ValueError(
+                    "The current release does not supports {type} type. "
+                    "Please check type.")
+        else:
+            raise ValueError(
+                "'shareCredentialsVersion' in the profile is "
+                f"{share_credentials_version} which is too new. "
+                f"The current release supports version {DeltaSharingProfile.CURRENT} and below. "
+                "Please upgrade to a newer release."
+            )
 
 
 @dataclass(frozen=True)
 class Share:
     name: str
 
     @staticmethod
@@ -97,15 +147,16 @@
     share: str
     schema: str
 
     @staticmethod
     def from_json(json) -> "Table":
         if isinstance(json, (str, bytes, bytearray)):
             json = loads(json)
-        return Table(name=json["name"], share=json["share"], schema=json["schema"])
+        return Table(name=json["name"], share=json["share"],
+                     schema=json["schema"])
 
 
 @dataclass(frozen=True)
 class Protocol:
     CURRENT: ClassVar[int] = 1
 
     min_reader_version: int
@@ -142,14 +193,17 @@
     id: Optional[str] = None
     name: Optional[str] = None
     description: Optional[str] = None
     format: Format = field(default_factory=Format)
     schema_string: Optional[str] = None
     configuration: Dict[str, str] = field(default_factory=dict)
     partition_columns: Sequence[str] = field(default_factory=list)
+    version: Optional[int] = None
+    size: Optional[int] = None
+    num_files: Optional[int] = None
 
     @staticmethod
     def from_json(json) -> "Metadata":
         if isinstance(json, (str, bytes, bytearray)):
             json = loads(json)
         if "configuration" in json:
             configuration = json["configuration"]
@@ -159,14 +213,17 @@
             id=json["id"],
             name=json.get("name", None),
             description=json.get("description", None),
             format=Format.from_json(json["format"]),
             schema_string=json["schemaString"],
             configuration=configuration,
             partition_columns=json["partitionColumns"],
+            version=json.get("version", None),
+            size=json.get("size", None),
+            num_files=json.get("numFiles", None)
         )
 
 
 @dataclass(frozen=True)
 class FileAction:
     url: str
     id: str
```

### Comparing `delta-sharing-0.6.7/delta_sharing/reader.py` & `delta-sharing-0.7.0/delta_sharing/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from typing import Any, Callable, Dict, Optional, Sequence
 from urllib.parse import urlparse
 from json import loads
+from urllib.request import getproxies
 
 import fsspec
 import pandas as pd
 from pyarrow.dataset import dataset
 
 from delta_sharing.converter import to_converters, get_empty_table
 from delta_sharing.protocol import AddCdcFile, CdfOptions, FileAction, Table
@@ -154,15 +155,19 @@
     ) -> pd.DataFrame:
         url = urlparse(action.url)
         if "storage.googleapis.com" in (url.netloc.lower()):
             # Apply the yarl patch for GCS pre-signed urls
             import delta_sharing._yarl_patch  # noqa: F401
 
         protocol = url.scheme
-        filesystem = fsspec.filesystem(protocol)
+        proxy = getproxies()
+        if len(proxy) != 0:
+            filesystem = fsspec.filesystem(protocol, client_kwargs={"trust_env":True})
+        else:
+            filesystem = fsspec.filesystem(protocol)
 
         pa_dataset = dataset(source=action.url, format="parquet", filesystem=filesystem)
         pa_table = pa_dataset.head(limit) if limit is not None else pa_dataset.to_table()
         pdf = pa_table.to_pandas(
             date_as_object=True, use_threads=False, split_blocks=True, self_destruct=True
         )
```

### Comparing `delta-sharing-0.6.7/delta_sharing/rest_client.py` & `delta-sharing-0.7.0/delta_sharing/rest_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -139,24 +139,73 @@
 class DataSharingRestClient:
     USER_AGENT: ClassVar[str] = _client_user_agent()
 
     def __init__(self, profile: DeltaSharingProfile, num_retries=10):
         self._profile = profile
         self._num_retries = num_retries
         self._sleeper = lambda sleep_ms: time.sleep(sleep_ms / 1000)
+        self.auth_session(profile)
 
+    def auth_session(self, profile):
         self._session = requests.Session()
+        self.__auth_broker(profile)
+        if urlparse(profile.endpoint).hostname == "localhost":
+            self._session.verify = False
+
+    def __auth_broker(self, profile):
+        if profile.share_credentials_version == 2:
+            if profile.type == "persistent_oauth2.0":
+                self.__auth_persistent_oauth2(profile)
+            elif profile.type == "bearer_token":
+                self.__auth_bearer_token(profile)
+            elif profile.type == "basic":
+                self.__auth_basic(profile)
+            else:
+                self.__auth_bearer_token(profile)
+        else:
+            self.__auth_bearer_token(profile)
+
+    def __auth_bearer_token(self, profile):
         self._session.headers.update(
             {
                 "Authorization": f"Bearer {profile.bearer_token}",
                 "User-Agent": DataSharingRestClient.USER_AGENT,
             }
         )
-        if urlparse(profile.endpoint).hostname == "localhost":
-            self._session.verify = False
+
+    def __auth_persistent_oauth2(self, profile):
+        headers = {"Content-Type": "application/x-www-form-urlencoded",
+                   "Accept": "application/json"}
+
+        response = requests.post(profile.token_endpoint,
+                                 data={"grant_type": "client_credentials"},
+                                 headers=headers,
+                                 auth=(profile.client_id,
+                                       profile.client_secret),)
+
+        bearer_token = "{}".format(response.json()["access_token"])
+
+        self._session.headers.update(
+            {
+                "Authorization": f"Bearer {bearer_token}",
+                "User-Agent": DataSharingRestClient.USER_AGENT,
+            }
+        )
+
+    def __auth_basic(self, profile):
+        self._session.auth = (profile.username, profile.password)
+
+        response = self._session.post(profile.endpoint,
+                                      data={"grant_type": "client_credentials"},)
+
+        self._session.headers.update(
+            {
+                "User-Agent": DataSharingRestClient.USER_AGENT,
+            }
+        )
 
     @retry_with_exponential_backoff
     def list_shares(
         self, *, max_results: Optional[int] = None, page_token: Optional[str] = None
     ) -> ListSharesResponse:
         data: Dict = {}
         if max_results is not None:
```

### Comparing `delta-sharing-0.6.7/delta_sharing/version.py` & `delta-sharing-0.7.0/delta_sharing/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.6.7"
+__version__ = "0.7.0"
```

### Comparing `delta-sharing-0.6.7/delta_sharing.egg-info/PKG-INFO` & `delta-sharing-0.7.0/delta_sharing.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: delta-sharing
-Version: 0.6.7
+Version: 0.7.0
 Summary: Python Connector for Delta Sharing
 Home-page: https://github.com/delta-io/delta-sharing/
 Author: The Delta Lake Project Authors
 Author-email: delta-users@googlegroups.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/delta-io/delta-sharing
 Project-URL: Documentation, https://github.com/delta-io/delta-sharing
 Project-URL: Issues, https://github.com/delta-io/delta-sharing/issues
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -20,14 +21,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: s3
 Provides-Extra: abfs
 Provides-Extra: adl
 Provides-Extra: gcs
 Provides-Extra: gs
+License-File: NOTICE.txt
 
 # Delta Sharing
 
 [Delta Sharing](https://delta.io/sharing) is an open protocol for secure real-time exchange of large datasets, which enables secure data sharing across different computing platforms. It lets organizations share access to existing [Delta Lake](https://delta.io) and [Apache Parquet](https://parquet.apache.org) tables with other organizations, who can then directly read the table in Pandas, Apache Spark, or any other software that implements the open protocol.
 
 This is the Python client library for Delta Sharing, which lets you load shared tables as [pandas](https://pandas.pydata.org/) DataFrames or as [Apache Spark](http://spark.apache.org/) DataFrames if running in PySpark with the [Apache Spark Connector library](https://github.com/delta-io/delta-sharing#set-up-apache-spark).
 
@@ -35,7 +37,9 @@
 
 1. Install using `pip install delta-sharing`.
 2. To use the Python Connector, see [the project docs](https://github.com/delta-io/delta-sharing) for details.
 
 ## Documentation
 
 This README only contains basic information about the Delta Sharing Python Connector. Please read [the project documentation](https://github.com/delta-io/delta-sharing) for full usage details.
+
+
```

### Comparing `delta-sharing-0.6.7/setup.py` & `delta-sharing-0.7.0/setup.py`

 * *Files identical despite different names*

