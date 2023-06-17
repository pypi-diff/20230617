# Comparing `tmp/extract_office_content-0.0.2-py3-none-any.whl.zip` & `tmp/extract_office_content-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10336 bytes, number of entries: 11
--rw-r--r--  2.0 unx      227 b- defN 23-Jun-09 07:00 extract_office_content/__init__.py
--rw-r--r--  2.0 unx     4272 b- defN 23-Jun-09 07:00 extract_office_content/extract_excel.py
--rw-r--r--  2.0 unx     3553 b- defN 23-Jun-09 07:00 extract_office_content/extract_ppt.py
--rw-r--r--  2.0 unx     6297 b- defN 23-Jun-09 07:00 extract_office_content/extract_word.py
--rw-r--r--  2.0 unx     2273 b- defN 23-Jun-09 07:00 extract_office_content/main.py
--rw-r--r--  2.0 unx      973 b- defN 23-Jun-09 07:00 extract_office_content/utils.py
--rw-r--r--  2.0 unx     4758 b- defN 23-Jun-09 07:00 extract_office_content-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 07:00 extract_office_content-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      245 b- defN 23-Jun-09 07:00 extract_office_content-0.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-09 07:00 extract_office_content-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1018 b- defN 23-Jun-09 07:00 extract_office_content-0.0.2.dist-info/RECORD
-11 files, 23731 bytes uncompressed, 8574 bytes compressed:  63.9%
+Zip file size: 10458 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      227 b- defN 23-Jun-17 00:52 extract_office_content/__init__.py
+-rw-r--r--  2.0 unx     4272 b- defN 23-Jun-17 00:52 extract_office_content/extract_excel.py
+-rw-r--r--  2.0 unx     3956 b- defN 23-Jun-17 00:52 extract_office_content/extract_ppt.py
+-rw-r--r--  2.0 unx     6297 b- defN 23-Jun-17 00:52 extract_office_content/extract_word.py
+-rw-r--r--  2.0 unx     2265 b- defN 23-Jun-17 00:52 extract_office_content/main.py
+-rw-r--r--  2.0 unx      973 b- defN 23-Jun-17 00:52 extract_office_content/utils.py
+-rw-r--r--  2.0 unx     4817 b- defN 23-Jun-17 00:52 extract_office_content-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-17 00:52 extract_office_content-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      245 b- defN 23-Jun-17 00:52 extract_office_content-0.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-17 00:52 extract_office_content-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1018 b- defN 23-Jun-17 00:52 extract_office_content-0.0.3.dist-info/RECORD
+11 files, 24185 bytes uncompressed, 8696 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: extract_office_content/main.py
 Comment: 
 
 Filename: extract_office_content/utils.py
 Comment: 
 
-Filename: extract_office_content-0.0.2.dist-info/METADATA
+Filename: extract_office_content-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: extract_office_content-0.0.2.dist-info/WHEEL
+Filename: extract_office_content-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: extract_office_content-0.0.2.dist-info/entry_points.txt
+Filename: extract_office_content-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: extract_office_content-0.0.2.dist-info/top_level.txt
+Filename: extract_office_content-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: extract_office_content-0.0.2.dist-info/RECORD
+Filename: extract_office_content-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## extract_office_content/extract_ppt.py

```diff
@@ -25,50 +25,55 @@
 
         Returns:
             List: txts from pptx.
         """
         if not Path(ppt_path).exists():
             raise FileNotFoundError(f'{ppt_path} does not exist.')
 
-        txts, imgs = self.extract_all(ppt_path)
+        txts, imgs, charts = self.extract_all(ppt_path)
 
         if save_img_dir:
-            self.save_img(imgs, save_img_dir)
+            if imgs:
+                self.save_object(imgs, save_img_dir, suffix='png')
+
+            if charts:
+                self.save_object(charts, save_img_dir, suffix='xlsx')
         return list(txts.values())
 
     def extract_all(self, ppt_path: str) -> Tuple[Dict, Dict]:
         prs = Presentation(ppt_path)
-        extract_txts, extract_imgs = {}, {}
+        extract_txts, extract_imgs, extract_charts = {}, {}, {}
         for i, slide in enumerate(prs.slides):
             cur_page = i + 1
-            cur_txts, cur_imgs = self.extract_one(slide)
+            cur_txts, cur_imgs, cur_charts = self.extract_one(slide)
 
             extract_txts[cur_page] = '\n'.join(cur_txts)
-            for cur_img in cur_imgs:
-                extract_imgs.setdefault(cur_page, []).append(cur_img)
-        return extract_txts, extract_imgs
+            extract_imgs.update({cur_page: cur_imgs})
+            extract_charts.update({cur_page: cur_charts})
+        return extract_txts, extract_imgs, extract_charts
 
-    def extract_one(self, slide: pptx.slide.Slide) -> List:
-        cur_page_content, cur_page_imgs = [], []
+    def extract_one(self, slide: pptx.slide.Slide) -> Tuple[List, List, List]:
+        cur_page_content, cur_page_imgs, cur_page_charts = [], [], []
         for shape in slide.shapes:
             if shape.has_text_frame:
                 txt = self.extract_text(shape.text)
                 if txt:
                     cur_page_content.append(txt)
             elif shape.has_table:
                 table_str = self.extract_table(shape.table)
                 cur_page_content.append(table_str)
             elif shape.has_chart:
-                pass
+                excel_bytes = shape.chart.part.chart_workbook.xlsx_part.blob
+                cur_page_charts.append(excel_bytes)
             elif hasattr(shape, 'image'):
                 img_bytes = self.extract_image(shape.image)
                 cur_page_imgs.append(img_bytes)
             else:
                 pass
-        return cur_page_content, cur_page_imgs
+        return cur_page_content, cur_page_imgs, cur_page_charts
 
     @staticmethod
     def extract_text(shape_text: str) -> Optional[str]:
         txt = shape_text.strip()
         if txt:
             return txt
         return None
@@ -78,26 +83,27 @@
         table_list = []
         for one_row in table_value.rows:
             each = ''
             for cell in one_row.cells:
                 each += cell.text_frame.text + ','
             table_list.append(each)
         table_df = pd.DataFrame(table_list)
-        return table_df.to_string()
+        return table_df.to_markdown(index=None)
 
     @staticmethod
     def extract_image(img_value: pptx.parts.image.Image) -> bytes:
         return img_value.blob
 
     @staticmethod
-    def save_img(imgs: Dict, save_img_dir: Union[str, Path]) -> None:
-        mkdir(save_img_dir)
-        for page_num, img_list in imgs.items():
-            for i, img in enumerate(img_list):
-                save_full_path = Path(save_img_dir) / f'{page_num}_{i+1}.png'
+    def save_object(objs: Dict,
+                    save_dir: Union[str, Path], suffix: str) -> None:
+        mkdir(save_dir)
+        for page_num, obj_list in objs.items():
+            for i, img in enumerate(obj_list):
+                save_full_path = Path(save_dir) / f'{page_num}_{i+1}.{suffix}'
                 with open(str(save_full_path), 'wb') as f:
                     f.write(img)
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('ppt_path', type=str)
```

## extract_office_content/main.py

```diff
@@ -14,28 +14,28 @@
 class ExtractOfficeContent():
     def __init__(self) -> None:
         self.excel = ExtractExcel()
         self.ppt = ExtractPPT()
         self.word = ExtractWord()
 
         self.doc_suffix = ['doc', 'docx']
-        self.excel_suffix= ['xls', 'xlsx']
+        self.excel_suffix = ['xls', 'xlsx']
         self.ppt_suffix = ['ppt', 'pptx']
 
     def __call__(self, file_content: Union[Path, str],
                  save_img_dir: str = None):
         file_content = str(file_content)
 
         if not file_content:
             raise ValueError(f'{file_content} must be Path or str.')
 
         file_type = self.which_type(file_content)
         all_suffix = self.doc_suffix + self.excel_suffix + self.ppt_suffix
         if file_type not in all_suffix:
-            raise ValueError(f'{file_type} must in {self.allowed_suffix}')
+            raise ValueError(f'{file_type} must in {all_suffix}')
 
         if file_type in self.doc_suffix:
             return self.word(file_content, save_img_dir)
 
         if file_type in self.excel_suffix:
             return self.excel(file_content, save_img_dir=save_img_dir)
```

## Comparing `extract_office_content-0.0.2.dist-info/METADATA` & `extract_office_content-0.0.3.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: extract-office-content
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tool for extracting content from office files.
 Home-page: https://github.com/SWHL/ExtractOfficeText.git
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
-Keywords: extract,office,text
+Keywords: extract,office,text,content
 Platform: Any
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7,<=3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6,<=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: lxml (>=4.9.1)
 Requires-Dist: openpyxl (>=3.1.2)
 Requires-Dist: pandas (>=1.3.5)
 Requires-Dist: pytest (>=7.1.2)
 Requires-Dist: python-docx (>=0.8.11)
 Requires-Dist: python-pptx (>=0.6.21)
```

### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: extract-office-content Version: 0.0.2 Summary: Tool
+Metadata-Version: 2.1 Name: extract-office-content Version: 0.0.3 Summary: Tool
 for extracting content from office files. Home-page: https://github.com/SWHL/
 ExtractOfficeText.git Author: SWHL Author-email: liekkaskono@163.com License:
-Apache-2.0 Keywords: extract,office,text Platform: Any Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Requires-Python: >=3.7,<=3.10 Description-Content-
-Type: text/markdown Requires-Dist: lxml (>=4.9.1) Requires-Dist: openpyxl
-(>=3.1.2) Requires-Dist: pandas (>=1.3.5) Requires-Dist: pytest (>=7.1.2)
-Requires-Dist: python-docx (>=0.8.11) Requires-Dist: python-pptx (>=0.6.21)
-Requires-Dist: tabulate Requires-Dist: filetype ## extract_office_content
+Apache-2.0 Keywords: extract,office,text,content Platform: Any Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Python: >=3.6,<=3.11 Description-Content-Type: text/
+markdown Requires-Dist: lxml (>=4.9.1) Requires-Dist: openpyxl (>=3.1.2)
+Requires-Dist: pandas (>=1.3.5) Requires-Dist: pytest (>=7.1.2) Requires-Dist:
+python-docx (>=0.8.11) Requires-Dist: python-pptx (>=0.6.21) Requires-Dist:
+tabulate Requires-Dist: filetype ## extract_office_content
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
 img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg] [PyPI] [https://
 static.pepy.tech/personalized-badge/
 extract_office_content?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads]
 ### Use 1. Install`extract_office_content` ```bash $ pip install
 extract_office_content ``` 2. Run by CLI. - Extract All office file's content.
 ```bash $ extract_office_content -h usage: extract_office_content [-h] [-
```

## Comparing `extract_office_content-0.0.2.dist-info/RECORD` & `extract_office_content-0.0.3.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 extract_office_content/__init__.py,sha256=Ge-pxaPmMXWiBzju-OCsdUwYXM8GLvY56qktBKTO3Xw,227
 extract_office_content/extract_excel.py,sha256=q107vT4nthsJZealOYn2k1jp6zlTcQ2xGsJQHO5Mmi0,4272
-extract_office_content/extract_ppt.py,sha256=1-TiNi8_uI-jSG-AsPk4sZxnEHAEWU-kjbRnuGE3JUY,3553
+extract_office_content/extract_ppt.py,sha256=lfiLMhV9CSPb8BBAd19hva7NK0dx7CthEeK8HrAHwt8,3956
 extract_office_content/extract_word.py,sha256=xFM0KiAyB4rtOYqrrS6M9JVhsnS_hTV62jBDOkFzJjc,6297
-extract_office_content/main.py,sha256=Eu6q2UlyKtTakAfOJWA4bN4RqcvPys8_rksvY_ZqTnw,2273
+extract_office_content/main.py,sha256=qj1dl1gnYuCQT-fRoiXL8zkPRxsslImEZQjoORlBX5Y,2265
 extract_office_content/utils.py,sha256=eNm28P-wu9TJRHob-tLrzTrpWJCqzLet73My8T6z1Ec,973
-extract_office_content-0.0.2.dist-info/METADATA,sha256=fIvTKYH0pqcCHYn2Fc8MO9EKanexbzlABkSi8cFoHxA,4758
-extract_office_content-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-extract_office_content-0.0.2.dist-info/entry_points.txt,sha256=JXiZmmPdeFuKjf78O0nnnTigzul8d99FV6YuamdcI6Y,245
-extract_office_content-0.0.2.dist-info/top_level.txt,sha256=quDoGD7DEfkl_J2tdoeRUbk5H4oKd5-dWIOLRaLB_mc,23
-extract_office_content-0.0.2.dist-info/RECORD,,
+extract_office_content-0.0.3.dist-info/METADATA,sha256=swjVNxQEKP67wrKOQNoDjibCnB-3QTAet0bjGNDNVIk,4817
+extract_office_content-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+extract_office_content-0.0.3.dist-info/entry_points.txt,sha256=JXiZmmPdeFuKjf78O0nnnTigzul8d99FV6YuamdcI6Y,245
+extract_office_content-0.0.3.dist-info/top_level.txt,sha256=quDoGD7DEfkl_J2tdoeRUbk5H4oKd5-dWIOLRaLB_mc,23
+extract_office_content-0.0.3.dist-info/RECORD,,
```

