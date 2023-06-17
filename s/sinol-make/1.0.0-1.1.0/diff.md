# Comparing `tmp/sinol-make-1.0.0.tar.gz` & `tmp/sinol-make-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinol-make-1.0.0.tar", last modified: Thu May 25 10:51:32 2023, max compression
+gzip compressed data, was "sinol-make-1.1.0.tar", last modified: Sat Jun 17 09:55:45 2023, max compression
```

## Comparing `sinol-make-1.0.0.tar` & `sinol-make-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:32.174860 sinol-make-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-25 10:51:21.000000 sinol-make-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-25 10:51:32.174860 sinol-make-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-25 10:51:21.000000 sinol-make-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-25 10:51:21.000000 sinol-make-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 10:51:32.174860 sinol-make-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:32.170860 sinol-make-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:32.170860 sinol-make-1.0.0/src/sinol_make/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:32.170860 sinol-make-1.0.0/src/sinol_make/commands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:32.170860 sinol-make-1.0.0/src/sinol_make/commands/run/
--rw-r--r--   0 runner    (1001) docker     (123)    25715 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/commands/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/commands/run/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:32.170860 sinol-make-1.0.0/src/sinol_make/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/helpers/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/helpers/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:32.174860 sinol-make-1.0.0/src/sinol_make/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/interfaces/BaseCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/interfaces/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-25 10:51:21.000000 sinol-make-1.0.0/src/sinol_make/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:51:32.170860 sinol-make-1.0.0/src/sinol_make.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-25 10:51:32.000000 sinol-make-1.0.0/src/sinol_make.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-25 10:51:32.000000 sinol-make-1.0.0/src/sinol_make.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 10:51:32.000000 sinol-make-1.0.0/src/sinol_make.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 10:51:32.000000 sinol-make-1.0.0/src/sinol_make.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 10:51:32.000000 sinol-make-1.0.0/src/sinol_make.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 10:51:32.000000 sinol-make-1.0.0/src/sinol_make.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.885949 sinol-make-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-17 09:55:35.000000 sinol-make-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-17 09:55:45.885949 sinol-make-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-17 09:55:35.000000 sinol-make-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-17 09:55:35.000000 sinol-make-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 09:55:45.885949 sinol-make-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.881949 sinol-make-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.881949 sinol-make-1.1.0/src/sinol_make/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.881949 sinol-make-1.1.0/src/sinol_make/commands/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.885949 sinol-make-1.1.0/src/sinol_make/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (123)    29611 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/commands/run/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.885949 sinol-make-1.1.0/src/sinol_make/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/helpers/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/helpers/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.885949 sinol-make-1.1.0/src/sinol_make/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/interfaces/BaseCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/interfaces/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.885949 sinol-make-1.1.0/src/sinol_make.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-17 09:55:45.000000 sinol-make-1.1.0/src/sinol_make.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-17 09:55:45.000000 sinol-make-1.1.0/src/sinol_make.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 09:55:45.000000 sinol-make-1.1.0/src/sinol_make.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-17 09:55:45.000000 sinol-make-1.1.0/src/sinol_make.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 09:55:45.000000 sinol-make-1.1.0/src/sinol_make.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 09:55:45.000000 sinol-make-1.1.0/src/sinol_make.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.885949 sinol-make-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-17 09:55:35.000000 sinol-make-1.1.0/tests/test_util.py
```

### Comparing `sinol-make-1.0.0/LICENSE` & `sinol-make-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sinol-make-1.0.0/pyproject.toml` & `sinol-make-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -37,7 +37,13 @@
 "Bug Tracker" = "https://github.com/sio2project/sinol-make/issues"
 
 [project.scripts]
 sinol-make = "sinol_make:main"
 
 [tool.setuptools.dynamic]
 version = { attr = "sinol_make.__version__" }
+
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+markers = [
+    "github_runner: Mark tests that require GitHub runner",
+]
```

### Comparing `sinol-make-1.0.0/src/sinol_make/commands/run/__init__.py` & `sinol-make-1.1.0/src/sinol_make/commands/run/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Modified version of https://sinol3.dasie.mimuw.edu.pl/oij/jury/package/-/blob/master/runner.py
 # Author of the original code: Bartosz Kostka <kostka@oij.edu.pl>
 # Version 0.6 (2021-08-29)
 
-from sinol_make.commands.run.structs import ResultChange, ValidationResult
+from sinol_make.commands.run.structs import ExecutionResult, ResultChange, ValidationResult, ExecutionData
 from sinol_make.interfaces.BaseCommand import BaseCommand
 from sinol_make.interfaces.Errors import CompilationError
 from sinol_make.helpers import compile, compiler
 import sinol_make.util as util
 import yaml, os, collections, sys, re, math, dictdiffer
 import multiprocessing as mp
 
@@ -19,35 +19,44 @@
 	def get_name(self):
 		return 'run'
 
 
 	def configure_subparser(self, subparser):
 		parser = subparser.add_parser(
 			'run',
-			help='Run current task',
-			description='Run current task'
+			help='Runs solutions in parallel on tests and verifies the expected solutions\' scores with the config.',
+			description='Runs selected solutions (by default all solutions) \
+				on selected tests (by default all tests) \
+				with a given number of cpus. \
+				Measures the solutions\' time with oiejq, unless specified otherwise. \
+				After running the solutions, it compares the solutions\' scores with the ones saved in config.yml.'
 		)
-		parser.add_argument('--programs', type=str, nargs='+',
-							help='programs to be run, for example prog/abc{b,s}*.{cpp,py}')
+
+		default_timetool = 'oiejq' if sys.platform == 'linux' else 'time'
+
+		parser.add_argument('--solutions', type=str, nargs='+',
+							help='solutions to be run, for example prog/abc{b,s}*.{cpp,py}')
 		parser.add_argument('--tests', type=str, nargs='+',
 							help='tests to be run, for example in/abc{0,1}*')
 		parser.add_argument('--cpus', type=int,
 							help='number of cpus to use, you have %d avaliable' % mp.cpu_count())
 		parser.add_argument('--tl', type=float, help='time limit (in s)')
 		parser.add_argument('--ml', type=float, help='memory limit (in MB)')
 		parser.add_argument('--hide_memory', dest='hide_memory', action='store_true',
 							help='hide memory usage in report')
-		parser.add_argument('--program_report', type=str,
-							help='file to store report from program executions (in markdown)')
+		parser.add_argument('--solutions_report', type=str,
+							help='file to store report from solution executions (in markdown)')
+		parser.add_argument('--time_tool', choices=['oiejq', 'time'], default=default_timetool,
+		      				help='tool to measure time and memory usage (default when possible: oiejq)')
 		parser.add_argument('--oiejq_path', type=str,
 		      				help='path to oiejq executable (default: `~/.local/bin/oiejq`)')
 		parser.add_argument('--c_compiler_path', type=str, default=compiler.get_c_compiler_path(),
-		    				help='C compiler to use (default for Linux and Windows: gcc, default for Mac: gcc-{9-12})')
+		    				help='C compiler to use (default for Linux and Windows: gcc, default for Mac: gcc-9 or gcc-10)')
 		parser.add_argument('--cpp_compiler_path', type=str, default=compiler.get_cpp_compiler_path(),
-		    				help='C++ compiler to use (default for Linux and Windows: g++, default for Mac: gcc-{9-12})')
+		    				help='C++ compiler to use (default for Linux and Windows: g++, default for Mac: g++-9 or g++-10)')
 		parser.add_argument('--python_interpreter_path', type=str, default=compiler.get_python_interpreter_path(),
 		    				help='Python interpreter to use (default: python3)')
 		parser.add_argument('--java_compiler_path', type=str, default=compiler.get_java_compiler_path(),
 		    				help='Java compiler to use (default: javac)')
 		parser.add_argument('--apply_suggestions', dest='apply_suggestions', action='store_true',
 		      				help='apply suggestions from expected scores report')
 
@@ -190,71 +199,148 @@
 		except CompilationError as e:
 			print(util.error("Compilation of file %s was unsuccessful."
 								% self.extract_file_name(solution)))
 			os.system("head -c 500 %s" % compile_log_file) # TODO: make this work on Windows
 			return False
 
 
-	def execute(self, execution):
-		(name, executable, test, time_limit, memory_limit, timetool_path) = execution
-		output_file = os.path.join(self.EXECUTIONS_DIR, name,
-								self.extract_test_no(test)+".out")
-		result_file = os.path.join(self.EXECUTIONS_DIR, name,
-								self.extract_test_no(test)+".res")
-		hard_time_limit_in_s = math.ceil(2*time_limit / 1000.0)
-
-		command = "MEM_LIMIT=%sK MEASURE_MEM=true timeout -k %ds -s SIGKILL %ds %s %s <%s >%s 2>%s" \
-				% (math.ceil(memory_limit), hard_time_limit_in_s,
-					hard_time_limit_in_s, timetool_path,
-					executable, test, output_file, result_file)
-		code = os.system(command)
-		result = {}
+	def execute_oiejq(self, command, result_file, output_file, answer_file, time_limit, memory_limit):
+		timeout_exit_code = os.system(command)
+		result = ExecutionResult(None, None, None)
 		with open(result_file) as r:
 			for line in r:
 				line = line.strip()
 				if ": " in line:
 					(key, value) = line.split(": ")[:2]
-					result[key] = value
-		if "Time" in result.keys():
-			result["Time"] = self.parse_time(result["Time"])
-		if "Memory" in result.keys():
-			result["Memory"] = self.parse_memory(result["Memory"])
-		if code == 35072:
-			result["Status"] = "TL"
-		elif "Time" in result.keys() and result["Time"] > time_limit:
-			result["Status"] = "TL"
-		elif "Memory" in result.keys() and result["Memory"] > memory_limit:
-			result["Status"] = "ML"
-		elif "Status" not in result.keys():
-			result["Status"] = "RE"
-		elif result["Status"] == "OK":
-			if result["Time"] > time_limit:
-				result["Status"] = "TL"
-			elif result["Memory"] > memory_limit:
-				result["Status"] = "ML"
+					if key == "Time":
+						result.Time = self.parse_time(value)
+					elif key == "Memory":
+						result.Memory = self.parse_memory(value)
+					else:
+						setattr(result, key, value)
+
+		if timeout_exit_code == 35072:
+			result.Status = "TL"
+		elif getattr(result, "Time") is not None and result.Time > time_limit:
+			result.Status = "TL"
+		elif getattr(result, "Memory") is not None and result.Memory > memory_limit:
+			result.Status = "ML"
+		elif getattr(result, "Status") is None:
+			result.Status = "RE"
+		elif result.Status == "OK":
+			if result.Time > time_limit:
+				result.Status = "TL"
+			elif result.Memory > memory_limit:
+				result.Status = "ML"
 			elif os.system("diff -q -Z %s %s >/dev/null"
-						% (output_file, self.get_output_file(test))):
-				result["Status"] = "WA"
+						% (output_file, answer_file)):
+				result.Status = "WA"
 		else:
-			result["Status"] = result["Status"][:2]
+			result.Status = result.Status[:2]
+
 		return result
 
-	def perform_executions(self, compiled_commands, names, solutions, report_file):
+
+	def execute_time(self, command, result_file, output_file, answer_file, time_limit, memory_limit):
+		timeout_exit_code = os.system(command)
+
+		result = ExecutionResult(None, None, None)
+		lines = open(result_file).readlines()
+		program_exit_code = None
+		if len(lines) == 3:
+			"""
+			If programs runs successfully, the output looks like this:
+			 - first line is CPU time in seconds
+			 - second line is memory in KB
+			 - third line is exit code
+			This format is defined by -f flag in time command.
+			"""
+			result.Time = round(float(lines[0].strip()) * 1000)
+			result.Memory = int(lines[1].strip())
+			program_exit_code = int(lines[2].strip())
+		if len(lines) > 0 and "Command terminated by signal " in lines[0]:
+			"""
+			If there was a runtime error, the first line is the error message with signal number.
+			For example:
+				Command terminated by signal 11
+			"""
+			program_exit_code = int(lines[0].strip().split(" ")[-1])
+
+		if program_exit_code != None and program_exit_code != 0:
+			result.Status = "RE"
+		elif timeout_exit_code != 0:
+			result.Status = "TL"
+		elif result.Time > time_limit:
+			result.Status = "TL"
+		elif result.Memory > memory_limit:
+			result.Status = "ML"
+		elif os.system("diff -q -Z %s %s >/dev/null" % (output_file, answer_file)):
+			result.Status = "WA"
+		else:
+			result.Status = "OK"
+
+		return result
+
+
+	def run_solution(self, data_for_execution: ExecutionData):
+		"""
+		Run an execution and return the result as ExecutionResult object.
+		"""
+
+		(name, executable, test, time_limit, memory_limit, timetool_path) = data_for_execution
+		file_no_ext = os.path.join(self.EXECUTIONS_DIR, name, self.extract_test_no(test))
+		output_file = file_no_ext + ".out"
+		result_file = file_no_ext + ".res"
+		hard_time_limit_in_s = math.ceil(2 * time_limit / 1000.0)
+
+		if self.args.time_tool == 'oiejq':
+			command = "MEM_LIMIT=%sK MEASURE_MEM=true timeout -k %ds -s SIGKILL %ds %s %s <%s >%s 2>%s" \
+					% (memory_limit, hard_time_limit_in_s,
+						hard_time_limit_in_s, timetool_path,
+						executable, test, output_file, result_file)
+
+			return self.execute_oiejq(command, result_file, output_file, self.get_output_file(test), time_limit, memory_limit)
+		elif self.args.time_tool == 'time':
+			if sys.platform == 'darwin':
+				timeout_name = 'gtimeout'
+				time_name = 'gtime'
+			elif sys.platform == 'linux':
+				timeout_name = 'timeout'
+				time_name = 'time'
+			elif sys.platform == 'win32' or sys.platform == 'cygwin':
+				raise Exception("Measuring time with GNU time on Windows is not supported.")
+
+			command = f'{timeout_name} -k {hard_time_limit_in_s}s {hard_time_limit_in_s}s ' \
+						f'{time_name} -f "%U\\n%M\\n%x" -o {result_file} {executable} <{test} >{output_file}'
+			return self.execute_time(command, result_file, output_file, self.get_output_file(test), time_limit, memory_limit)
+
+
+	def update_group_status(self, group_status, new_status):
+		order = ["TL", "ML", "RE", "WA", "OK"]
+		if order.index(new_status) < order.index(group_status):
+			return new_status
+		return group_status
+
+	def run_solutions(self, compiled_commands, names, solutions, report_file):
+		"""
+		Run solutions on tests and print the results as a table to stdout.
+		"""
+
 		executions = []
 		all_results = collections.defaultdict(
 			lambda: collections.defaultdict(lambda: collections.defaultdict(map)))
 		for (name, executable, result) in compiled_commands:
 			if result:
 				for test in self.tests:
 					executions.append((name, executable, test, self.time_limit, self.memory_limit, self.timetool_path))
-					all_results[name][self.get_group(test)][test] = {"Status": "  "}
+					all_results[name][self.get_group(test)][test] = ExecutionResult("  ", None, None)
 				os.makedirs(os.path.join(self.EXECUTIONS_DIR, name), exist_ok=True)
 			else:
 				for test in self.tests:
-					all_results[name][self.get_group(test)][test] = {"Status": "CE"}
+					all_results[name][self.get_group(test)][test] = ExecutionResult("CE", None, None)
 		print()
 		executions.sort(key = lambda x: (self.get_executable_key(x[1]), x[2]))
 		program_groups_scores = collections.defaultdict(dict)
 
 		def print_view(output_file=None):
 			def print_stream(*values, end='\n'):
 				if output_file is not None:
@@ -292,28 +378,30 @@
 				print_stream()
 				for group in self.groups:
 					print_stream("%6s" % group, end=" | ")
 					for program in program_group:
 						results = all_results[program][group]
 						group_status = "OK"
 						for test in results:
-							status = results[test]["Status"]
-							if "Time" in results[test].keys():
+							status = results[test].Status
+							if getattr(results[test], "Time") is not None:
 								program_times[program] = max(
-									program_times[program], results[test]["Time"])
+									program_times[program], results[test].Time)
 							elif status == "TL":
 								program_times[program] = 2 * self.time_limit
-							if "Memory" in results[test].keys():
+							if getattr(results[test], "Memory") is not None:
 								program_memory[program] = max(
-									program_memory[program], results[test]["Memory"])
+									program_memory[program], results[test].Memory)
 							elif status == "ML":
 								program_memory[program] = 2 * self.memory_limit
-							if status != "OK":
-								group_status = status
-								break
+							if status == "  ":
+								group_status = "  "
+							else:
+								group_status = self.update_group_status(group_status, status)
+
 						print_stream("%3s" % util.bold(util.color_green(group_status)) if group_status == "OK" else util.bold(util.color_red(group_status)),
 							"%3s/%3s" % (self.scores[group] if group_status == "OK" else "---", self.scores[group]),
 							end=" | ")
 						program_scores[program] += self.scores[group] if group_status == "OK" else 0
 						program_groups_scores[program][group] = group_status
 					print_stream()
 				print_stream(6*" ", end=" | ")
@@ -344,37 +432,37 @@
 				# 	for program in program_group:
 				# 		print_stream(10*" ", end=" | ")
 				# 	print_stream()
 				# 	for test in self.tests:
 				# 		print_stream("%6s" % self.extract_test_no(test), end=" | ")
 				# 		for program in program_group:
 				# 			result = all_results[program][self.get_group(test)][test]
-				# 			status = result["Status"]
+				# 			status = result.Status
 				# 			if status == "  ": print_stream(10*' ', end=" | ")
 				# 			else:
 				# 				print_stream("%3s" % self.colorize_status(status),
-				# 					("%17s" % self.color_time(result["Time"], self.time_limit)) if "Time" in result.keys() else 7*" ", end=" | ")
+				# 					("%17s" % self.color_time(result.Time, self.time_limit)) if getattr(result, "Time") is not None else 7*" ", end=" | ")
 				# 		print_stream()
 				# 		if not self.args.hide_memory:
 				# 			print_stream(6*" ", end=" | ")
 				# 			for program in program_group:
 				# 				result = all_results[program][self.get_group(test)][test]
-				# 				print_stream(("%20s" % self.color_memory(result["Memory"], self.memory_limit))  if "Memory" in result.keys() else 10*" ", end=" | ")
+				# 				print_stream(("%20s" % self.color_memory(result.Memory, self.memory_limit))  if getattr(result, "Memory") is not None else 10*" ", end=" | ")
 				# 			print_stream()
 				# 	print_stream()
 				print_stream(10*len(program_group)*' ')
 
 			if output_file is not None:
 				os.system('sed -i -r "s/\x1B\[([0-9]{1,3}(;[0-9]{1,2})?)?[mGK]//g" %s' % output_file) # TODO: make this work on Windows
 				print("Report has been saved to", util.bold(output_file))
 				print()
 
 		print("Performing %d executions..." % len(executions))
 		with mp.Pool(self.cpus) as pool:
-			for i, result in enumerate(pool.imap(self.execute, executions)):
+			for i, result in enumerate(pool.imap(self.run_solution, executions)):
 				(name, executable, test) = executions[i][:3]
 				all_results[name][self.get_group(test)][test] = result
 				print_view()
 		if report_file:
 			print_view(report_file)
 		return program_groups_scores
 
@@ -385,22 +473,22 @@
 			if group != 0 and group not in self.config["scores"]:
 				util.exit_with_error(f'Group {group} doesn\'t have points specified in config file.')
 			if result == "OK" and group != 0:
 				points += self.config["scores"][group]
 		return points
 
 
-	def run_solutions(self, solutions):
+	def compile_and_run(self, solutions):
 		compilation_results = self.compile_solutions(solutions)
 		os.makedirs(self.EXECUTIONS_DIR, exist_ok=True)
 		executables = [os.path.join(self.EXECUTABLES_DIR, self.get_executable(solution))
 							for solution in solutions]
 		compiled_commands = zip(solutions, executables, compilation_results)
 		names = solutions
-		return self.perform_executions(compiled_commands, names, solutions, self.args.program_report)
+		return self.run_solutions(compiled_commands, names, solutions, self.args.solutions_report)
 
 
 	def print_expected_scores(self, expected_scores):
 		yaml_dict = { "sinol_expected_scores": expected_scores }
 		print(yaml.dump(yaml_dict, default_flow_style=None))
 
 
@@ -411,15 +499,15 @@
 			new_expected_scores[solution] = {
 				"expected": results[solution],
 				"points": self.calculate_points(results[solution])
 			}
 
 		config_expected_scores = self.config.get("sinol_expected_scores", {})
 		used_solutions = results.keys()
-		if self.args.programs == None and config_expected_scores: # If no solutions were specified, use all programs from config
+		if self.args.solutions == None and config_expected_scores: # If no solutions were specified, use all solutions from config
 			used_solutions = config_expected_scores.keys()
 
 		used_groups = set()
 		if self.args.tests == None and config_expected_scores: # If no groups were specified, use all groups from config
 			for solution in config_expected_scores.keys():
 				for group in config_expected_scores[solution]["expected"]:
 					used_groups.add(group)
@@ -461,15 +549,15 @@
 					for solution in change:
 						added_solutions.add(solution[0])
 				elif field[1] == "expected": # Groups were added
 					for group in change:
 						added_groups.add(group[0])
 			elif type == "remove":
 				# We check whether a solution was removed only when sinol_make was run on all of them
-				if field == '' and self.args.programs == None and config_expected_scores:
+				if field == '' and self.args.solutions == None and config_expected_scores:
 					for solution in change:
 						removed_solutions.add(solution[0])
 				# We check whether a group was removed only when sinol_make was run on all of them
 				elif field[1] == "expected" and self.args.tests == None and config_expected_scores:
 					for group in change:
 						removed_groups.add(group[0])
 			elif type == "change":
@@ -552,88 +640,101 @@
 		self.EXECUTIONS_DIR = os.path.join(self.TMP_DIR, "executions")
 		self.EXECUTABLES_DIR = os.path.join(self.TMP_DIR, "executables")
 		self.SOURCE_EXTENSIONS = ['.c', '.cpp', '.py', '.java']
 		self.PROGRAMS_IN_ROW = 8
 		self.SOLUTIONS_RE = re.compile(r"^%s[bs]?[0-9]*\.(cpp|cc|java|py|pas)$" % self.ID)
 
 
-	def run(self, args):
-		if not util.check_if_project():
-			print(util.warning('You are not in a project directory (couldn\'t find config.yml in current directory).'))
-			exit(1)
-
-		self.set_constants()
-		self.args = args
-		try:
-			self.config = yaml.load(open("config.yml"), Loader=yaml.FullLoader)
-		except AttributeError:
-			self.config = yaml.load(open("config.yml"))
-
-		if not 'title' in self.config.keys():
-			util.exit_with_error('Title was not defined in config.yml.')
-		if not 'time_limit' in self.config.keys():
-			util.exit_with_error('Time limit was not defined in config.yml.')
-		if not 'memory_limit' in self.config.keys():
-			util.exit_with_error('Memory limit was not defined in config.yml.')
-		if not 'scores' in self.config.keys():
-			util.exit_with_error('Scores were not defined in config.yml.')
-
+	def validate_arguments(self, args):
 		for solution in self.get_solutions(None):
 			ext = os.path.splitext(solution)[1]
 			compiler = ""
 			tried = ""
 			flag = ""
 			if ext == '.c' and args.c_compiler_path is None:
 				compiler = 'C compiler'
 				flag = '--c_compiler_path'
 				if sys.platform == 'darwin':
-					tried = 'gcc-{9,10,11,12}'
+					tried = 'gcc-{9,10}'
 				else:
 					tried = 'gcc'
 			elif ext == '.cpp' and args.cpp_compiler_path is None:
 				compiler = 'C++ compiler'
 				flag = '--cpp_compiler_path'
 				if sys.platform == 'darwin':
-					tried = 'g++-{9,10,11,12}'
+					tried = 'g++-{9,10}'
 				else:
 					tried = 'g++'
 			elif ext == '.py' and args.python_interpreter_path is None:
 				compiler = 'Python interpreter'
 				flag = '--python_interpreter_path'
 				tried = 'python3'
 			elif ext == '.java' and args.java_compiler_path is None:
 				compiler = 'Java compiler'
 				flag = '--java_compiler_path'
 				tried = 'javac'
 
 			if compiler != "":
 				util.exit_with_error('Couldn\'t find a %s. Tried %s. Try specifying a compiler with %s.' % (compiler, tried, flag))
 
-		self.compilers = {
+		compilers = {
 			'c_compiler_path': args.c_compiler_path,
 			'cpp_compiler_path': args.cpp_compiler_path,
 			'python_interpreter_path': args.python_interpreter_path,
 			'java_compiler_path': args.java_compiler_path
 		}
 
-		if 'oiejq_path' in args and args.oiejq_path is not None:
-			if not util.check_oiejq(args.oiejq_path):
-				util.exit_with_error('Invalid oiejq path.')
-			self.timetool_path = args.oiejq_path
-		else:
-			self.timetool_path = util.get_oiejq_path()
-		if self.timetool_path is None:
-			util.exit_with_error('oiejq is not installed.')
+		timetool_path = None
+		if args.time_tool == 'oiejq':
+			if sys.platform != 'linux':
+				util.exit_with_error('oiejq is only available on Linux.')
+			if 'oiejq_path' in args and args.oiejq_path is not None:
+				if not util.check_oiejq(args.oiejq_path):
+					util.exit_with_error('Invalid oiejq path.')
+				timetool_path = args.oiejq_path
+			else:
+				timetool_path = util.get_oiejq_path()
+			if timetool_path is None:
+				util.exit_with_error('oiejq is not installed.')
+		elif args.time_tool == 'time':
+			if sys.platform == 'win32' or sys.platform == 'cygwin':
+				util.exit_with_error('Measuring with `time` is not supported on Windows.')
+			timetool_path = 'time'
+
+		return compilers, timetool_path
+
+	def run(self, args):
+		if not util.check_if_project():
+			print(util.warning('You are not in a project directory (couldn\'t find config.yml in current directory).'))
+			exit(1)
+
+		self.set_constants()
+		self.args = args
+		try:
+			self.config = yaml.load(open("config.yml"), Loader=yaml.FullLoader)
+		except AttributeError:
+			self.config = yaml.load(open("config.yml"))
+
+		if not 'title' in self.config.keys():
+			util.exit_with_error('Title was not defined in config.yml.')
+		if not 'time_limit' in self.config.keys():
+			util.exit_with_error('Time limit was not defined in config.yml.')
+		if not 'memory_limit' in self.config.keys():
+			util.exit_with_error('Memory limit was not defined in config.yml.')
+		if not 'scores' in self.config.keys():
+			util.exit_with_error('Scores were not defined in config.yml.')
+
+		self.compilers, self.timetool_path = self.validate_arguments(args)
 
 		title = self.config["title"]
 		print("Task %s (%s)" % (title, self.ID))
 		config_time_limit = self.config["time_limit"]
 		config_memory_limit = self.config["memory_limit"]
 		self.time_limit = args.tl * 1000.0 if args.tl is not None else config_time_limit
-		self.memory_limit = args.ml * 1024.0 if args.ml is not None else config_memory_limit
+		self.memory_limit = args.ml * 1024 if args.ml is not None else config_memory_limit
 		self.cpus = args.cpus or mp.cpu_count()
 		if self.time_limit == config_time_limit:
 			print("Time limit (in ms):", self.time_limit)
 		else:
 			print("Time limit (in ms):", self.time_limit,
 				util.warning(("[originally was %.1f ms]" % config_time_limit)))
 		if self.memory_limit == config_memory_limit:
@@ -652,11 +753,11 @@
 			print(util.warning("WARN: Scores sum up to %d (instead of 100)." % total_score))
 		print()
 
 		self.tests = self.get_tests(args.tests)
 		self.groups = list(sorted(set([self.get_group(test) for test in self.tests])))
 		self.possible_score = self.get_possible_score(self.groups)
 
-		solutions = self.get_solutions(self.args.programs)
-		results = self.run_solutions(solutions)
+		solutions = self.get_solutions(self.args.solutions)
+		results = self.compile_and_run(solutions)
 		validation_results = self.validate_expected_scores(results)
 		self.print_expected_scores_diff(validation_results)
```

### Comparing `sinol-make-1.0.0/src/sinol_make/helpers/compile.py` & `sinol-make-1.1.0/src/sinol_make/helpers/compile.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.0.0/src/sinol_make/helpers/compiler.py` & `sinol-make-1.1.0/src/sinol_make/helpers/compiler.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 	if sys.platform == 'win32' or sys.platform == 'cygwin' or sys.platform == 'linux':
 		if not check_if_installed('gcc'):
 			return None
 		else:
 			return 'gcc'
 	elif sys.platform == 'darwin':
-		for i in range(9, 13):
+		for i in [9, 10, 11]:
 			compiler = 'gcc-' + str(i)
 			if check_if_installed(compiler):
 				return compiler
 
 		return None
 
 def get_cpp_compiler_path():
@@ -39,15 +39,15 @@
 
 	if sys.platform == 'win32' or sys.platform == 'cygwin' or sys.platform == 'linux':
 		if not check_if_installed('g++'):
 			return None
 		else:
 			return 'g++'
 	elif sys.platform == 'darwin':
-		for i in range(9, 13):
+		for i in [9, 10, 11]:
 			compiler = 'g++-' + str(i)
 			if check_if_installed(compiler):
 				return compiler
 
 		return None
 
 def get_python_interpreter_path():
```

### Comparing `sinol-make-1.0.0/src/sinol_make/util.py` & `sinol-make-1.1.0/src/sinol_make/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,32 +64,35 @@
 
 	if sys.platform != 'linux':
 		return False
 	if check_oiejq():
 		return True
 
 	if not os.path.exists(os.path.expanduser('~/.local/bin')):
-		os.makedirs(os.path.expanduser('~/.local/bin'))
+		os.makedirs(os.path.expanduser('~/.local/bin'), exist_ok=True)
 
-	request = requests.get('https://oij.edu.pl/zawodnik/srodowisko/oiejq.tar.gz')
+	try:
+		request = requests.get('https://oij.edu.pl/zawodnik/srodowisko/oiejq.tar.gz')
+	except requests.exceptions.ConnectionError:
+		raise Exception('Couldn\'t download oiejq (https://oij.edu.pl/zawodnik/srodowisko/oiejq.tar.gz couldn\'t connect)')
 	if request.status_code != 200:
 		raise Exception('Couldn\'t download oiejq (https://oij.edu.pl/zawodnik/srodowisko/oiejq.tar.gz returned status code: ' + str(request.status_code) + ')')
 	open('/tmp/oiejq.tar.gz', 'wb').write(request.content)
 
 	def strip(tar):
 		l = len('oiejq/')
 		for member in tar.getmembers():
 			member.name = member.name[l:]
 			yield member
 
 	tar = tarfile.open('/tmp/oiejq.tar.gz')
 	tar.extractall(path=os.path.expanduser('~/.local/bin'), members=strip(tar))
 	tar.close()
 	os.remove('/tmp/oiejq.tar.gz')
-	os.rename(os.path.expanduser('~/.local/bin/oiejq'), os.path.expanduser('~/.local/bin/oiejq'))
+	os.rename(os.path.expanduser('~/.local/bin/oiejq.sh'), os.path.expanduser('~/.local/bin/oiejq'))
 
 	return check_oiejq()
 
 
 def get_oiejq_path():
 	if not check_oiejq():
 		return None
```

### Comparing `sinol-make-1.0.0/src/sinol_make.egg-info/SOURCES.txt` & `sinol-make-1.1.0/src/sinol_make.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 src/sinol_make/commands/run/__init__.py
 src/sinol_make/commands/run/structs.py
 src/sinol_make/helpers/__init__.py
 src/sinol_make/helpers/compile.py
 src/sinol_make/helpers/compiler.py
 src/sinol_make/interfaces/BaseCommand.py
 src/sinol_make/interfaces/Errors.py
-src/sinol_make/interfaces/__init__.py
+src/sinol_make/interfaces/__init__.py
+tests/test_util.py
```

