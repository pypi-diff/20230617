# Comparing `tmp/cloud_radar-0.8.0a1.tar.gz` & `tmp/cloud_radar-0.8.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_radar-0.8.0a1.tar", max compression
+gzip compressed data, was "cloud_radar-0.8.1a0.tar", max compression
```

## Comparing `cloud_radar-0.8.0a1.tar` & `cloud_radar-0.8.1a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-06-14 15:29:38.872218 cloud_radar-0.8.0a1/LICENSE.txt
--rw-r--r--   0        0        0    13927 2023-06-14 15:29:38.872218 cloud_radar-0.8.0a1/README.md
--rw-r--r--   0        0        0     1435 2023-06-14 15:29:52.756453 cloud_radar-0.8.0a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-14 15:29:38.872218 cloud_radar-0.8.0a1/src/cloud_radar/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 15:29:38.872218 cloud_radar-0.8.0a1/src/cloud_radar/cf/__init__.py
--rw-r--r--   0        0        0       48 2023-06-14 15:29:38.872218 cloud_radar-0.8.0a1/src/cloud_radar/cf/e2e/__init__.py
--rw-r--r--   0        0        0     1677 2023-06-14 15:29:38.872218 cloud_radar-0.8.0a1/src/cloud_radar/cf/e2e/_stack.py
--rw-r--r--   0        0        0       57 2023-06-14 15:29:38.872218 cloud_radar-0.8.0a1/src/cloud_radar/cf/unit/__init__.py
--rw-r--r--   0        0        0      711 2023-06-14 15:29:38.872218 cloud_radar-0.8.0a1/src/cloud_radar/cf/unit/_condition.py
--rw-r--r--   0        0        0     1822 2023-06-14 15:29:38.872218 cloud_radar-0.8.0a1/src/cloud_radar/cf/unit/_output.py
--rw-r--r--   0        0        0     3199 2023-06-14 15:29:38.872218 cloud_radar-0.8.0a1/src/cloud_radar/cf/unit/_parameter.py
--rw-r--r--   0        0        0     3872 2023-06-14 15:29:38.872218 cloud_radar-0.8.0a1/src/cloud_radar/cf/unit/_resource.py
--rw-r--r--   0        0        0     5230 2023-06-14 15:29:38.876218 cloud_radar-0.8.0a1/src/cloud_radar/cf/unit/_stack.py
--rw-r--r--   0        0        0    15434 2023-06-14 15:29:38.876218 cloud_radar-0.8.0a1/src/cloud_radar/cf/unit/_template.py
--rw-r--r--   0        0        0    24791 2023-06-14 15:29:38.876218 cloud_radar-0.8.0a1/src/cloud_radar/cf/unit/functions.py
--rw-r--r--   0        0        0    15083 1970-01-01 00:00:00.000000 cloud_radar-0.8.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 03:13:35.373149 cloud_radar-0.8.1a0/LICENSE.txt
+-rw-r--r--   0        0        0    13927 2023-06-16 03:13:35.373149 cloud_radar-0.8.1a0/README.md
+-rw-r--r--   0        0        0     1435 2023-06-16 03:13:47.249409 cloud_radar-0.8.1a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-16 03:13:35.377150 cloud_radar-0.8.1a0/src/cloud_radar/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 03:13:35.377150 cloud_radar-0.8.1a0/src/cloud_radar/cf/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-16 03:13:35.377150 cloud_radar-0.8.1a0/src/cloud_radar/cf/e2e/__init__.py
+-rw-r--r--   0        0        0     1677 2023-06-16 03:13:35.377150 cloud_radar-0.8.1a0/src/cloud_radar/cf/e2e/_stack.py
+-rw-r--r--   0        0        0       57 2023-06-16 03:13:35.377150 cloud_radar-0.8.1a0/src/cloud_radar/cf/unit/__init__.py
+-rw-r--r--   0        0        0      711 2023-06-16 03:13:35.377150 cloud_radar-0.8.1a0/src/cloud_radar/cf/unit/_condition.py
+-rw-r--r--   0        0        0     1822 2023-06-16 03:13:35.377150 cloud_radar-0.8.1a0/src/cloud_radar/cf/unit/_output.py
+-rw-r--r--   0        0        0     3199 2023-06-16 03:13:35.377150 cloud_radar-0.8.1a0/src/cloud_radar/cf/unit/_parameter.py
+-rw-r--r--   0        0        0     3872 2023-06-16 03:13:35.377150 cloud_radar-0.8.1a0/src/cloud_radar/cf/unit/_resource.py
+-rw-r--r--   0        0        0     5230 2023-06-16 03:13:35.377150 cloud_radar-0.8.1a0/src/cloud_radar/cf/unit/_stack.py
+-rw-r--r--   0        0        0    20552 2023-06-16 03:13:35.377150 cloud_radar-0.8.1a0/src/cloud_radar/cf/unit/_template.py
+-rw-r--r--   0        0        0    24791 2023-06-16 03:13:35.377150 cloud_radar-0.8.1a0/src/cloud_radar/cf/unit/functions.py
+-rw-r--r--   0        0        0    15083 1970-01-01 00:00:00.000000 cloud_radar-0.8.1a0/PKG-INFO
```

### Comparing `cloud_radar-0.8.0a1/LICENSE.txt` & `cloud_radar-0.8.1a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.0a1/README.md` & `cloud_radar-0.8.1a0/README.md`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.0a1/pyproject.toml` & `cloud_radar-0.8.1a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloud-radar"
-version = "0.8.0a1"
+version = "0.8.1a0"
 description = "Run functional tests on cloudformation stacks."
 readme = "README.md"
 authors = ["Levi Blaney <shadycuz@gmail.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/DontShaveTheYak/cloud-radar"
 keywords = ["aws", "cloudformation", "cloud-radar", "testing", "taskcat", "cloud", "radar"]
 classifiers = [
```

### Comparing `cloud_radar-0.8.0a1/src/cloud_radar/cf/e2e/_stack.py` & `cloud_radar-0.8.1a0/src/cloud_radar/cf/e2e/_stack.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.0a1/src/cloud_radar/cf/unit/_condition.py` & `cloud_radar-0.8.1a0/src/cloud_radar/cf/unit/_condition.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.0a1/src/cloud_radar/cf/unit/_output.py` & `cloud_radar-0.8.1a0/src/cloud_radar/cf/unit/_output.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.0a1/src/cloud_radar/cf/unit/_parameter.py` & `cloud_radar-0.8.1a0/src/cloud_radar/cf/unit/_parameter.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.0a1/src/cloud_radar/cf/unit/_resource.py` & `cloud_radar-0.8.1a0/src/cloud_radar/cf/unit/_resource.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.0a1/src/cloud_radar/cf/unit/_stack.py` & `cloud_radar-0.8.1a0/src/cloud_radar/cf/unit/_stack.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.0a1/src/cloud_radar/cf/unit/_template.py` & `cloud_radar-0.8.1a0/src/cloud_radar/cf/unit/_template.py`

 * *Files 18% similar despite different names*

```diff
@@ -369,25 +369,163 @@
         t_params: dict = self.template["Parameters"]
 
         if set(parameters) - set(t_params):
             raise ValueError("You passed a Parameter that was not in the Template.")
 
         for p_name, p_value in t_params.items():
             if p_name in parameters:
+                validate_parameter_constraints(
+                    p_name, t_params[p_name], parameters[p_name]
+                )
+
                 t_params[p_name]["Value"] = parameters[p_name]
                 continue
 
             if "Default" not in p_value:
                 raise ValueError(
                     "Must provide values for parameters that don't have a default value."
                 )
 
             t_params[p_name]["Value"] = p_value["Default"]
 
 
+def validate_parameter_constraints(
+    parameter_name: str, parameter_definition: dict, parameter_value: str
+):
+    """
+    Validate that the parameter value matches any constraints
+    for allowed values, allowed patterns etc.
+    This method will raise a ValueError if any validation constraints
+    are not met.
+    Args:
+        parameter_name (str): The name of the parameter being validated
+        parameter_definition (Dict): The parameter definition being validated
+                                    against
+        parameter_value (str): The supplied parameter value being validated
+    """
+    if parameter_definition["Type"] == "String":
+        validate_string_parameter_constraints(
+            parameter_name, parameter_definition, parameter_value
+        )
+    elif parameter_definition["Type"] == "CommaDelimitedList":
+        # When applied to a parameter of type CommaDelimitedList,
+        # each value in the list must meet the String type criteria
+        for part in parameter_value.split(","):
+            validate_string_parameter_constraints(
+                parameter_name, parameter_definition, part.strip()
+            )
+    elif parameter_definition["Type"] == "Number":
+        validate_number_parameter_constraints(
+            parameter_name, parameter_definition, parameter_value
+        )
+    elif parameter_definition["Type"] == "List<Number>":
+        # The docs are not as clear here but I think it will be
+        # the same as CommaDelimitedList - run the number parameter
+        # constraints for each item in the list
+        for part in parameter_value.split(","):
+            validate_number_parameter_constraints(
+                parameter_name, parameter_definition, part.strip()
+            )
+
+
+def validate_number_parameter_constraints(
+    parameter_name: str, parameter_definition: dict, parameter_value: str
+):
+    """
+    Validate that the parameter value matches any constraints
+    that are applicable for Number value parameters
+    (min/max value)
+    This method will raise a ValueError if any validation constraints
+    are not met.
+    Args:
+        parameter_name (str): The name of the parameter being validated
+        parameter_definition (Dict): The parameter definition being validated
+                                    against
+        parameter_value (str): The supplied parameter value being validated
+    """
+    if "MinValue" in parameter_definition and int(parameter_value) < int(
+        parameter_definition["MinValue"]
+    ):
+        raise ValueError(
+            (
+                f"Value {parameter_value} is below the minimum value for"
+                f" parameter {parameter_name}"
+            )
+        )
+
+    if "MaxValue" in parameter_definition and int(parameter_value) > int(
+        parameter_definition["MaxValue"]
+    ):
+        raise ValueError(
+            (
+                f"Value {parameter_value} is above the maximum value for"
+                f" parameter {parameter_name}"
+            )
+        )
+
+
+def validate_string_parameter_constraints(
+    parameter_name: str, parameter_definition: dict, parameter_value: str
+):
+    """
+    Validate that the parameter value matches any constraints
+    that are applicable for String value parameters
+    (allowed values, allowed patterns, min/max length)
+    This method will raise a ValueError if any validation constraints
+    are not met.
+    Args:
+        parameter_name (str): The name of the parameter being validated
+        parameter_definition (Dict): The parameter definition being validated
+                                    against
+        parameter_value (str): The supplied parameter value being validated
+    """
+
+    # Compare allowed values
+    if (
+        "AllowedValues" in parameter_definition
+        and parameter_value not in parameter_definition["AllowedValues"]
+    ):
+        raise ValueError(
+            (
+                f"Value {parameter_value} not in allowed "
+                f"values for parameter {parameter_name}"
+            )
+        )
+
+    if "AllowedPattern" in parameter_definition and not re.match(
+        parameter_definition["AllowedPattern"], parameter_value
+    ):
+        raise ValueError(
+            (
+                f"Value {parameter_value} does not match the AllowedPattern "
+                f"for parameter {parameter_name}"
+            )
+        )
+
+    if "MinLength" in parameter_definition and len(parameter_value) < int(
+        parameter_definition["MinLength"]
+    ):
+        raise ValueError(
+            (
+                f"Value {parameter_value} is shorter than the minimum length for"
+                f" parameter {parameter_name}"
+            )
+        )
+
+    if "MaxLength" in parameter_definition and len(parameter_value) > int(
+        parameter_definition["MaxLength"]
+    ):
+        raise ValueError(
+            (
+                f"Value {parameter_value} is longer than the maximum length for"
+                f" parameter {parameter_name}"
+            )
+        )
+
+
 def add_metadata(template: Dict, region: str) -> None:
     """This functions adds the current region to the template
     as metadate because we can't treat Region like a normal pseduo
     variables because we don't want to update the class var for every run.
 
     Args:
         template (Dict): The template you want to update.
```

### Comparing `cloud_radar-0.8.0a1/src/cloud_radar/cf/unit/functions.py` & `cloud_radar-0.8.1a0/src/cloud_radar/cf/unit/functions.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.0a1/PKG-INFO` & `cloud_radar-0.8.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-radar
-Version: 0.8.0a1
+Version: 0.8.1a0
 Summary: Run functional tests on cloudformation stacks.
 Home-page: https://github.com/DontShaveTheYak/cloud-radar
 License: Apache-2.0
 Keywords: aws,cloudformation,cloud-radar,testing,taskcat,cloud,radar
 Author: Levi Blaney
 Author-email: shadycuz@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-radar Version: 0.8.0a1 Summary: Run
+Metadata-Version: 2.1 Name: cloud-radar Version: 0.8.1a0 Summary: Run
 functional tests on cloudformation stacks. Home-page: https://github.com/
 DontShaveTheYak/cloud-radar License: Apache-2.0 Keywords:
 aws,cloudformation,cloud-radar,testing,taskcat,cloud,radar Author: Levi Blaney
 Author-email: shadycuz@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

