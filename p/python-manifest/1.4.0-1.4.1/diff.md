# Comparing `tmp/python_manifest-1.4.0-py3-none-any.whl.zip` & `tmp/python_manifest-1.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 19891 bytes, number of entries: 22
+Zip file size: 20072 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      230 b- defN 80-Jan-01 00:00 manifest/__init__.py
--rw-r--r--  2.0 unx    10808 b- defN 80-Jan-01 00:00 manifest/base.py
+-rw-r--r--  2.0 unx    10821 b- defN 80-Jan-01 00:00 manifest/base.py
 -rw-r--r--  2.0 unx      460 b- defN 80-Jan-01 00:00 manifest/hooks/__init__.py
 -rw-r--r--  2.0 unx      549 b- defN 80-Jan-01 00:00 manifest/hooks/builtin.py
 -rw-r--r--  2.0 unx      382 b- defN 80-Jan-01 00:00 manifest/hooks/expressions/__init__.py
 -rw-r--r--  2.0 unx     4581 b- defN 80-Jan-01 00:00 manifest/hooks/expressions/operations.py
 -rw-r--r--  2.0 unx     3238 b- defN 80-Jan-01 00:00 manifest/hooks/expressions/resolve.py
 -rw-r--r--  2.0 unx     2128 b- defN 80-Jan-01 00:00 manifest/hooks/interface.py
 -rw-r--r--  2.0 unx     2085 b- defN 80-Jan-01 00:00 manifest/instantiable.py
--rw-r--r--  2.0 unx    12035 b- defN 80-Jan-01 00:00 manifest/parse.py
+-rw-r--r--  2.0 unx    12327 b- defN 80-Jan-01 00:00 manifest/parse.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 manifest/py.typed
 -rw-r--r--  2.0 unx      386 b- defN 80-Jan-01 00:00 manifest/serializers/__init__.py
 -rw-r--r--  2.0 unx      272 b- defN 80-Jan-01 00:00 manifest/serializers/base.py
 -rw-r--r--  2.0 unx      503 b- defN 80-Jan-01 00:00 manifest/serializers/jsons.py
 -rw-r--r--  2.0 unx      353 b- defN 80-Jan-01 00:00 manifest/serializers/noop.py
 -rw-r--r--  2.0 unx      356 b- defN 80-Jan-01 00:00 manifest/serializers/tomls.py
 -rw-r--r--  2.0 unx      350 b- defN 80-Jan-01 00:00 manifest/serializers/yamls.py
--rw-r--r--  2.0 unx     7718 b- defN 80-Jan-01 00:00 manifest/utils.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 python_manifest-1.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5565 b- defN 80-Jan-01 00:00 python_manifest-1.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 python_manifest-1.4.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1820 b- defN 16-Jan-01 00:00 python_manifest-1.4.0.dist-info/RECORD
-22 files, 54985 bytes uncompressed, 16931 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx     8185 b- defN 80-Jan-01 00:00 manifest/utils.py
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 python_manifest-1.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5565 b- defN 80-Jan-01 00:00 python_manifest-1.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 python_manifest-1.4.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1820 b- defN 16-Jan-01 00:00 python_manifest-1.4.1.dist-info/RECORD
+22 files, 55757 bytes uncompressed, 17112 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: manifest/serializers/yamls.py
 Comment: 
 
 Filename: manifest/utils.py
 Comment: 
 
-Filename: python_manifest-1.4.0.dist-info/LICENSE
+Filename: python_manifest-1.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: python_manifest-1.4.0.dist-info/METADATA
+Filename: python_manifest-1.4.1.dist-info/METADATA
 Comment: 
 
-Filename: python_manifest-1.4.0.dist-info/WHEEL
+Filename: python_manifest-1.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: python_manifest-1.4.0.dist-info/RECORD
+Filename: python_manifest-1.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## manifest/base.py

```diff
@@ -118,15 +118,15 @@
         parsed_env_vars = parse_env_vars(
             env_vars=env_vars,
             prefix=env_prefix,
             delimiter=env_delimiter
         )
 
         # Parse any key_values provided
-        parsed_overrides = parse_key_values(key_values)
+        parsed_overrides = parse_key_values(key_values, coerce=True)
 
         # Merge everything together into a single material dictionary
         material = merge_dicts(parsed_files, parsed_env_vars, parsed_overrides, kwargs)
 
         return cls(**material)
 
     @classmethod
```

## manifest/parse.py

```diff
@@ -330,44 +330,48 @@
             for key, val in env_vars.items()
             # Only parse environment variables that start with the prefix
             if key.startswith(prefix)
         ]
     )
 
 
-def parse_key_value(key_value: str) -> dict:
+def parse_key_value(key_value: str, coerce: bool = False) -> dict:
     """
     Parse a key-value pair in the format "a.b.c=value" and return a dictionary.
 
     :param key_value: A key-value pair in the format "key=value".
     :type key_value: str
+    :param coerce: Whether to coerce the value to a basic type. Defaults to False.
+    :type coerce: bool
     :return: A dictionary containing the parsed key-value pair.
     :rtype: dict[str, Any]
     """
     k, v = key_value.split("=")
-    return set_by_dot_path({}, k, coerce_to_basic_types(v))
+    return set_by_dot_path({}, k, v if not coerce else coerce_to_basic_types(v))
 
 
-def parse_key_values(key_values: list[str]) -> dict:
+def parse_key_values(key_values: list[str], coerce: bool = False) -> dict:
     """
     Parse a list of dot-delimited key value strings and return a nested dictionary.
 
     This function takes a list of dot-delimited strings in the format "a.b.c=value"
     and returns a nested dictionary where each key in the dictionary represents
     a level of nesting in the original dot-delimited string.
 
     :param key_values: A list of dot-delimited strings.
     :type key_values: List[str]
+    :param coerce: Whether to coerce the values to basic types. Defaults to False.
+    :type coerce: bool
     :returns: A nested dictionary containing the parsed key-value pairs.
     :rtype: dict
 
     :Example:
         >>> kvs = ["a.b.c=1", "a.b.d=2", "a.e=3"]
         >>> parse_key_values(kvs)
         {'a': {'b': {'c': '1', 'd': '2'}, 'e': '3'}}
     """
     return merge_dicts(
         *[
-            parse_key_value(key_value)
+            parse_key_value(key_value, coerce=coerce)
             for key_value in key_values
         ]
     )
```

## manifest/utils.py

```diff
@@ -212,47 +212,63 @@
     # parse the URL and get the path
     _, path = url_to_fs(file_path)
     file_name, file_extension = os.path.splitext(path)
 
     return file_extension
 
 
+def coerce_sequence(value: list | tuple) -> list:
+    return [coerce_to_basic_types(item) for item in value]
+
+def coerce_dict(value: dict) -> dict:
+    return {k: coerce_to_basic_types(v) for k, v in value.items()}
+
+def coerce_object(value: object) -> dict:
+    if hasattr(value, '__dict__'):
+        try:
+            return coerce_dict(value.__dict__)
+        except AttributeError:
+            pass
+    return {}
+
+
+def coerce_str(value: str) -> Union[int, float, str, bool, None]:
+    normalized = value.strip().lower()
+    if normalized in ['true', 'false']:
+        return normalized == 'true'
+    elif normalized in ['none', 'null']:
+        return None
+    return coerce_num(value)
+
+
+def coerce_num(value: Union[int, float, str]) -> Union[int, float, str]:
+    try:
+        if "." not in str(value):
+            return int(value)
+        else:
+            return float(value)
+    except ValueError:
+        return str(value)
+
+
 def coerce_to_basic_types(value: Any) -> Union[int, float, bool, str, list, dict, None]:
     """
-    Coerces a given value to basic types, including int, float, bool, and str.
+    Coerces a given value to basic types, including int, float, bool, and str, list, dict, and None.
 
     :param value: The value to be coerced.
     :type value: Any
 
     :return: The coerced value.
     :rtype: Union[int, float, bool, str, List, Dict, None]
     """
-
     if isinstance(value, (list, tuple)):
-        return [coerce_to_basic_types(item) for item in value]
+        return coerce_sequence(value)
     elif isinstance(value, dict):
-        return {k: coerce_to_basic_types(v) for k, v in value.items()}
+        return coerce_dict(value)
     elif hasattr(value, '__dict__'):
-        try:
-            return {k: coerce_to_basic_types(v) for k, v in value.__dict__.items()}
-        except:
-            pass
+        return coerce_object(value)
     elif isinstance(value, str):
-        normalized = value.strip().lower()
-        if normalized in ['true', 'false']:
-            return normalized == 'true'
-        elif normalized in ['none', 'null']:
-            return None
-    elif isinstance(value, bool):
+        return coerce_str(value)
+    elif isinstance(value, bool) or value is None:
         return value
-
-    try:
-        if float(value).is_integer():
-            return int(value)
-        else:
-            return float(value)
-    except:
-        try:
-            return str(value)
-        except:
-            pass
-    return None
+    else:
+        return coerce_num(value)
```

## Comparing `python_manifest-1.4.0.dist-info/LICENSE` & `python_manifest-1.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `python_manifest-1.4.0.dist-info/METADATA` & `python_manifest-1.4.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-manifest
-Version: 1.4.0
+Version: 1.4.1
 Summary: A modern toolkit for working with application manifests and configurations.
 Home-page: https://github.com/emergentmethods/python-manifest
 License: MIT
 Author: Timothy Pogue
 Author-email: tim@emergentmethods.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `python_manifest-1.4.0.dist-info/RECORD` & `python_manifest-1.4.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 manifest/__init__.py,sha256=lPR8D6XQ8nBPlRQEKelo78kQ0gMKANeprcMEZKRevwo,230
-manifest/base.py,sha256=TuG5sE6PS-qo4XoP9fVBdmcQo_x90Z2pw79qv_yLN6M,10808
+manifest/base.py,sha256=uUGZG_F3ysyNFDMza-QzxgVtEZibERIIZaI2POQ7jOs,10821
 manifest/hooks/__init__.py,sha256=xGWUkgzWM7Dp_cMDvqk8bRzi9fiX8GYBzOcVmtWJwuo,460
 manifest/hooks/builtin.py,sha256=EqeD6B9BnA21MdVZiZ54Gz1w7hNnjMBkc64PIzKC-Zw,549
 manifest/hooks/expressions/__init__.py,sha256=hvVL1tr9aCSH7EFeph99CJvKWCP_V4m5KStZx9Hmsqw,382
 manifest/hooks/expressions/operations.py,sha256=PoVZ69D7MTrl5iWze34Gl10WA6sdH7l505T1jKQNiUU,4581
 manifest/hooks/expressions/resolve.py,sha256=VF0l2MTeGGVqCCjQEeFj0Dxqlbz4Hq_jX022Dr0gIu8,3238
 manifest/hooks/interface.py,sha256=xKE-3E3yUV4FuLJWPiMR5UCe6pa-cwSIoP4zK0zxzuM,2128
 manifest/instantiable.py,sha256=TlzW04amYQF26X_iqJU2MMsvplCMogUM6XTwljdwFcc,2085
-manifest/parse.py,sha256=aBjUcUThYdLazCJFOGpgSZRC6mQVLIIyzAx5tUzQ4Uk,12035
+manifest/parse.py,sha256=ldOn4HRMcgORIhtMRShB8XxD1axoy9h-ZH-zMKyOHFM,12327
 manifest/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 manifest/serializers/__init__.py,sha256=4d2mNeR4nZTdHC7Dg5ab7_whcXF_BsXvrhm8whJMeas,386
 manifest/serializers/base.py,sha256=So6sMP502D0fXN84Np0a_c5IGyq4gLWmMXfDwN6xAPg,272
 manifest/serializers/jsons.py,sha256=iK5Tswidrc3CLqeg4YaBNH7Ev6C7cVAQo6pEmDjncIM,503
 manifest/serializers/noop.py,sha256=x0sqDyLDFI-g6K5EnXUex3UVmwLvq-nMFoBj_iNpTys,353
 manifest/serializers/tomls.py,sha256=QxSGa4nWs3SqJAF-Y_64zGfEn_BgPOVs5-bxvS7X6Ro,356
 manifest/serializers/yamls.py,sha256=th77AOLV4I10t_SOLIlqQAsiSGzACzia71vGIi-1Cf0,350
-manifest/utils.py,sha256=bs7Pan15CW8sNldVq0-xuVzYL24vjxpVlzstyHDsH-M,7718
-python_manifest-1.4.0.dist-info/LICENSE,sha256=DEqEB7tSTdQp6PHFAw4I1MyZU02bPaXoSULcNI_49bw,1078
-python_manifest-1.4.0.dist-info/METADATA,sha256=QVTlEkZOmVYghYK8gnR6dYoaQ6zZENV7r-kJyUtxQJw,5565
-python_manifest-1.4.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-python_manifest-1.4.0.dist-info/RECORD,,
+manifest/utils.py,sha256=C5LvlfKPvPEQwBQ7Uq_h4OPNjt-plquJff7qNdHtVHg,8185
+python_manifest-1.4.1.dist-info/LICENSE,sha256=DEqEB7tSTdQp6PHFAw4I1MyZU02bPaXoSULcNI_49bw,1078
+python_manifest-1.4.1.dist-info/METADATA,sha256=p6gM0dWnVkDSXjTg9xS5bIHN8Ff9VNsGMf-ZtCQRYNE,5565
+python_manifest-1.4.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+python_manifest-1.4.1.dist-info/RECORD,,
```

