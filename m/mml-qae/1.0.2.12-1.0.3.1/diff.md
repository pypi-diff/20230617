# Comparing `tmp/mml_qae-1.0.2.12.tar.gz` & `tmp/mml_qae-1.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mml_qae-1.0.2.12.tar", last modified: Sat Jun 10 09:45:49 2023, max compression
+gzip compressed data, was "dist\mml_qae-1.0.3.1.tar", last modified: Sat Jun 17 09:55:02 2023, max compression
```

## Comparing `mml_qae-1.0.2.12.tar` & `mml_qae-1.0.3.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/
--rw-rw-rw-   0        0        0        0 2023-05-13 07:15:44.000000 mml_qae-1.0.2.12/LICENSE
--rw-rw-rw-   0        0        0     4396 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/PKG-INFO
--rw-rw-rw-   0        0        0     3633 2023-06-10 09:35:00.000000 mml_qae-1.0.2.12/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/mml_qae/
--rw-rw-rw-   0        0        0     1960 2023-05-26 14:52:53.000000 mml_qae-1.0.2.12/mml_qae/Chinese_dealing.py
--rw-rw-rw-   0        0        0     1916 2023-05-15 13:52:21.000000 mml_qae-1.0.2.12/mml_qae/MoreErrors.py
--rw-rw-rw-   0        0        0        0 2023-05-13 07:17:18.000000 mml_qae-1.0.2.12/mml_qae/__init__.py
--rw-rw-rw-   0        0        0     3025 2023-06-10 09:42:23.000000 mml_qae-1.0.2.12/mml_qae/lists_of_number.py
--rw-rw-rw-   0        0        0     1416 2023-05-26 15:00:20.000000 mml_qae-1.0.2.12/mml_qae/one_list_of_number.py
-drwxrwxrwx   0        0        0        0 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/mml_qae.egg-info/
--rw-rw-rw-   0        0        0     4396 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/mml_qae.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/mml_qae.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/mml_qae.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/mml_qae.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      690 2023-06-10 09:45:38.000000 mml_qae-1.0.2.12/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-06-10 09:45:34.000000 mml_qae-1.0.2.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:55:02.000000 mml_qae-1.0.3.1/
+-rw-rw-rw-   0        0        0        0 2023-05-13 07:15:44.000000 mml_qae-1.0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     4800 2023-06-17 09:55:02.000000 mml_qae-1.0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4038 2023-06-17 09:53:53.000000 mml_qae-1.0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 09:55:02.000000 mml_qae-1.0.3.1/mml_qae/
+-rw-rw-rw-   0        0        0     1956 2023-06-17 09:50:50.000000 mml_qae-1.0.3.1/mml_qae/Chinese_dealing.py
+-rw-rw-rw-   0        0        0     1916 2023-05-15 13:52:21.000000 mml_qae-1.0.3.1/mml_qae/MoreErrors.py
+-rw-rw-rw-   0        0        0      372 2023-06-17 09:38:29.000000 mml_qae-1.0.3.1/mml_qae/__init__.py
+-rw-rw-rw-   0        0        0     1134 2023-06-17 09:54:58.000000 mml_qae-1.0.3.1/mml_qae/easy_web.py
+-rw-rw-rw-   0        0        0     2051 2023-06-13 13:51:38.000000 mml_qae-1.0.3.1/mml_qae/lists_of_number.py
+-rw-rw-rw-   0        0        0     1416 2023-05-26 15:00:20.000000 mml_qae-1.0.3.1/mml_qae/one_list_of_number.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:55:02.000000 mml_qae-1.0.3.1/mml_qae.egg-info/
+-rw-rw-rw-   0        0        0     4800 2023-06-17 09:55:02.000000 mml_qae-1.0.3.1/mml_qae.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-06-17 09:55:02.000000 mml_qae-1.0.3.1/mml_qae.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 09:55:02.000000 mml_qae-1.0.3.1/mml_qae.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-17 09:55:02.000000 mml_qae-1.0.3.1/mml_qae.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      689 2023-06-17 09:54:07.000000 mml_qae-1.0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-17 09:55:02.000000 mml_qae-1.0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      668 2023-06-17 09:54:02.000000 mml_qae-1.0.3.1/setup.py
```

### Comparing `mml_qae-1.0.2.12/PKG-INFO` & `mml_qae-1.0.3.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mml_qae
-Version: 1.0.2.12
+Version: 1.0.3.1
 Summary: The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning.
 Home-page: https://www.python.org
 Author: ETRO_secondleader
 Author-email: ETRO_secondleader <ETRO_gfyx@163.com>
 Project-URL: Homepage, https://github.com/pypa/mml_qae
 Project-URL: Author's Git, https://github.com/ZYpS-leader?tab=repositories
 Classifier: Programming Language :: Python :: 3
@@ -26,48 +26,35 @@
 + 1.0.1 ----------- 略微扩充了方法.
 + 1.0.1.1 --------- 向pypi.org中扩充了项目描述.
 + 1.0.1.2 --------- 向pypi.org中扩充了说明文档.(由于作者脑抽忘记再1.0.1.1时上传了不得不新增一个版本)
 + 1.0.1.3 --------- 加入了子模块MoreErrors以提供更多错误支持.
 + 1.0.1.4 2023.5.15 突然引起的恶性错误,此为紧急修复版本.
 + 1.0.2.10 2023.5.26 中文语言处理(简易版).在测试中本版本出现了一些问题待修复.请见谅.
 + 1.0.2.11 2023.6.10 修复了上次更新的遗留问题.
++ 1.0.3.1 2023.6.17  增加了基于socket的简易网络模块.
 ---
 ## 开发者发言
 + We now have packages to deal with big data like statsmodels, sklearn, Spark, or packages to deal with natural language, such as jieba or spaCy. I admit that those packages are really useful while facing whith tons of csv data. BUT! I think we need a nicer package to deal with data, don't we? So, the mml-qae package(the whole name is My Machine Learning-Quicker and Easier) is here to help you. Alright, so, I have to say that I didn't do anything new, but I put those complex codes together into grand-new methods, so that you will be able to deal with MachineLearning and DataDealing. I started this project on 14th, May 2023 with version 1.0.1. In a more proper way, I worked on this project with my team ETRO(to see the Author's Email). I promise to update it regularly, but I cannot say how long the interval between two updataions will be for certain. Another thing needed to be paid attentioned is, this package only works at Python3.7.2, and you MUST pip install the packages needed in mml, like statsmodels. I will speak of all those packages you need to preinstall in README.md. Last but not least, never use 'from mml-qae import *'. Many methods in mml are the same name with the built-in functions! That'll be all, and have fun with MachineLearning and DataDealing!
 + Packages needed
 > + statsmodels
 > + sklearn
 > + jieba
 > + spaCy
 > + pandas
 > + numpy
 > + matplotlib
 > + wordcloud
 > + opencv-python
 ---
-## 历史版本(包括部分未公布的版本)
-+ 1 简易大数据处理与网络构建
-> +  1.0 预发布版本
-> > + 1.0.0 
->      初代版本，无项目描述。
-> > + 1.0.1
->      修复1.0.0中的明显问题。
-> > > + 1.0.1.1  加入项目描述.
-> > > + 1.0.1.2  加入帮助文档README.md并修复一些小问题
-> > > + 1.0.1.3  加入一些自定义错误和修复一些小问题
-> >  + 1.0.2
->      加入封装好的自然语言处理快捷方法。
-> > > + 1.0.2.1  加入中文处理模型(初步).
-> > > + 1.0.2.2  加入英语处理模型.
-> >  + 1.0.3     修复1.0版本的bug和问题。
-> +  1.1 完善版本
-> >  + 1.1.1 加入数据库处理方法。
-> > > + 1.1.1.1 MySQL
-> > > + 1.1.1.2 NoSQL
-> > > + 1.1.1.3 更多数据库
-> >  + 1.1.2 Spark多线程方法封装
-> > > + 1.1.2.1 多线程封装
-> > > + 1.1.2.2 集群管理方法封装
-> >  + 1.1.3 简易网络构建方法封装
-> > > + 1.1.3.1 本地index.html的构建方法封装
-> > > + 1.1.3.2 爬虫的封装
-> + 1.2 修复版本
+## Documents for easily using
+### builtins
+In this package, it usually doesn't have a started print. But if you DO NOT have all the packages we need, it will raise a ImportError just after import. The common builtin values are like __versions__,__name__ or sth. like __doc__.
+### Chinese_dealing
+With this package, you can use the following methods:
+#### add(words,tag)
+The two values are all must-needed. They must be same-shape lists, and the elements of both must correspond one-to-one. All elements must be strings. They will be added as new words one by one in the jieba.
+#### make_words_list(text)
+The parameter text must be given. This method will split the given text into several words and return the list form.
+#### make_words_list_with_tags(text)
+The parameter text must be given. This method splits the given text into several words and returns a list format, including the part of speech of each word; The return format is two lists, each containing participles and corresponding parts of speech.
+#### make_words_list_with_extra_words(text,path1,path2)
+To use this method, you must download jiebapos.xlsx and data3-1.txt from Git at https://github.com/ZYpS-leader/mml-qae. Pass in their absolute paths on the local machine, which should end with ".../jiebapos. xlsx" and ".../data3-1. txt". The return value is the same as make_words_list_with_tags method.
```

### Comparing `mml_qae-1.0.2.12/mml_qae/Chinese_dealing.py` & `mml_qae-1.0.3.1/mml_qae/Chinese_dealing.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,8 +38,8 @@
         words.append(i)
     sjk=pd.DataFrame(words,columns=["word","词性","year"])
     jpbs=pd.read_excel(path1,header=0)
     words_renamed=sjk.join(jpbs.set_index("词性英文名称"),on="词性") 
     stopwords=open(path2,encoding="utf-8").read().replace(" ","")
     Stopped_words=stopwords.split("\n")
     df_words=words_renamed[words_renamed.apply(lambda x:x.loc["word"] not in Stopped_words,axis=1)]
-    return sjk,words_renamed,df_words
+    return words_renamed,df_words
```

### Comparing `mml_qae-1.0.2.12/mml_qae/MoreErrors.py` & `mml_qae-1.0.3.1/mml_qae/MoreErrors.py`

 * *Files identical despite different names*

### Comparing `mml_qae-1.0.2.12/mml_qae/one_list_of_number.py` & `mml_qae-1.0.3.1/mml_qae/one_list_of_number.py`

 * *Files identical despite different names*

### Comparing `mml_qae-1.0.2.12/mml_qae.egg-info/PKG-INFO` & `mml_qae-1.0.3.1/mml_qae.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mml-qae
-Version: 1.0.2.12
+Version: 1.0.3.1
 Summary: The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning.
 Home-page: https://www.python.org
 Author: ETRO_secondleader
 Author-email: ETRO_secondleader <ETRO_gfyx@163.com>
 Project-URL: Homepage, https://github.com/pypa/mml_qae
 Project-URL: Author's Git, https://github.com/ZYpS-leader?tab=repositories
 Classifier: Programming Language :: Python :: 3
@@ -26,48 +26,35 @@
 + 1.0.1 ----------- 略微扩充了方法.
 + 1.0.1.1 --------- 向pypi.org中扩充了项目描述.
 + 1.0.1.2 --------- 向pypi.org中扩充了说明文档.(由于作者脑抽忘记再1.0.1.1时上传了不得不新增一个版本)
 + 1.0.1.3 --------- 加入了子模块MoreErrors以提供更多错误支持.
 + 1.0.1.4 2023.5.15 突然引起的恶性错误,此为紧急修复版本.
 + 1.0.2.10 2023.5.26 中文语言处理(简易版).在测试中本版本出现了一些问题待修复.请见谅.
 + 1.0.2.11 2023.6.10 修复了上次更新的遗留问题.
++ 1.0.3.1 2023.6.17  增加了基于socket的简易网络模块.
 ---
 ## 开发者发言
 + We now have packages to deal with big data like statsmodels, sklearn, Spark, or packages to deal with natural language, such as jieba or spaCy. I admit that those packages are really useful while facing whith tons of csv data. BUT! I think we need a nicer package to deal with data, don't we? So, the mml-qae package(the whole name is My Machine Learning-Quicker and Easier) is here to help you. Alright, so, I have to say that I didn't do anything new, but I put those complex codes together into grand-new methods, so that you will be able to deal with MachineLearning and DataDealing. I started this project on 14th, May 2023 with version 1.0.1. In a more proper way, I worked on this project with my team ETRO(to see the Author's Email). I promise to update it regularly, but I cannot say how long the interval between two updataions will be for certain. Another thing needed to be paid attentioned is, this package only works at Python3.7.2, and you MUST pip install the packages needed in mml, like statsmodels. I will speak of all those packages you need to preinstall in README.md. Last but not least, never use 'from mml-qae import *'. Many methods in mml are the same name with the built-in functions! That'll be all, and have fun with MachineLearning and DataDealing!
 + Packages needed
 > + statsmodels
 > + sklearn
 > + jieba
 > + spaCy
 > + pandas
 > + numpy
 > + matplotlib
 > + wordcloud
 > + opencv-python
 ---
-## 历史版本(包括部分未公布的版本)
-+ 1 简易大数据处理与网络构建
-> +  1.0 预发布版本
-> > + 1.0.0 
->      初代版本，无项目描述。
-> > + 1.0.1
->      修复1.0.0中的明显问题。
-> > > + 1.0.1.1  加入项目描述.
-> > > + 1.0.1.2  加入帮助文档README.md并修复一些小问题
-> > > + 1.0.1.3  加入一些自定义错误和修复一些小问题
-> >  + 1.0.2
->      加入封装好的自然语言处理快捷方法。
-> > > + 1.0.2.1  加入中文处理模型(初步).
-> > > + 1.0.2.2  加入英语处理模型.
-> >  + 1.0.3     修复1.0版本的bug和问题。
-> +  1.1 完善版本
-> >  + 1.1.1 加入数据库处理方法。
-> > > + 1.1.1.1 MySQL
-> > > + 1.1.1.2 NoSQL
-> > > + 1.1.1.3 更多数据库
-> >  + 1.1.2 Spark多线程方法封装
-> > > + 1.1.2.1 多线程封装
-> > > + 1.1.2.2 集群管理方法封装
-> >  + 1.1.3 简易网络构建方法封装
-> > > + 1.1.3.1 本地index.html的构建方法封装
-> > > + 1.1.3.2 爬虫的封装
-> + 1.2 修复版本
+## Documents for easily using
+### builtins
+In this package, it usually doesn't have a started print. But if you DO NOT have all the packages we need, it will raise a ImportError just after import. The common builtin values are like __versions__,__name__ or sth. like __doc__.
+### Chinese_dealing
+With this package, you can use the following methods:
+#### add(words,tag)
+The two values are all must-needed. They must be same-shape lists, and the elements of both must correspond one-to-one. All elements must be strings. They will be added as new words one by one in the jieba.
+#### make_words_list(text)
+The parameter text must be given. This method will split the given text into several words and return the list form.
+#### make_words_list_with_tags(text)
+The parameter text must be given. This method splits the given text into several words and returns a list format, including the part of speech of each word; The return format is two lists, each containing participles and corresponding parts of speech.
+#### make_words_list_with_extra_words(text,path1,path2)
+To use this method, you must download jiebapos.xlsx and data3-1.txt from Git at https://github.com/ZYpS-leader/mml-qae. Pass in their absolute paths on the local machine, which should end with ".../jiebapos. xlsx" and ".../data3-1. txt". The return value is the same as make_words_list_with_tags method.
```

### Comparing `mml_qae-1.0.2.12/pyproject.toml` & `mml_qae-1.0.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mml_qae"
-version = "1.0.2.12"
+version = "1.0.3.1"
 authors = [
   { name="ETRO_secondleader", email="ETRO_gfyx@163.com" },
 ]
 description = "The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning."
 readme = "README.md"
 requires-python = "==3.7.2"
 classifiers = [
```

### Comparing `mml_qae-1.0.2.12/setup.py` & `mml_qae-1.0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools 
 
 with open("README.md", "r",encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
       name='mml_qae',
-      version='1.0.2.12',
+      version='1.0.3.1',
       description='The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='ETRO_secondleader',
       author_email='ETRO_gfyx@163.com',
       url='https://www.python.org', 
       packages=setuptools.find_packages(),
```

