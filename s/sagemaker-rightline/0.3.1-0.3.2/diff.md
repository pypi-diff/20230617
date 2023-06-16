# Comparing `tmp/sagemaker-rightline-0.3.1.tar.gz` & `tmp/sagemaker-rightline-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-rightline-0.3.1.tar", last modified: Wed Jun 14 14:30:10 2023, max compression
+gzip compressed data, was "sagemaker-rightline-0.3.2.tar", last modified: Fri Jun 16 22:08:46 2023, max compression
```

## Comparing `sagemaker-rightline-0.3.1.tar` & `sagemaker-rightline-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:30:10.850690 sagemaker-rightline-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-06-14 14:30:10.850690 sagemaker-rightline-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:30:10.846690 sagemaker-rightline-0.3.1/sagemaker_rightline/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 14:30:00.000000 sagemaker-rightline-0.3.1/sagemaker_rightline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/sagemaker_rightline/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/sagemaker_rightline/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    26341 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/sagemaker_rightline/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:30:10.850690 sagemaker-rightline-0.3.1/sagemaker_rightline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-06-14 14:30:10.000000 sagemaker-rightline-0.3.1/sagemaker_rightline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-14 14:30:10.000000 sagemaker-rightline-0.3.1/sagemaker_rightline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:30:10.000000 sagemaker-rightline-0.3.1/sagemaker_rightline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 14:30:10.000000 sagemaker-rightline-0.3.1/sagemaker_rightline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 14:30:10.000000 sagemaker-rightline-0.3.1/sagemaker_rightline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 14:30:10.850690 sagemaker-rightline-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:30:10.850690 sagemaker-rightline-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-06-14 14:29:54.000000 sagemaker-rightline-0.3.1/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:08:46.301270 sagemaker-rightline-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-16 22:08:46.301270 sagemaker-rightline-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:08:46.301270 sagemaker-rightline-0.3.2/sagemaker_rightline/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 22:08:39.000000 sagemaker-rightline-0.3.2/sagemaker_rightline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/sagemaker_rightline/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/sagemaker_rightline/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30124 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/sagemaker_rightline/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:08:46.301270 sagemaker-rightline-0.3.2/sagemaker_rightline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-16 22:08:46.000000 sagemaker-rightline-0.3.2/sagemaker_rightline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-16 22:08:46.000000 sagemaker-rightline-0.3.2/sagemaker_rightline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 22:08:46.000000 sagemaker-rightline-0.3.2/sagemaker_rightline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-16 22:08:46.000000 sagemaker-rightline-0.3.2/sagemaker_rightline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 22:08:46.000000 sagemaker-rightline-0.3.2/sagemaker_rightline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 22:08:46.301270 sagemaker-rightline-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:08:46.301270 sagemaker-rightline-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27313 2023-06-16 22:08:35.000000 sagemaker-rightline-0.3.2/tests/test_validations.py
```

### Comparing `sagemaker-rightline-0.3.1/LICENSE` & `sagemaker-rightline-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.1/PKG-INFO` & `sagemaker-rightline-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -84,14 +84,15 @@
   - `StepNetworkConfigAsExpected`
   - `StepLambdaFunctionExists`
   - `StepRoleNameExists`
   - `StepRoleNameAsExpected`
   - `StepTagsAsExpected`
   - `StepInputsAsExpected`
   - `StepOutputsAsExpected`
+  - `StepInputOutputAsExpected`
 
 In most cases, a `Validation` subclass requires passing a `Rule` object to its constructor.
 
 ### 📜 Rules
 A `Rule` is a class that inherits from the `Rule` base class.
 It is responsible for defining the rule that a `Validation` checks for.
 For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyIdAsExpected` will check that
@@ -124,14 +125,15 @@
     StepNetworkConfigAsExpected,
     StepLambdaFunctionExists,
     StepRoleNameExists,
     StepRoleNameAsExpected,
     StepTagsAsExpected,
     StepInputsAsExpected,
     StepOutputsAsExpected,
+    StepOutputsMatchInputsAsExpected,
 )
 
 # Import a dummy pipeline
 from tests.fixtures.pipeline import get_sagemaker_pipeline, DUMMY_BUCKET
 
 sm_pipeline = get_sagemaker_pipeline()
 
@@ -192,14 +194,28 @@
                 destination=f"s3://{DUMMY_BUCKET}/output-1",
                 output_name="output-1",
             )
         ],
         step_name="sm_processing_step_spark",  # optional
         rule=Contains(),
     ),
+    StepOutputsMatchInputsAsExpected(
+        inputs_outputs_expected=[
+            {
+                "input": {
+                    "step_name": "sm_processing_step_sklearn",
+                    "input_name": "input-1",
+                },
+                "output": {
+                    "step_name": "sm_processing_step_sklearn",
+                    "output_name": "output-1",
+                },
+            }
+        ]
+    ),
 ]
 
 # Add Validations and SageMaker Pipeline to Configuration
 cm = Configuration(
     validations=validations,
     sagemaker_pipeline=sm_pipeline,
 )
```

### Comparing `sagemaker-rightline-0.3.1/README.md` & `sagemaker-rightline-0.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
   - `StepNetworkConfigAsExpected`
   - `StepLambdaFunctionExists`
   - `StepRoleNameExists`
   - `StepRoleNameAsExpected`
   - `StepTagsAsExpected`
   - `StepInputsAsExpected`
   - `StepOutputsAsExpected`
+  - `StepInputOutputAsExpected`
 
 In most cases, a `Validation` subclass requires passing a `Rule` object to its constructor.
 
 ### 📜 Rules
 A `Rule` is a class that inherits from the `Rule` base class.
 It is responsible for defining the rule that a `Validation` checks for.
 For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyIdAsExpected` will check that
@@ -79,14 +80,15 @@
     StepNetworkConfigAsExpected,
     StepLambdaFunctionExists,
     StepRoleNameExists,
     StepRoleNameAsExpected,
     StepTagsAsExpected,
     StepInputsAsExpected,
     StepOutputsAsExpected,
+    StepOutputsMatchInputsAsExpected,
 )
 
 # Import a dummy pipeline
 from tests.fixtures.pipeline import get_sagemaker_pipeline, DUMMY_BUCKET
 
 sm_pipeline = get_sagemaker_pipeline()
 
@@ -147,14 +149,28 @@
                 destination=f"s3://{DUMMY_BUCKET}/output-1",
                 output_name="output-1",
             )
         ],
         step_name="sm_processing_step_spark",  # optional
         rule=Contains(),
     ),
+    StepOutputsMatchInputsAsExpected(
+        inputs_outputs_expected=[
+            {
+                "input": {
+                    "step_name": "sm_processing_step_sklearn",
+                    "input_name": "input-1",
+                },
+                "output": {
+                    "step_name": "sm_processing_step_sklearn",
+                    "output_name": "output-1",
+                },
+            }
+        ]
+    ),
 ]
 
 # Add Validations and SageMaker Pipeline to Configuration
 cm = Configuration(
     validations=validations,
     sagemaker_pipeline=sm_pipeline,
 )
```

### Comparing `sagemaker-rightline-0.3.1/pyproject.toml` & `sagemaker-rightline-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.1/sagemaker_rightline/model.py` & `sagemaker-rightline-0.3.2/sagemaker_rightline/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,27 +52,29 @@
         """
         raise NotImplementedError
 
 
 class Validation(ABC):
     """Abstract class for validations."""
 
-    def __init__(self, paths: List[str], name: str, rule: Optional[Rule] = None) -> None:
+    def __init__(
+        self, name: str, paths: Optional[List[str]] = None, rule: Optional[Rule] = None
+    ) -> None:
         """Initialize a Validation object.
 
         :param paths: list of paths to the attributes to be validated
         :type paths: List[str]
         :param name: name of the validation
         :type name: str
         :param rule: rule to be applied to the validation, defaults to None
         :type rule: Optional[Rule]
         :return:
         :rtype:
         """
-        self.paths: List[str] = paths
+        self.paths: List[Optional[str]] = paths if paths else []
         self.name: str = name
         self.rule: Rule = rule
 
     @staticmethod
     def get_filtered_attributes(filter_subject: Iterable[object], path: str) -> List[object]:
         """Get filtered attributes from path.
```

### Comparing `sagemaker-rightline-0.3.1/sagemaker_rightline/rules.py` & `sagemaker-rightline-0.3.2/sagemaker_rightline/rules.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.1/sagemaker_rightline/validations.py` & `sagemaker-rightline-0.3.2/sagemaker_rightline/validations.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from sagemaker.inputs import FileSystemInput, TrainingInput
 from sagemaker.processing import NetworkConfig, ProcessingInput, ProcessingOutput
 from sagemaker.workflow.entities import PipelineVariable
 from sagemaker.workflow.parameters import Parameter
 from sagemaker.workflow.pipeline import Pipeline
 
 from sagemaker_rightline.model import Rule, Validation, ValidationResult
+from sagemaker_rightline.rules import Equals
 
 
 class PipelineParametersAsExpected(Validation):
     """Validate Pipeline Parameters.
 
     This validation will check if the parameters in the pipeline are as
     expected.
@@ -702,7 +703,110 @@
         """
 
         outputs_observed = Validation.get_attribute(sagemaker_pipeline, self.paths)
         outputs_observed_formatted = [x.__dict__ for y in outputs_observed for x in y]
         outputs_expected_formatted = [x.__dict__ for x in self.outputs_expected]
         result = self.rule.run(outputs_observed_formatted, outputs_expected_formatted, self.name)
         return result
+
+
+class StepOutputsMatchInputsAsExpected(Validation):
+    """Validate Outputs <> Inputs of Pipeline Step."""
+
+    def __init__(self, inputs_outputs_expected: List[Dict[str, Dict[str, str]]]) -> None:
+        """Initialize StepTagsAsExpected validation.
+
+        :param inputs_outputs_expected: Expected Input and Output per step name
+        :type inputs_outputs_expected: Dict[str, Dict[str, str]]
+        :return: None
+        :rtype: None
+        """
+        name = "StepOutputsMatchInputsAsExpected"
+        super().__init__(
+            name=name,
+            rule=Equals(),
+        )
+        self.inputs_outputs_expected: List[Dict[str, Dict[str, str]]] = inputs_outputs_expected
+
+    @staticmethod
+    def get_step_by_name(
+        sagemaker_pipeline: Pipeline, step_name: str
+    ) -> "ProcessingStep":  # noqa F821
+        """Get ProcessingStep by name.
+
+        :param sagemaker_pipeline: SageMaker Pipeline
+        :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
+        :param step_name: Name of Step
+        :type step_name: str
+        :return: ProcessingStep
+        :rtype: ProcessingStep
+        """
+        for step in sagemaker_pipeline.steps:
+            if step.name == step_name:
+                return step
+        raise ValueError(f"Step {step_name} not found in Pipeline")
+
+    @staticmethod
+    def get_input_output_by_name(
+        step: "ProcessingStep", name: str, kind: str  # noqa F821
+    ) -> Union["ProcessingInput", "ProcessingOutput"]:
+        """Get ProcessingInput or ProcessingOutput by name.
+
+        :param step: ProcessingStep
+        :type step: ProcessingStep
+        :param name: Name of Input or Output
+        :type name: str
+        :return: ProcessingInput or ProcessingOutput
+        :rtype: Union[ProcessingInput, ProcessingOutput]
+        """
+        if kind == "input":
+            for input in step.inputs:
+                if input.input_name == name:
+                    return input
+        elif kind == "output":
+            for output in step.outputs:
+                if output.output_name == name:
+                    return output
+        else:
+            raise ValueError(f"Kind {kind} not supported. Must be one of 'input' or 'output'.")
+
+    def run(
+        self,
+        sagemaker_pipeline: Pipeline,
+    ) -> ValidationResult:
+        """Runs validation of Step Inputs on Pipeline.
+
+        :param sagemaker_pipeline: SageMaker Pipeline
+        :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
+        :return: validation result
+        :rtype: ValidationResult
+        """
+
+        input_kw = "input"
+        output_kw = "output"
+
+        results = []
+        for pair in self.inputs_outputs_expected:
+            input_step_name = pair[input_kw]["step_name"]
+            input_name = pair[input_kw]["input_name"]
+            output_step_name = pair[output_kw]["step_name"]
+            output_name = pair[output_kw]["output_name"]
+
+            input_step = StepOutputsMatchInputsAsExpected.get_step_by_name(
+                sagemaker_pipeline, input_step_name
+            )
+            output_step = StepOutputsMatchInputsAsExpected.get_step_by_name(
+                sagemaker_pipeline, output_step_name
+            )
+
+            input = StepOutputsMatchInputsAsExpected.get_input_output_by_name(
+                input_step, input_name, input_kw
+            )
+            output = StepOutputsMatchInputsAsExpected.get_input_output_by_name(
+                output_step, output_name, output_kw
+            )
+            results.append((input.source, output.destination))
+        return self.rule.run(
+            observed=[x[0] for x in results],
+            expected=[x[1] for x in results],
+            validation_name=self.name,
+        )
```

### Comparing `sagemaker-rightline-0.3.1/sagemaker_rightline.egg-info/PKG-INFO` & `sagemaker-rightline-0.3.2/sagemaker_rightline.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -84,14 +84,15 @@
   - `StepNetworkConfigAsExpected`
   - `StepLambdaFunctionExists`
   - `StepRoleNameExists`
   - `StepRoleNameAsExpected`
   - `StepTagsAsExpected`
   - `StepInputsAsExpected`
   - `StepOutputsAsExpected`
+  - `StepInputOutputAsExpected`
 
 In most cases, a `Validation` subclass requires passing a `Rule` object to its constructor.
 
 ### 📜 Rules
 A `Rule` is a class that inherits from the `Rule` base class.
 It is responsible for defining the rule that a `Validation` checks for.
 For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyIdAsExpected` will check that
@@ -124,14 +125,15 @@
     StepNetworkConfigAsExpected,
     StepLambdaFunctionExists,
     StepRoleNameExists,
     StepRoleNameAsExpected,
     StepTagsAsExpected,
     StepInputsAsExpected,
     StepOutputsAsExpected,
+    StepOutputsMatchInputsAsExpected,
 )
 
 # Import a dummy pipeline
 from tests.fixtures.pipeline import get_sagemaker_pipeline, DUMMY_BUCKET
 
 sm_pipeline = get_sagemaker_pipeline()
 
@@ -192,14 +194,28 @@
                 destination=f"s3://{DUMMY_BUCKET}/output-1",
                 output_name="output-1",
             )
         ],
         step_name="sm_processing_step_spark",  # optional
         rule=Contains(),
     ),
+    StepOutputsMatchInputsAsExpected(
+        inputs_outputs_expected=[
+            {
+                "input": {
+                    "step_name": "sm_processing_step_sklearn",
+                    "input_name": "input-1",
+                },
+                "output": {
+                    "step_name": "sm_processing_step_sklearn",
+                    "output_name": "output-1",
+                },
+            }
+        ]
+    ),
 ]
 
 # Add Validations and SageMaker Pipeline to Configuration
 cm = Configuration(
     validations=validations,
     sagemaker_pipeline=sm_pipeline,
 )
```

### Comparing `sagemaker-rightline-0.3.1/tests/test_model.py` & `sagemaker-rightline-0.3.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.1/tests/test_rules.py` & `sagemaker-rightline-0.3.2/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.1/tests/test_validations.py` & `sagemaker-rightline-0.3.2/tests/test_validations.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     PipelineParametersAsExpected,
     StepImagesExist,
     StepInputsAsExpected,
     StepKmsKeyIdAsExpected,
     StepLambdaFunctionExists,
     StepNetworkConfigAsExpected,
     StepOutputsAsExpected,
+    StepOutputsMatchInputsAsExpected,
     StepRoleNameAsExpected,
     StepRoleNameExists,
     StepTagsAsExpected,
 )
 from tests.fixtures.constants import (
     TEST_ACCOUNT_ID,
     TEST_LAMBDA_FUNC_NAME,
@@ -566,15 +567,15 @@
 @pytest.mark.parametrize(
     "rule,inputs_expected,step_name,success",
     [
         [
             Equals,
             [
                 ProcessingInput(
-                    source=f"s3://{DUMMY_BUCKET}/input-1",
+                    source=f"s3://{DUMMY_BUCKET}/output-1",
                     destination="/opt/ml/processing/input",
                     input_name="input-1",
                 ),
                 ProcessingInput(
                     source=f"s3://{DUMMY_BUCKET}/input-2",
                     destination="/opt/ml/processing/input",
                     input_name="input-2",
@@ -588,15 +589,15 @@
             [
                 ProcessingInput(
                     source=f"s3://{DUMMY_BUCKET}/input-2",
                     destination="/opt/ml/processing/input",
                     input_name="input-2",
                 ),
                 ProcessingInput(
-                    source=f"s3://{DUMMY_BUCKET}/input-1",
+                    source=f"s3://{DUMMY_BUCKET}/output-1",
                     destination="/opt/ml/processing/input",
                     input_name="input-1",
                 ),
             ],
             "sm_processing_step_sklearn",
             True,
         ],
@@ -802,7 +803,90 @@
     step_outputs_validation = StepOutputsAsExpected(
         outputs_expected=outputs_expected,
         step_name=step_name,
         rule=rule(),
     )
     result = step_outputs_validation.run(sagemaker_pipeline)
     assert result.success == success
+
+
+@pytest.mark.parametrize(
+    "inputs_outputs_expected,success,raise_error",
+    [
+        [
+            [
+                {
+                    "input": {
+                        "step_name": "sm_processing_step_sklearn",
+                        "input_name": "input-1",
+                    },
+                    "output": {
+                        "step_name": "sm_processing_step_sklearn",
+                        "output_name": "output-1",
+                    },
+                }
+            ],
+            True,
+            False,
+        ],
+        [
+            [
+                {
+                    "input": {
+                        "step_name": "sm_processing_step_sklearn",
+                        "input_name": "input-1",
+                    },
+                    "output": {
+                        "step_name": "sm_processing_step_sklearn",
+                        "output_name": "output-2",
+                    },
+                }
+            ],
+            False,
+            False,
+        ],
+        [
+            [
+                {
+                    "input": {
+                        "step_name": "sm_processing_step_sklearn",
+                        "input_name": "input-1",
+                    },
+                    "output": {
+                        "step_name": "step_doesnt_exist",
+                        "output_name": "output-1",
+                    },
+                }
+            ],
+            False,
+            True,
+        ],
+        [
+            [
+                {
+                    "input": {
+                        "step_name": "sm_processing_step_sklearn",
+                        "input_name": "input-doesnt-exist1",
+                    },
+                    "output": {
+                        "step_name": "sm_processing_step_sklearn",
+                        "output_name": "output-1",
+                    },
+                }
+            ],
+            False,
+            True,
+        ],
+    ],
+)
+def test_step_outputs_match_inputs_as_expected(
+    sagemaker_pipeline, inputs_outputs_expected, success, raise_error
+) -> None:
+    step_outputs_validation = StepOutputsMatchInputsAsExpected(
+        inputs_outputs_expected=inputs_outputs_expected,
+    )
+    if raise_error:
+        with pytest.raises((ValueError, AttributeError)):
+            _ = step_outputs_validation.run(sagemaker_pipeline)
+    else:
+        result = step_outputs_validation.run(sagemaker_pipeline)
+        assert result.success is success
```

