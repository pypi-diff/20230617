# Comparing `tmp/lamin_logger-0.5.2.tar.gz` & `tmp/lamin_logger-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_logger-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_logger-0.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_logger-0.5.2.tar` & `lamin_logger-0.5.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2370 2023-06-15 15:58:17.266637 lamin_logger-0.5.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-20 18:46:24.119961 lamin_logger-0.5.2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-20 18:46:24.120069 lamin_logger-0.5.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2022-07-20 18:46:24.120174 lamin_logger-0.5.2/.gitignore
--rw-r--r--   0        0        0     1798 2023-06-15 18:19:51.176749 lamin_logger-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-08-08 17:06:33.128130 lamin_logger-0.5.2/LICENSE
--rw-r--r--   0        0        0      357 2022-07-20 18:49:33.932419 lamin_logger-0.5.2/README.md
--rw-r--r--   0        0        0       54 2022-07-20 18:46:24.120507 lamin_logger-0.5.2/docs/api.md
--rw-r--r--   0        0        0     3331 2023-06-16 10:33:14.536633 lamin_logger-0.5.2/docs/changelog.md
--rw-r--r--   0        0        0      124 2022-07-23 18:45:50.337637 lamin_logger-0.5.2/docs/index.md
--rw-r--r--   0        0        0     1360 2023-06-15 15:57:57.600362 lamin_logger-0.5.2/docs/quickstart.ipynb
--rw-r--r--   0        0        0      138 2022-07-20 18:46:24.121862 lamin_logger-0.5.2/lamin-project.yaml
--rw-r--r--   0        0        0      291 2023-06-16 10:33:08.339442 lamin_logger-0.5.2/lamin_logger/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-15 18:19:51.177212 lamin_logger-0.5.2/lamin_logger/_core.py
--rw-r--r--   0        0        0     7600 2023-06-16 10:31:45.152421 lamin_logger-0.5.2/lamin_logger/_logger.py
--rw-r--r--   0        0        0     4157 2023-06-15 22:43:54.438557 lamin_logger-0.5.2/lamin_logger/_lookup.py
--rw-r--r--   0        0        0     4107 2023-06-15 15:58:17.267398 lamin_logger-0.5.2/lamin_logger/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-06-15 18:19:51.177576 lamin_logger-0.5.2/lamin_logger/_python_version.py
--rw-r--r--   0        0        0     2758 2023-06-15 15:58:17.267495 lamin_logger-0.5.2/lamin_logger/_search.py
--rw-r--r--   0        0        0      334 2023-06-15 15:58:17.267619 lamin_logger-0.5.2/noxfile.py
--rw-r--r--   0        0        0      952 2023-06-15 18:19:51.177764 lamin_logger-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      115 2023-06-15 18:19:51.177888 lamin_logger-0.5.2/tests/test_base.py
--rw-r--r--   0        0        0     1356 2023-06-15 15:58:17.267845 lamin_logger-0.5.2/tests/test_lookup.py
--rw-r--r--   0        0        0     2140 2023-06-15 15:58:17.267943 lamin_logger-0.5.2/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-06-15 15:58:17.268069 lamin_logger-0.5.2/tests/test_notebooks.py
--rw-r--r--   0        0        0     2101 2023-06-15 15:58:17.268162 lamin_logger-0.5.2/tests/test_search.py
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.5.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.5.3/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.5.3/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.5.3/LICENSE
+-rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.5.3/README.md
+-rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.5.3/docs/api.md
+-rw-r--r--   0        0        0     3652 2023-06-17 12:56:53.174044 lamin_logger-0.5.3/docs/changelog.md
+-rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.5.3/docs/index.md
+-rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.5.3/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.5.3/lamin-project.yaml
+-rw-r--r--   0        0        0      291 2023-06-17 12:56:43.924366 lamin_logger-0.5.3/lamin_logger/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.5.3/lamin_logger/_core.py
+-rw-r--r--   0        0        0     7600 2023-06-17 12:43:22.076152 lamin_logger-0.5.3/lamin_logger/_logger.py
+-rw-r--r--   0        0        0     4202 2023-06-17 12:43:22.076659 lamin_logger-0.5.3/lamin_logger/_lookup.py
+-rw-r--r--   0        0        0     4133 2023-06-17 12:43:22.077076 lamin_logger-0.5.3/lamin_logger/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.5.3/lamin_logger/_python_version.py
+-rw-r--r--   0        0        0     2758 2023-06-15 15:21:07.826983 lamin_logger-0.5.3/lamin_logger/_search.py
+-rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.5.3/noxfile.py
+-rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.5.3/tests/test_base.py
+-rw-r--r--   0        0        0     1489 2023-06-17 12:43:22.077768 lamin_logger-0.5.3/tests/test_lookup.py
+-rw-r--r--   0        0        0     3464 2023-06-17 12:43:22.078102 lamin_logger-0.5.3/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.5.3/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2472 2023-06-17 12:56:11.419218 lamin_logger-0.5.3/tests/test_search.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.5.3/PKG-INFO
```

### Comparing `lamin_logger-0.5.2/.github/workflows/build.yml` & `lamin_logger-0.5.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.2/.github/workflows/latest-changes.yml` & `lamin_logger-0.5.3/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.2/.gitignore` & `lamin_logger-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.2/.pre-commit-config.yaml` & `lamin_logger-0.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.2/LICENSE` & `lamin_logger-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.2/docs/changelog.md` & `lamin_logger-0.5.3/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🧪 Test every line of search | [25](https://github.com/laminlabs/lamin-logger/pull/25) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-17 | 0.5.3
+🚑️ Fix empty string input for `map_synonyms` | [24](https://github.com/laminlabs/lamin-logger/pull/24) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-17 |
 💄 Log to stdout rather than stderr | [23](https://github.com/laminlabs/lamin-logger/pull/23) | [falexwolf](https://github.com/falexwolf) | 2023-06-16 | 0.5.2
 ✨ Lookup can also return sql records | [22](https://github.com/laminlabs/lamin-logger/pull/22) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-15 | 0.5.1
 ✨ Remove loguru and replace with standard (Scanpy-based) logger | [18](https://github.com/laminlabs/lamin-logger/pull/18) | [falexwolf](https://github.com/falexwolf) | 2023-06-15 | 0.5.0
 🚚 Moved search and map_synonyms from bionty here | [21](https://github.com/laminlabs/lamin-logger/pull/21) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-15 | 0.4.0
 🚚 Temporarily added lookup | [20](https://github.com/laminlabs/lamin-logger/pull/20) | [falexwolf](https://github.com/falexwolf) | 2023-06-14 | 0.3.4
 ✨ Added download level, changed info icon to 💬 | [19](https://github.com/laminlabs/lamin-logger/pull/19) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-27 | 0.3.2
 :sparkles: Add hint level | [17](https://github.com/laminlabs/lamin-logger/pull/17) | [falexwolf](https://github.com/falexwolf) | 2023-04-05 | 0.3.0
```

### Comparing `lamin_logger-0.5.2/docs/quickstart.ipynb` & `lamin_logger-0.5.3/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.2/lamin_logger/_core.py` & `lamin_logger-0.5.3/lamin_logger/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.2/lamin_logger/_logger.py` & `lamin_logger-0.5.3/lamin_logger/_logger.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.2/lamin_logger/_lookup.py` & `lamin_logger-0.5.3/lamin_logger/_lookup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,16 @@
         records = df.itertuples(index=False, name=tuple_name)
         values = df[field]
     df_dict: Dict = {}  # a dict of namedtuples as records and values as keys
     for i, row in enumerate(records):  # type:ignore
         value = values[i]  # type:ignore
         if not isinstance(value, str):
             continue
+        if value == "":
+            continue
         if value in df_dict:
             _append_records_to_list(df_dict=df_dict, value=value, record=row)
         else:
             df_dict[value] = row
     return df_dict
```

### Comparing `lamin_logger-0.5.2/lamin_logger/_map_synonyms.py` & `lamin_logger-0.5.3/lamin_logger/_map_synonyms.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             f"synonyms_field '{synonyms_field}' is invalid! Available fields"
             f" are: {list(df.columns)}"
         )
     if field == synonyms_field:
         raise KeyError("synonyms_field must be different from field!")
 
     alias_map = explode_aggregated_column_to_expand(
-        df,
+        df=df,
         aggregated_col=synonyms_field,
         target_col=field,
         sep=sep,
     )[field]
 
     if return_mapper:
         mapped_dict = {
@@ -109,8 +109,8 @@
     add_df = pd.DataFrame(data={target_col: add_values, aggregated_col: add_values})
 
     # aggregate the target column so that the new index (aggregated column) is unique
     df_concat = pd.concat([exploded_df, add_df])
     df_concat = df_concat.astype(str)
     df_concat = df_concat.groupby(aggregated_col).agg(sep.join)
 
-    return df_concat
+    return df_concat[df_concat.index != ""]
```

### Comparing `lamin_logger-0.5.2/lamin_logger/_python_version.py` & `lamin_logger-0.5.3/lamin_logger/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.2/lamin_logger/_search.py` & `lamin_logger-0.5.3/lamin_logger/_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.2/pyproject.toml` & `lamin_logger-0.5.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -35,12 +35,7 @@
 [tool.black]
 preview = true
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
-
-[tool.coverage.run]
-omit = [
-    "lamin_logger/*",
-]
```

### Comparing `lamin_logger-0.5.2/tests/test_lookup.py` & `lamin_logger-0.5.3/tests/test_lookup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,23 @@
 
 from lamin_logger._lookup import Lookup
 
 
 def test_lookup():
     df = pd.DataFrame(
         {
-            "name": ["Sample 1", "Sample 1", "sample 1", "1 sample"],
-            "meta1": ["metadata~1", "metadata~1~1", "metadata~1~1~1", "1 metadata"],
+            "name": ["Sample 1", "Sample 1", "sample 1", "1 sample", "", None],
+            "meta1": [
+                "metadata~1",
+                "metadata~1~1",
+                "metadata~1~1~1",
+                "1 metadata",
+                None,
+                None,
+            ],
         }
     )
 
     inst = Lookup(df=df, field="name", tuple_name="TestTuple", prefix="prefix")
     lookup = inst.lookup()
 
     assert len(lookup.sample_1) == 3
```

### Comparing `lamin_logger-0.5.2/tests/test_map_synonyms.py` & `lamin_logger-0.5.3/tests/test_map_synonyms.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,34 +50,83 @@
     expected_synonym_mapping = ["A1CF", "A1BG", "BRCA2", "FANCD20"]
     assert mapping == expected_synonym_mapping
 
 
 def test_map_synonyms_return_mapper(genes):
     gene_symbols, df = genes
 
-    mapping = map_synonyms(
+    mapper = map_synonyms(
         df=df, identifiers=gene_symbols, field="symbol", return_mapper=True
     )
 
-    expected_synonym_mapping = {"FANCD1": "BRCA2"}
+    assert mapper == {"FANCD1": "BRCA2"}
 
-    assert mapping == expected_synonym_mapping
+
+def test_map_synonyms_empty_values(genes):
+    _, df = genes
+
+    result = map_synonyms(
+        df=df,
+        identifiers=["", " ", None, "CD3", "FANCD1"],
+        field="symbol",
+        return_mapper=False,
+    )
+    assert result == ["", " ", None, "CD3", "BRCA2"]
+
+    mapper = map_synonyms(
+        df=df,
+        identifiers=["", " ", None, "CD3", "FANCD1"],
+        field="symbol",
+        return_mapper=True,
+    )
+    assert mapper == {"FANCD1": "BRCA2"}
 
 
 def test_unsupported_field(genes):
     gene_symbols, df = genes
     with pytest.raises(KeyError):
         map_synonyms(df=df, identifiers=gene_symbols, field="name", return_mapper=False)
+    with pytest.raises(KeyError):
+        map_synonyms(
+            df=df,
+            identifiers=gene_symbols,
+            field="symbol",
+            synonyms_field="name",
+            return_mapper=False,
+        )
+    with pytest.raises(KeyError):
+        map_synonyms(
+            df=df,
+            identifiers=gene_symbols,
+            field="symbol",
+            synonyms_field="symbol",
+            return_mapper=False,
+        )
 
 
 def test_explode_aggregated_column_to_expand(genes):
     _, df = genes
     with pytest.raises(AssertionError):
         explode_aggregated_column_to_expand(
             df=df, aggregated_col="synonyms", target_col="synonyms"
         )
 
     res = explode_aggregated_column_to_expand(
         df=df, aggregated_col="synonyms", target_col="symbol"
     )
     assert res.index.name == "synonyms"
-    assert res.shape == (27, 1)
+    assert res.shape == (26, 1)
+
+    with pytest.raises(KeyError):
+        explode_aggregated_column_to_expand(df=df, aggregated_col="name")
+
+    res = explode_aggregated_column_to_expand(
+        df=df, aggregated_col="synonyms", target_col=None
+    )
+    assert "index" in res.columns
+    assert df.index.name == "index"
+
+    df.index.name = "index-name"
+    res = explode_aggregated_column_to_expand(
+        df=df, aggregated_col="synonyms", target_col=None
+    )
+    assert "index-name" in res.columns
```

### Comparing `lamin_logger-0.5.2/tests/test_search.py` & `lamin_logger-0.5.3/tests/test_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,7 +63,22 @@
     res = search(df=df, string="A cell", synonyms_field=None)
     assert len(res) == 2
 
 
 def test_search_non_default_field(df):
     res = search(df=df, string="type F enteroendocrine", field="synonyms")
     res.synonyms == "type F enteroendocrine cell"
+
+
+def test_search_case_sensitive(df):
+    res = search(df=df, string="b cell", case_sensitive=True)
+    assert len(res) == 3
+
+    res = search(df=df, string="b cell", case_sensitive=False)
+    assert res.name == "B cell"
+
+
+def test_search_return_none(df):
+    import pandas as pd
+
+    res = search(df=pd.DataFrame([], columns=["name"]), string="")
+    assert res is None
```

### Comparing `lamin_logger-0.5.2/PKG-INFO` & `lamin_logger-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_logger
-Version: 0.5.2
+Version: 0.5.3
 Summary: Logging setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

