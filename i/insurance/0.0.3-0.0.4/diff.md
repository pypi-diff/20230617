# Comparing `tmp/insurance-0.0.3.tar.gz` & `tmp/insurance-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insurance-0.0.3.tar", last modified: Sat Jun 17 11:17:04 2023, max compression
+gzip compressed data, was "insurance-0.0.4.tar", last modified: Sat Jun 17 11:30:19 2023, max compression
```

## Comparing `insurance-0.0.3.tar` & `insurance-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 11:17:04.349453 insurance-0.0.3/
--rw-rw-rw-   0        0        0      421 2023-06-16 16:24:14.000000 insurance-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      480 2023-06-17 11:17:04.347454 insurance-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-17 11:17:04.303450 insurance-0.0.3/insurance.egg-info/
--rw-rw-rw-   0        0        0      480 2023-06-17 11:17:04.000000 insurance-0.0.3/insurance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      701 2023-06-17 11:17:04.000000 insurance-0.0.3/insurance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 11:17:04.000000 insurance-0.0.3/insurance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      189 2023-06-17 11:17:04.000000 insurance-0.0.3/insurance.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-17 11:17:04.000000 insurance-0.0.3/insurance.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-17 11:17:04.318453 insurance-0.0.3/my_model/
--rw-rw-rw-   0        0        0        7 2023-06-17 11:14:02.000000 insurance-0.0.3/my_model/VERSION
--rw-rw-rw-   0        0        0      867 2023-06-13 17:31:06.000000 insurance-0.0.3/my_model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 11:17:04.321451 insurance-0.0.3/my_model/config/
--rw-rw-rw-   0        0        0        0 2023-06-08 18:33:12.000000 insurance-0.0.3/my_model/config/__init__.py
--rw-rw-rw-   0        0        0     2180 2023-06-17 07:59:48.000000 insurance-0.0.3/my_model/config/core.py
--rw-rw-rw-   0        0        0      481 2023-06-17 08:40:37.000000 insurance-0.0.3/my_model/config.yml
-drwxrwxrwx   0        0        0        0 2023-06-17 11:17:04.329454 insurance-0.0.3/my_model/datasets/
--rw-rw-rw-   0        0        0        0 2023-06-08 18:33:12.000000 insurance-0.0.3/my_model/datasets/__init__.py
--rw-rw-rw-   0        0        0    16761 2023-06-16 16:26:26.000000 insurance-0.0.3/my_model/datasets/test.csv
--rw-rw-rw-   0        0        0    38971 2023-06-16 16:00:50.000000 insurance-0.0.3/my_model/datasets/train.csv
--rw-rw-rw-   0        0        0     1173 2023-06-17 08:02:07.000000 insurance-0.0.3/my_model/pipeline.py
--rw-rw-rw-   0        0        0     1233 2023-06-17 09:12:55.000000 insurance-0.0.3/my_model/predict.py
-drwxrwxrwx   0        0        0        0 2023-06-17 11:17:04.335450 insurance-0.0.3/my_model/processing/
--rw-rw-rw-   0        0        0        0 2023-06-13 17:31:06.000000 insurance-0.0.3/my_model/processing/__init__.py
--rw-rw-rw-   0        0        0     1669 2023-06-16 15:48:07.000000 insurance-0.0.3/my_model/processing/data_manager.py
--rw-rw-rw-   0        0        0     1894 2023-06-17 11:00:23.000000 insurance-0.0.3/my_model/processing/validation.py
--rw-rw-rw-   0        0        0     1447 2023-06-17 08:02:09.000000 insurance-0.0.3/my_model/train_pipeline.py
-drwxrwxrwx   0        0        0        0 2023-06-17 11:17:04.337453 insurance-0.0.3/my_model/trained_models/
--rw-rw-rw-   0        0        0     4083 2023-06-15 19:37:56.000000 insurance-0.0.3/my_model/trained_models/pl_insurance_0.0.3.pkl
--rw-rw-rw-   0        0        0     1991 2023-06-13 17:31:06.000000 insurance-0.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-17 11:17:04.342452 insurance-0.0.3/requirements/
--rw-rw-rw-   0        0        0      576 2023-06-14 18:12:15.000000 insurance-0.0.3/requirements/requirements.txt
--rw-rw-rw-   0        0        0      298 2023-06-13 17:31:06.000000 insurance-0.0.3/requirements/test_requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 11:17:04.349453 insurance-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1349 2023-06-17 09:15:14.000000 insurance-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 11:17:04.345467 insurance-0.0.3/tests/
--rw-rw-rw-   0        0        0      590 2023-06-16 16:26:50.000000 insurance-0.0.3/tests/test_prediction.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:30:19.680277 insurance-0.0.4/
+-rw-rw-rw-   0        0        0      421 2023-06-16 16:24:14.000000 insurance-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      480 2023-06-17 11:30:19.677272 insurance-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-17 11:30:19.625264 insurance-0.0.4/insurance.egg-info/
+-rw-rw-rw-   0        0        0      480 2023-06-17 11:30:19.000000 insurance-0.0.4/insurance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      701 2023-06-17 11:30:19.000000 insurance-0.0.4/insurance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 11:30:19.000000 insurance-0.0.4/insurance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      189 2023-06-17 11:30:19.000000 insurance-0.0.4/insurance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-17 11:30:19.000000 insurance-0.0.4/insurance.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 11:30:19.640266 insurance-0.0.4/my_model/
+-rw-rw-rw-   0        0        0        7 2023-06-17 11:28:49.000000 insurance-0.0.4/my_model/VERSION
+-rw-rw-rw-   0        0        0      867 2023-06-13 17:31:06.000000 insurance-0.0.4/my_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:30:19.644267 insurance-0.0.4/my_model/config/
+-rw-rw-rw-   0        0        0        0 2023-06-08 18:33:12.000000 insurance-0.0.4/my_model/config/__init__.py
+-rw-rw-rw-   0        0        0     2180 2023-06-17 07:59:48.000000 insurance-0.0.4/my_model/config/core.py
+-rw-rw-rw-   0        0        0      481 2023-06-17 08:40:37.000000 insurance-0.0.4/my_model/config.yml
+drwxrwxrwx   0        0        0        0 2023-06-17 11:30:19.650265 insurance-0.0.4/my_model/datasets/
+-rw-rw-rw-   0        0        0        0 2023-06-08 18:33:12.000000 insurance-0.0.4/my_model/datasets/__init__.py
+-rw-rw-rw-   0        0        0    16761 2023-06-16 16:26:26.000000 insurance-0.0.4/my_model/datasets/test.csv
+-rw-rw-rw-   0        0        0    38971 2023-06-16 16:00:50.000000 insurance-0.0.4/my_model/datasets/train.csv
+-rw-rw-rw-   0        0        0     1173 2023-06-17 08:02:07.000000 insurance-0.0.4/my_model/pipeline.py
+-rw-rw-rw-   0        0        0     1233 2023-06-17 09:12:55.000000 insurance-0.0.4/my_model/predict.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:30:19.667266 insurance-0.0.4/my_model/processing/
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:31:06.000000 insurance-0.0.4/my_model/processing/__init__.py
+-rw-rw-rw-   0        0        0     1669 2023-06-16 15:48:07.000000 insurance-0.0.4/my_model/processing/data_manager.py
+-rw-rw-rw-   0        0        0     1893 2023-06-17 11:28:19.000000 insurance-0.0.4/my_model/processing/validation.py
+-rw-rw-rw-   0        0        0     1447 2023-06-17 08:02:09.000000 insurance-0.0.4/my_model/train_pipeline.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:30:19.669268 insurance-0.0.4/my_model/trained_models/
+-rw-rw-rw-   0        0        0     4083 2023-06-15 19:37:56.000000 insurance-0.0.4/my_model/trained_models/pl_insurance_0.0.4.pkl
+-rw-rw-rw-   0        0        0     1991 2023-06-13 17:31:06.000000 insurance-0.0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-17 11:30:19.673266 insurance-0.0.4/requirements/
+-rw-rw-rw-   0        0        0      576 2023-06-14 18:12:15.000000 insurance-0.0.4/requirements/requirements.txt
+-rw-rw-rw-   0        0        0      298 2023-06-13 17:31:06.000000 insurance-0.0.4/requirements/test_requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 11:30:19.681267 insurance-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1349 2023-06-17 09:15:14.000000 insurance-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:30:19.674266 insurance-0.0.4/tests/
+-rw-rw-rw-   0        0        0      590 2023-06-16 16:26:50.000000 insurance-0.0.4/tests/test_prediction.py
```

### Comparing `insurance-0.0.3/insurance.egg-info/SOURCES.txt` & `insurance-0.0.4/insurance.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 my_model/config/core.py
 my_model/datasets/__init__.py
 my_model/datasets/test.csv
 my_model/datasets/train.csv
 my_model/processing/__init__.py
 my_model/processing/data_manager.py
 my_model/processing/validation.py
-my_model/trained_models/pl_insurance_0.0.3.pkl
+my_model/trained_models/pl_insurance_0.0.4.pkl
 requirements/requirements.txt
 requirements/test_requirements.txt
 tests/test_prediction.py
```

### Comparing `insurance-0.0.3/my_model/__init__.py` & `insurance-0.0.4/my_model/__init__.py`

 * *Files identical despite different names*

### Comparing `insurance-0.0.3/my_model/config/core.py` & `insurance-0.0.4/my_model/config/core.py`

 * *Files identical despite different names*

### Comparing `insurance-0.0.3/my_model/datasets/test.csv` & `insurance-0.0.4/my_model/datasets/test.csv`

 * *Files identical despite different names*

### Comparing `insurance-0.0.3/my_model/datasets/train.csv` & `insurance-0.0.4/my_model/datasets/train.csv`

 * *Files identical despite different names*

### Comparing `insurance-0.0.3/my_model/pipeline.py` & `insurance-0.0.4/my_model/pipeline.py`

 * *Files identical despite different names*

### Comparing `insurance-0.0.3/my_model/predict.py` & `insurance-0.0.4/my_model/predict.py`

 * *Files identical despite different names*

### Comparing `insurance-0.0.3/my_model/processing/data_manager.py` & `insurance-0.0.4/my_model/processing/data_manager.py`

 * *Files identical despite different names*

### Comparing `insurance-0.0.3/my_model/processing/validation.py` & `insurance-0.0.4/my_model/processing/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     try:
         # replace numpy nans so that pydantic can validate
 #        MultipleGenderDataInputs(inputs=validated_data.replace({np.nan: None}).to_dict(orient="records"))
         MultipleGenderDataInputs(inputs=relevant_data.replace({np.nan: None}).to_dict(orient="records"))
     except ValidationError as error:
         errors = error.json()
 
-    return validated_data, errors
+    return relevant_data, errors
 
 
 class GenderDataInputSchema(BaseModel):
     age: Optional[int]
     bmi: Optional[float]
     sex: Optional[str]
     smoker: Optional[str]
```

### Comparing `insurance-0.0.3/my_model/train_pipeline.py` & `insurance-0.0.4/my_model/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `insurance-0.0.3/my_model/trained_models/pl_insurance_0.0.3.pkl` & `insurance-0.0.4/my_model/trained_models/pl_insurance_0.0.4.pkl`

 * *Files identical despite different names*

### Comparing `insurance-0.0.3/pyproject.toml` & `insurance-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `insurance-0.0.3/requirements/requirements.txt` & `insurance-0.0.4/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `insurance-0.0.3/setup.py` & `insurance-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `insurance-0.0.3/tests/test_prediction.py` & `insurance-0.0.4/tests/test_prediction.py`

 * *Files identical despite different names*

