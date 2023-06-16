# Comparing `tmp/reasoner_validator-3.5.8.tar.gz` & `tmp/reasoner_validator-3.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.5.8.tar", max compression
+gzip compressed data, was "reasoner_validator-3.5.9.tar", max compression
```

## Comparing `reasoner_validator-3.5.8.tar` & `reasoner_validator-3.5.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1153 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/LICENSE
--rw-r--r--   0        0        0    12606 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/README.md
--rw-r--r--   0        0        0      131 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/Makefile
--rw-r--r--   0        0        0     2291 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/conf.py
--rw-r--r--   0        0        0    19034 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/index.rst
--rw-r--r--   0        0        0      795 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/make.bat
--rw-r--r--   0        0        0      136 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    36025 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2093 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/pyproject.toml
--rw-r--r--   0        0        0    34621 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    63110 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    39243 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0    26862 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4350 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0     9718 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    13781 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0     9922 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/versioning.py
--rw-r--r--   0        0        0        0 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/tests/conftest.py
--rw-r--r--   0        0        0   113749 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    42178 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/tests/test_data/sample_trapi_schema.yaml
--rw-r--r--   0        0        0    31899 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/tests/test_response_validator.py
--rw-r--r--   0        0        0     4533 2023-06-16 04:51:42.751725 reasoner_validator-3.5.8/tests/test_semver.py
--rw-r--r--   0        0        0     1746 2023-06-16 04:51:42.751725 reasoner_validator-3.5.8/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    26543 2023-06-16 04:51:42.751725 reasoner_validator-3.5.8/tests/test_validate.py
--rw-r--r--   0        0        0    19013 2023-06-16 04:51:42.751725 reasoner_validator-3.5.8/tests/test_validation_report.py
--rw-r--r--   0        0        0     2061 2023-06-16 04:51:42.751725 reasoner_validator-3.5.8/tests/test_workflows.py
--rw-r--r--   0        0        0    14645 1970-01-01 00:00:00.000000 reasoner_validator-3.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/LICENSE
+-rw-r--r--   0        0        0    12606 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/README.md
+-rw-r--r--   0        0        0      131 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/Makefile
+-rw-r--r--   0        0        0     2291 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/conf.py
+-rw-r--r--   0        0        0    19034 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    35674 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2093 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/pyproject.toml
+-rw-r--r--   0        0        0    34621 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    62655 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    38874 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0    26862 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4350 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0     9718 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    13781 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0     9922 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0        0 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/conftest.py
+-rw-r--r--   0        0        0   114174 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    42178 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/test_data/sample_trapi_schema.yaml
+-rw-r--r--   0        0        0    31899 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/test_response_validator.py
+-rw-r--r--   0        0        0     4533 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/test_semver.py
+-rw-r--r--   0        0        0     1746 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    26543 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/test_validate.py
+-rw-r--r--   0        0        0    19013 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2061 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/test_workflows.py
+-rw-r--r--   0        0        0    14645 1970-01-01 00:00:00.000000 reasoner_validator-3.5.9/PKG-INFO
```

### Comparing `reasoner_validator-3.5.8/LICENSE` & `reasoner_validator-3.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/README.md` & `reasoner_validator-3.5.9/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/docs/Makefile` & `reasoner_validator-3.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/docs/conf.py` & `reasoner_validator-3.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/docs/index.rst` & `reasoner_validator-3.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/docs/make.bat` & `reasoner_validator-3.5.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/docs/validation_codes_dictionary.md` & `reasoner_validator-3.5.9/docs/validation_codes_dictionary.md`

 * *Files 1% similar despite different names*

```diff
@@ -238,22 +238,14 @@
 
 **Message:** Edge has an attribute_type_id that has a non-Biolink CURIE prefix mapped to Biolink
 
 **Context:** edge_id, identifier
 
 **Description:** Non-Biolink CURIEs are tolerated, but not preferred, as term value for the attribute_type_id properties of edge attributes.
 
-### warning.knowledge_graph.edge.attribute.type_id.unknown_prefix
-
-**Message:** Edge has an attribute_type_id that has a CURIE prefix namespace unknown to Biolink
-
-**Context:** edge_id, identifier
-
-**Description:** The namespaces of 'attribute_type_id' terms may be incomplete with respect to Biolink Model version being used in the knowledge graph.
-
 ### warning.knowledge_graph.edge.attribute.type_id.deprecated
 
 **Message:** Edge has a deprecated attribute_type_id
 
 **Context:** identifier
 
 **Description:** Edge 'attribute_type_id' is deprecated in current model, to be removed in the future. Review Biolink Model for replacement.
```

### Comparing `reasoner_validator-3.5.8/pyproject.toml` & `reasoner_validator-3.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.5.8"
+version = "3.5.9"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-3.5.8/reasoner_validator/__init__.py` & `reasoner_validator-3.5.9/reasoner_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.5.9/reasoner_validator/biolink/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -567,28 +567,19 @@
                                                         infores == ara_source:
                                                     found_ara_knowledge_source = True
                                                 elif kp_source and \
                                                         attribute_type_id == kp_source_type and \
                                                         infores == kp_source:
                                                     found_kp_knowledge_source = True
 
-                        # if not a Biolink association_slot, at least,
-                        # check if it is an id prefix known to Biolink.
-                        # We won't call it a hard error, but issue a warning
-                        elif not self.bmt.get_element_by_prefix(prefix):
+                        # if not a Biolink 'association_slot', at least, check if the 'attribute_type_id' has a
+                        # namespace (prefix) known to Biolink. We won't call it a hard error, but issue a warning
+                        elif not self.bmt.get_element_by_prefix(attribute_type_id):
                             self.report(
-                                code="warning.knowledge_graph.edge.attribute.type_id.unknown_prefix",
-                                identifier=attribute_type_id,
-                                edge_id=edge_id
-                            )
-                        # TODO: probably need to take a closer look at validating outlier terms here
-                        #       Maybe enumerations will help
-                        else:
-                            self.report(
-                                code="info.knowledge_graph.edge.attribute.type_id.non_biolink_prefix",
+                                code="warning.knowledge_graph.edge.attribute.type_id.non_biolink_prefix",
                                 identifier=attribute_type_id,
                                 edge_id=edge_id
                             )
 
             # Edge provenance tags only recorded in Edge attributes prior to TRAPI 1.4.0-beta
             if not self.minimum_required_trapi_version("1.4.0-beta") and self.validate_biolink():
                 # After all the attributes have been scanned,
```

### Comparing `reasoner_validator-3.5.8/reasoner_validator/codes.yaml` & `reasoner_validator-3.5.9/reasoner_validator/codes.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -209,20 +209,14 @@
             $description: "Edge 'attribute_type_id' value should generally be a term defined within the biolink:association_slot hierarchy."
           non_biolink_prefix:
             $message: "Edge has an attribute_type_id that has a non-Biolink CURIE prefix mapped to Biolink"
             $context:
               - edge_id
               - identifier
             $description: "Non-Biolink CURIEs are tolerated, but not preferred, as term value for the attribute_type_id properties of edge attributes."
-          unknown_prefix:
-            $message: "Edge has an attribute_type_id that has a CURIE prefix namespace unknown to Biolink"
-            $context:
-              - edge_id
-              - identifier
-            $description: "The namespaces of 'attribute_type_id' terms may be incomplete with respect to Biolink Model version being used in the knowledge graph."
           deprecated:
             $message: "Edge has a deprecated attribute_type_id"
             $context:
               - identifier
             $description: "Edge 'attribute_type_id' is deprecated in current model, to be removed in the future. Review Biolink Model for replacement."
       provenance:
         multiple_primary:
```

### Comparing `reasoner_validator-3.5.8/reasoner_validator/report.py` & `reasoner_validator-3.5.9/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/reasoner_validator/sri/util.py` & `reasoner_validator-3.5.9/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.5.9/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.5.9/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/reasoner_validator/validation_codes.py` & `reasoner_validator-3.5.9/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/reasoner_validator/versioning.py` & `reasoner_validator-3.5.9/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.5.9/tests/test_biolink_compliance_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1026,20 +1026,35 @@
         ),
         (
             # Query 2. Empty attributes
             {
                 "attributes": []
             },
             get_ara_test_case(),
-            # "Edge has empty attributes!"
+            # "Edge has empty attributes!" Allowed
             ""
         ),
+        (
+            # Query 3. EDAM-DATA:2526 ought to have an acceptable namespace
+            {
+                "attributes": [
+                    {
+                        "attribute_type_id": "EDAM-DATA:2526",
+                        "value": "some-value"
+                    }
+                ]
+            },
+            get_ara_test_case(),
+            # "Edge has an acceptable namespace prefix
+            ""
+        )
+        # CHEMBL.COMPOUND:CHEMBL112--biolink:occurs_together_in_literature_with->NCBIGene:762
     ]
 )
-def test_post_1_4_0_trapi_validate_missing_or_empty_attributes(query: Tuple):
+def test_post_1_4_0_trapi_validate_attributes(query: Tuple):
     validator = BiolinkValidator(
         graph_type=TRAPIGraphType.Knowledge_Graph,
         biolink_version=LATEST_BIOLINK_MODEL_VERSION,
         sources=query[1]
     )
     validator.validate_attributes(edge_id="test_validate_attributes unit test", edge=query[0])
     check_messages(validator, query[2])
@@ -2682,16 +2697,15 @@
                             }
                         ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Edge attribute_type_id 'foo:bar' " +
             # f"has a CURIE prefix namespace unknown to Biolink!"
-            # TODO: Code for validating this is commented out pending a BMT repair of the test
-            "warning.knowledge_graph.edge.attribute.type_id.unknown_prefix"
+            "warning.knowledge_graph.edge.attribute.type_id.non_biolink_prefix"
         ),
         (   # Query 26:  # An earlier Biolink Model won't recognize a category not found in its specified release
             "1.8.2",
             {
                 # Sample nodes
                 'nodes': {
                     "NCBIGene:29974": {
```

### Comparing `reasoner_validator-3.5.8/tests/test_data/sample_trapi_schema.yaml` & `reasoner_validator-3.5.9/tests/test_data/sample_trapi_schema.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/tests/test_response_validator.py` & `reasoner_validator-3.5.9/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/tests/test_semver.py` & `reasoner_validator-3.5.9/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/tests/test_trapi_versioning.py` & `reasoner_validator-3.5.9/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/tests/test_validate.py` & `reasoner_validator-3.5.9/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/tests/test_validation_report.py` & `reasoner_validator-3.5.9/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/tests/test_workflows.py` & `reasoner_validator-3.5.9/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.8/PKG-INFO` & `reasoner_validator-3.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.5.8
+Version: 3.5.9
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

