# Comparing `tmp/openi-beta-0.1.2.tar.gz` & `tmp/openi-beta-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-0.1.2.tar", last modified: Fri Jun 16 06:49:33 2023, max compression
+gzip compressed data, was "openi-beta-0.1.3.tar", last modified: Sat Jun 17 05:12:08 2023, max compression
```

## Comparing `openi-beta-0.1.2.tar` & `openi-beta-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:49:33.690150 openi-beta-0.1.2/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-16 06:49:33.690011 openi-beta-0.1.2/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-16 06:44:09.000000 openi-beta-0.1.2/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-16 06:49:33.690199 openi-beta-0.1.2/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)     1145 2023-06-16 06:49:19.000000 openi-beta-0.1.2/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:49:33.687357 openi-beta-0.1.2/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:49:33.688134 openi-beta-0.1.2/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-16 06:44:09.000000 openi-beta-0.1.2/src/openi/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      358 2023-06-16 06:44:09.000000 openi-beta-0.1.2/src/openi/constants.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:49:33.688624 openi-beta-0.1.2/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-15 09:50:35.000000 openi-beta-0.1.2/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)    10839 2023-06-16 06:48:18.000000 openi-beta-0.1.2/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:49:33.688866 openi-beta-0.1.2/src/openi/utils/
--rw-r--r--   0 jochen10518   (501) staff       (20)      418 2023-06-16 06:44:09.000000 openi-beta-0.1.2/src/openi/utils/logger.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:49:33.689630 openi-beta-0.1.2/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-16 06:49:33.000000 openi-beta-0.1.2/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-16 06:49:33.000000 openi-beta-0.1.2/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-16 06:49:33.000000 openi-beta-0.1.2/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-16 06:49:33.000000 openi-beta-0.1.2/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-16 06:49:33.000000 openi-beta-0.1.2/src/openi_beta.egg-info/top_level.txt
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:49:33.689780 openi-beta-0.1.2/test/
--rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-16 06:44:09.000000 openi-beta-0.1.2/test/test_upload_multi.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-17 05:12:08.418805 openi-beta-0.1.3/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-17 05:12:08.418604 openi-beta-0.1.3/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-16 13:05:18.000000 openi-beta-0.1.3/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-17 05:12:08.419400 openi-beta-0.1.3/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1145 2023-06-17 05:11:58.000000 openi-beta-0.1.3/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-17 05:12:08.415353 openi-beta-0.1.3/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-17 05:12:08.416193 openi-beta-0.1.3/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-16 13:05:18.000000 openi-beta-0.1.3/src/openi/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      357 2023-06-16 17:19:00.000000 openi-beta-0.1.3/src/openi/constants.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-17 05:12:08.416791 openi-beta-0.1.3/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-15 09:50:35.000000 openi-beta-0.1.3/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    13175 2023-06-17 03:46:26.000000 openi-beta-0.1.3/src/openi/dataset/dataset.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-17 05:12:08.417088 openi-beta-0.1.3/src/openi/utils/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      419 2023-06-16 16:05:51.000000 openi-beta-0.1.3/src/openi/utils/logger.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-17 05:12:08.418098 openi-beta-0.1.3/src/openi_beta.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-17 05:12:08.000000 openi-beta-0.1.3/src/openi_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-17 05:12:08.000000 openi-beta-0.1.3/src/openi_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-17 05:12:08.000000 openi-beta-0.1.3/src/openi_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-17 05:12:08.000000 openi-beta-0.1.3/src/openi_beta.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-17 05:12:08.000000 openi-beta-0.1.3/src/openi_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-17 05:12:08.418241 openi-beta-0.1.3/test/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-16 13:05:18.000000 openi-beta-0.1.3/test/test_upload_multi.py
```

### Comparing `openi-beta-0.1.2/PKG-INFO` & `openi-beta-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.1.2
+Version: 0.1.3
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.1.2/README.md` & `openi-beta-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `openi-beta-0.1.2/setup.py` & `openi-beta-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi-beta',
-    version='0.1.2',
+    version='0.1.3',
     description='A test package for openi pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi',
     author='chenzh05',
     author_email='chenzh.ds@outlook.com',
```

### Comparing `openi-beta-0.1.2/src/openi/dataset/dataset.py` & `openi-beta-0.1.3/src/openi/dataset/dataset.py`

 * *Files 26% similar despite different names*

```diff
@@ -48,216 +48,262 @@
         if "\\" in self.filepath:
             self.filename = self.filepath.split("\\")[-1]
         else:
             self.filename = self.filepath.split("/")[-1]
 
         self.size = os.path.getsize(self.filepath)
         self.upload_url = dict()
-
+#FileObject: {self.__dict__}
     """
     APIs implementation
     """
     def getChunks(self):
         params = {
             "access_token": self.token,
             "dataset_id": self.dataset_id,
             "md5": self.md5,
             "file_name": self.filename,
             "type": self.upload_type,
         }
         x = requests.get('{}attachments/get_chunks'.format(self.app_url), params=params)
+
         if x.status_code == 200:
+            logging.info(f'{x.url} {x} {x.reason} | params return: {x.json()}')
             self.upload_id = x.json()["uploadID"]
             self.uuid = x.json()["uuid"]
-            self.uploaded_chunks = x.json()["chunks"]
+            if "datasetName" in x.json():
+                self.datasetName = x.json()["datasetName"]
             if x.json()["uploaded"] == '1':
                 self.uploaded = True
             else:
                 self.uploaded = False
+            try:
+                return [int(i.split('-')[0]) for i in x.json()["chunks"].split(',') if i != '']
+            except:
+                logging.error(f' {x.url} {x} {x.reason} | getChunks.["chunks"] not returned.')
+                raise ValueError(
+                    " f'❌ getChunks failed.")
         else:
-            logging.error(f'{x} {x.reason} {x.text} | FileObject: {self.__dict__}')
+            logging.error(f'{x.url} {x} {x.reason}')
             raise ConnectionRefusedError(
-                f'❌ <{x.status_code} {x.reason}> {x.text}')
+                f'❌ <{x.status_code} {x.reason}>')
 
     def getDatasetID(self):
         params = {"access_token": self.token}
         x = requests.get('{}datasets/{}/{}/'.format(self.app_url, self.username, self.repo), params=params)
         if x.status_code == 200:
             try:
+                logging.info(f'{x.url} {x} {x.reason} | params return: {x.json()}')
                 self.dataset_id = x.json()["data"][0]["id"]
             except Exception as e:
-                logging.error(f'{x} {x.reason} {x.text} | FileObject: {self.__dict__}')
+                logging.error(f'{x.url} {x} {x.reason} | dataset does not exist, please create dataset before uploading files.')
                 raise ValueError(
                     f'❌ repo [{self.username}/{self.repo}]: dataset does not exist, please create dataset before uploading files.')
         else:
-            logging.error(f'{x} {x.reason} | FileObject: {self.__dict__}')
+            logging.error(f'{x.url} {x} {x.reason}')
             raise ConnectionRefusedError(
                 f'❌ <{x.status_code} {x.reason}>')
 
     def newMultipart(self):
         params = {
             "access_token": self.token,
             "dataset_id": self.dataset_id,
             "md5": self.md5,
             "file_name": self.filename,
             "type": self.upload_type,
             "totalChunkCounts": self.total_chunk_counts,
             "size": self.size
         }
         x = requests.get('{}attachments/new_multipart'.format(self.app_url), params=params)
-        if x.json()["result_code"] == "0":
+
+        try:
+        #if x.json()["result_code"] == "0":
+            logging.info(f'{x.url} {x} {x.reason} | params return: {x.json()}')
             self.upload_id = x.json()["uploadID"]
             self.uuid = x.json()["uuid"]
-        else:
-            logging.info(f'{x} {x.reason} {x.json()} | FileObject: {self.__dict__}')
+        #else:
+        except:
+            logging.error(f'{x.url} {x} {x.reason} | {x.json()}')
             raise ConnectionRefusedError(
-                f'❌ <{x.status_code} {x.reason}> {x.json()["msg"]}')
+                f'❌ <{x.status_code} {x.reason}>') # {x.json()["msg"]}')
 
     def getMultipartURL(self, chunk_number, chunk_size):
         params = {
             "access_token": self.token,
             "dataset_id": self.dataset_id,
             "file_name": self.filename,
             "type": self.upload_type,
             "chunkNumber": chunk_number,
             "size": chunk_size,
             "uploadID": self.upload_id,
             "uuid": self.uuid
         }
-        x = requests.get('{}attachments/get_multipart_url'.format(self.app_url), params=params)
-        if x.status_code == 200:
-            self.upload_url[chunk_number] = x.json()["url"]
-        else:
-            logging.error(f'{x} {x.reason} {x.text} | FileObject: {self.__dict__}')
-            raise ConnectionRefusedError(
-                f'❌ <{x.status_code} {x.reason}> {x.text}')
 
-    def putUpload(self, chunk_number, start, chunk_size):
+        retry = 0
+        while retry < 3:
+            try:
+                x = requests.get('{}attachments/get_multipart_url'.format(self.app_url), params=params)
+                if x.status_code == 200:
+                    logging.info(f'{x.url} {x} {x.reason} | params return: {x.json()}')
+                    return x.json()["url"]
+            except:
+                logging.error(f'{x.url} {x} retry={retry+1} {x.reason}')
+                print(f'getMultiUrl chunk [{chunk_number}], retry={retry+1}')
+                retry += 1
+        logging.error(f'{x.url} {x} {x.reason} | reach max retry, getMultiUrl chunk [{chunk_number}] failed.')
+        raise ConnectionRefusedError(
+            f'❌ <{x.status_code} {x.reason}> | getMultiUrl chunk [{chunk_number}] failed.')
+
+    def putUpload(self, url, chunk_number, file_chunk_data):
         headers = {"Content-Type": "text/plain"} if self.upload_type == 0 else {}
-        file_chunk_data = None
-        with open(self.filepath, 'rb') as f:
-            f.seek(start)
-            file_chunk_data = f.read(chunk_size)
-        x = requests.put(self.upload_url[chunk_number], data=file_chunk_data, headers=headers)
-        logging.info(f'putUpload {x} {x.reason} - {self.username}/{self.filename}/{self.cluster} - chunk #{chunk_number}, uploading bytes {start} to {start + chunk_size}')
-        if x.status_code != 200:
-            logging.error(f'{x} {x.reason} {x.text} | FileObject: {self.__dict__}')
-            raise ConnectionRefusedError(
-                f'❌ <{x.status_code} {x.reason}> "upload chunk [{chunk_number}] failed."')
+
+        retry = 0
+        while retry < 3:
+            try:
+                x = requests.put(url, data=file_chunk_data, headers=headers)
+                logging.info(f'{x} {x.reason} {x.url} | etag: {x.headers["ETag"]}')
+                return x.headers["ETag"]
+            except:
+                logging.error(f'{x.url} {x} retry={retry+1} {x.reason} | putUpload chunk [{chunk_number}] failed.')
+                print(f'putUpload chunk [{chunk_number}], retry={retry+1}')
+                retry += 1
+
+        logging.error(f'{x.url} {x} {x.reason} | reach max retry, putUpload chunk [{chunk_number}] failed.')
+        raise ConnectionRefusedError(
+            f'❌ <{x.status_code} {x.reason}> | upload chunk [{chunk_number}] failed.')
 
     def completeMultipart(self):
         params = {
             "access_token": self.token,
             "dataset_id": self.dataset_id,
             "file_name": self.filename,
             "type": self.upload_type,
             "size": self.size,
             "uploadID": self.upload_id,
             "uuid": self.uuid
         }
         x = requests.post('{}attachments/complete_multipart'.format(self.app_url), params=params)
-        logging.info(f'completeMultipart - {x} {x.reason} - {self.username}/{self.filename}/{self.cluster}')
+        logging.info(f'{x.url} {x} {x.reason} | finished completeMultipart | Fileobject: {self.__dict__}')
         if x.status_code != 200:
-            logging.error(f'{x} {x.reason} {x.text} | FileObject: {self.__dict__}')
+            logging.error(f'{x.url} {x} {x.reason} | {x.text}')
             raise ConnectionRefusedError(
                 f'❌ <{x.status_code} {x.reason}> {x.text}')
         if x.json()["result_code"] == "-1":
-            logging.error(f'{x} {x.reason} {x.json()} | FileObject: {self.__dict__}')
+            logging.error(f'{x} {x.reason} | {x.json()}')
             raise ConnectionRefusedError(
                 f'❌ <{x.status_code} {x.reason}> {x.json()["msg"]}')
-
     """
     utils functions
     """
 
-    def stdOut(self, message=""):
-        asctime = datetime.now().strftime("%H:%M:%S")
-        return (f'{asctime}|{self.filename}|{self.cluster}|{message}')
+    def get_time(self, message=""):
+        return datetime.now().strftime("%H:%M:%S")
+        #return (f'{asctime}|{self.filename}|{self.cluster}|{message}')
 
     def filePreprocess(self):
         self.getDatasetID()
         if self.size == 0:
             logging.error(f'[{self.filename}] File size is 0 | FileObject: {self.__dict__}')
             raise ValueError(
                 f'❌ [{self.filename}] File size is 0')
         if self.size > MAX_FILE_SIZE:
             logging.error(f'[{self.filename}] File size exceeds 200GB | FileObject: {self.__dict__}')
             raise ValueError(
                 f'❌ [{self.filename}] File size exceeds 200GB')
 
-        chunk_size = SMALL_FILE_CHUNK_SIZE if self.size < SMALL_FILE_SIZE else LARGE_FILE_CHUNK_SIZE
-        self.total_chunk_counts = math.ceil(self.size / chunk_size)
-        self.chunks = {n: (n - 1) * chunk_size for n in range(1, self.total_chunk_counts + 1)}
+        self.chunk_size = SMALL_FILE_CHUNK_SIZE if self.size < SMALL_FILE_SIZE else LARGE_FILE_CHUNK_SIZE
+        self.total_chunk_counts = math.ceil(self.size / self.chunk_size)
+        #self.chunks = {n: (n - 1) * self.chunk_size for n in range(1, self.total_chunk_counts + 1)}
         self.calculateMD5()
 
     def calculateMD5(self):
-        with open(self.filepath, 'rb') as f:
-            data = f.read()
-        self.md5 = hashlib.md5(data).hexdigest()
+        """
+        计算文件的md5
+        :param self.filepath:
+        :return:
+        """
+        m = hashlib.md5()  # 创建md5对象
+        with open(self.filepath, 'rb') as fobj:
+            while True:
+                data = fobj.read(4096)
+                if not data:
+                    break
+                m.update(data)  # 更新md5对象
+
+        self.md5 = m.hexdigest()  # 返回md5对象
 
     """
     Main functions
     uploadProgressBar(): upload file with progress bar.
     uploadMain(): control flow function.
     """
 
     def uploadProgressBar(self, chunks):
-        u = self.total_chunk_counts - len(chunks)
-
+        _progress = self.chunk_size * (self.total_chunk_counts - len(chunks))
         bar_format = '{desc}{percentage:3.0f}%|{bar}{r_bar}'
-        with tqdm(total=self.size, leave=True, unit='B', unit_scale=True, unit_divisor=1000, desc=self.stdOut(),
-                  bar_format=bar_format) as pbar:
-            chunk_size = SMALL_FILE_CHUNK_SIZE if self.size < SMALL_FILE_SIZE else LARGE_FILE_CHUNK_SIZE
-
-            # checkpoint
-            if u != 0:
-                pbar.update(chunk_size * u)
-
-            # upload chunks
-            for n, v in chunks.items():
-                chunk_size = min(self.size - v, self.size, chunk_size)
-                self.getMultipartURL(n, chunk_size)
-                self.putUpload(n, v, chunk_size)
+        desc = f'{self.get_time()} - Uploading: '
+        with tqdm(total=self.size, leave=True, unit='B', unit_scale=True, unit_divisor=1000, desc=desc,
+                  bar_format=bar_format, initial=_progress) as pbar:
+            for n in chunks:
+                start_position = (n - 1) * self.chunk_size
+                chunk_size = min(self.size, self.chunk_size, self.size - start_position)
+                with open(self.filepath, 'rb') as file:
+                    file.seek(start_position)  # Move the file pointer to the desired start position
+                    data = file.read(chunk_size)  # Read the specified chunk size from the current position
+                url = self.getMultipartURL(n, chunk_size)
+                etag = self.putUpload(url, n, data)
+                if etag is None:
+                    raise RuntimeError(
+                        f'❌ Upload failed: {self.filename}({self.cluster}) '
+                        f'chunk {n} failed to upload.')
                 pbar.update(chunk_size)
-                #logging.info(f"[{self.filename}]: chunk {n} - uploaded bytes {v} to {v+ chunk_size}.")
+                logging.info(f'chunk {n} uploaded. | FileObject: {self.__dict__}')
+
 
     def uploadMain(self):
 
-        print(self.stdOut('dataset file processing & checking...'))
+        print(f'{self.get_time()} - `{self.filename}({self.cluster})` dataset file processing & checking...')
         # preprocess
         self.filePreprocess()
+        logging.info(f'file check finished. | FileObject: {self.__dict__}')
+
         # checking upload status
-        self.getChunks()
+        uploaded_chunks = self.getChunks()
+
 
-        # upload starts
+        #upload starts
         if self.uuid != '':
             if self.uploaded:
-                logging.error(f'Upload failed: [{self.filename} - {self.cluster}], already exists, cannot be uploaded again. | FileObject: {self.__dict__}')
+                logging.error(f'Upload failed: `{self.filename}({self.cluster})` already exists in `{self.datasetName}`, cannot be uploaded again. | FileObject: {self.__dict__}')
                 raise ValueError(
-                    f'❌ Upload failed: [{self.filename} - {self.cluster}], already exists, cannot be uploaded again.')
+                    f'❌ Upload failed: `{self.filename}({self.cluster})` already exists in `{self.datasetName}`, cannot be uploaded again. ')
             else:
-                print(self.stdOut('continue upload...'))
-                uploaded_chunks = [int(i.split('-')[0]) for i in self.uploaded_chunks.split(',') if i != '']
-                continue_chunks = {i: self.chunks[i] for i in self.chunks if i not in uploaded_chunks}
+                # uploaded_chunks = [int(i.split('-')[0]) for i in self.uploaded_chunks.split(',') if i != '']
+                # continue_chunks = {i: self.chunks[i] for i in self.chunks if i not in uploaded_chunks}
                 # re-upload last chunk from checkpoint
-                if uploaded_chunks:
-                    last_chunk_index = max(uploaded_chunks)
-                    continue_chunks[last_chunk_index] = self.chunks[last_chunk_index]
-                continue_chunks = OrderedDict(sorted(continue_chunks.items()))
+                # if uploaded_chunks:
+                #     last_chunk_index = max(uploaded_chunks)
+                #     continue_chunks[last_chunk_index] = self.chunks[last_chunk_index]
+                # continue_chunks = OrderedDict(sorted(continue_chunks.items()))
+                # uploaded_chunks = [int(i.split('-')[0]) for i in self.uploaded_chunks.split(',') if i != '']
+                uploaded_chunks = sorted(uploaded_chunks)[:-1]
+                continue_chunks = [i for i in range(1, self.total_chunk_counts+1) if i not in uploaded_chunks]
+                continue_chunks = sorted(continue_chunks)
                 self.uploadProgressBar(continue_chunks)
 
         else:
-            print(self.stdOut('start new upload...'))
+        #if not self.uploaded:
             self.newMultipart()
-            self.uploadProgressBar(self.chunks)
+            chunks = [i for i in range(1, self.total_chunk_counts + 1)]
+            self.uploadProgressBar(chunks)
 
         self.completeMultipart()
         url = f"{self.app_url.split('api')[0]}{self.username}/{self.repo}/datasets"
-        print(self.stdOut(f'🎉 Successfully uploaded, view on link: {url}'))
-
+        print(f'{self.get_time()} - 🎉 Successfully uploaded, view on link: {url}')
+        logging.info(f'successfully uploaded. | FileObject: {self.__dict__}')
 
 def upload_file(file, username, repository, token, cluster="NPU", app_url=APP_URL):
     d = DatasetUploadFile(
         file=file,
         username=username,
         repository=repository,
         token=token,
```

### Comparing `openi-beta-0.1.2/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-0.1.3/src/openi_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.1.2
+Version: 0.1.3
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.1.2/test/test_upload_multi.py` & `openi-beta-0.1.3/test/test_upload_multi.py`

 * *Files identical despite different names*

