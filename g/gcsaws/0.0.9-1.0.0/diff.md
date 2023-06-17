# Comparing `tmp/gcsaws-0.0.9.tar.gz` & `tmp/gcsaws-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcsaws-0.0.9.tar", last modified: Mon May  8 10:40:03 2023, max compression
+gzip compressed data, was "gcsaws-1.0.0.tar", last modified: Sat Jun 17 13:13:38 2023, max compression
```

## Comparing `gcsaws-0.0.9.tar` & `gcsaws-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 10:40:03.967439 gcsaws-0.0.9/
--rw-rw-rw-   0        0        0     1091 2023-05-07 12:57:03.000000 gcsaws-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      412 2023-05-08 10:40:03.967439 gcsaws-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0        8 2023-05-07 12:56:41.000000 gcsaws-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 10:40:03.953121 gcsaws-0.0.9/gcsaws/
--rw-rw-rw-   0        0        0      226 2023-05-08 10:38:04.000000 gcsaws-0.0.9/gcsaws/__init__.py
--rw-rw-rw-   0        0        0      684 2023-05-08 07:29:33.000000 gcsaws-0.0.9/gcsaws/helpers.py
--rw-rw-rw-   0        0        0     8262 2023-05-08 09:24:20.000000 gcsaws-0.0.9/gcsaws/nodes.py
--rw-rw-rw-   0        0        0     4156 2023-05-08 08:41:10.000000 gcsaws-0.0.9/gcsaws/visitor_procedure.py
--rw-rw-rw-   0        0        0     3417 2023-05-08 09:37:22.000000 gcsaws-0.0.9/gcsaws/visitor_validation.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:40:03.963349 gcsaws-0.0.9/gcsaws.egg-info/
--rw-rw-rw-   0        0        0      412 2023-05-08 10:40:03.000000 gcsaws-0.0.9/gcsaws.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-05-08 10:40:03.000000 gcsaws-0.0.9/gcsaws.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 10:40:03.000000 gcsaws-0.0.9/gcsaws.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-08 10:40:03.000000 gcsaws-0.0.9/gcsaws.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-08 10:40:03.000000 gcsaws-0.0.9/gcsaws.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      663 2023-05-08 10:39:08.000000 gcsaws-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 10:40:03.967439 gcsaws-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-08 10:40:03.966437 gcsaws-0.0.9/tests/
--rw-rw-rw-   0        0        0      810 2023-05-07 11:28:19.000000 gcsaws-0.0.9/tests/test_create_target_list.py
--rw-rw-rw-   0        0        0     3460 2023-05-08 08:36:21.000000 gcsaws-0.0.9/tests/test_simple.py
--rw-rw-rw-   0        0        0     1129 2023-05-08 10:36:09.000000 gcsaws-0.0.9/tests/test_validation.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:13:38.280856 gcsaws-1.0.0/
+-rw-rw-rw-   0        0        0     1091 2023-05-15 08:49:30.000000 gcsaws-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      435 2023-06-17 13:13:38.280856 gcsaws-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0        8 2023-05-15 08:49:30.000000 gcsaws-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 13:13:38.249588 gcsaws-1.0.0/gcsaws/
+-rw-rw-rw-   0        0        0      156 2023-06-16 21:58:00.000000 gcsaws-1.0.0/gcsaws/__init__.py
+-rw-rw-rw-   0        0        0     1900 2023-06-17 13:08:59.000000 gcsaws-1.0.0/gcsaws/helpers.py
+-rw-rw-rw-   0        0        0     8829 2023-06-17 12:22:27.000000 gcsaws-1.0.0/gcsaws/nodes.py
+-rw-rw-rw-   0        0        0     6177 2023-06-16 21:58:00.000000 gcsaws-1.0.0/gcsaws/visitor_overview.py
+-rw-rw-rw-   0        0        0     4156 2023-05-15 08:49:30.000000 gcsaws-1.0.0/gcsaws/visitor_procedure.py
+-rw-rw-rw-   0        0        0     1459 2023-06-16 21:58:00.000000 gcsaws-1.0.0/gcsaws/visitor_save_scripts.py
+-rw-rw-rw-   0        0        0     4633 2023-06-16 21:58:00.000000 gcsaws-1.0.0/gcsaws/visitor_validation.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:13:38.265224 gcsaws-1.0.0/gcsaws.egg-info/
+-rw-rw-rw-   0        0        0      435 2023-06-17 13:13:38.000000 gcsaws-1.0.0/gcsaws.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      503 2023-06-17 13:13:38.000000 gcsaws-1.0.0/gcsaws.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 13:13:38.000000 gcsaws-1.0.0/gcsaws.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-06-17 13:13:38.000000 gcsaws-1.0.0/gcsaws.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-17 13:13:38.000000 gcsaws-1.0.0/gcsaws.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      739 2023-06-17 13:13:14.000000 gcsaws-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-17 13:13:38.296477 gcsaws-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-17 13:13:38.280856 gcsaws-1.0.0/tests/
+-rw-rw-rw-   0        0        0      810 2023-05-15 08:49:30.000000 gcsaws-1.0.0/tests/test_create_target_list.py
+-rw-rw-rw-   0        0        0    10119 2023-06-17 13:12:53.000000 gcsaws-1.0.0/tests/test_flatten.py
+-rw-rw-rw-   0        0        0     1311 2023-06-17 11:24:00.000000 gcsaws-1.0.0/tests/test_generate_script.py
+-rw-rw-rw-   0        0        0     1730 2023-06-17 11:25:04.000000 gcsaws-1.0.0/tests/test_overview.py
+-rw-rw-rw-   0        0        0     3468 2023-05-15 08:49:30.000000 gcsaws-1.0.0/tests/test_simple.py
+-rw-rw-rw-   0        0        0     1124 2023-06-16 21:58:00.000000 gcsaws-1.0.0/tests/test_validation.py
```

### Comparing `gcsaws-0.0.9/LICENSE` & `gcsaws-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcsaws-0.0.9/gcsaws/nodes.py` & `gcsaws-1.0.0/gcsaws/nodes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,329 +1,351 @@
-from __future__ import annotations
-
-from typing import TypeVar, Optional
-
-from gcscore.mod import *
-
-T = TypeVar('T')
-
-__all__ = ['HasIdentifier', 'HasCompaction', 'HasCommand', 'HasTargets', 'HasPayload', 'HasScriptType',
-           'HasInstanceState', 'HasFunctionName', 'HasInstanceState', 'HasDurationSeconds', 'AcceptChildScript',
-           'AcceptChildPause', 'AcceptChildWait', 'AcceptChildScriptTemplate', 'AcceptChildStepFunction',
-           'AcceptChildRunInOrder', 'AcceptChildRunInParallel', 'NodeRunInOrder', 'NodeRunInParallel', 'NodeWait',
-           'NodePause', 'NodeScript', 'NodeScriptTemplate', 'NodeStepFunction', 'NodeChangeInstanceState']
-
-
-# <editor-fold desc="Trait attributes">
-
-class HasDurationSeconds:
-    gcsaws_duration: int = 5
-
-    def duration(self: T, duration: int) -> T:
-        """
-        Sets the duration in seconds for the node.
-        :param duration: the duration in seconds
-        :return: self
-        """
-        self.gcsaws_duration = duration
-        return self
-
-
-class HasIdentifier:
-    gcsaws_identifier: str = ''
-
-    def identifier(self: T, identifier_: str) -> T:
-        """
-        Sets the identifier in order to make it clearly identified in the resume tool.
-        :param identifier_: the identifier
-        :return: self
-        """
-        self.gcsaws_identifier = identifier_
-        return self
-
-
-class HasScriptType:
-    gcsaws_script_type: str = None
-
-    def shell(self: T) -> T:
-        """
-        Makes the node run a shell script/command.
-        :return: self
-        """
-        self.gcsaws_script_type = 'shell'
-        return self
-
-    def powershell(self: T) -> T:
-        """
-        Make the node run a powershell script/command.
-        :return: self
-        """
-        self.gcsaws_script_type = 'powershell'
-        return self
-
-
-class HasCommand:
-    gcsaws_command: Optional[str] = None
-
-    def command(self: T, cmd: str) -> T:
-        """
-        Sets the node command or script.
-        :param cmd:
-        :return:
-        """
-        self.gcsaws_command = cmd
-        return self
-
-
-class HasTargets:
-    gcsaws_targets: list[dict]
-    gcsaws_targets_initialized: bool
-
-    def __gcs__init__(self, **_):
-        self.gcsaws_targets = []
-        self.gcsaws_targets_initialized = False
-
-    def on_targets(self: T, targets: list[dict]) -> T:
-        """
-        Adds the targets to the node.
-        :param targets: list of the targets
-        :return: self
-        """
-        self.gcsaws_targets.extend(targets)
-        self.gcsaws_targets_initialized = True
-        return self
-
-
-class HasCompaction:
-    gcsaws_compaction: bool = False
-
-    def compact(self: T) -> T:
-        """
-        Indicate that the content of the node (scripts...) should be compacted.
-        :return: self
-        """
-        self.gcsaws_compaction = True
-        return self
-
-
-class HasFunctionName:
-    gcsaws_function_name: str = None
-
-    def function_name(self: T, name: str) -> T:
-        """
-        Sets the name of the function called by the node.
-        :param name: function's name
-        :return: self
-        """
-        self.gcsaws_function_name = name
-        return self
-
-
-class HasPayload:
-    gcsaws_payload: dict = None
-
-    def payload(self: T, payload: dict) -> T:
-        """
-        Sets the payload of the node.
-        :param payload: the payload dictionary
-        :return: self
-        """
-        self.gcsaws_payload = payload
-        return self
-
-
-class HasInstanceState:
-    gcsaws_instance_state: str = None
-
-    def power_on(self: T) -> T:
-        """
-        Mark the wanted state as "running"
-        :return: self
-        """
-        self.gcsaws_instance_state = 'running'
-        return self
-
-    def power_off(self: T) -> T:
-        """
-        Mark the wanted state as "stopped"
-        :return: self
-        """
-        self.gcsaws_instance_state = 'stopped'
-        return self
-
-
-# </editor-fold>
-
-# <editor-fold desc="Traits for children">
-
-class AcceptChildWait:
-    def wait(self: HasChildren, name: str) -> NodeWait:
-        """
-        Waits a certain amount of seconds before continuing the execution.
-        :param name: node's name
-        :return: the child node wait
-        """
-        return add_child(self, NodeWait, name=name)
-
-
-class AcceptChildPause:
-    def pause(self: HasChildren, name: str) -> NodePause:
-        """
-        Waits for the user to resume the automation.
-        :param name: node's name
-        :return: the child node pause
-        """
-        return add_child(self, NodePause, name=name)
-
-
-class AcceptChildRunInOrder:
-    def run_in_order(self: HasChildren, name: str) -> NodeRunInOrder:
-        """
-        Starts a new in order procedure part.
-        :param name: node's name
-        :return: the child node
-        """
-        return add_child(self, NodeRunInOrder, name=name)
-
-
-class AcceptChildRunInParallel:
-    def run_in_parallel(self: HasChildren, name: str) -> NodeRunInParallel:
-        """
-        Starts a new parallelized nodes procedure part.
-        :param name: node's name
-        :return: the child node
-        """
-        return add_child(self, NodeRunInParallel, name=name)
-
-
-class AcceptChildScript:
-    def run_script(self: HasChildren, name: str) -> NodeScript:
-        """
-        Runs a script on the given servers.
-        :param name: node's name
-        :return: the child node
-        """
-        return add_child(self, NodeScript, name=name)
-
-
-class AcceptChildScriptTemplate:
-    def run_script_template(self: HasChildren, name: str) -> NodeScriptTemplate:
-        """
-        Renders the script command and runs it on the servers.
-        :param name: node's name
-        :return: the child node
-        """
-        return add_child(self, NodeScriptTemplate, name=name)
-
-
-class AcceptChildStepFunction:
-    def run_step_function(self: HasChildren, name: str) -> NodeStepFunction:
-        """
-        Run a step function.
-        :param name: node's name
-        :return: the child node
-        """
-        return add_child(self, NodeStepFunction, name=name)
-
-
-class AcceptChildChangeInstanceState:
-    def change_instance_state(self: HasChildren, name: str) -> NodeChangeInstanceState:
-        """
-        Power on or off the targets.
-        :param name: node(s name
-        :return: the child node
-        """
-        return add_child(self, NodeChangeInstanceState, name=name)
-
-
-# </editor-fold>
-
-# <editor-fold desc="Nodes">
-class _ComposedNode(
-    BaseNode,
-    HasName,
-    HasDescription,
-    HasChildren,
-    AcceptAnonymousChild,
-    AcceptMerge,
-    AcceptChildWait,
-    AcceptChildPause,
-    AcceptChildRunInOrder,
-    AcceptChildRunInParallel,
-    AcceptChildScript,
-    AcceptChildScriptTemplate,
-    AcceptChildStepFunction,
-    AcceptChildChangeInstanceState
-):
-    pass
-
-
-class NodeRunInParallel(_ComposedNode):
-    __visitor_method__ = 'visit_run_in_parallel'
-
-
-class NodeRunInOrder(_ComposedNode):
-    __visitor_method__ = 'visit_run_in_order'
-
-
-class NodeWait(
-    BaseNode,
-    HasName,
-    HasDescription,
-    HasDurationSeconds
-):
-    __visitor_method__ = 'visit_wait'
-
-
-class NodePause(
-    BaseNode,
-    HasName,
-    HasDescription,
-    HasIdentifier
-):
-    __visitor_method__ = 'visit_pause'
-
-
-class NodeScript(
-    BaseNode,
-    HasName,
-    HasDescription,
-    HasScriptType,
-    HasCommand,
-    HasTargets,
-    HasCompaction
-):
-    __visitor_method__ = 'visit_script'
-
-
-class NodeScriptTemplate(
-    BaseNode,
-    HasName,
-    HasDescription,
-    HasScriptType,
-    HasCommand,
-    HasTargets,
-    HasCompaction
-):
-    __visitor_method__ = 'visit_script_template'
-
-
-class NodeStepFunction(
-    BaseNode,
-    HasName,
-    HasDescription,
-    HasFunctionName,
-    HasPayload
-):
-    __visitor_method__ = 'visit_step_function'
-
-
-class NodeChangeInstanceState(
-    BaseNode,
-    HasName,
-    HasDescription,
-    HasTargets,
-    HasInstanceState
-):
-    __visitor_method__ = 'visit_change_instance_state'
-
-# </editor-fold>
+from __future__ import annotations
+
+import random
+from typing import TypeVar, Optional, Union
+
+from gcscore.mod import *
+
+T = TypeVar('T')
+
+__all__ = ['HasIdentifier', 'HasCompaction', 'HasCommand', 'HasTargets', 'HasPayload', 'HasScriptType',
+           'HasInstanceState', 'HasFunctionName', 'HasInstanceState', 'HasDurationSeconds', 'AcceptChildScript',
+           'AcceptChildPause', 'AcceptChildWait', 'AcceptChildScriptTemplate', 'AcceptChildStepFunction',
+           'AcceptChildRunInOrder', 'AcceptChildRunInParallel', 'NodeRunInOrder', 'NodeRunInParallel', 'NodeWait',
+           'NodePause', 'NodeScript', 'NodeScriptTemplate', 'NodeStepFunction', 'NodeChangeInstanceState',
+           'ComposableNode']
+
+
+# <editor-fold desc="Trait attributes">
+
+class HasDurationSeconds:
+    gcsaws_duration: int = 5
+
+    def duration(self: T, duration: int) -> T:
+        """
+        Sets the duration in seconds for the node.
+        :param duration: the duration in seconds
+        :return: self
+        """
+        self.gcsaws_duration = duration
+        return self
+
+
+class HasIdentifier:
+    gcsaws_identifier: str = ''
+
+    def identifier(self: T, identifier_: str) -> T:
+        """
+        Sets the identifier in order to make it clearly identified in the resume tool.
+        :param identifier_: the identifier
+        :return: self
+        """
+        self.gcsaws_identifier = identifier_
+        return self
+
+
+class HasScriptType:
+    gcsaws_script_type: str = None
+
+    def shell(self: T) -> T:
+        """
+        Makes the node run a shell script/command.
+        :return: self
+        """
+        self.gcsaws_script_type = 'shell'
+        return self
+
+    def powershell(self: T) -> T:
+        """
+        Make the node run a powershell script/command.
+        :return: self
+        """
+        self.gcsaws_script_type = 'powershell'
+        return self
+
+
+class HasCommand:
+    gcsaws_command: Optional[str] = None
+    gcsaws_command_source: Optional[str] = None
+
+    def command(self: T, cmd: str) -> T:
+        """
+        Sets the node command or script.
+        :param cmd:
+        :return:
+        """
+        self.gcsaws_command = cmd
+        self.gcsaws_command_source = cmd
+        return self
+
+
+class HasTargets:
+    gcsaws_targets: list[dict]
+    gcsaws_targets_initialized: bool
+
+    def __gcs__init__(self, **_):
+        self.gcsaws_targets = []
+        self.gcsaws_targets_initialized = False
+
+    def on_targets(self: T, targets: list[dict]) -> T:
+        """
+        Adds the targets to the node.
+        :param targets: list of the targets
+        :return: self
+        """
+        self.gcsaws_targets.extend(targets)
+        self.gcsaws_targets_initialized = True
+        return self
+
+
+class HasCompaction:
+    gcsaws_compaction: bool = False
+
+    def compact(self: T, do_compact: bool = True) -> T:
+        """
+        Indicate that the content of the node (scripts...) should be compacted.
+        :param do_compact: whether the compaction should be activated or not (default: True)
+        :return: self
+        """
+        self.gcsaws_compaction = do_compact
+        return self
+
+
+class HasFunctionName:
+    gcsaws_function_name: str = None
+
+    def function_name(self: T, name: str) -> T:
+        """
+        Sets the name of the function called by the node.
+        :param name: function's name
+        :return: self
+        """
+        self.gcsaws_function_name = name
+        return self
+
+
+class HasPayload:
+    gcsaws_payload: dict = None
+
+    def payload(self: T, payload: dict) -> T:
+        """
+        Sets the payload of the node.
+        :param payload: the payload dictionary
+        :return: self
+        """
+        self.gcsaws_payload = payload
+        return self
+
+
+class HasInstanceState:
+    gcsaws_instance_state: str = None
+
+    def power_on(self: T) -> T:
+        """
+        Mark the wanted state as "running"
+        :return: self
+        """
+        self.gcsaws_instance_state = 'running'
+        return self
+
+    def power_off(self: T) -> T:
+        """
+        Mark the wanted state as "stopped"
+        :return: self
+        """
+        self.gcsaws_instance_state = 'stopped'
+        return self
+
+
+# </editor-fold>
+
+# <editor-fold desc="Traits for children">
+
+class AcceptChildWait:
+    def wait(self: HasChildren, name: str) -> NodeWait:
+        """
+        Waits a certain amount of seconds before continuing the execution.
+        :param name: node's name
+        :return: the child node wait
+        """
+        return add_child(self, NodeWait, name=name)
+
+
+class AcceptChildPause:
+    def pause(self: HasChildren, name: str) -> NodePause:
+        """
+        Waits for the user to resume the automation.
+        :param name: node's name
+        :return: the child node pause
+        """
+        return add_child(self, NodePause, name=name)
+
+
+class AcceptChildRunInOrder:
+    def run_in_order(self: HasChildren, name: str) -> NodeRunInOrder:
+        """
+        Starts a new in order procedure part.
+        :param name: node's name
+        :return: the child node
+        """
+        return add_child(self, NodeRunInOrder, name=name)
+
+
+class AcceptChildRunInParallel:
+    def run_in_parallel(self: HasChildren, name: str) -> NodeRunInParallel:
+        """
+        Starts a new parallelized nodes procedure part.
+        :param name: node's name
+        :return: the child node
+        """
+        return add_child(self, NodeRunInParallel, name=name)
+
+
+class AcceptChildScript:
+    def run_script(self: HasChildren, name: str) -> NodeScript:
+        """
+        Runs a script on the given servers.
+        :param name: node's name
+        :return: the child node
+        """
+        return add_child(self, NodeScript, name=name)
+
+
+class AcceptChildScriptTemplate:
+    def run_script_template(self: HasChildren, name: str) -> NodeScriptTemplate:
+        """
+        Renders the script command and runs it on the servers.
+        :param name: node's name
+        :return: the child node
+        """
+        return add_child(self, NodeScriptTemplate, name=name)
+
+
+class AcceptChildStepFunction:
+    def run_step_function(self: HasChildren, name: str) -> NodeStepFunction:
+        """
+        Run a step function.
+        :param name: node's name
+        :return: the child node
+        """
+        return add_child(self, NodeStepFunction, name=name)
+
+
+class AcceptChildChangeInstanceState:
+    def change_instance_state(self: HasChildren, name: str) -> NodeChangeInstanceState:
+        """
+        Power on or off the targets.
+        :param name: node(s name
+        :return: the child node
+        """
+        return add_child(self, NodeChangeInstanceState, name=name)
+
+
+class AcceptChildProcedure:
+    def child_procedure(self: AcceptAnonymousChild, procedure_file: str, context: BaseContext, method: str = 'main'):
+        """
+        Include the procedure in the parent procedure.
+        :param procedure_file: the procedure generator
+        :param context: the generation context
+        :param method: the method to use in the procedure file
+        """
+        name = str(random.randint(0, 1_000_000_000))
+        proc = getattr(import_module(name, procedure_file), method)(context)
+        self.child(proc)
+
+
+# </editor-fold>
+
+# <editor-fold desc="Nodes">
+class _ComposedNode(
+    BaseNode,
+    HasName,
+    HasDescription,
+    HasChildren,
+    AcceptAnonymousChild,
+    AcceptMerge,
+    AcceptChildWait,
+    AcceptChildPause,
+    AcceptChildRunInOrder,
+    AcceptChildRunInParallel,
+    AcceptChildScript,
+    AcceptChildScriptTemplate,
+    AcceptChildStepFunction,
+    AcceptChildChangeInstanceState,
+    AcceptChildProcedure
+):
+    pass
+
+
+class NodeRunInParallel(_ComposedNode):
+    __visitor_method__ = 'visit_run_in_parallel'
+
+
+class NodeRunInOrder(_ComposedNode):
+    __visitor_method__ = 'visit_run_in_order'
+
+
+class NodeWait(
+    BaseNode,
+    HasName,
+    HasDescription,
+    HasDurationSeconds
+):
+    __visitor_method__ = 'visit_wait'
+
+
+class NodePause(
+    BaseNode,
+    HasName,
+    HasDescription,
+    HasIdentifier
+):
+    __visitor_method__ = 'visit_pause'
+
+
+class NodeScript(
+    BaseNode,
+    HasName,
+    HasDescription,
+    HasScriptType,
+    HasCommand,
+    HasTargets,
+    HasCompaction
+):
+    __visitor_method__ = 'visit_script'
+
+
+class NodeScriptTemplate(
+    BaseNode,
+    HasName,
+    HasDescription,
+    HasScriptType,
+    HasCommand,
+    HasTargets,
+    HasCompaction
+):
+    __visitor_method__ = 'visit_script_template'
+
+
+class NodeStepFunction(
+    BaseNode,
+    HasName,
+    HasDescription,
+    HasFunctionName,
+    HasPayload
+):
+    __visitor_method__ = 'visit_step_function'
+
+
+class NodeChangeInstanceState(
+    BaseNode,
+    HasName,
+    HasDescription,
+    HasTargets,
+    HasInstanceState
+):
+    __visitor_method__ = 'visit_change_instance_state'
+
+
+ComposableNode = Union[NodeRunInOrder, NodeRunInParallel]
+
+# </editor-fold>
```

### Comparing `gcsaws-0.0.9/gcsaws/visitor_procedure.py` & `gcsaws-1.0.0/gcsaws/visitor_procedure.py`

 * *Files identical despite different names*

### Comparing `gcsaws-0.0.9/pyproject.toml` & `gcsaws-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,30 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "gcsaws"
-version = "0.0.9"
-authors = [
-    { name="Leikt", email="leikt.solreihin@gmail.com" },
-]
-description = "GCS implementation for the aws-automation package."
-readme = "README.md"
-requires-python = ">=3.9"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-    "gcscore>=0.0.16"
-]
-#[project.urls]
-#"Homepage" = "https://github.com/pypa/sampleproject"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "gcsaws"
+version = "1.0.0"
+authors = [
+    { name = "Leikt", email = "leikt.solreihin@gmail.com" },
+]
+description = "GCS implementation for the aws-automation package."
+readme = "README.md"
+requires-python = ">=3.9"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    "gcscore>=0.0.22",
+    "rich>=13.3.5"
+]
+optional-dependencies.build = [
+    "build>=0.10.0",
+    "twine>=4.0.2"
+]
+
+#[project.urls]
+#"Homepage" = "https://github.com/pypa/sampleproject"
 #"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `gcsaws-0.0.9/tests/test_create_target_list.py` & `gcsaws-1.0.0/tests/test_create_target_list.py`

 * *Files identical despite different names*

### Comparing `gcsaws-0.0.9/tests/test_simple.py` & `gcsaws-1.0.0/tests/test_simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         sub_proc.wait('hello').duration(15)
 
         sub_proc2 = NodeRunInOrder(name='sub2')
         sub_proc2.wait('XOXO').duration(5)
         root.child(sub_proc2)
 
         # Visit
-        visitor_state = VisitorStateProcedure(None, None)
+        visitor_state = VisitorStateProcedure(None, None)  # NOQA
         visitor = Visitor()
         setup_procedure_visitor(visitor)
         visitor.visit(root, visitor_state)
         final = visitor_state.root[0]
         pass
 
     def test_script_template(self):
```

### Comparing `gcsaws-0.0.9/tests/test_validation.py` & `gcsaws-1.0.0/tests/test_validation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-import unittest
-from gcsaws import *
-
-from gcscore.mod import Visitor
-from gcscore.mod.validation import VisitorStateValidation
-
-class TestErrorLogging(unittest.TestCase):
-    def test_valid_proc(self):
-        proc = new_procedure('test')
-        proc.wait('test_wait')
-
-        rip = proc.run_in_parallel('X')
-        rip.pause('A').identifier('ABC')
-
-        # Validation
-        visitor = Visitor()
-        visitor_state = VisitorStateValidation()
-        setup_validation_visitor(visitor)
-        visitor.visit(proc, visitor_state)  # Should not raise any error
-
-    def test_invalid_proc(self):
-        proc = new_procedure('invalid_proc')
-        proc.wait('invalid_wait').duration(-5)
-        proc.pause('4651d=)àç')
-        proc.run_step_function('my_sf')
-
-        rip = proc.run_in_parallel('blah')
-        rip.run_script('booya')
-        rip.change_instance_state('madara!!!')
-
-        # Validation
-        visitor = Visitor()
-        visitor_state = VisitorStateValidation(only_log_errors=True)
-        setup_validation_visitor(visitor)
-        visitor.visit(proc, visitor_state)
+import unittest
+from gcsaws import *
+
+from gcscore.mod import Visitor
+from gcsaws.visitor_validation import VisitorStateValidation, setup_validation_visitor
+
+
+class TestErrorLogging(unittest.TestCase):
+    def test_valid_proc(self):
+        proc = new_procedure('test')
+        proc.wait('test_wait')
+
+        rip = proc.run_in_parallel('X')
+        rip.pause('A').identifier('ABC')
+
+        # Validation
+        visitor = Visitor()
+        visitor_state = VisitorStateValidation()
+        setup_validation_visitor(visitor)
+        visitor.visit(proc, visitor_state)  # Should not raise any error
+
+    def test_invalid_proc(self):
+        proc = new_procedure('invalid_proc')
+        proc.wait('invalid_wait').duration(-5)
+        proc.pause('4651d=)àç')
+        proc.run_step_function('my_sf')
+
+        rip = proc.run_in_parallel('blah')
+        rip.run_script('booya')
+        rip.change_instance_state('madara!!!')
+
+        # Validation
+        visitor = Visitor()
+        visitor_state = VisitorStateValidation(only_log_errors=True)
+        setup_validation_visitor(visitor)
+        visitor.visit(proc, visitor_state)
```

