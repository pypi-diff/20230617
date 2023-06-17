# Comparing `tmp/xanalyzer-0.2.6.tar.gz` & `tmp/xanalyzer-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xanalyzer-0.2.6.tar", last modified: Sun Feb 12 03:07:54 2023, max compression
+gzip compressed data, was "dist\xanalyzer-0.2.7.tar", last modified: Sat Jun 17 12:01:17 2023, max compression
```

## Comparing `xanalyzer-0.2.6.tar` & `xanalyzer-0.2.7.tar`

### file list

```diff
@@ -1,40 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 03:07:54.000000 xanalyzer-0.2.6/
--rw-rw-rw-   0        0        0     3106 2023-02-12 03:07:54.000000 xanalyzer-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     2833 2023-01-21 05:07:31.000000 xanalyzer-0.2.6/README.md
--rw-rw-rw-   0        0        0      189 2023-01-14 13:51:04.000000 xanalyzer-0.2.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-12 03:07:54.000000 xanalyzer-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      706 2022-12-26 13:43:53.000000 xanalyzer-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-12 03:07:54.000000 xanalyzer-0.2.6/tests/
--rw-rw-rw-   0        0        0        0 2022-03-09 15:03:39.000000 xanalyzer-0.2.6/tests/__init__.py
--rw-rw-rw-   0        0        0      473 2023-01-08 01:18:58.000000 xanalyzer-0.2.6/tests/test_elf_size.py
--rw-rw-rw-   0        0        0     3451 2022-12-26 13:45:01.000000 xanalyzer-0.2.6/tests/test_filetype.py
--rw-rw-rw-   0        0        0     1367 2023-01-09 15:05:50.000000 xanalyzer-0.2.6/tests/test_packer.py
--rw-rw-rw-   0        0        0      594 2022-12-26 13:45:38.000000 xanalyzer-0.2.6/tests/test_pe_cert_name.py
--rw-rw-rw-   0        0        0     1093 2022-12-26 13:45:45.000000 xanalyzer-0.2.6/tests/test_pe_compile_time.py
--rw-rw-rw-   0        0        0      505 2022-12-26 13:45:55.000000 xanalyzer-0.2.6/tests/test_pe_pdb.py
--rw-rw-rw-   0        0        0      797 2022-12-26 13:46:10.000000 xanalyzer-0.2.6/tests/test_pe_resource.py
--rw-rw-rw-   0        0        0      468 2022-12-26 13:46:18.000000 xanalyzer-0.2.6/tests/test_pe_size.py
--rw-rw-rw-   0        0        0      682 2022-12-26 13:46:27.000000 xanalyzer-0.2.6/tests/test_pe_versioninfo.py
--rw-rw-rw-   0        0        0      852 2022-12-26 13:46:32.000000 xanalyzer-0.2.6/tests/test_windows_style_file_size.py
-drwxrwxrwx   0        0        0        0 2023-02-12 03:07:54.000000 xanalyzer-0.2.6/xanalyzer/
--rw-rw-rw-   0        0        0        5 2023-02-12 03:04:16.000000 xanalyzer-0.2.6/xanalyzer/VERSION
--rw-rw-rw-   0        0        0        0 2019-12-08 16:15:13.000000 xanalyzer-0.2.6/xanalyzer/__init__.py
--rw-rw-rw-   0        0        0      967 2022-12-26 13:37:44.000000 xanalyzer-0.2.6/xanalyzer/config.py
-drwxrwxrwx   0        0        0        0 2023-02-12 03:07:54.000000 xanalyzer-0.2.6/xanalyzer/data/
--rw-rw-rw-   0        0        0   499735 2022-03-06 14:41:53.000000 xanalyzer-0.2.6/xanalyzer/data/UserDB.TXT
--rw-rw-rw-   0        0        0      994 2022-11-19 06:18:52.000000 xanalyzer-0.2.6/xanalyzer/data/tools_info.json
--rw-rw-rw-   0        0        0    12933 2023-02-09 14:46:01.000000 xanalyzer-0.2.6/xanalyzer/file.py
-drwxrwxrwx   0        0        0        0 2023-02-12 03:07:54.000000 xanalyzer-0.2.6/xanalyzer/file_process/
--rw-rw-rw-   0        0        0        0 2019-12-08 15:36:09.000000 xanalyzer-0.2.6/xanalyzer/file_process/__init__.py
--rw-rw-rw-   0        0        0     2203 2023-01-08 01:18:58.000000 xanalyzer-0.2.6/xanalyzer/file_process/elf.py
--rw-rw-rw-   0        0        0    14094 2023-01-21 05:16:09.000000 xanalyzer-0.2.6/xanalyzer/file_process/pe.py
--rw-rw-rw-   0        0        0     2311 2022-12-26 14:22:14.000000 xanalyzer-0.2.6/xanalyzer/main.py
--rw-rw-rw-   0        0        0     7725 2022-12-26 15:06:12.000000 xanalyzer-0.2.6/xanalyzer/url.py
--rw-rw-rw-   0        0        0      729 2022-12-26 13:43:38.000000 xanalyzer-0.2.6/xanalyzer/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-12 03:07:54.000000 xanalyzer-0.2.6/xanalyzer.egg-info/
--rw-rw-rw-   0        0        0     3106 2023-02-12 03:07:54.000000 xanalyzer-0.2.6/xanalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      809 2023-02-12 03:07:54.000000 xanalyzer-0.2.6/xanalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-12 03:07:54.000000 xanalyzer-0.2.6/xanalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-02-12 03:07:54.000000 xanalyzer-0.2.6/xanalyzer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      196 2023-02-12 03:07:54.000000 xanalyzer-0.2.6/xanalyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-02-12 03:07:54.000000 xanalyzer-0.2.6/xanalyzer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 12:01:17.000000 xanalyzer-0.2.7/
+-rw-rw-rw-   0        0        0     3382 2023-06-17 12:01:17.000000 xanalyzer-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3228 2023-06-17 11:54:10.000000 xanalyzer-0.2.7/README.md
+-rw-rw-rw-   0        0        0      209 2023-06-17 09:05:09.000000 xanalyzer-0.2.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 12:01:17.000000 xanalyzer-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      748 2023-06-17 10:14:32.000000 xanalyzer-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 12:01:17.000000 xanalyzer-0.2.7/tests/
+-rw-rw-rw-   0        0        0        0 2022-03-09 15:03:39.000000 xanalyzer-0.2.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      473 2023-01-08 01:18:58.000000 xanalyzer-0.2.7/tests/test_elf_size.py
+-rw-rw-rw-   0        0        0     3539 2023-02-18 14:03:31.000000 xanalyzer-0.2.7/tests/test_filetype.py
+-rw-rw-rw-   0        0        0     1751 2023-06-16 23:29:58.000000 xanalyzer-0.2.7/tests/test_packer.py
+-rw-rw-rw-   0        0        0      594 2022-12-26 13:45:38.000000 xanalyzer-0.2.7/tests/test_pe_cert_name.py
+-rw-rw-rw-   0        0        0     1093 2022-12-26 13:45:45.000000 xanalyzer-0.2.7/tests/test_pe_compile_time.py
+-rw-rw-rw-   0        0        0      412 2023-06-10 14:41:58.000000 xanalyzer-0.2.7/tests/test_pe_dll_name.py
+-rw-rw-rw-   0        0        0      505 2022-12-26 13:45:55.000000 xanalyzer-0.2.7/tests/test_pe_pdb.py
+-rw-rw-rw-   0        0        0      797 2022-12-26 13:46:10.000000 xanalyzer-0.2.7/tests/test_pe_resource.py
+-rw-rw-rw-   0        0        0      468 2022-12-26 13:46:18.000000 xanalyzer-0.2.7/tests/test_pe_size.py
+-rw-rw-rw-   0        0        0      682 2022-12-26 13:46:27.000000 xanalyzer-0.2.7/tests/test_pe_versioninfo.py
+-rw-rw-rw-   0        0        0      852 2022-12-26 13:46:32.000000 xanalyzer-0.2.7/tests/test_windows_style_file_size.py
+drwxrwxrwx   0        0        0        0 2023-06-17 12:01:17.000000 xanalyzer-0.2.7/xanalyzer/
+-rw-rw-rw-   0        0        0        5 2023-06-17 00:08:23.000000 xanalyzer-0.2.7/xanalyzer/VERSION
+-rw-rw-rw-   0        0        0        0 2019-12-08 16:15:13.000000 xanalyzer-0.2.7/xanalyzer/__init__.py
+-rw-rw-rw-   0        0        0     1042 2023-06-16 23:35:52.000000 xanalyzer-0.2.7/xanalyzer/config.py
+drwxrwxrwx   0        0        0        0 2023-06-17 12:01:17.000000 xanalyzer-0.2.7/xanalyzer/data/
+-rw-rw-rw-   0        0        0   499735 2022-03-06 14:41:53.000000 xanalyzer-0.2.7/xanalyzer/data/UserDB.TXT
+-rw-rw-rw-   0        0        0      994 2022-11-19 06:18:52.000000 xanalyzer-0.2.7/xanalyzer/data/tools_info.json
+drwxrwxrwx   0        0        0        0 2023-06-17 12:01:17.000000 xanalyzer-0.2.7/xanalyzer/data/yara_rules/
+drwxrwxrwx   0        0        0        0 2023-06-17 12:01:17.000000 xanalyzer-0.2.7/xanalyzer/data/yara_rules/packers/
+-rw-rw-rw-   0        0        0      425 2023-06-16 23:32:45.000000 xanalyzer-0.2.7/xanalyzer/data/yara_rules/packers/UPX_PE.yar
+-rw-rw-rw-   0        0        0    13755 2023-06-16 23:50:27.000000 xanalyzer-0.2.7/xanalyzer/file.py
+drwxrwxrwx   0        0        0        0 2023-06-17 12:01:17.000000 xanalyzer-0.2.7/xanalyzer/file_process/
+-rw-rw-rw-   0        0        0        0 2019-12-08 15:36:09.000000 xanalyzer-0.2.7/xanalyzer/file_process/__init__.py
+-rw-rw-rw-   0        0        0     2207 2023-06-16 23:50:03.000000 xanalyzer-0.2.7/xanalyzer/file_process/elf.py
+-rw-rw-rw-   0        0        0    15048 2023-06-16 23:50:12.000000 xanalyzer-0.2.7/xanalyzer/file_process/pe.py
+-rw-rw-rw-   0        0        0     2405 2023-06-16 23:50:43.000000 xanalyzer-0.2.7/xanalyzer/main.py
+-rw-rw-rw-   0        0        0     7727 2023-06-16 23:50:52.000000 xanalyzer-0.2.7/xanalyzer/url.py
+-rw-rw-rw-   0        0        0      729 2023-06-16 23:51:03.000000 xanalyzer-0.2.7/xanalyzer/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-17 12:01:17.000000 xanalyzer-0.2.7/xanalyzer.egg-info/
+-rw-rw-rw-   0        0        0     3382 2023-06-17 12:01:16.000000 xanalyzer-0.2.7/xanalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      880 2023-06-17 12:01:17.000000 xanalyzer-0.2.7/xanalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 12:01:16.000000 xanalyzer-0.2.7/xanalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-17 12:01:16.000000 xanalyzer-0.2.7/xanalyzer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      215 2023-06-17 12:01:16.000000 xanalyzer-0.2.7/xanalyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-17 12:01:16.000000 xanalyzer-0.2.7/xanalyzer.egg-info/top_level.txt
```

### Comparing `xanalyzer-0.2.6/PKG-INFO` & `xanalyzer-0.2.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 Metadata-Version: 2.1
 Name: xanalyzer
-Version: 0.2.6
+Version: 0.2.7
 Summary: Analyzer for files and urls
 Author: qux-bbb
 Description-Content-Type: text/markdown
 
 # xanalyzer
 
-静态分析文件和url，python3下运行。  
+[English](README-en.md)  
+
+简单分析文件和url，python3下运行。  
 
 1. 文件
     - md5/sha256
     - 文件类型
     - 文件大小
     - 字符串扫描
     - PE文件
         - PE大小
         - 编译时间
         - pdb路径
         - 版本信息
         - 证书验证
         - 节区名称
+        - DLL名称
         - 查壳
         - 资源段扫描
     - ELF文件
         - ELF大小
         - 查壳
     - 建议使用的工具
 2. url(website)
     - 域名解析ip
     - 获取robots.txt文件
     - 站内链接扫描(--deep)
     - 站内子域名扫描(--deep)
 
 ## 安装
-方法1 - 使用pipx安装：  
+使用pipx安装：  
 ```r
+# pipx: https://pypa.github.io/pipx/  
+pip install pipx
+pipx ensurepath
 pipx install xanalyzer
-# 还可以用来升级，但是不能检查升级
+# 还可以用来升级，但是不能检查新版本
 pipx upgrade xanalyzer
 ```
-pipx: https://pypa.github.io/pipx/  
-
-方法2 - 从源码安装：  
-```r
-git clone https://github.com/qux-bbb/xanalyzer
-cd xanalyzer
-python setup.py install
-```
 
 如果系统是 Debian/Ubuntu，需要安装依赖：  
 ```r
 sudo apt-get install libmagic1
 ```
 
 ## 使用帮助
@@ -77,28 +75,35 @@
 ```
 
 ## 开发
 ```r
 git clone https://github.com/qux-bbb/xanalyzer
 cd xanalyzer
 virtualenv venv
+# windws使用虚拟环境: .\venv\Scripts\activate
+# linux使用虚拟环境: source venv/bin/activate
 pip install -r requirements.txt
 python setup.py develop
+# 退出虚拟环境: deactivate
 ```
 这样之后就可以用pycharm或vscode开发调试了  
 
 ## 打包发布
 该步骤仅本人使用  
 
-打包前确保版本号和CHANGELOG.md已更新  
+打包前确保版本号和CHANGELOG.md已更新，清空dist文件夹  
 
-安装依赖并打包：  
+安装依赖、通过测试项、打包：  
 ```r
+# windws使用虚拟环境: .\venv\Scripts\activate
+# linux使用虚拟环境: source venv/bin/activate
 pip install -r requirements.my.txt
+pytest
 python setup.py sdist bdist_wheel
+# 退出虚拟环境: deactivate
 ```
 
 重新打开一个命令行，转到dist文件夹下本地安装，检查基本功能，举例：  
 ```r
 pipx uninstall xanalyzer
 pipx install ./xanalyzer-0.2.3.tar.gz
 xanalyzer --version
```

### Comparing `xanalyzer-0.2.6/setup.py` & `xanalyzer-0.2.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup(
     name="xanalyzer",
     version=open("xanalyzer/VERSION", "r").read(),
     packages=find_packages(),
     package_data={
         "xanalyzer": [
             "data/UserDB.TXT",
+            "data/yara_rules/packers/*",
             "data/tools_info.json",
             "VERSION",
         ],
     },
     author="qux-bbb",
     description="Analyzer for files and urls",
     long_description=open("README.md", "r", encoding="utf8").read(),
```

### Comparing `xanalyzer-0.2.6/tests/test_filetype.py` & `xanalyzer-0.2.7/tests/test_filetype.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,17 @@
         # 常用压缩包
         "hello.zip_",
         "hello.7z_",
         "hello.rar_",
         # 流量包文件
         "http.pcap_",
         "http.pcapng_",
+        # linux shell 脚本文件
+        "hello_bash.sh_",
+        "hello_sh.sh_",
     ]
     for filename in filenames:
         expect_ext = ["." + filename[:-1].split(".")[1]]
         file_path = cur_dir_path / "test_data" / filename
         file_analyzer = FileAnalyzer(file_path)
         assert file_analyzer.possible_extension_names == expect_ext
```

### Comparing `xanalyzer-0.2.6/tests/test_packer.py` & `xanalyzer-0.2.7/tests/test_packer.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,26 @@
     upxed_path = cur_dir_path / "test_data" / "Hello_upx.exe_"
     file_analyzer = FileAnalyzer(upxed_path)
     pe_analyzer = PeAnalyzer(file_analyzer)
     matches = pe_analyzer.get_packer_result()
     assert matches == ["UPX 3.96"]
 
 
+def test_common_exe_upx_packer():
+    upxed_path = (
+        cur_dir_path
+        / "test_data"
+        / "d32e87c4b81738b45db582db8293293096637f5d50af7dd5d9a0162a0747498a_blackmoon_common_upx"
+    )
+    file_analyzer = FileAnalyzer(upxed_path)
+    pe_analyzer = PeAnalyzer(file_analyzer)
+    matches = pe_analyzer.get_packer_result()
+    assert matches == ["UPX 3.96"]
+
+
 def test_elf_upx_packer():
     upxed_path = cur_dir_path / "test_data" / "Hello64_elf_static_upx_"
     file_analyzer = FileAnalyzer(upxed_path)
     elf_analyzer = ElfAnalyzer(file_analyzer)
     matches = elf_analyzer.get_packer_result()
     assert matches == ["UPX 3.96"]
```

### Comparing `xanalyzer-0.2.6/tests/test_pe_cert_name.py` & `xanalyzer-0.2.7/tests/test_pe_cert_name.py`

 * *Files identical despite different names*

### Comparing `xanalyzer-0.2.6/tests/test_pe_compile_time.py` & `xanalyzer-0.2.7/tests/test_pe_compile_time.py`

 * *Files identical despite different names*

### Comparing `xanalyzer-0.2.6/tests/test_pe_resource.py` & `xanalyzer-0.2.7/tests/test_pe_resource.py`

 * *Files identical despite different names*

### Comparing `xanalyzer-0.2.6/tests/test_pe_versioninfo.py` & `xanalyzer-0.2.7/tests/test_pe_versioninfo.py`

 * *Files identical despite different names*

### Comparing `xanalyzer-0.2.6/tests/test_windows_style_file_size.py` & `xanalyzer-0.2.7/tests/test_windows_style_file_size.py`

 * *Files identical despite different names*

### Comparing `xanalyzer-0.2.6/xanalyzer/config.py` & `xanalyzer-0.2.7/xanalyzer/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pathlib import Path
 
 
 class Config:
     home_dir = Path(__file__).parent
     # UserDB.TXT文件默认是GBK编码, 需要简单处理一下, 去掉乱码, 新的UserDB.TXT加了新的规则, peutils解析不了
     peid_signature_path = home_dir / "data" / "UserDB.TXT"
+    packer_yara_rules_path = home_dir / "data" / "yara_rules" / "packers"
     tools_info_path = home_dir / "data" / "tools_info.json"
     VERSION = open(home_dir / "VERSION", "r").read().strip()
 
     conf = {}
 
     @classmethod
     def init(cls, save_flag):
```

### Comparing `xanalyzer-0.2.6/xanalyzer/data/UserDB.TXT` & `xanalyzer-0.2.7/xanalyzer/data/UserDB.TXT`

 * *Files identical despite different names*

### Comparing `xanalyzer-0.2.6/xanalyzer/data/tools_info.json` & `xanalyzer-0.2.7/xanalyzer/data/tools_info.json`

 * *Files identical despite different names*

### Comparing `xanalyzer-0.2.6/xanalyzer/file.py` & `xanalyzer-0.2.7/xanalyzer/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,57 @@
 import io
+import json
 import os
 import re
-import json
-import magic
-from pathlib import Path
 from hashlib import md5, sha256
+from pathlib import Path
 from zipfile import ZipFile
 
-from xanalyzer.utils import log
-from xanalyzer.file_process.pe import PeAnalyzer
-from xanalyzer.file_process.elf import ElfAnalyzer
+import magic
+import yara
+
 from xanalyzer.config import Config
+from xanalyzer.file_process.elf import ElfAnalyzer
+from xanalyzer.file_process.pe import PeAnalyzer
+from xanalyzer.utils import log
 
 
 class FileAnalyzer:
+    packer_yara_rules = None
+
     def __init__(self, file_path):
         self.file_path = file_path
         self.file_size = os.path.getsize(self.file_path)
         the_file = open(self.file_path, "rb")
         the_content = the_file.read()
         the_file.close()
         self.file_type, self.possible_extension_names = self.guess_type_and_ext(
             the_content
         )
         self.packer_list = []
         self.pe_resource_type_list = []
 
+        self.init_packer_yara_rules()
+
+    @classmethod
+    def init_packer_yara_rules(cls):
+        if cls.packer_yara_rules:
+            return
+        yara_filenames = os.listdir(Config.packer_yara_rules_path)
+        yara_dict = {}
+        for yara_filename in yara_filenames:
+            yara_path = os.path.join(
+                Config.packer_yara_rules_path, yara_filename
+            )
+            yara_dict[yara_filename] = yara_path
+        cls.packer_yara_rules = yara.compile(filepaths=yara_dict)
+
+    def packer_yara_match(self):
+        return self.packer_yara_rules.match(str(self.file_path))
+
     def guess_type_and_ext(self, the_content):
         """
         猜测文件类型和扩展名
         :return: file_type, possible_extension_names
         """
         # magic.from_file不能通过中文路径读取文件，暂时使用magic.from_buffer
         the_file_type = magic.from_buffer(the_content)
@@ -115,14 +137,18 @@
             the_ext = [".avi"]
         elif the_file_type.startswith(("ASCII text", "UTF-8 Unicode text")):
             the_ext = [".txt"]
         elif the_file_type.startswith("tcpdump capture file"):
             the_ext = [".pcap"]
         elif the_file_type.startswith("pcap-ng capture file"):
             the_ext = [".pcapng"]
+        elif the_file_type.startswith(
+            ("Bourne-Again shell script", "POSIX shell script")
+        ):
+            the_ext = [".sh"]
 
         return the_file_type, the_ext
 
     @staticmethod
     def get_windows_style_file_size(tmp_size):
         """
         得到windows风格的文件大小展示
```

### Comparing `xanalyzer-0.2.6/xanalyzer/file_process/elf.py` & `xanalyzer-0.2.7/xanalyzer/file_process/elf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import re
+
 from elftools.elf.elffile import ELFFile
+
 from xanalyzer.utils import log
 
 
 class ElfAnalyzer:
     file_analyzer = None
 
     def __init__(self, file_analyzer):
```

### Comparing `xanalyzer-0.2.6/xanalyzer/file_process/pe.py` & `xanalyzer-0.2.7/xanalyzer/file_process/pe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 import re
+from datetime import datetime
+
 import pefile
 import peutils
-from datetime import datetime
 from signify.authenticode.signed_pe import SignedPEFile
 
 from xanalyzer.config import Config
 from xanalyzer.utils import log
 
 
 class PeAnalyzer:
     file_analyzer = None
     pe_file = None
+    peid_signatures = None
 
     def __init__(self, file_analyzer):
         self.file_analyzer = file_analyzer
         self.pe_file = pefile.PE(self.file_analyzer.file_path)
 
+        self.init_peid_signatures()
+
     def __del__(self):
         self.pe_file.close()
 
+    @classmethod
+    def init_peid_signatures(cls):
+        if cls.peid_signatures:
+            return
+        cls.peid_signatures = peutils.SignatureDatabase(Config.peid_signature_path)
+
     def get_pe_size(self):
         """
         计算真实PE大小
         """
         if not self.pe_file.sections:
             return
 
@@ -101,17 +111,30 @@
 
     def get_pdb_path(self):
         for debug_entry in getattr(self.pe_file, "DIRECTORY_ENTRY_DEBUG", []):
             if hasattr(debug_entry.entry, "PdbFileName"):
                 return debug_entry.entry.PdbFileName.strip(b"\x00").decode("utf8")
         return
 
+    def get_dll_name(self):
+        if self.file_analyzer.possible_extension_names != [".dll"]:
+            return
+        if hasattr(self.pe_file, "DIRECTORY_ENTRY_EXPORT"):
+            return self.pe_file.DIRECTORY_ENTRY_EXPORT.name
+        return
+
     def get_packer_result(self):
-        signatures = peutils.SignatureDatabase(Config.peid_signature_path)
-        matches = signatures.match(self.pe_file, ep_only=True)
+        matches = self.peid_signatures.match(self.pe_file, ep_only=True)
+
+        if not matches:
+            yara_matches = self.file_analyzer.packer_yara_match()
+            if yara_matches:
+                matches = []
+                for yara_match in yara_matches:
+                    matches.append(yara_match.rule)
 
         if matches:
             for i in range(len(matches)):
                 if matches[i].startswith("UPX"):
                     the_file = open(self.file_analyzer.file_path, "rb")
                     file_content = the_file.read()
                     the_file.close()
@@ -277,14 +300,22 @@
         输出节区名
         """
         section_names = []
         for section in self.pe_file.sections:
             section_names.append(section.Name.strip(b"\x00"))
         log.info(f"section names: {section_names}")
 
+    def dll_name_scan(self):
+        """
+        如果是dll，尝试输出dll名称
+        """
+        dll_name = self.get_dll_name()
+        if dll_name:
+            log.info(f"dll name: {dll_name}")
+
     def packer_scan(self):
         """
         查壳
         """
         matches = self.get_packer_result()
         if matches:
             self.file_analyzer.packer_list.extend(matches)
@@ -338,9 +369,10 @@
     def run(self):
         self.pe_size_scan()
         self.compile_time_scan()
         self.pdb_scan()
         self.versioninfo_scan()
         self.cert_scan()
         self.section_name_scan()
+        self.dll_name_scan()
         self.packer_scan()
         self.resource_scan()
```

### Comparing `xanalyzer-0.2.6/xanalyzer/main.py` & `xanalyzer-0.2.7/xanalyzer/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,35 @@
-import os
 import argparse
+import os
 from pathlib import Path
 
+from xanalyzer.config import Config
 from xanalyzer.file import FileAnalyzer
 from xanalyzer.url import UrlAnalyzer
-from xanalyzer.utils import log, init_log
-from xanalyzer.config import Config
+from xanalyzer.utils import init_log, log
+
+file_path_list = []
+
+
+def get_all_path(the_path):
+    """获取所有路径，深度优先
+
+    Args:
+        the_path (string): 一个路径
+    """
+    if os.path.isfile(the_path):
+        file_path_list.append(the_path)
+        return
+
+    a_path = None
+    for a_path in Path(the_path).iterdir():
+        get_all_path(a_path)
+
+    if not a_path:  # 空文件夹，提示一下
+        log.warning(f"folder is empty: {the_path}")
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog="xanalyzer", description="Process some files and urls."
     )
     group = parser.add_mutually_exclusive_group(required=True)
@@ -33,28 +53,20 @@
     init_log()
 
     log.info("=" * 80)
 
     deep_flag = args.deep
 
     if args.file:
-        file_paths = []
         for the_path in args.file:
             if not os.path.exists(the_path):
                 log.warning("{} does not exist!!!".format(the_path))
                 continue
-            if os.path.isdir(the_path):
-                for a_path in Path(the_path).iterdir():
-                    if not a_path.is_file():
-                        log.warning(f"{a_path} is not a file, will be ignored")
-                        continue
-                    file_paths.append(str(a_path))
-            else:
-                file_paths.append(the_path)
-        for file_path in file_paths:
+            get_all_path(the_path)
+        for file_path in file_path_list:
             log.info("processing {}".format(file_path))
             file_analyzer = FileAnalyzer(file_path)
             file_analyzer.run()
             log.info("-" * 80)
     if args.url:
         log.info("processing {}".format(args.url))
         url_analyzer = UrlAnalyzer(args.url, deep_flag)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xanalyzer-0.2.6/xanalyzer/url.py` & `xanalyzer-0.2.7/xanalyzer/url.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import re
 import socket
+from urllib.parse import urljoin, urlparse
+
 import requests
-from urllib.parse import urlparse, urljoin
 
-from xanalyzer.utils import log
 from xanalyzer.config import Config
+from xanalyzer.utils import log
 
 
 class UrlAnalyzer:
     url = None
     parsed_url = None
     main_url = None
     hostname = None
```

### Comparing `xanalyzer-0.2.6/xanalyzer/utils.py` & `xanalyzer-0.2.7/xanalyzer/utils.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import os
 import logging
+import os
+
 import coloredlogs
 
 from xanalyzer.config import Config
 
-
 log = logging.getLogger("xanalyzer")
 
 
 def init_log():
     # 指定logger输出格式 -8s: 指定宽度为8，减号表示左对齐
     basic_fmt = "%(asctime)s %(levelname)-8s: %(message)s"
```

### Comparing `xanalyzer-0.2.6/xanalyzer.egg-info/PKG-INFO` & `xanalyzer-0.2.7/xanalyzer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 Metadata-Version: 2.1
 Name: xanalyzer
-Version: 0.2.6
+Version: 0.2.7
 Summary: Analyzer for files and urls
 Author: qux-bbb
 Description-Content-Type: text/markdown
 
 # xanalyzer
 
-静态分析文件和url，python3下运行。  
+[English](README-en.md)  
+
+简单分析文件和url，python3下运行。  
 
 1. 文件
     - md5/sha256
     - 文件类型
     - 文件大小
     - 字符串扫描
     - PE文件
         - PE大小
         - 编译时间
         - pdb路径
         - 版本信息
         - 证书验证
         - 节区名称
+        - DLL名称
         - 查壳
         - 资源段扫描
     - ELF文件
         - ELF大小
         - 查壳
     - 建议使用的工具
 2. url(website)
     - 域名解析ip
     - 获取robots.txt文件
     - 站内链接扫描(--deep)
     - 站内子域名扫描(--deep)
 
 ## 安装
-方法1 - 使用pipx安装：  
+使用pipx安装：  
 ```r
+# pipx: https://pypa.github.io/pipx/  
+pip install pipx
+pipx ensurepath
 pipx install xanalyzer
-# 还可以用来升级，但是不能检查升级
+# 还可以用来升级，但是不能检查新版本
 pipx upgrade xanalyzer
 ```
-pipx: https://pypa.github.io/pipx/  
-
-方法2 - 从源码安装：  
-```r
-git clone https://github.com/qux-bbb/xanalyzer
-cd xanalyzer
-python setup.py install
-```
 
 如果系统是 Debian/Ubuntu，需要安装依赖：  
 ```r
 sudo apt-get install libmagic1
 ```
 
 ## 使用帮助
@@ -77,28 +75,35 @@
 ```
 
 ## 开发
 ```r
 git clone https://github.com/qux-bbb/xanalyzer
 cd xanalyzer
 virtualenv venv
+# windws使用虚拟环境: .\venv\Scripts\activate
+# linux使用虚拟环境: source venv/bin/activate
 pip install -r requirements.txt
 python setup.py develop
+# 退出虚拟环境: deactivate
 ```
 这样之后就可以用pycharm或vscode开发调试了  
 
 ## 打包发布
 该步骤仅本人使用  
 
-打包前确保版本号和CHANGELOG.md已更新  
+打包前确保版本号和CHANGELOG.md已更新，清空dist文件夹  
 
-安装依赖并打包：  
+安装依赖、通过测试项、打包：  
 ```r
+# windws使用虚拟环境: .\venv\Scripts\activate
+# linux使用虚拟环境: source venv/bin/activate
 pip install -r requirements.my.txt
+pytest
 python setup.py sdist bdist_wheel
+# 退出虚拟环境: deactivate
 ```
 
 重新打开一个命令行，转到dist文件夹下本地安装，检查基本功能，举例：  
 ```r
 pipx uninstall xanalyzer
 pipx install ./xanalyzer-0.2.3.tar.gz
 xanalyzer --version
```

### Comparing `xanalyzer-0.2.6/xanalyzer.egg-info/SOURCES.txt` & `xanalyzer-0.2.7/xanalyzer.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 setup.py
 tests/__init__.py
 tests/test_elf_size.py
 tests/test_filetype.py
 tests/test_packer.py
 tests/test_pe_cert_name.py
 tests/test_pe_compile_time.py
+tests/test_pe_dll_name.py
 tests/test_pe_pdb.py
 tests/test_pe_resource.py
 tests/test_pe_size.py
 tests/test_pe_versioninfo.py
 tests/test_windows_style_file_size.py
 xanalyzer/VERSION
 xanalyzer/__init__.py
@@ -23,10 +24,11 @@
 xanalyzer.egg-info/dependency_links.txt
 xanalyzer.egg-info/entry_points.txt
 xanalyzer.egg-info/requires.txt
 xanalyzer.egg-info/top_level.txt
 xanalyzer/../requirements.txt
 xanalyzer/data/UserDB.TXT
 xanalyzer/data/tools_info.json
+xanalyzer/data/yara_rules/packers/UPX_PE.yar
 xanalyzer/file_process/__init__.py
 xanalyzer/file_process/elf.py
 xanalyzer/file_process/pe.py
```

