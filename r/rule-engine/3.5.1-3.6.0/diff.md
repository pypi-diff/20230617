# Comparing `tmp/rule-engine-3.5.1.tar.gz` & `tmp/rule-engine-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rule-engine-3.5.1.tar", last modified: Sat Feb 25 19:33:47 2023, max compression
+gzip compressed data, was "rule-engine-3.6.0.tar", last modified: Sat Jun 17 16:22:33 2023, max compression
```

## Comparing `rule-engine-3.5.1.tar` & `rule-engine-3.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:33:47.071578 rule-engine-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-02-25 19:33:17.000000 rule-engine-3.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-02-25 19:33:47.071578 rule-engine-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-02-25 19:33:17.000000 rule-engine-3.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:33:47.071578 rule-engine-3.5.1/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:33:47.071578 rule-engine-3.5.1/lib/rule_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-02-25 19:33:17.000000 rule-engine-3.5.1/lib/rule_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-02-25 19:33:17.000000 rule-engine-3.5.1/lib/rule_engine/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49125 2023-02-25 19:33:17.000000 rule-engine-3.5.1/lib/rule_engine/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-02-25 19:33:17.000000 rule-engine-3.5.1/lib/rule_engine/debug_repl.py
--rw-r--r--   0 runner    (1001) docker     (123)    26440 2023-02-25 19:33:17.000000 rule-engine-3.5.1/lib/rule_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-02-25 19:33:17.000000 rule-engine-3.5.1/lib/rule_engine/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-02-25 19:33:17.000000 rule-engine-3.5.1/lib/rule_engine/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-02-25 19:33:17.000000 rule-engine-3.5.1/lib/rule_engine/suggestions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18478 2023-02-25 19:33:17.000000 rule-engine-3.5.1/lib/rule_engine/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:33:47.071578 rule-engine-3.5.1/lib/rule_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-02-25 19:33:47.000000 rule-engine-3.5.1/lib/rule_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-02-25 19:33:47.000000 rule-engine-3.5.1/lib/rule_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 19:33:47.000000 rule-engine-3.5.1/lib/rule_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-25 19:33:47.000000 rule-engine-3.5.1/lib/rule_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-25 19:33:47.000000 rule-engine-3.5.1/lib/rule_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-25 19:33:47.071578 rule-engine-3.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3692 2023-02-25 19:33:17.000000 rule-engine-3.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:22:33.023142 rule-engine-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-17 16:22:03.000000 rule-engine-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-06-17 16:22:33.023142 rule-engine-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-17 16:22:03.000000 rule-engine-3.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:22:33.019142 rule-engine-3.6.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:22:33.019142 rule-engine-3.6.0/lib/rule_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49596 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/debug_repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26440 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18552 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/suggestions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18478 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:22:33.023142 rule-engine-3.6.0/lib/rule_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-06-17 16:22:32.000000 rule-engine-3.6.0/lib/rule_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-17 16:22:32.000000 rule-engine-3.6.0/lib/rule_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 16:22:32.000000 rule-engine-3.6.0/lib/rule_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-17 16:22:32.000000 rule-engine-3.6.0/lib/rule_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 16:22:32.000000 rule-engine-3.6.0/lib/rule_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 16:22:33.023142 rule-engine-3.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3732 2023-06-17 16:22:03.000000 rule-engine-3.6.0/setup.py
```

### Comparing `rule-engine-3.5.1/LICENSE` & `rule-engine-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rule-engine-3.5.1/PKG-INFO` & `rule-engine-3.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: rule-engine
-Version: 3.5.1
+Version: 3.6.0
 Summary: A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.
 Home-page: https://github.com/zeroSteiner/rule-engine
 Author: Spencer McIntyre
 Author-email: zeroSteiner@gmail.com
 Maintainer: Spencer McIntyre
 Maintainer-email: zeroSteiner@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -29,16 +27,16 @@
 |badge-build| |badge-pypi|
 
 A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.
 
 Documentation is available at https://zeroSteiner.github.io/rule-engine/.
 
 :Warning:
-  The next minor version (3.6) will be the last to support Python versions 3.4 and 3.5. There is currently no timeline
-  for its release. The following version, either 3.7 or 4.0, will not suport Python versions 3.4 or 3.5.
+  Version 3.6 is the last to support Python versions 3.4 and 3.5. The next version, either 3.7 or 4.0, will drop them.
+  There is currently no timeline for its release.
 
 Rule Engine expressions are written in their own language, defined as strings in Python. The syntax is most similar to
 Python with some inspiration from Ruby. Some features of this language includes:
 
 - Optional type hinting
 - Matching strings with regular expressions
 - Datetime datatypes
```

### Comparing `rule-engine-3.5.1/README.rst` & `rule-engine-3.6.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 |badge-build| |badge-pypi|
 
 A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.
 
 Documentation is available at https://zeroSteiner.github.io/rule-engine/.
 
 :Warning:
-  The next minor version (3.6) will be the last to support Python versions 3.4 and 3.5. There is currently no timeline
-  for its release. The following version, either 3.7 or 4.0, will not suport Python versions 3.4 or 3.5.
+  Version 3.6 is the last to support Python versions 3.4 and 3.5. The next version, either 3.7 or 4.0, will drop them.
+  There is currently no timeline for its release.
 
 Rule Engine expressions are written in their own language, defined as strings in Python. The syntax is most similar to
 Python with some inspiration from Ruby. Some features of this language includes:
 
 - Optional type hinting
 - Matching strings with regular expressions
 - Datetime datatypes
```

### Comparing `rule-engine-3.5.1/lib/rule_engine/__init__.py` & `rule-engine-3.6.0/lib/rule_engine/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 #  LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 #  DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 #  THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 #  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-__version__ = '3.5.1'
+__version__ = '3.6.0'
 
 from .engine import resolve_attribute
 from .engine import resolve_item
 from .engine import type_resolver_from_dict
 from .engine import Context
 from .engine import Rule
```

### Comparing `rule-engine-3.5.1/lib/rule_engine/_utils.py` & `rule-engine-3.6.0/lib/rule_engine/_utils.py`

 * *Files identical despite different names*

### Comparing `rule-engine-3.5.1/lib/rule_engine/ast.py` & `rule-engine-3.6.0/lib/rule_engine/ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,25 @@
 		instance of itself, otherwise return a reduced :py:class:`.ExpressionBase` to replace it.
 
 		:return: Either a reduced version of this node or itself.
 		:rtype: :py:class:`.ExpressionBase`
 		"""
 		return self
 
+class Comment(ASTNodeBase):
+	__slots__ = ('value',)
+	def __init__(self, value):
+		self.value = value
+
+	def __repr__(self):
+		return "<{0} {1!r}>".format(self.__class__.__name__, self.value)
+
+	def to_graphviz(self, digraph, *args, **kwargs):
+		digraph.node(str(id(self)), "{}\n{!r}".format(self.__class__.__name__, self.value))
+
 ################################################################################
 # Base Expression Classes
 ################################################################################
 class ExpressionBase(ASTNodeBase):
 	__slots__ = ('context',)
 	result_type = DataType.UNDEFINED
 	"""The data type of the result of successful evaluation."""
@@ -1021,36 +1032,39 @@
 		raise errors.SymbolTypeError(self.name, is_value=value, is_type=value_type, expected_type=self.result_type)
 
 	def to_graphviz(self, digraph, *args, **kwargs):
 		digraph.node(str(id(self)), "{}\nname={!r}".format(self.__class__.__name__, self.name))
 
 class Statement(ASTNodeBase):
 	"""A class representing the top level statement of the grammar text."""
-	__slots__ = ('context', 'expression')
-	def __init__(self, context, expression):
+	__slots__ = ('context', 'expression', 'comment')
+	def __init__(self, context, expression, comment=None):
 		"""
 		:param context: The context to use for evaluating the statement.
 		:type context: :py:class:`~rule_engine.engine.Context`
 		:param expression: The top level expression of the statement.
 		:type expression: :py:class:`~.ExpressionBase`
 		"""
 		self.context = context
 		self.expression = expression
+		self.comment = comment
 
 	@classmethod
-	def build(cls, context, expression):
-		return cls(context, expression.build()).reduce()
+	def build(cls, context, expression, **kwargs):
+		return cls(context, expression.build(), **kwargs).reduce()
 
 	def evaluate(self, thing):
 		return self.expression.evaluate(thing)
 
 	def to_graphviz(self, digraph, *args, **kwargs):
 		super(Statement, self).to_graphviz(digraph, *args, **kwargs)
 		self.expression.to_graphviz(digraph, *args, **kwargs)
 		digraph.edge(str(id(self)), str(id(self.expression)))
+		if self.comment:
+			self.comment.to_graphviz(digraph, *args, **kwargs)
 
 class TernaryExpression(ExpressionBase):
 	"""
 	A class for representing ternary expressions from the grammar text. These involve evaluating :py:attr:`.condition`
 	before evaluating either :py:attr:`.case_true` or :py:attr:`.case_false` based on the results.
 	"""
 	def __init__(self, context, condition, case_true, case_false):
```

### Comparing `rule-engine-3.5.1/lib/rule_engine/debug_repl.py` & `rule-engine-3.6.0/lib/rule_engine/debug_repl.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,17 @@
 		try:
 			rule = engine.Rule(rule_text, context=context)
 			result = rule.evaluate(thing)
 		except errors.EngineError as error:
 			print("{}: {}".format(error.__class__.__name__, error.message))
 			if isinstance(error, (errors.AttributeResolutionError, errors.SymbolResolutionError)) and error.suggestion:
 				print("Did you mean '{}'?".format(error.suggestion))
+			elif isinstance(error, errors.RegexSyntaxError):
+				print("  Regex:   {!r}".format(error.error.pattern))
+				print("  Details: {} at position {}".format(error.error.msg, error.error.pos))
 			if arguments.debug:
 				traceback.print_exc()
 		except Exception as error:
 			traceback.print_exc()
 		else:
 			print('result: ')
 			pprint.pprint(result, indent=4)
```

### Comparing `rule-engine-3.5.1/lib/rule_engine/engine.py` & `rule-engine-3.6.0/lib/rule_engine/engine.py`

 * *Files identical despite different names*

### Comparing `rule-engine-3.5.1/lib/rule_engine/errors.py` & `rule-engine-3.6.0/lib/rule_engine/errors.py`

 * *Files identical despite different names*

### Comparing `rule-engine-3.5.1/lib/rule_engine/parser.py` & `rule-engine-3.6.0/lib/rule_engine/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 		'not': 'NOT',
 		'for': 'FOR',
 		'if': 'IF'
 	}
 	tokens = (
 		'DATETIME', 'TIMEDELTA', 'FLOAT', 'STRING', 'SYMBOL',
 		'LPAREN', 'RPAREN', 'QMARK', 'COLON', 'COMMA',
-		'LBRACKET', 'RBRACKET', 'LBRACE', 'RBRACE'
+		'LBRACKET', 'RBRACKET', 'LBRACE', 'RBRACE', 'COMMENT'
 	) + tuple(set(list(reserved_words.values()) + list(op_names.values())))
 
 	t_ignore = ' \t'
 	# Tokens
 	t_BWAND            = r'\&'
 	t_BWOR             = r'\|'
 	t_BWXOR            = r'\^'
@@ -272,28 +272,38 @@
 	def t_SYMBOL(self, t):
 		r'\$?[a-zA-Z_][a-zA-Z0-9_]*'
 		if t.value in ('elif', 'else', 'while'):
 			raise errors.RuleSyntaxError("syntax error (the {} keyword is reserved for future use)".format(t.value))
 		t.type = self.reserved_words.get(t.value, 'SYMBOL')
 		return t
 
+	def t_COMMENT(self, t):
+		r'\#.*$'
+		return t
+
 	def t_newline(self, t):
 		r'\n+'
 		t.lexer.lineno += t.value.count("\n")
 
 	def t_error(self, t):
 		raise errors.RuleSyntaxError("syntax error (illegal character {0!r})".format(t.value[0]), t)
 
 	# Parsing Rules
 	def p_error(self, token):
 		raise errors.RuleSyntaxError('syntax error', token)
 
 	def p_statement_expr(self, p):
-		'statement : expression'
-		p[0] = _DeferredAstNode(ast.Statement, args=(self.context, p[1]))
+		"""
+		statement : expression
+		          | expression COMMENT
+		"""
+		kwargs = {}
+		if len(p) == 3:
+			kwargs['comment'] = ast.Comment(p[2][1:].strip())
+		p[0] = _DeferredAstNode(ast.Statement, args=(self.context, p[1]), kwargs=kwargs)
 
 	def p_expression_getattr(self, p):
 		"""
 		object : object ATTR SYMBOL
 		       | object ATTR_SAFE SYMBOL
 		"""
 		op_name = self.op_names.get(p[2])
```

### Comparing `rule-engine-3.5.1/lib/rule_engine/suggestions.py` & `rule-engine-3.6.0/lib/rule_engine/suggestions.py`

 * *Files identical despite different names*

### Comparing `rule-engine-3.5.1/lib/rule_engine/types.py` & `rule-engine-3.6.0/lib/rule_engine/types.py`

 * *Files identical despite different names*

### Comparing `rule-engine-3.5.1/lib/rule_engine.egg-info/PKG-INFO` & `rule-engine-3.6.0/lib/rule_engine.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: rule-engine
-Version: 3.5.1
+Version: 3.6.0
 Summary: A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.
 Home-page: https://github.com/zeroSteiner/rule-engine
 Author: Spencer McIntyre
 Author-email: zeroSteiner@gmail.com
 Maintainer: Spencer McIntyre
 Maintainer-email: zeroSteiner@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -29,16 +27,16 @@
 |badge-build| |badge-pypi|
 
 A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.
 
 Documentation is available at https://zeroSteiner.github.io/rule-engine/.
 
 :Warning:
-  The next minor version (3.6) will be the last to support Python versions 3.4 and 3.5. There is currently no timeline
-  for its release. The following version, either 3.7 or 4.0, will not suport Python versions 3.4 or 3.5.
+  Version 3.6 is the last to support Python versions 3.4 and 3.5. The next version, either 3.7 or 4.0, will drop them.
+  There is currently no timeline for its release.
 
 Rule Engine expressions are written in their own language, defined as strings in Python. The syntax is most similar to
 Python with some inspiration from Ruby. Some features of this language includes:
 
 - Optional type hinting
 - Matching strings with regular expressions
 - Datetime datatypes
```

### Comparing `rule-engine-3.5.1/setup.py` & `rule-engine-3.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,16 +80,16 @@
 	packages=find_packages('lib'),
 	classifiers=[
 		'Development Status :: 5 - Production/Stable',
 		'Environment :: Console',
 		'Intended Audience :: Developers',
 		'License :: OSI Approved :: BSD License',
 		'Operating System :: OS Independent',
-		'Programming Language :: Python :: 3.4',
-		'Programming Language :: Python :: 3.5',
+		#'Programming Language :: Python :: 3.4',  # dropped in v3.6
+		#'Programming Language :: Python :: 3.5',  # dropped in v3.6
 		'Programming Language :: Python :: 3.6',
 		'Programming Language :: Python :: 3.7',
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3.9',
 		'Programming Language :: Python :: 3.10',
 		'Programming Language :: Python :: 3.11',
 		'Topic :: Software Development :: Libraries :: Python Modules'
```

