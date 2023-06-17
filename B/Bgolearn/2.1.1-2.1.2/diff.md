# Comparing `tmp/Bgolearn-2.1.1.tar.gz` & `tmp/Bgolearn-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bgolearn-2.1.1.tar", last modified: Fri Jun  9 00:10:45 2023, max compression
+gzip compressed data, was "Bgolearn-2.1.2.tar", last modified: Sat Jun 17 08:18:13 2023, max compression
```

## Comparing `Bgolearn-2.1.1.tar` & `Bgolearn-2.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-09 00:10:45.002756 Bgolearn-2.1.1/
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-09 00:10:45.001865 Bgolearn-2.1.1/Bgolearn/
--rwxr-xr-x   0 jacob      (501) staff       (20)    24205 2023-04-06 12:56:14.000000 Bgolearn-2.1.1/Bgolearn/BGO_eval.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     3932 2023-04-23 02:14:51.000000 Bgolearn-2.1.1/Bgolearn/BGOclf.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    18438 2022-10-13 07:31:41.000000 Bgolearn-2.1.1/Bgolearn/BGOmax.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    18412 2022-10-14 04:10:19.000000 Bgolearn-2.1.1/Bgolearn/BGOmin.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    21169 2023-06-09 00:10:03.000000 Bgolearn-2.1.1/Bgolearn/BGOsampling.py
--rwxr-xr-x   0 jacob      (501) staff       (20)      508 2023-06-09 00:06:27.000000 Bgolearn-2.1.1/Bgolearn/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-09 00:10:45.002462 Bgolearn-2.1.1/Bgolearn.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-06-09 00:10:44.000000 Bgolearn-2.1.1/Bgolearn.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      300 2023-06-09 00:10:44.000000 Bgolearn-2.1.1/Bgolearn.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-06-09 00:10:44.000000 Bgolearn-2.1.1/Bgolearn.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       43 2023-06-09 00:10:44.000000 Bgolearn-2.1.1/Bgolearn.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        9 2023-06-09 00:10:44.000000 Bgolearn-2.1.1/Bgolearn.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-06-09 00:10:45.002627 Bgolearn-2.1.1/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)     1917 2022-11-06 12:06:03.000000 Bgolearn-2.1.1/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-06-09 00:10:45.002798 Bgolearn-2.1.1/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1366 2023-06-09 00:10:21.000000 Bgolearn-2.1.1/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-17 08:18:13.905232 Bgolearn-2.1.2/
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-17 08:18:13.904304 Bgolearn-2.1.2/Bgolearn/
+-rwxr-xr-x   0 jacob      (501) staff       (20)    24205 2023-04-06 12:56:14.000000 Bgolearn-2.1.2/Bgolearn/BGO_eval.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     3932 2023-04-23 02:14:51.000000 Bgolearn-2.1.2/Bgolearn/BGOclf.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    18438 2022-10-13 07:31:41.000000 Bgolearn-2.1.2/Bgolearn/BGOmax.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    18412 2022-10-14 04:10:19.000000 Bgolearn-2.1.2/Bgolearn/BGOmin.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    21249 2023-06-17 08:17:00.000000 Bgolearn-2.1.2/Bgolearn/BGOsampling.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)      508 2023-06-09 00:06:27.000000 Bgolearn-2.1.2/Bgolearn/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-17 08:18:13.904925 Bgolearn-2.1.2/Bgolearn.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-06-17 08:18:13.000000 Bgolearn-2.1.2/Bgolearn.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      300 2023-06-17 08:18:13.000000 Bgolearn-2.1.2/Bgolearn.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-06-17 08:18:13.000000 Bgolearn-2.1.2/Bgolearn.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       43 2023-06-17 08:18:13.000000 Bgolearn-2.1.2/Bgolearn.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        9 2023-06-17 08:18:13.000000 Bgolearn-2.1.2/Bgolearn.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-06-17 08:18:13.905100 Bgolearn-2.1.2/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)     1917 2022-11-06 12:06:03.000000 Bgolearn-2.1.2/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-06-17 08:18:13.905276 Bgolearn-2.1.2/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1366 2023-06-17 08:17:20.000000 Bgolearn-2.1.2/setup.py
```

### Comparing `Bgolearn-2.1.1/Bgolearn/BGO_eval.py` & `Bgolearn-2.1.2/Bgolearn/BGO_eval.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.1.1/Bgolearn/BGOclf.py` & `Bgolearn-2.1.2/Bgolearn/BGOclf.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.1.1/Bgolearn/BGOmax.py` & `Bgolearn-2.1.2/Bgolearn/BGOmax.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.1.1/Bgolearn/BGOmin.py` & `Bgolearn-2.1.2/Bgolearn/BGOmin.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.1.1/Bgolearn/BGOsampling.py` & `Bgolearn-2.1.2/Bgolearn/BGOsampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,47 +101,47 @@
                 kernel = 1 * RBF() 
                 if noise_std == None:
                     # call the default model;
                     class Kriging_model(object):
                         def fit_pre(self,xtrain,ytrain,xtest,):
                             # estimating Noise Level of training dataset
                             noise_ker = WhiteKernel(noise_level_bounds=(0.001,0.5))
-                            GPr = GaussianProcessRegressor(kernel= 1 * RBF()+noise_ker,normalize_y=True).fit(xtrain,ytrain)
+                            GPr = GaussianProcessRegressor(kernel= 1 * RBF()+noise_ker,normalize_y=True).fit(np.array(xtrain),ytrain)
                             noise_level = np.exp(GPr.kernel_.theta[1])
         
                             # ret_std is a placeholder for homogenous noise
                             # instantiated mode
-                            mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = noise_level).fit(xtrain,ytrain)
+                            mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = noise_level).fit(np.array(xtrain),ytrain)
                             # defined the attribute's outputs
                             mean,std = mdoel.predict(xtest,return_std=True)
                             return mean,std 
                     print('The internal model is instantiated with optimized homogenous noise')  
 
                 elif type(noise_std) == float:
                     # call the default model;
                     class Kriging_model(object):
                         def fit_pre(self,xtrain,ytrain,xtest,):
                             # ret_std is a placeholder for homogenous noise
                             # instantiated mode
-                            mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = noise_std**2).fit(xtrain,ytrain)
+                            mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = noise_std**2).fit(np.array(xtrain),ytrain)
                             # defined the attribute's outputs
                             mean,std = mdoel.predict(xtest,return_std=True)
                             return mean,std 
                     print('The internal model is instantiated with homogenous noise: %s' % noise_std)  
                 
                 elif type(noise_std) == np.ndarray:
                     # call the default model;
                     class Kriging_model(object):
                         def fit_pre(self,xtrain,ytrain,xtest,ret_std = 0.0):
                             # instantiated model
                             if len(xtrain) == len(noise_std):
-                                mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = noise_std**2).fit(xtrain,ytrain)
+                                mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = noise_std**2).fit(np.array(xtrain),ytrain)
                             elif len(xtrain) == len(noise_std) + 1:
                                 new_alpha = np.append(noise_std,ret_std)
-                                mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = new_alpha**2).fit(xtrain,ytrain)
+                                mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = new_alpha**2).fit(np.array(xtrain),ytrain)
                             else:
                                 print('the input data is not muached with heterogenous noise size') 
                             # defined the attribute's outputs
                             mean,std = mdoel.predict(xtest,return_std=True)
                             return mean,std  
                     print('The internal model is instantiated with heterogenous noise')
             else: 
@@ -333,30 +333,30 @@
             kernel = RBF() 
             if type(noise_std) == float:
                 # call the default model;
                 class Kriging_model(object):
                     def fit_pre(self,xtrain,ytrain,xtest,):
                         # ret_std is a placeholder for homogenous noise
                         # instantiated mode
-                        mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = noise_std**2).fit(xtrain,ytrain)
+                        mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = noise_std**2).fit(np.array(xtrain),ytrain)
                         # defined the attribute's outputs
                         mean,std = mdoel.predict(xtest,return_std=True)
                         return mean,std 
                 print('The internal model is instantiated with homogenous noise: %s' % noise_std)  
                 
             elif type(noise_std) == np.ndarray:
                 # call the default model;
                 class Kriging_model(object):
                     def fit_pre(self,xtrain,ytrain,xtest,ret_std = 0.0):
                         # instantiated model
                         if len(xtrain) == len(noise_std):
-                            mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = noise_std**2).fit(xtrain,ytrain)
+                            mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = noise_std**2).fit(np.array(xtrain),ytrain)
                         elif len(xtrain) == len(noise_std) + 1:
                             new_alpha = np.append(noise_std,ret_std)
-                            mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = new_alpha**2).fit(xtrain,ytrain)
+                            mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = new_alpha**2).fit(np.array(xtrain),ytrain)
                         else:
                             print('the input data is not muached with heterogenous noise size') 
                         # defined the attribute's outputs
                         mean,std = mdoel.predict(xtest,return_std=True)
                         return mean,std  
                 print('The internal model is instantiated with heterogenous noise')
         else:
```

### Comparing `Bgolearn-2.1.1/Bgolearn.egg-info/PKG-INFO` & `Bgolearn-2.1.2/Bgolearn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bgolearn
-Version: 2.1.1
+Version: 2.1.2
 Summary: A Bayesian global optimization package for material design
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `Bgolearn-2.1.1/PKG-INFO` & `Bgolearn-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bgolearn
-Version: 2.1.1
+Version: 2.1.2
 Summary: A Bayesian global optimization package for material design
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `Bgolearn-2.1.1/README.md` & `Bgolearn-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.1.1/setup.py` & `Bgolearn-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='Bgolearn',  # 包名
-    version='2.1.1',  # 版本
+    version='2.1.2',  # 版本
     description="A Bayesian global optimization package for material design",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

