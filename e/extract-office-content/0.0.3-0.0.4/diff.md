# Comparing `tmp/extract_office_content-0.0.3-py3-none-any.whl.zip` & `tmp/extract_office_content-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10458 bytes, number of entries: 11
--rw-r--r--  2.0 unx      227 b- defN 23-Jun-17 00:52 extract_office_content/__init__.py
--rw-r--r--  2.0 unx     4272 b- defN 23-Jun-17 00:52 extract_office_content/extract_excel.py
--rw-r--r--  2.0 unx     3956 b- defN 23-Jun-17 00:52 extract_office_content/extract_ppt.py
--rw-r--r--  2.0 unx     6297 b- defN 23-Jun-17 00:52 extract_office_content/extract_word.py
--rw-r--r--  2.0 unx     2265 b- defN 23-Jun-17 00:52 extract_office_content/main.py
--rw-r--r--  2.0 unx      973 b- defN 23-Jun-17 00:52 extract_office_content/utils.py
--rw-r--r--  2.0 unx     4817 b- defN 23-Jun-17 00:52 extract_office_content-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-17 00:52 extract_office_content-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx      245 b- defN 23-Jun-17 00:52 extract_office_content-0.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-17 00:52 extract_office_content-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1018 b- defN 23-Jun-17 00:52 extract_office_content-0.0.3.dist-info/RECORD
-11 files, 24185 bytes uncompressed, 8696 bytes compressed:  64.0%
+Zip file size: 10708 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      227 b- defN 23-Jun-17 07:05 extract_office_content/__init__.py
+-rw-r--r--  2.0 unx     4475 b- defN 23-Jun-17 07:05 extract_office_content/extract_excel.py
+-rw-r--r--  2.0 unx     4186 b- defN 23-Jun-17 07:05 extract_office_content/extract_ppt.py
+-rw-r--r--  2.0 unx     6492 b- defN 23-Jun-17 07:05 extract_office_content/extract_word.py
+-rw-r--r--  2.0 unx     2265 b- defN 23-Jun-17 07:05 extract_office_content/main.py
+-rw-r--r--  2.0 unx      973 b- defN 23-Jun-17 07:05 extract_office_content/utils.py
+-rw-r--r--  2.0 unx     5316 b- defN 23-Jun-17 07:06 extract_office_content-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-17 07:06 extract_office_content-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx      245 b- defN 23-Jun-17 07:06 extract_office_content-0.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-17 07:06 extract_office_content-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1018 b- defN 23-Jun-17 07:06 extract_office_content-0.0.4.dist-info/RECORD
+11 files, 25312 bytes uncompressed, 8946 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: extract_office_content/main.py
 Comment: 
 
 Filename: extract_office_content/utils.py
 Comment: 
 
-Filename: extract_office_content-0.0.3.dist-info/METADATA
+Filename: extract_office_content-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: extract_office_content-0.0.3.dist-info/WHEEL
+Filename: extract_office_content-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: extract_office_content-0.0.3.dist-info/entry_points.txt
+Filename: extract_office_content-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: extract_office_content-0.0.3.dist-info/top_level.txt
+Filename: extract_office_content-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: extract_office_content-0.0.3.dist-info/RECORD
+Filename: extract_office_content-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## extract_office_content/extract_excel.py

```diff
@@ -1,10 +1,11 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
+from io import BytesIO
 import argparse
 import tempfile
 import uuid
 import warnings
 import zipfile
 from pathlib import Path
 from typing import List, Union
@@ -16,29 +17,33 @@
 from .utils import mkdir
 
 
 class ExtractExcel():
     def __init__(self,):
         self.img_suffix = [".jpg", ".jpeg", ".png", ".bmp"]
 
-    def __call__(self, excel_path: Union[str, Path],
+    def __call__(self, excel_content: Union[str, Path, bytes],
                  out_format: str = 'markdown',
                  save_img_dir: str = None) -> List:
-        if not Path(excel_path).exists():
-            raise FileNotFoundError(f'{excel_path} does not exist.')
 
-        excel_path = str(excel_path)
-        wb = self.unmerge_cell(excel_path)
+        if isinstance(excel_content, (str, Path)):
+            if not Path(excel_content).exists():
+                raise FileNotFoundError(f'{excel_content} does not exist.')
+            excel_content = str(excel_content)
+        elif isinstance(excel_content, bytes):
+            excel_content = BytesIO(excel_content)
+
+        wb = self.unmerge_cell(excel_content)
         data_table = self.extract_table(wb, out_format)
 
         if save_img_dir:
             try:
-                self.extract_imgs(excel_path, save_img_dir)
+                self.extract_imgs(excel_content, save_img_dir)
             except FileExistsError:
-                warnings.warn(f'The {excel_path} does not contain any images.')
+                warnings.warn(f'The {excel_content} does not contain any images.')
 
         return data_table
 
     def unmerge_cell(self, file_name: str) -> Workbook:
         wb = openpyxl.load_workbook(file_name)
         for sheet_name in wb.sheetnames:
             sheet = wb[sheet_name]
@@ -82,19 +87,17 @@
             out_format = f'to_{out_format}'
 
         try:
             return getattr(df_table, out_format)()
         except AttributeError as exc:
             raise AttributeError(f'{out_format} is not supported.') from exc
 
-    def extract_imgs(self, excel_path: str,
+    def extract_imgs(self, excel_content: Union[str, Path, bytes],
                      save_img_dir: Union[str, Path]) -> None:
-        excel_path = Path(excel_path)
-
-        with zipfile.ZipFile(excel_path) as zf:
+        with zipfile.ZipFile(excel_content) as zf:
             file_list = zf.namelist()
 
             img_list = [path for path in file_list
                         if Path(path).suffix in self.img_suffix]
 
             if not img_list:
                 raise FileExistsError('The xl/media is not existed.')
```

## extract_office_content/extract_ppt.py

```diff
@@ -1,10 +1,11 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
+from io import BytesIO
 import argparse
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 import pptx
 from pptx import Presentation
@@ -12,38 +13,41 @@
 from .utils import mkdir
 
 
 class ExtractPPT():
     def __init__(self, ):
         pass
 
-    def __call__(self, ppt_path: str, save_img_dir: str = None) -> List:
+    def __call__(self, ppt_content: Union[str, bytes],
+                 save_img_dir: str = None) -> List:
         """Extract content and images of ppt.
 
         Args:
-            ppt_path (str): the path of ppt.
+            ppt_content (str, bytes): the path of ppt.
             save_img_dir (str, optional): The directory for saving images. Defaults to None.
 
         Returns:
             List: txts from pptx.
         """
-        if not Path(ppt_path).exists():
-            raise FileNotFoundError(f'{ppt_path} does not exist.')
-
-        txts, imgs, charts = self.extract_all(ppt_path)
+        if isinstance(ppt_content, str):
+            if not Path(ppt_content).exists():
+                raise FileNotFoundError(f'{ppt_content} does not exist.')
+        elif isinstance(ppt_content, bytes):
+            ppt_content = BytesIO(ppt_content)
 
+        txts, imgs, charts = self.extract_all(ppt_content)
         if save_img_dir:
             if imgs:
                 self.save_object(imgs, save_img_dir, suffix='png')
 
             if charts:
                 self.save_object(charts, save_img_dir, suffix='xlsx')
         return list(txts.values())
 
-    def extract_all(self, ppt_path: str) -> Tuple[Dict, Dict]:
+    def extract_all(self, ppt_path: Union[str, bytes]) -> Tuple[Dict, Dict]:
         prs = Presentation(ppt_path)
         extract_txts, extract_imgs, extract_charts = {}, {}, {}
         for i, slide in enumerate(prs.slides):
             cur_page = i + 1
             cur_txts, cur_imgs, cur_charts = self.extract_one(slide)
 
             extract_txts[cur_page] = '\n'.join(cur_txts)
```

## extract_office_content/extract_word.py

```diff
@@ -1,44 +1,47 @@
 #! /usr/bin/env python
 # Modified from https://github.com/ankushshah89/python-docx2txt
+from io import BytesIO
 import argparse
-import os
 import re
-import sys
 import xml.etree.ElementTree as ET
 import zipfile
 from pathlib import Path
-import lxml.etree as etree
+from typing import Union
 
 import docx
+import lxml.etree as etree
 import pandas as pd
 from docx.document import Document
 from docx.oxml.table import CT_Tbl
 from docx.table import Table, _Cell
+
 from .utils import is_contain, mkdir
 
 
 class ExtractWord():
     def __init__(self, ):
         self.img_suffix = [".jpg", ".jpeg", ".png", ".bmp"]
         self.nsmap = {
             'w': 'http://schemas.openxmlformats.org/wordprocessingml/2006/main'
         }
         self.extract_table = ExtractWordTable()
         self.parser = etree.XMLParser()
 
-    def __call__(self, docx_path: str, save_img_dir=None):
-        if not Path(docx_path).exists():
-            raise FileNotFoundError(f'{docx_path} does not exist.')
+    def __call__(self, docx_content: Union[str, bytes], save_img_dir=None):
+        if isinstance(docx_content, str) and not Path(docx_content).exists():
+            raise FileNotFoundError(f'{docx_content} does not exist.')
+        elif isinstance(docx_content, bytes):
+            docx_content = BytesIO(docx_content)
 
-        self.table_content = self.extract_table(docx_path)
+        self.table_content = self.extract_table(docx_content)
         text = ''
 
-        # unzip the docx_path in memory
-        zipf = zipfile.ZipFile(docx_path)
+        # unzip the docx_content in memory
+        zipf = zipfile.ZipFile(docx_content)
         filelist = zipf.namelist()
 
         header_files, footer_files, img_files = [], [], []
         header_xmls = 'word/header[0-9]*.xml'
         footer_xmls = 'word/footer[0-9]*.xml'
 
         for fname in filelist:
@@ -119,17 +122,17 @@
         return table_txts
 
 
 class ExtractWordTable():
     def __init__(self,):
         pass
 
-    def __call__(self, docx_path):
+    def __call__(self, docx_content):
         curr_content = []
-        doc = docx.Document(docx_path)
+        doc = docx.Document(docx_content)
         for block in self.iter_block_items(doc):
             if is_contain(block.style.name, ['Table', 'Table Grid']):
                 df = self.get_table_dataframe(block)
                 try:
                     curr_content.append(f'\n{df.to_markdown()}')
                 except:
                     curr_content.append(f'\n{df}')
```

## Comparing `extract_office_content-0.0.3.dist-info/METADATA` & `extract_office_content-0.0.4.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extract-office-content
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool for extracting content from office files.
 Home-page: https://github.com/SWHL/ExtractOfficeText.git
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: extract,office,text,content
 Platform: Any
@@ -98,21 +98,19 @@
 
         $ extract_excel tests/test_files/excel_example.xlsx
         ```
 3. Run by python script.
    - Extract all.
         ```python
         from pathlib import Path
-
         from extract_office_content import ExtractOfficeContent
 
 
         extracter = ExtractOfficeContent()
 
-
         file_list = list(Path('tests/test_files').iterdir())
 
         for file_path in file_list:
             res = extracter(file_path)
             print(res)
         ```
     - Extract Word.
@@ -120,36 +118,51 @@
         from extract_office_content import ExtractWord
 
 
         word_extract = ExtractWord()
 
         word_path = 'tests/test_files/word_example.docx'
         text = word_extract(word_path, "outputs/word")
+
+        # or bytes
+        with open(word_path, 'rb') as f:
+            word_content = f.read()
+        text = word_extract(word_content, "outputs/word")
         print(text)
         ```
     - Extract PPT.
         ```python
         from pathlib import Path
 
         from extract_office_content import ExtractPPT
 
         ppt_extracter = ExtractPPT()
 
         ppt_path = 'tests/test_files/ppt_example.pptx'
         save_dir = 'outputs'
         save_img_dir = Path(save_dir) / Path(ppt_path).stem
         res = ppt_extracter(ppt_path, save_img_dir=str(save_img_dir))
+
+        # or bytes
+        with open(ppt_path, 'rb') as f:
+            ppt_content = f.read()
+        res = ppt_extracter(ppt_content, save_img_dir=str(save_img_dir))
         print(res)
         ```
     - Extract Excel.
         ```python
         from extract_office_content import ExtractExcel
 
         excel_extract = ExtractExcel()
 
         excel_path = 'tests/test_files/excel_with_image.xlsx'
         res  = excel_extract(excel_path, out_format='markdown', save_img_dir='1')
+
+        # or
+        with open(excel_path, 'rb') as f:
+            excel_content = f.read()
+        res  = excel_extract(excel_content, out_format='markdown', save_img_dir='1')
         print(res)
         ```
 
 ### See details for [ExtractOfficeContent](https://github.com/SWHL/ExtractOfficeContent).
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: extract-office-content Version: 0.0.3 Summary: Tool
+Metadata-Version: 2.1 Name: extract-office-content Version: 0.0.4 Summary: Tool
 for extracting content from office files. Home-page: https://github.com/SWHL/
 ExtractOfficeText.git Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Keywords: extract,office,text,content Platform: Any Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Python: >=3.6,<=3.11 Description-Content-Type: text/
@@ -35,17 +35,22 @@
 SAVE_IMG_DIR $ extract_excel tests/test_files/excel_example.xlsx ``` 3. Run by
 python script. - Extract all. ```python from pathlib import Path from
 extract_office_content import ExtractOfficeContent extracter =
 ExtractOfficeContent() file_list = list(Path('tests/test_files').iterdir()) for
 file_path in file_list: res = extracter(file_path) print(res) ``` - Extract
 Word. ```python from extract_office_content import ExtractWord word_extract =
 ExtractWord() word_path = 'tests/test_files/word_example.docx' text =
-word_extract(word_path, "outputs/word") print(text) ``` - Extract PPT.
-```python from pathlib import Path from extract_office_content import
-ExtractPPT ppt_extracter = ExtractPPT() ppt_path = 'tests/test_files/
-ppt_example.pptx' save_dir = 'outputs' save_img_dir = Path(save_dir) / Path
-(ppt_path).stem res = ppt_extracter(ppt_path, save_img_dir=str(save_img_dir))
-print(res) ``` - Extract Excel. ```python from extract_office_content import
-ExtractExcel excel_extract = ExtractExcel() excel_path = 'tests/test_files/
+word_extract(word_path, "outputs/word") # or bytes with open(word_path, 'rb')
+as f: word_content = f.read() text = word_extract(word_content, "outputs/word")
+print(text) ``` - Extract PPT. ```python from pathlib import Path from
+extract_office_content import ExtractPPT ppt_extracter = ExtractPPT() ppt_path
+= 'tests/test_files/ppt_example.pptx' save_dir = 'outputs' save_img_dir = Path
+(save_dir) / Path(ppt_path).stem res = ppt_extracter(ppt_path, save_img_dir=str
+(save_img_dir)) # or bytes with open(ppt_path, 'rb') as f: ppt_content = f.read
+() res = ppt_extracter(ppt_content, save_img_dir=str(save_img_dir)) print(res)
+``` - Extract Excel. ```python from extract_office_content import ExtractExcel
+excel_extract = ExtractExcel() excel_path = 'tests/test_files/
 excel_with_image.xlsx' res = excel_extract(excel_path, out_format='markdown',
-save_img_dir='1') print(res) ``` ### See details for [ExtractOfficeContent]
-(https://github.com/SWHL/ExtractOfficeContent).
+save_img_dir='1') # or with open(excel_path, 'rb') as f: excel_content = f.read
+() res = excel_extract(excel_content, out_format='markdown', save_img_dir='1')
+print(res) ``` ### See details for [ExtractOfficeContent](https://github.com/
+SWHL/ExtractOfficeContent).
```

## Comparing `extract_office_content-0.0.3.dist-info/RECORD` & `extract_office_content-0.0.4.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 extract_office_content/__init__.py,sha256=Ge-pxaPmMXWiBzju-OCsdUwYXM8GLvY56qktBKTO3Xw,227
-extract_office_content/extract_excel.py,sha256=q107vT4nthsJZealOYn2k1jp6zlTcQ2xGsJQHO5Mmi0,4272
-extract_office_content/extract_ppt.py,sha256=lfiLMhV9CSPb8BBAd19hva7NK0dx7CthEeK8HrAHwt8,3956
-extract_office_content/extract_word.py,sha256=xFM0KiAyB4rtOYqrrS6M9JVhsnS_hTV62jBDOkFzJjc,6297
+extract_office_content/extract_excel.py,sha256=vJmR9htMPNA_Dx6wWNngycGtm9IZQvlAEJXmOGxtFmA,4475
+extract_office_content/extract_ppt.py,sha256=Rl_-CyLnh8TQ1Dc6uJgjqvhpHtowlw7gNRjSuK9TPGQ,4186
+extract_office_content/extract_word.py,sha256=FhjWBh9vSMeNc-ECgkAXB8-0uTmHjyImRDgymuO8ZwM,6492
 extract_office_content/main.py,sha256=qj1dl1gnYuCQT-fRoiXL8zkPRxsslImEZQjoORlBX5Y,2265
 extract_office_content/utils.py,sha256=eNm28P-wu9TJRHob-tLrzTrpWJCqzLet73My8T6z1Ec,973
-extract_office_content-0.0.3.dist-info/METADATA,sha256=swjVNxQEKP67wrKOQNoDjibCnB-3QTAet0bjGNDNVIk,4817
-extract_office_content-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-extract_office_content-0.0.3.dist-info/entry_points.txt,sha256=JXiZmmPdeFuKjf78O0nnnTigzul8d99FV6YuamdcI6Y,245
-extract_office_content-0.0.3.dist-info/top_level.txt,sha256=quDoGD7DEfkl_J2tdoeRUbk5H4oKd5-dWIOLRaLB_mc,23
-extract_office_content-0.0.3.dist-info/RECORD,,
+extract_office_content-0.0.4.dist-info/METADATA,sha256=YmRMHIVSwxByzcj_38WW_8vub1ADchFOK3CJ8SPS59g,5316
+extract_office_content-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+extract_office_content-0.0.4.dist-info/entry_points.txt,sha256=JXiZmmPdeFuKjf78O0nnnTigzul8d99FV6YuamdcI6Y,245
+extract_office_content-0.0.4.dist-info/top_level.txt,sha256=quDoGD7DEfkl_J2tdoeRUbk5H4oKd5-dWIOLRaLB_mc,23
+extract_office_content-0.0.4.dist-info/RECORD,,
```

