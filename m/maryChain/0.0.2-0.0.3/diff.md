# Comparing `tmp/maryChain-0.0.2.tar.gz` & `tmp/maryChain-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maryChain-0.0.2.tar", last modified: Wed Jun 14 14:39:01 2023, max compression
+gzip compressed data, was "maryChain-0.0.3.tar", last modified: Sat Jun 17 12:43:54 2023, max compression
```

## Comparing `maryChain-0.0.2.tar` & `maryChain-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-06-14 14:39:01.258734 maryChain-0.0.2/
--rw-r--r--   0 alessioricco   (501) staff       (20)     1070 2023-06-14 11:53:05.000000 maryChain-0.0.2/LICENSE
--rw-r--r--   0 alessioricco   (501) staff       (20)     7430 2023-06-14 14:39:01.258469 maryChain-0.0.2/PKG-INFO
--rw-r--r--   0 alessioricco   (501) staff       (20)     6601 2023-06-14 12:25:32.000000 maryChain-0.0.2/README.md
-drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-06-14 14:39:01.255822 maryChain-0.0.2/maryChain/
--rw-r--r--   0 alessioricco   (501) staff       (20)        0 2023-06-11 22:34:10.000000 maryChain-0.0.2/maryChain/__init__.py
--rw-r--r--   0 alessioricco   (501) staff       (20)    25622 2023-06-14 14:37:37.000000 maryChain-0.0.2/maryChain/maryChain.py
--rw-r--r--   0 alessioricco   (501) staff       (20)    32183 2023-06-13 19:41:24.000000 maryChain-0.0.2/maryChain/maryChainAST.py
--rw-r--r--   0 alessioricco   (501) staff       (20)    13166 2023-06-14 12:17:08.000000 maryChain-0.0.2/maryChain/parsetab.py
-drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-06-14 14:39:01.258152 maryChain-0.0.2/maryChain.egg-info/
--rw-r--r--   0 alessioricco   (501) staff       (20)     7430 2023-06-14 14:39:01.000000 maryChain-0.0.2/maryChain.egg-info/PKG-INFO
--rw-r--r--   0 alessioricco   (501) staff       (20)      283 2023-06-14 14:39:01.000000 maryChain-0.0.2/maryChain.egg-info/SOURCES.txt
--rw-r--r--   0 alessioricco   (501) staff       (20)        1 2023-06-14 14:39:01.000000 maryChain-0.0.2/maryChain.egg-info/dependency_links.txt
--rw-r--r--   0 alessioricco   (501) staff       (20)        4 2023-06-14 14:39:01.000000 maryChain-0.0.2/maryChain.egg-info/requires.txt
--rw-r--r--   0 alessioricco   (501) staff       (20)       10 2023-06-14 14:39:01.000000 maryChain-0.0.2/maryChain.egg-info/top_level.txt
--rw-r--r--   0 alessioricco   (501) staff       (20)       38 2023-06-14 14:39:01.258809 maryChain-0.0.2/setup.cfg
--rw-r--r--   0 alessioricco   (501) staff       (20)     1642 2023-06-14 14:33:58.000000 maryChain-0.0.2/setup.py
+drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-06-17 12:43:54.951859 maryChain-0.0.3/
+-rw-r--r--   0 alessioricco   (501) staff       (20)     1070 2023-06-14 11:53:05.000000 maryChain-0.0.3/LICENSE
+-rw-r--r--   0 alessioricco   (501) staff       (20)     4394 2023-06-17 12:43:54.951672 maryChain-0.0.3/PKG-INFO
+-rw-r--r--   0 alessioricco   (501) staff       (20)     3545 2023-06-17 12:36:30.000000 maryChain-0.0.3/README.md
+drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-06-17 12:43:54.950113 maryChain-0.0.3/maryChain/
+-rw-r--r--   0 alessioricco   (501) staff       (20)        0 2023-06-11 22:34:10.000000 maryChain-0.0.3/maryChain/__init__.py
+-rw-r--r--   0 alessioricco   (501) staff       (20)    20431 2023-06-17 12:39:47.000000 maryChain-0.0.3/maryChain/maryChain.py
+-rw-r--r--   0 alessioricco   (501) staff       (20)    32292 2023-06-17 12:06:20.000000 maryChain-0.0.3/maryChain/maryChainAST.py
+-rw-r--r--   0 alessioricco   (501) staff       (20)    14750 2023-06-17 11:03:06.000000 maryChain-0.0.3/maryChain/parsetab.py
+drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-06-17 12:43:54.951398 maryChain-0.0.3/maryChain.egg-info/
+-rw-r--r--   0 alessioricco   (501) staff       (20)     4394 2023-06-17 12:43:54.000000 maryChain-0.0.3/maryChain.egg-info/PKG-INFO
+-rw-r--r--   0 alessioricco   (501) staff       (20)      283 2023-06-17 12:43:54.000000 maryChain-0.0.3/maryChain.egg-info/SOURCES.txt
+-rw-r--r--   0 alessioricco   (501) staff       (20)        1 2023-06-17 12:43:54.000000 maryChain-0.0.3/maryChain.egg-info/dependency_links.txt
+-rw-r--r--   0 alessioricco   (501) staff       (20)        4 2023-06-17 12:43:54.000000 maryChain-0.0.3/maryChain.egg-info/requires.txt
+-rw-r--r--   0 alessioricco   (501) staff       (20)       10 2023-06-17 12:43:54.000000 maryChain-0.0.3/maryChain.egg-info/top_level.txt
+-rw-r--r--   0 alessioricco   (501) staff       (20)       38 2023-06-17 12:43:54.951910 maryChain-0.0.3/setup.cfg
+-rw-r--r--   0 alessioricco   (501) staff       (20)     1662 2023-06-17 12:43:42.000000 maryChain-0.0.3/setup.py
```

### Comparing `maryChain-0.0.2/LICENSE` & `maryChain-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `maryChain-0.0.2/maryChain/maryChain.py` & `maryChain-0.0.3/maryChain/maryChain.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,15 @@
 '''BNF
-<program> ::= <defn>* <expr>?
-<expression> ::= <term>
-              | <term> "+" <expression>
-              | <term> "-" <expression>
-              | <term> "*" <expression>
-              | <term> "/" <expression>
-              | "(" <expression> ")"
-              | <term> "==" <expression>
-              | <term> "<" <expression>
-              | <term> ">" <expression>
-              | <term> "<=" <expression>
-              | <term> ">=" <expression>
-              | "if" <expression> "then" <expression> "else" <expression>
-              | "while" <expression> "do" <expression>
-              | "lazy" <expression>
-              | "{" <expression> "}"
-              | "lambda" "(" <args> ")" <expression>
-              | <expression> "|" <expression>
-
-<term> ::= <factor>
-        | <string>
-        | <number>
-        | <boolean>
-        | <function_call>
-
-<factor> ::= <number>
-           | <string>
-           | "true"
-           | "false"
-
-<function_call> ::= <function_call> "(" <args> ")"
-                  | <identifier> "(" <args> ")"
-                  | <identifier>
 
-<args> ::= <arg>
-         | <args> "," <arg>
-
-<arg> ::= <expression>
 '''
 
 # Importing necessary libraries
 from ply import lex, yacc
 from maryChain.maryChainAST import Program, BinOp, UnaryOperation, Number, String, Boolean, Identifier, LetIn, LambdaFunction
-from maryChain.maryChainAST import FunctionDef, FunctionCall, While, IfThenElse, IfThen, Lazy, Pipe, Import
+from maryChain.maryChainAST import FunctionCall, While, IfThenElse, IfThen, Lazy, Pipe, Import, CurriedFunction, Assignment
 import maryChain.maryChainAST as AST
 
 # Define the list of tokens that the lexer will recognize
 # Define the list of tokens that the lexer will recognize.
 # These tokens represent the different types of elements that can appear in the language's syntax.
 # Each token corresponds to a specific type of character sequence that can appear in the language's source code.
 tokens = (
@@ -140,43 +103,24 @@
     # 'import' is used for importing libraries.
     'import': 'IMPORT',
     'as': 'AS'
     # add other reserved words here
 }
 
 
-# Define operator precedence rules.
-# These rules dictate the order in which operations are performed when evaluating expressions, 
-# i.e., which operations are done first.
-# Each rule is a tuple where the first element is the associativity of the operators ('left' or 'right'),
-# and the remaining elements are the operator(s) at that level of precedence.
+
 precedence = (
-    # The pipe operator has the lowest precedence and is left-associative.
     ('left', 'PIPE'),
-
-    # The logical OR operator is next in line with left associativity.
     ('left', 'OR'),
-
-    # The logical AND operator follows with left associativity.
     ('left', 'AND'),
-
-    # The logical NOT operator is next with left associativity.
     ('left', 'NOT'),
-
-    # The equality and relational operators all have the same level of precedence and are left-associative.
-    ('left', 'EQUALITY', 'GREATER', 'LESS', 'GREATEREQUAL', 'LESSEQUAL'),
-
-    # The addition and subtraction operators are at the next level of precedence, also left-associative.
+    ('nonassoc', 'EQUALITY', 'GREATER', 'LESS', 'GREATEREQUAL', 'LESSEQUAL'),
+    ('right', 'UMINUS'),
     ('left', 'PLUS', 'MINUS'),
-
-    # The multiplication and division operators are next with higher precedence, left-associative.
     ('left', 'TIMES', 'DIVIDE'),
-
-    # The unary minus operator has the highest precedence and is right-associative.
-    ('right', 'UMINUS'),
 )
 
 
 # Define regular expressions for each token
 t_DEF = r'def'
 # t_PLACEHOLDER = r'_'
 t_PLUS = r'\+'
@@ -254,19 +198,15 @@
 
 
 # --------------------------------------------------------------
 # Initialize the lexer
 lexer = lex.lex()
 
 def p_program(t):
-    '''program : definitions imports expression
-               | imports expression
-               | definitions expression
-               | imports
-               | definitions
+    '''program : imports expression
                | expression'''
     """
     Handles the parsing of the whole program.
     
     The function handles the parsing of the program which consists of function definitions,
     imports, and the main expression. Each component is optional and can appear zero or more
     times (for definitions and imports) or at most once (for expression).
@@ -276,42 +216,58 @@
 
     Sets:
     t[0]: A Program object, representing the whole program.
     """
 
     if len(t) == 2:
         imports = []
-        definitions = []
         expression = t[1]
         if isinstance(t[1],list):
             if len(t[1])> 0:
                 if isinstance(t[1][0], Import):
                     imports = t[1]
                     expression = None
-                elif isinstance(t[1][0], FunctionDef):
-                    definitions = t[1]
-                    expression = None
             
-        t[0] = Program(imports, definitions, expression)
+        t[0] = Program(imports, expression)
 
     elif len(t) == 3:
-        # is definition or expresssion?
-        imports = []
-        definitions = []
-        if isinstance(t[1],list):
-            if len(t[1])> 0:
-                if isinstance(t[1][0], Import):
-                    imports = t[1]
-                elif isinstance(t[1][0], FunctionDef):
-                    definitions = t[1]
+            # is definition or expresssion?
+            imports = []
+            if isinstance(t[1],list):
+                if len(t[1])> 0:
+                    if isinstance(t[1][0], Import):
+                        imports = t[1]
+
+
+            t[0] = Program(imports, t[2])
+
+# --------------------------------------------------------------
+
+def p_import(t):
+    'import : IMPORT IDENTIFIER AS IDENTIFIER'
+    print("Import statement detected: ", t[2], t[4])
+    t[0] = Import(t[2], t[4])
+
+def p_imports(t):
+    '''
+    imports : import
+            | imports import
+    '''
+    # if there's only one import statement
+    if len(t) == 2:
+        t[0] = [t[1]]
+    # if there's more than one import statement
+    else:
+        t[1].append(t[2])
+        t[0] = t[1]
 
-        t[0] = Program(definitions, imports, t[2])
-    elif len(t) == 4:
-        t[0] = Program(t[1], t[2], t[3])
+def p_expression_assignment(t):
+    'expression : IDENTIFIER EQUALS expression'
 
+    t[0] = Assignment(t[1], t[3])
 
 def p_expression_let_in(t):
     'expression : LET IDENTIFIER EQUALS expression IN expression'
     """
     Handles the parsing of 'let in' expressions.
 
     The function handles the 'let' keyword syntax which is used to declare variables.
@@ -326,70 +282,41 @@
 
     Sets:
     t[0]: A LetIn object, representing the variable assignment and scope for the 'let in'
           construct.
     """
     t[0] = LetIn(t[2], t[4], t[6])
 
-
-
 def p_expression_binop(t):
     '''expression : expression PLUS expression
                   | expression MINUS expression
                   | expression TIMES expression
+                  | expression EQUALITY expression
+                  | expression GREATER expression
+                  | expression LESS expression
+                  | expression GREATEREQUAL expression
+                  | expression LESSEQUAL expression
                   | expression DIVIDE expression'''
     """
     Handles the parsing of binary operations.
 
     The function handles the basic binary mathematical operations: addition, subtraction,
-    multiplication, and division. For a given operation 'expression OPERATOR expression', it
+    multiplication, and division. For a given operation 'expression BINOPS expression', it
     constructs a BinOp object with the two expressions and the operator as arguments.
 
     Parameters:
     t: A list where each element represents a component of the syntax being parsed. The elements
-       correspond to the 'expression OPERATOR expression' structure.
+       correspond to the 'expression BINOPS expression' structure.
 
     Sets:
     t[0]: A BinOp object, representing the binary operation.
     """
     t[0] = BinOp(t[1], t[2], t[3])
 
 
-# --------------------------------------------------------------
-#  import
-def p_namespace(p):
-    '''namespace : IDENTIFIER
-                 | namespace DOT IDENTIFIER'''
-    if len(p) == 2:
-        # If namespace is a single identifier, make it a one-element list
-        p[0] = [p[1]]
-    else:
-        # If namespace is another namespace followed by an identifier, 
-        # append the identifier to the list of identifiers in the namespace
-        p[0] = p[1] + [p[3]]
-
-def p_import(t):
-    'import : IMPORT IDENTIFIER AS IDENTIFIER'
-    print("Import statement detected: ", t[2], t[4])
-    t[0] = Import(t[2], t[4])
-
-def p_imports(t):
-    '''
-    imports : import
-            | imports import
-    '''
-    # if there's only one import statement
-    if len(t) == 2:
-        t[0] = [t[1]]
-    # if there's more than one import statement
-    else:
-        t[1].append(t[2])
-        t[0] = t[1]
-
-
 # Rule for unary minus operation
 def p_expression_uminus(t):
     'expression : MINUS expression %prec UMINUS'
     t[0] = UnaryOperation('-', t[2])  # Represent unary minus as a UnaryOperation.
 
 def p_expression_paren(t):
     'expression : LPAREN expression RPAREN'
@@ -479,15 +406,15 @@
     Sets:
     t[0]: A Lazy object, representing the lazy evaluation construct.
     """
     t[0] = Lazy(t[2])  # Wrap the expression in a Lazy node.
 
 
 def p_expression_braces(t):
-    'expression : LCBRACE expression RCBRACE'
+    'term : LCBRACE term RCBRACE'
     """
     Handles the parsing of expressions within braces in the language.
 
     The function processes constructs that are enclosed within braces '{}'. For an input of the form
     '{expression}', it constructs a Lazy object with the expression as an argument.
 
     Parameters:
@@ -497,15 +424,15 @@
     Sets:
     t[0]: A Lazy object, representing the expression enclosed in braces.
     """
     t[0] = Lazy(t[2])  # Wrap the expression in a Lazy node.
 
 
 def p_expression_lambda(t):
-    'expression : LAMBDA LPAREN args RPAREN expression'
+    'lambda : LAMBDA LPAREN args RPAREN expression'
     """
     Handles the parsing of lambda expressions in the language.
 
     The function processes constructs of the form 'lambda (args) expression'. It creates a LambdaFunction 
     object with the arguments and the body expression as parameters.
 
     Parameters:
@@ -532,15 +459,16 @@
 
     Sets:
     p[0]: A Pipe object, representing the pipe operation.
     """
     p[0] = Pipe(p[1], p[3])  # Create a new Pipe node.
 
 def p_expression_func_call(t):
-    'expression : function_call'
+    '''expression : function_call 
+                  | lambda'''
     """
     Handles the parsing of function calls in the language.
 
     The function processes constructs where a function is called. It sets the parsed function call
     as the expression's value.
 
     Parameters:
@@ -601,99 +529,36 @@
         print(f"Offending value: {value}")
 
 
 
 # -------------------------------------------------------------------
 # Rule for function calls
 
-def p_function_definition(t):
-    'function_definition : FUNC IDENTIFIER LPAREN args RPAREN LCBRACE expression RCBRACE'
-    """
-    Parses function definition expressions.
-
-    This function parses a function definition, which consists of the 'func' keyword,
-    followed by an identifier (the function's name), parentheses enclosing arguments 
-    (if any), and a block of code enclosed in curly braces. 
-
-    After successful parsing, a FunctionDef object is constructed with the function name, 
-    arguments, and the expression (body of the function) as arguments.
-
-    Parameters:
-    t: A PLY lex token instance. It is a tuple where t[2] is the function's name, t[4] is 
-       the function's arguments, and t[7] is the body of the function (an expression).
-
-    Returns:
-    None
-    """
-    # FunctionDef is a hypothetical class to store function definitions. This will need to be 
-    # defined elsewhere in your code. It takes the function name, the arguments, and the body 
-    # of the function (an expression).
-    t[0] = FunctionDef(t[2], t[4], t[7]) 
-
-def p_definitions(t):
-    '''
-    definitions : function_definition
-                | definitions function_definition
-    '''
-    # if there's only one function definition
-    if len(t) == 2:
-        t[0] = [t[1]]
-    # if there's more than one function definition
-    else:
-        t[1].append(t[2])
-        t[0] = t[1]
-
-
-# def p_function_call(t):
-    '''function_call : function_call LPAREN args RPAREN
-                     | IDENTIFIER LPAREN args RPAREN
-                     | IDENTIFIER'''
-    """
-    Parses function call expressions.
-
-    This function parses a function call, which may be a simple function call with or without 
-    arguments, or a chained function call with or without arguments. It constructs a FunctionCall 
-    object with the function's name and arguments.
-
-    Parameters:
-    t: A PLY lex token instance. If it is a simple function call, t[1] is the function's name 
-       and t[3] are the function's arguments. If it is a chained function call, t[1] is the 
-       previous function call, and t[3] are the arguments of the next function in the chain.
-
-    Returns:
-    None
-    """
-    # # Check if there are arguments in the function call, if not set it to an empty list
-    # args = [] if len(t) == 2 else t[3]
-    # # Get the function name (it can be an identifier or another function call in case of function chaining)
-    # function_name = t[1]
-    # # FunctionCall and Identifier are hypothetical classes to store function calls and identifiers.
-    # # These will need to be defined elsewhere in your code. FunctionCall takes the function name 
-    # # (wrapped in an Identifier instance) and the arguments of the function.
-    # t[0] = FunctionCall(Identifier(function_name), args) 
-
-
 def p_function_call(t):
     '''function_call : function_call LPAREN args RPAREN
-                     | IDENTIFIER LPAREN args RPAREN
+                     | function_call LPAREN RPAREN
+                     | lambda LPAREN args RPAREN
                      | IDENTIFIER'''
-    if len(t) == 4 and isinstance(t[2], FunctionCall):
-        # Function call following another function call
-        # Treat it as currying
-        t[0] = FunctionCall(t[2], [t[4]])
+    if len(t) == 4:
+        # function_call LPAREN args RPAREN
+        # a function call with arguments
+        t[0] = FunctionCall(t[1], t[3])
     elif len(t) == 2:
-        # Single function call
-        args = []
-        function_name = t[1]
-        t[0] = FunctionCall(Identifier(function_name), args)
-    else:
-        # Function call with arguments
-        args = t[3]
-        function_name = t[1]
-        t[0] = FunctionCall(Identifier(function_name), args)
+        # IDENTIFIER
+        # could be an entity of type function (a lambda associated with a variable)
+        t[0] = Identifier(t[1])
+    elif len(t) == 5:
+        # Function call with arguments followed by another function call or identifier
+        if isinstance(t[3], FunctionCall) or isinstance(t[3], Identifier):
+            t[0] = FunctionCall(t[1], [t[3]])
+        elif isinstance(t[1],LambdaFunction):
+            t[0] = FunctionCall(t[1],t[3])
+        else:
+            # Handle currying
+            t[0] = CurriedFunction(t[1], [t[3]])
 
 
 def p_args(t):
     '''args : args COMMA arg
             | arg
             | '''
     """
@@ -769,11 +634,11 @@
         return None
 
     # Otherwise, evaluate the AST using the evaluate method of the AST class
     result = AST.evaluate(ast)
 
     # If the result is a Lazy node, evaluate it to get the final result
     if isinstance(result, Lazy):
-        result = result.evaluate()
+        result = result.evaluate(AST.ENVIRONMENT)
 
     # Return the result of the evaluation
     return result
```

### Comparing `maryChain-0.0.2/maryChain/maryChainAST.py` & `maryChain-0.0.3/maryChain/maryChainAST.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,62 @@
 from abc import ABC, abstractmethod
 import importlib
 import inspect
-import sys, os
-import types
+# import sys, os
+from functools import partial, wraps
 
-core_lib = os.path.dirname(os.path.realpath(__file__)) + '/../Workers'
-sys.path.append("/Users/alessioricco/Documents/GitHub/GPTWorkers")
-print(sys.path)
+# --------------------------------------------------------------
+
+def curry(func):
+    if isinstance(func, partial):
+        # Handle functools.partial objects
+        num_required_args = func.func.__code__.co_argcount
+        num_wrapped_args = len(func.args) + len(func.keywords)
+
+        @wraps(func)
+        def curried(*args, **kwargs):
+            all_args = func.args + args
+            all_kwargs = {**func.keywords, **kwargs}
+            evaluated_args = [arg.evaluate({}) if isinstance(arg,Evaluable) else arg for arg in args]
+
+            if len(all_args) + len(all_kwargs) >= num_required_args:
+                return func(*evaluated_args, **all_kwargs)
+            else:
+                return curry(partial(func.func, *evaluated_args, **all_kwargs))
+
+        return curried
+    elif isinstance(func, LambdaFunctionValue):
+        num_required_args = len(func.args)
+
+        @wraps(func)
+        def curried(*args, **kwargs):
+            evaluated_args = [arg.evaluate({}) if isinstance(arg,Evaluable) else arg for arg in args]
+            if len(args) + len(kwargs) >= num_required_args:
+                # return func(*evaluated_args, **kwargs)
+                return func.evaluate({},*evaluated_args)
+            else:
+                return curry(partial(func, *evaluated_args, **kwargs))
+        return curried
+    else:
+        # Handle regular functions
+        num_required_args = func.__code__.co_argcount
+
+        @wraps(func)
+        def curried(*args, **kwargs):
+            evaluated_args = [arg.evaluate({}) if isinstance(arg,Evaluable) else arg for arg in args]
+            if len(args) + len(kwargs) >= num_required_args:
+                return func(*evaluated_args, **kwargs)
+            else:
+                return curry(partial(func, *evaluated_args, **kwargs))
+
+        return curried
 
+def curry_builtin(func):
+    # Define a lambda that wraps the built-in function
+    return lambda *args, **kwargs: func(*args, **kwargs)
 
 def add_module_functions_to_dict(module_name,alias):
     # core.hello()
     try:
         module=importlib.import_module(module_name)
     except ModuleNotFoundError:
         print(f"The module {module_name} was not found.")
@@ -21,16 +66,16 @@
 
     for(name,func) in inspect.getmembers(module,inspect.getmodule):
         if callable(func):
             try:
                 args = inspect.getfullargspec(func).args
             except:
                 args = []
-            FUNCTION_DICT[alias][name]=FunctionDef(name,args,curry(func))
-
+            FUNCTION_DICT[alias][name]=curry_builtin(func)
+            # FUNCTION_DICT[alias][name]=FunctionDef(name,args,curry(func))
 
 
 # Now you can add the functions of a module to the FUNCTION_DICT like this:
 # add_module_functions_to_dict('aleph')
 
 
 class Evaluable(ABC):
@@ -45,15 +90,15 @@
     This class has an abstract method `evaluate`, which should be implemented by all subclasses to define their evaluation semantics.
 
     The evaluate method of a class representing an evaluable entity in maryChain takes keyword arguments (`kwargs`) 
     which could be used to provide context necessary for evaluation, such as a dictionary of variable names and their values. 
     """
 
     @abstractmethod
-    def evaluate(self, **kwargs):
+    def evaluate(self, env):
         """
         Abstract method for evaluating an entity.
 
         This method is meant to be overridden by each concrete subclass of Evaluable. The overriding method 
         should implement the specific evaluation semantics of the entity it represents.
 
         Parameters:
@@ -69,237 +114,117 @@
     """
     Abstract base class for all expressions in the maryChain language.
     Inherits from the Evaluable abstract base class.
     """
     pass
 
 class Program(Evaluable):
-    def __init__(self, definitions, imports, expression):
-        self.definitions = definitions
+    def __init__(self, imports, expression):
+
         self.imports = imports
         self.expression = expression
 
-    def evaluate(self):
-        for definition in self.definitions:
-            definition.evaluate()
+    def evaluate(self,env):
 
         for import_stmt in self.imports:
-            import_stmt.evaluate()
+            import_stmt.evaluate(env)
 
         if self.expression:
-            return self.expression.evaluate()
+            return self.expression.evaluate(env)
 
 class Import(Expression):
     def __init__(self, module_parts, alias):
         # self.module_name = '.'.join(module_parts)
         self.module_name = module_parts
         self.alias = alias
 
-    def evaluate(self):
+    def evaluate(self,env):
         add_module_functions_to_dict(self.module_name, self.alias)
 
 
 
-# --------------------------------------------------------------
-#  external functions
-def print_func(x):
-    if isinstance(x, Lazy):
-        x = x.evaluate()
-    print(x)
-    return x
-
-def add_func(x, y):
-    if isinstance(x, Lazy):
-        x = x.evaluate()
-    if isinstance(y, Lazy):
-        y = y.evaluate()
-    return x + y
-
-def eval_func(x):
-    return x.func()
-
-def curry(func):
-    """
-    This function transforms a given function into a curried function.
-    
-    Currying is a technique in functional programming where a function with multiple arguments is 
-    transformed into a sequence of functions, each with a single argument. 
-    For example, a function of two arguments, f(x, y), produces a function of one argument, g(y) = f(x, y), 
-    which can be called with one argument to produce the result.
-
-    Parameters:
-    func (function): The function to be curried.
-
-    Returns:
-    function: The curried version of the original function.
-    """
-    
-    def curried(*args, **kwargs):
-        """
-        This function represents the curried version of the original function.
-        
-        It tries to call the original function with the provided arguments. 
-        If a TypeError occurs because one argument is missing, it returns a new function that 
-        takes one argument and calls the original function with the previously provided arguments 
-        and this new argument.
-        """
-        try:
-            return func(*args, **kwargs)
-        except TypeError as e:
-            if 'missing 1 required positional argument' in str(e):
-                return lambda x: func(*args, x, **kwargs)
-            else:
-                raise e
-
-    return curried  # Return the curried function.
-
-
-# def curry(func):
-#     def curried(*args, **kwargs):
-#         if len(args) + len(kwargs) >= func.__code__.co_argcount:
-#             return func(*args, **kwargs)
-#         else:
-#             # Return a new FunctionDef instance
-#             return FunctionDef(func.__name__, func.__code__.co_varnames[len(args):], curried)
-#     return curried
-
 
 
 # --------------------------------------------------------------
 #  environment
 
-ENVIRONMENT = {}
+ENVIRONMENT = {'👽':'Alessio Ricco'}
 
 # --------------------------------------------------------------
 
-class FunctionDef:
-    """
-    Represents a function definition in the maryChain language. Functions can either be user-defined or 
-    built-in functions.
-    """
-
-    def __init__(self, name, args, body):
-        """
-        Initialize a function definition with a name, a list of argument names, and a body.
-        
-        Parameters:
-        name (str): The name of the function.
-        args (list): The names of the arguments of the function.
-        body (expression): The body of the function which can be an expression or a Python callable 
-                           (for built-in functions).
-        """
-        self.name = name
+class CurriedFunction(Expression):
+    def __init__(self, func, args):
+        self.func = func
         self.args = args
-        self.expected_args = len(args)
 
-        # Check if the body is a function, in which case this is a built-in function
-        if callable(body):
-            self.is_builtin = True
-            self.func = body
-        else:
-            self.is_builtin = False
-            self.body = body
+    def evaluate(self,env):
 
-    def evaluate(self, **kwargs):
-        """
-        Evaluates the function definition by adding it to the global environment and returning itself.
-        
-        Returns:
-        FunctionDef: This function definition.
-        """
-        if len(self.args) == 0:
-            return self.body
-        ENVIRONMENT[self.name] = self
-        return self
+        print(f"evaluate: CurriedFunction f:{self.func} a:{self.args} k:{env}")
 
-    # def __call__(self, *args):
-        """
-        Defines how the function definition behaves when called. If the function is built-in, it simply 
-        calls the function with the provided arguments. Otherwise, it updates the local environment with 
-        the function arguments and evaluates the body of the function in this environment.
-
-        If not all arguments are provided, it returns a new function that takes the remaining arguments.
-
-        Parameters:
-        args (list): The arguments to call the function with.
+        # Apply currying to the function being curried
+        curried_func = curry(self.func.evaluate(env))
 
-        Returns:
-        expression: The result of evaluating the function body.
-        """
-        # if self.is_builtin:
-        #     return self.func(*args)
-        
-        # if len(args) > len(self.args):
-        #     raise TypeError(f"{self.name} takes {len(self.args)} arguments but {len(args)} were given")
+        # Apply the partially applied arguments to the curried function
+        # evaluated_args = [arg.evaluate() for arg in self.args]
+        evaluated_args = []
+        args0 = self.args[0]
+        for arg in args0:
+
+            if isinstance(arg,list) and isinstance(arg[0],Evaluable):
+                evaluated_args.append(arg)
+                continue
+
+            if isinstance(arg,Evaluable):
+                evaluated_args.append(arg)
+                continue
+            
+            evaluated_args.append(arg)
 
-        # # Make a copy of the global environment and update it with the function arguments
-        # local_env = ENVIRONMENT.copy()
-        # local_env.update(zip(self.args, args))
-
-        # if len(args) < len(self.args):
-        #     # Not all arguments provided, return a new function that takes the remaining arguments
-        #     remaining_args = self.args[len(args):]
-        #     return curry(FunctionDef(self.name, remaining_args, self.body).evaluate(local_env))
-
-        # # Evaluate the body of the function in the local environment and return the result
-        # return self.body.evaluate(local_env)
-
-    def __call__(self,*args):
-        if self.is_builtin:
-            return curry(self.func)(*args)
-        if len(args)>len(self.args):
-            raise TypeError(f"{self.name} takes {len(self.args)} arguments but {len(args)} were given")
-        local_env=ENVIRONMENT.copy()
-        local_env.update(zip(self.args,args))
-        if len(args)<len(self.args):
-            remaining_args=self.args[len(args):]
-            return curry(FunctionDef(self.name,remaining_args,self.body).evaluate(local_env))
-        return self.body.evaluate(local_env)
+        return curried_func(*evaluated_args)
 
 class FunctionCall(Expression):
     def __init__(self, func, args):
         self.func = func
         self.args = args
 
-    def evaluate(self, **kwargs):
-        func = None
-        if isinstance(self.func, Identifier):
-            # Look up function by name
-            name = self.func.name
-            if self.func.name in ENVIRONMENT:
-                func = ENVIRONMENT[self.func.name]
-            else:
-                # namespace
-                if "." in name:  # Check if func is a qualified function name
-                    module_name, func_name = name.split(".")
-                    if (module_name not in FUNCTION_DICT) or (func_name not in FUNCTION_DICT[module_name]):
-                        raise ValueError(f"Function {self.func} is not defined")
-                    func = FUNCTION_DICT[module_name][func_name]
+    '''function_call : function_call LPAREN args RPAREN
+                     | function_call LPAREN RPAREN
+                     | IDENTIFIER'''
+
+    def evaluate(self,env):
+            print(f"evaluate: FunctionCall f:{self.func} a:{self.args} k:{env}")
+            func = None
+
+            # Check if it's a curried function
+            if isinstance(self.func, CurriedFunction):
+                func = self.func
+
+            # Check if it's an Identifier
+            elif isinstance(self.func, Identifier):
+                ident = self.func.evaluate()
+                if isinstance(ident, CurriedFunction):
+                    func = ident
+                elif isinstance(ident, FunctionCall):
+                    func = ident
                 else:
-                    func = FUNCTION_DICT[self.func.name]
-        elif isinstance(self.func, FunctionCall):
-            # Evaluate inner function call to get function
-            func = self.func.evaluate()
-        else:
-            raise ValueError(f"Function {self.func} is not defined")
+                    raise ValueError(f"Identifier {self.func.name} is not a function or lambda")
 
-        if func.is_builtin:
-            # If the function is a built-in function, call it with the provided arguments
-            # This will raise an exception if there are too few arguments
-            evaluated_args = [arg.evaluate() for arg in self.args]
-            return func(*evaluated_args)
-        else:
-            # If the function is a user-defined function and there are too few arguments, return a new FunctionDef for currying
-            if len(self.args) < func.expected_args:
-                return FunctionDef(func.name, func.args[len(self.args):], func.body)
-
-            # If there are enough arguments, evaluate the function call as normal
-            evaluated_args = [arg.evaluate() for arg in self.args]
-            return func(*evaluated_args)
+            # Check if it's a regular FunctionCall
+            elif isinstance(self.func, FunctionCall):
+                func = self.func
+            elif isinstance(self.func, LambdaFunction):
+                func = self.func
+                evaluated_args = [arg.evaluate(env) for arg in self.args]
+                return func.evaluate(env).evaluate(env,*evaluated_args)
+            
+            if func:
+                evaluated_args = [arg.evaluate(env) for arg in self.args]
+                return func.evaluate(*evaluated_args)
 
+            raise ValueError("Invalid function call")
 
 class LetIn(Expression):
     """
     This class represents a "let-in" expression in the maryChain language. A let-in expression
     is used to bind a value to an identifier in a certain scope. The syntax is as follows:
 
         let <identifier> = <expression> in <body>
@@ -318,39 +243,50 @@
                 to bind to the identifier.
             body: The body of the let-in expression, where the identifier is bound to the value.
         """
         self.identifier = identifier
         self.value_expression = value_expression
         self.body = body
 
-    def evaluate(self):
+    def evaluate(self,env):
         """
         Evaluates the let-in expression.
 
         This is done by first evaluating the value expression, then creating a new scope where the 
         identifier is bound to the value. The body of the let-in expression is then evaluated in this new 
         scope. Finally, the old scope is restored.
 
         Returns:
             The result of evaluating the body of the let-in expression.
         """
         # Evaluate the value expression and create a new scope where the identifier is bound to the value.
-        value = self.value_expression.evaluate()
-        new_env = ENVIRONMENT.copy()
+        value = self.value_expression.evaluate(env)
+        # new_env = ENVIRONMENT.copy()
+        new_env = env.copy()
         new_env[self.identifier] = value
 
         # Evaluate the body in the new scope.
-        old_env = ENVIRONMENT
-        ENVIRONMENT = new_env
+        # old_env = ENVIRONMENT
+        # ENVIRONMENT = new_env
         try:
-            return self.body.evaluate()
+            return self.body.evaluate(new_env)
         finally:
-            ENVIRONMENT = old_env  # Restore the old environment
+            pass
+            # ENVIRONMENT = old_env  # Restore the old environment
 
+class Assignment(Expression):
+    def __init__(self, identifier, value_expression):
+        self.identifier = identifier
+        self.value_expression = value_expression
 
+    def evaluate(self,env):
+        value = self.value_expression.evaluate(env)
+        # new_env = env.copy()
+        env[self.identifier] = value
+        return value
 
 class BinOp(Expression):
     """
     This class represents a binary operation in the maryChain language. A binary operation is 
     an operation that takes two operands and performs a specified operation on them.
 
     The supported operators are:
@@ -377,50 +313,50 @@
             op: The operator of the binary operation.
             right: The right operand of the binary operation.
         """
         self.left = left
         self.op = op
         self.right = right
 
-    def evaluate(self, **kwargs):
+    def evaluate(self, env):
         """
         Evaluates the binary operation and returns the result.
 
         This is done by first evaluating the left and right operands, then applying the operator to the results.
 
         Returns:
             The result of the binary operation.
 
         Raises:
             ValueError: If the operator is not supported.
         """
         if self.op == '+':
-            return evaluate(self.left) + evaluate(self.right)
+            return evaluate(self.left,env) + evaluate(self.right,env)
         if self.op == '-':
-            return evaluate(self.left) - evaluate(self.right)
+            return evaluate(self.left,env) - evaluate(self.right,env)
         if self.op == '*':
-            return evaluate(self.left) * evaluate(self.right)
+            return evaluate(self.left,env) * evaluate(self.right,env)
         if self.op == '/':
-            return evaluate(self.left) / evaluate(self.right)
+            return evaluate(self.left,env) / evaluate(self.right,env)
         if self.op == '&&':
-            return evaluate(self.left) and evaluate(self.right)
+            return evaluate(self.left,env) and evaluate(self.right,env)
         if self.op == '||':
-            return evaluate(self.left) or evaluate(self.right) 
+            return evaluate(self.left,env) or evaluate(self.right,env) 
         if self.op == '->':
-            return not evaluate(self.left) or evaluate(self.right)
+            return not evaluate(self.left,env) or evaluate(self.right,env)
         if self.op == '>':
-            return evaluate(self.left) > evaluate(self.right) 
+            return evaluate(self.left,env) > evaluate(self.right,env) 
         if self.op == '<':
-            return evaluate(self.left) < evaluate(self.right)    
+            return evaluate(self.left,env) < evaluate(self.right,env)    
         if self.op == '>=':
-            return evaluate(self.left) >= evaluate(self.right)   
+            return evaluate(self.left,env) >= evaluate(self.right,env)   
         if self.op == '<=':
-            return evaluate(self.left) <= evaluate(self.right) 
+            return evaluate(self.left,env) <= evaluate(self.right,env) 
         if self.op == '==':
-            return evaluate(self.left) == evaluate(self.right) 
+            return evaluate(self.left,env) == evaluate(self.right,env) 
         raise ValueError(f'Unknown operator: {self.operator}')
 
 
 class Number(Expression):
     """
     This class represents a numeric literal in the maryChain language. 
 
@@ -439,15 +375,15 @@
         """
         self.value = value
         try:
             self.value = int(value)
         except ValueError:
             self.value = float(value)
 
-    def evaluate(self, **kwargs):
+    def evaluate(self,env):
         """
         Evaluates the number, which in practice means returning the numeric value.
 
         Returns:
             The numeric value of the Number instance.
         """
         return self.value
@@ -465,15 +401,15 @@
         Initializes a new instance of the String class.
 
         Args:
             value: The string value represented by the instance.
         """
         self.value = value
 
-    def evaluate(self, **kwargs):
+    def evaluate(self,env):
         """
         Evaluates the string, which in practice means returning the string value.
 
         Returns:
             The string value of the String instance.
         """
         return self.value
@@ -491,15 +427,15 @@
         Initializes a new instance of the Boolean class.
 
         Args:
             value: The boolean value represented by the instance.
         """
         self.value = bool(value)
 
-    def evaluate(self, **kwargs):
+    def evaluate(self,env):
         """
         Evaluates the boolean, which in practice means returning the boolean value.
 
         Returns:
             The boolean value of the Boolean instance.
         """
         return self.value
@@ -518,32 +454,43 @@
         Initializes a new instance of the Identifier class.
 
         Args:
             name: The name of the variable or function this identifier refers to.
         """
         self.name = name
 
-    def evaluate(self, **kwargs):
+    def evaluate(self, env):
         """
         Evaluates the Identifier. If the identifier name is in the environment, its value is returned. 
         If the name corresponds to a function in the function dictionary, the name is returned. 
         If the name is an instance of a function call, it is evaluated.
 
         Returns:
             The value of the Identifier if it exists in the environment, its name if it exists in the function dictionary,
             or the result of its evaluation if it is a FunctionCall.
         """
-        if self.name in ENVIRONMENT:
-            return ENVIRONMENT[self.name]
-        if self.name in FUNCTION_DICT:
-            return self.name
-        if isinstance(self.name, FunctionCall):
-            return self.name.evaluate()
-        return None
 
+        name = self.name
+
+        if self.name in env:
+            return env[self.name]
+        elif self.name in ENVIRONMENT:
+            return ENVIRONMENT[self.name]
+        elif self.name in FUNCTION_DICT:
+            return FUNCTION_DICT[self.name]
+        
+        if "." in name:  # Check if func is a qualified function name
+            module_name, func_name = name.split(".")
+            if (module_name not in FUNCTION_DICT) or (func_name not in FUNCTION_DICT[module_name]):
+                raise ValueError(f"Function {self.func} is not defined")
+            return FUNCTION_DICT[module_name][func_name]
+
+        # if isinstance(self.name, FunctionCall):
+        #     return self.name.evaluate()
+        return name
 
 class UnaryOperation(Expression):
     """
     This class represents a unary operation in the maryChain language. 
 
     The `UnaryOperation` class inherits from the `Expression` class and encapsulates an operator and 
     an operand for operations such as unary minus and logical not.
@@ -556,15 +503,15 @@
         Args:
             operator: The operator of the unary operation. It could be '-' for unary minus or 'not' for logical not.
             operand: The operand on which the unary operation is to be performed.
         """
         self.operator = operator
         self.operand = operand
 
-    def evaluate(self, **kwargs):
+    def evaluate(self,env):
         """
         Evaluates the UnaryOperation. If the operator is '-', the negation of the operand is returned.
         If the operator is 'not', the logical not of the operand is returned.
 
         Returns:
             The result of the unary operation on the operand.
 
@@ -593,33 +540,39 @@
             condition: The condition of the while loop. It should be an expression that evaluates to a boolean.
             body: The body of the while loop. It's a sequence of expressions that will be executed 
                   as long as the condition is True.
         """
         self.condition = condition
         self.body = body
 
-    def evaluate(self, **kwargs):
+    def evaluate(self,env):
         """
         Evaluates the While loop. The condition is checked before each iteration. 
         If the condition is True, the body is executed, otherwise the loop is exited.
 
         Returns:
             The result of the last expression evaluated in the body of the loop.
 
         Raises:
             None
         """
-        result = self.condition.evaluate()
-        while result != False:
-            result = self.body.evaluate()
-            if self.condition.evaluate() == False:
-                break
-        return result
+        # result = self.condition.evaluate(env)
+        # while result != False:
+        #     result = self.body.evaluate(env)
+        #     if self.condition.evaluate(env) == False:
+        #         break
+        b_result = None
+        c_result = self.condition.evaluate(env)
+        while c_result:
+            b_result = self.body.evaluate(env)
+            c_result = self.condition.evaluate(env)
+            # if self.condition.evaluate(env) == False:
+            #     break
+        return b_result
 
-    
 class IfThenElse(Expression):
     """
     This class represents a conditional "if-then-else" statement in the maryChain language.
 
     The `IfThenElse` class inherits from the `Expression` class and encapsulates a condition,
     an expression to evaluate if the condition is true, and another expression to evaluate if
     the condition is false.
@@ -634,15 +587,15 @@
             true_expr: The expression that will be evaluated if the condition is true.
             false_expr: The expression that will be evaluated if the condition is false.
         """
         self.condition = condition
         self.true_expr = true_expr
         self.false_expr = false_expr
 
-    def evaluate(self, **kwargs):
+    def evaluate(self,env):
         """
         Evaluates the IfThenElse statement. 
 
         The condition is evaluated first. If the condition is True, the true_expr is evaluated and its 
         result is returned. If the condition is False, the false_expr is evaluated and its result is returned.
 
         Returns:
@@ -653,15 +606,14 @@
             None
         """
         if evaluate(self.condition):
             return evaluate(self.true_expr)
         else:
             return evaluate(self.false_expr)
 
-        
 class IfThen(Expression):
     """
     The IfThen class represents a conditional expression in a programming language. 
     It contains a condition and an expression that gets evaluated if the condition is true.
     """
 
     def __init__(self, condition, true_expr):
@@ -670,36 +622,34 @@
 
         :param condition: The condition of the 'if' statement.
         :param true_expr: The expression to be evaluated if the condition is true.
         """
         self.condition = condition
         self.true_expr = true_expr
 
-    def evaluate(self, **kwargs):
+    def evaluate(self,env):
         """
         Evaluate the IfThen expression. If the condition is true, evaluate and return the true expression. 
         If the condition is false, return the last evaluated result in the environment. 
         If there is no last result in the environment, return None.
 
         :return: Result of evaluating the true expression if the condition is true, 
                  or the last result in the environment if the condition is false.
         """
         # Evaluate the condition
-        if self.condition.evaluate():
+        if self.condition.evaluate(env):
             # If the condition is true, evaluate and return the true expression
-            return self.true_expr.evaluate()
-        elif '%lastresult%' in ENVIRONMENT:
-            # If the condition is false, return the last evaluated result in the environment
-            return ENVIRONMENT['%lastresult%']
+            return self.true_expr.evaluate(env)
+        # elif '%lastresult%' in ENVIRONMENT:
+        #     # If the condition is false, return the last evaluated result in the environment
+        #     return ENVIRONMENT['%lastresult%']
         else:
             # If there is no last result in the environment, return None
             return None  
 
-
-
 class Lazy(Expression):
     """
     The Lazy class represents a lazy evaluation of an expression in a programming language. 
     It contains a function and its evaluated state and value.
     """
 
     def __init__(self, func):
@@ -708,15 +658,15 @@
 
         :param func: The function to be evaluated.
         """
         self.func = func
         self.is_evaluated = False  # Indicates if the function has been evaluated
         self.value = None  # Holds the result of the evaluation
 
-    def evaluate(self, **kwargs):
+    def evaluate(self,env):
         """
         Evaluate the Lazy expression if it hasn't been evaluated before. 
         The result is cached for future uses.
 
         :return: Result of evaluating the function.
         """
         # If the function hasn't been evaluated before
@@ -741,15 +691,14 @@
         # If the function has been evaluated
         if self.is_evaluated:
             return f"<Evaluated lazy object with value: {self.value}>"
         else:
             # If the function hasn't been evaluated
             return "<Unevaluated lazy object>"
 
-
 class Pipe(Expression):
     """
     The Pipe class represents a pipeline operation in a programming language.
     A pipeline operation is one where the result of one operation (left) is used as the input to another operation (right).
     """
 
     def __init__(self, left, right):
@@ -758,30 +707,57 @@
 
         :param left: The left expression to be evaluated first.
         :param right: The right expression that takes the result of the left expression as an argument.
         """
         self.left = left
         self.right = right
 
-    def evaluate(self, **kwargs):
+    def evaluate(self,env):
         """
         Evaluate the Pipe expression. 
         The left expression is evaluated first and its result is fed as an argument to the right expression.
 
         :return: Result of evaluating the right expression with the result of the left expression.
         """
         # Evaluate the left expression and store its result in a special variable '%lastresult%'
-        ENVIRONMENT['%lastresult%'] = self.left.evaluate()
+        # ENVIRONMENT['%lastresult%'] = self.left.evaluate()
 
         # Insert the result of the left expression as the first argument of the right expression
-        self.right.args.insert(0, self.left)
-
+        func = None
+        if isinstance(self.right,FunctionCall):
+            func = self.right
+            func.args.insert(0, self.left)
+            return func.evaluate(env)
+            # return l.evaluate(*func.args)
+        
+        if isinstance(self.right,Identifier):  
+            name = self.right.name  
+            if isinstance(name,str) and name in ENVIRONMENT:
+                if isinstance(ENVIRONMENT[name],FunctionCall):
+                    func = ENVIRONMENT[name]
+                    func.args.insert(0, self.left)
+                    l = func.evaluate(env)
+                    return l.evaluate(*func.args)
+
+            elif isinstance(name,str) and name in FUNCTION_DICT:
+                func = FUNCTION_DICT[name]
+                if isinstance(func,LambdaFunction):        
+                    l = func.evaluate(env)
+                    return l.evaluate(self.left)
+                elif callable(func):
+                    return func(self.left.evaluate(env))
+                
+        if isinstance(self.right,CurriedFunction):
+            # function = self.right.func
+            # args = self.right.args
+            self.right.args[0].insert(0, self.left)
+            return self.right.evaluate(env)
+                        
         # Evaluate the right expression and return the result
-        return self.right.evaluate()
-
+        return self.right.evaluate(env)
 
 class LambdaFunctionValue(Expression):
     """
     The LambdaFunctionValue class represents a lambda function in a programming language.
     A lambda function is a small anonymous function that can take any number of arguments but can have only one expression.
     """
 
@@ -791,34 +767,51 @@
 
         :param args: The arguments that the lambda function accepts.
         :param body: The expression that forms the body of the lambda function.
         """
         self.args = args
         self.body = body
 
-    def __call__(self, *args):
+    def evaluate(self, env, *args):
         """
         Define the behavior of the LambdaFunctionValue instance when it's 'called' like a function.
         If the number of arguments provided during the call doesn't match the lambda function's arguments,
         a TypeError is raised.
 
         :param args: The arguments provided during the function call.
         :return: Result of evaluating the lambda function's body with the provided arguments.
         """
+
+        print(f"evaluate: LambdaFunctionValue f:{self.body} a:{self.args} k:{args}")
+
         # Check if the number of arguments provided during the call matches the number of arguments the function accepts
-        if len(args) != len(self.args):
+        # if len(args) != len(self.args):
+        #     raise TypeError("wrong number of arguments")
+        if len(args) > len(self.args):
             raise TypeError("wrong number of arguments")
-
+        
         # Create a local environment where the arguments are bound to their values
         local_env = ENVIRONMENT.copy()
-        local_env.update(zip(self.args, args))
+        local_env.update(zip([arg.evaluate(env) for arg in self.args], args))
 
-        # Evaluate the function's body in the local environment and return the result
-        return self.body.evaluate(local_env)
+        body = self.body
+        local_args = []
+        if callable(body):
+            for arg in args:
+                value = arg
+                if isinstance(value,Evaluable):
+                    value = arg.evaluate(local_env)
+                local_args.append(value)
+            return body(*local_args)
 
+        # Evaluate the function's body in the local environment and return the result
+        return body.evaluate(local_env)
+    
+    # def evaluate(self):
+    #     pass
 
 
 class LambdaFunction(Expression):
     """
     The LambdaFunction class represents a lambda function definition in a programming language. 
     This class is used to create a lambda function object (LambdaFunctionValue) when evaluated.
     """
@@ -829,48 +822,60 @@
 
         :param args: The arguments that the lambda function accepts.
         :param body: The expression that forms the body of the lambda function.
         """
         self.args = args
         self.body = body
 
-    def evaluate(self):
+    def evaluate(self,env):
         """
         Evaluate the lambda function to a LambdaFunctionValue object which can be called like a function.
 
         :return: A LambdaFunctionValue object that represents the lambda function.
         """
+        print(f"evaluate: LambdaFunction f:{self.body} a:{self.args} ")
         return LambdaFunctionValue(self.args, self.body)
 
+def out_func(x):
+    if isinstance(x, Lazy):
+        x = x.evaluate()
+    print(x)
+    return x
+
+def add_func(x, y):
+    if isinstance(x, Lazy):
+        x = x.evaluate()
+    if isinstance(y, Lazy):
+        y = y.evaluate()
+    return x + y
+
+# def eval_func(x):
+#     return x.func()
 
 FUNCTION_DICT = {
     # This dictionary maps function names to FunctionDef instances that implement the function.
 
     # The 'out' function prints its argument and returns None. 
     # It's implemented with the 'print_func' function and curried to allow partial application.
-    'out': FunctionDef('out', ['x'], curry(print_func)),
+    'out': (out_func),
 
     # The 'add' function adds its two arguments. 
     # It's implemented with the 'add_func' function and curried to allow partial application.
-    'add': FunctionDef('add', ['x', 'y'], curry(add_func)),
+    'add': (add_func),
 
     # The 'eval' function evaluates its argument as a maryChain expression. 
     # It's implemented with the 'eval_func' function and curried to allow partial application.
-    'eval': FunctionDef('eval', ['x'], curry(eval_func)),
+    # 'eval': (eval_func),
 }
 
-# def exec(s):
-#     node = None
-#     return evaluate(node)
-
 def inject_parsing(parse):
-    FUNCTION_DICT['exec'] = FunctionDef('exec', ['s'], curry(lambda x: evaluate(parse(x))))
+    FUNCTION_DICT['exec'] = (lambda x: evaluate(parse(x)))
     return 
 
-def evaluate(node):
+def evaluate(node, env=ENVIRONMENT):
     """
     The evaluate function is used to evaluate different types of nodes in an abstract syntax tree (AST).
     It returns the evaluated result of the node.
 
     :param node: A node in the AST. The node could be a string, integer, float, or an instance of Expression class.
     :return: The evaluated result of the node.
     """
@@ -887,13 +892,11 @@
     
     if isinstance(node, float):
         # If the node is a float, return the float itself
         return node
     
     if isinstance(node, Evaluable):
         # If the node is an instance of Expression class, evaluate the expression and return the result
-        return node.evaluate()
+        return node.evaluate(env)
     
     # If the node is none of the above types, raise a ValueError
     raise ValueError(f'Unknown node type: {node}')
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `maryChain-0.0.2/maryChain/parsetab.py` & `maryChain-0.0.3/maryChain/parsetab.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,71 +2,70 @@
 # parsetab.py
 # This file is automatically generated. Do not edit.
 # pylint: disable=W,C,R
 _tabversion = '3.10'
 
 _lr_method = 'LALR'
 
-_lr_signature = 'leftPIPEleftORleftANDleftNOTleftEQUALITYGREATERLESSGREATEREQUALLESSEQUALleftPLUSMINUSleftTIMESDIVIDErightUMINUSAND AS BOOLEAN BOOLEANCAST CATCH COMMA DEF DIVIDE DO DOT DOUBLECAST ELSE EMPTY EQUALITY EQUALS FALSE FINALLY FOREACH FUNC GREATER GREATEREQUAL HEAD IDENTIFIER IF IMPLIES IMPORT IN INTEGERCAST LAMBDA LAZY LBRACK LCBRACE LEN LESS LESSEQUAL LET LPAREN MINUS NAMESPACE_OP NOT NULL NUMBER OR PIPE PLUS RBRACK RCBRACE RPAREN STRING STRINGCAST TAIL THEN TIMES TRUE TRY WHILEprogram : definitions imports expression\n               | imports expression\n               | definitions expression\n               | imports\n               | definitions\n               | expressionexpression : LET IDENTIFIER EQUALS expression IN expressionexpression : expression PLUS expression\n                  | expression MINUS expression\n                  | expression TIMES expression\n                  | expression DIVIDE expressionnamespace : IDENTIFIER\n                 | namespace DOT IDENTIFIERimport : IMPORT IDENTIFIER AS IDENTIFIER\n    imports : import\n            | imports import\n    expression : MINUS expression %prec UMINUSexpression : LPAREN expression RPARENterm : factorfactor : STRINGfactor : NUMBERfactor : TRUE\n              | FALSEexpression : WHILE expression DO expressionexpression : IF expression THEN expression ELSE expressionexpression : IF expression THEN expressionexpression : LAZY expressionexpression : LCBRACE expression RCBRACEexpression : LAMBDA LPAREN args RPAREN expressionexpression : expression PIPE expressionexpression : function_callexpression : termfunction_definition : FUNC IDENTIFIER LPAREN args RPAREN LCBRACE expression RCBRACE\n    definitions : function_definition\n                | definitions function_definition\n    function_call : function_call LPAREN args RPAREN\n                     | IDENTIFIER LPAREN args RPAREN\n                     | IDENTIFIERargs : args COMMA arg\n            | arg\n            | arg : expression'
+_lr_signature = 'leftPIPEleftORleftANDleftNOTnonassocEQUALITYGREATERLESSGREATEREQUALLESSEQUALrightUMINUSleftPLUSMINUSleftTIMESDIVIDEAND AS BOOLEAN BOOLEANCAST CATCH COMMA DEF DIVIDE DO DOT DOUBLECAST ELSE EMPTY EQUALITY EQUALS FALSE FINALLY FOREACH FUNC GREATER GREATEREQUAL HEAD IDENTIFIER IF IMPLIES IMPORT IN INTEGERCAST LAMBDA LAZY LBRACK LCBRACE LEN LESS LESSEQUAL LET LPAREN MINUS NAMESPACE_OP NOT NULL NUMBER OR PIPE PLUS RBRACK RCBRACE RPAREN STRING STRINGCAST TAIL THEN TIMES TRUE TRY WHILEprogram : imports expression\n               | expressionimport : IMPORT IDENTIFIER AS IDENTIFIER\n    imports : import\n            | imports import\n    expression : IDENTIFIER EQUALS expressionexpression : LET IDENTIFIER EQUALS expression IN expressionexpression : expression PLUS expression\n                  | expression MINUS expression\n                  | expression TIMES expression\n                  | expression EQUALITY expression\n                  | expression GREATER expression\n                  | expression LESS expression\n                  | expression GREATEREQUAL expression\n                  | expression LESSEQUAL expression\n                  | expression DIVIDE expressionexpression : MINUS expression %prec UMINUSexpression : LPAREN expression RPARENterm : factorfactor : STRINGfactor : NUMBERfactor : TRUE\n              | FALSEexpression : WHILE expression DO expressionexpression : IF expression THEN expression ELSE expressionexpression : IF expression THEN expressionexpression : LAZY expressionterm : LCBRACE term RCBRACElambda : LAMBDA LPAREN args RPAREN expressionexpression : expression PIPE expressionexpression : function_call \n                  | lambdaexpression : termfunction_call : function_call LPAREN args RPAREN\n                     | function_call LPAREN RPAREN\n                     | lambda LPAREN args RPAREN\n                     | IDENTIFIERargs : args COMMA arg\n            | arg\n            | arg : expression'
     
-_lr_action_items = {'LET':([0,2,3,5,6,9,10,11,12,13,14,25,27,29,30,31,32,33,34,36,43,44,53,58,59,63,67,70,73,74,76,81,83,],[7,7,7,-34,-15,7,7,7,7,7,7,7,-35,-16,7,7,7,7,7,7,7,7,7,7,7,7,7,7,-14,7,7,7,-33,]),'MINUS':([0,2,3,4,5,6,8,9,10,11,12,13,14,16,17,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,36,37,38,39,40,41,42,43,44,47,48,49,50,51,52,53,56,57,58,59,60,63,65,66,67,68,69,70,71,73,74,76,77,79,80,81,82,83,],[9,9,9,31,-34,-15,-38,9,9,9,9,9,9,-31,-32,-19,-20,-21,-22,-23,9,31,-35,31,-16,9,9,9,9,9,9,-17,31,31,31,31,31,9,9,31,-8,-9,-10,-11,31,9,31,-18,9,9,-28,9,31,-37,9,31,31,9,-36,-14,9,9,31,31,31,9,31,-33,]),'LPAREN':([0,2,3,5,6,8,9,10,11,12,13,14,15,16,25,27,29,30,31,32,33,34,36,43,44,45,53,58,59,63,66,67,70,71,73,74,76,81,83,],[10,10,10,-34,-15,36,10,10,10,10,10,10,43,44,10,-35,-16,10,10,10,10,10,10,10,10,63,10,10,10,10,-37,10,10,-36,-14,10,10,10,-33,]),'WHILE':([0,2,3,5,6,9,10,11,12,13,14,25,27,29,30,31,32,33,34,36,43,44,53,58,59,63,67,70,73,74,76,81,83,],[11,11,11,-34,-15,11,11,11,11,11,11,11,-35,-16,11,11,11,11,11,11,11,11,11,11,11,11,11,11,-14,11,11,11,-33,]),'IF':([0,2,3,5,6,9,10,11,12,13,14,25,27,29,30,31,32,33,34,36,43,44,53,58,59,63,67,70,73,74,76,81,83,],[12,12,12,-34,-15,12,12,12,12,12,12,12,-35,-16,12,12,12,12,12,12,12,12,12,12,12,12,12,12,-14,12,12,12,-33,]),'LAZY':([0,2,3,5,6,9,10,11,12,13,14,25,27,29,30,31,32,33,34,36,43,44,53,58,59,63,67,70,73,74,76,81,83,],[13,13,13,-34,-15,13,13,13,13,13,13,13,-35,-16,13,13,13,13,13,13,13,13,13,13,13,13,13,13,-14,13,13,13,-33,]),'LCBRACE':([0,2,3,5,6,9,10,11,12,13,14,25,27,29,30,31,32,33,34,36,43,44,53,58,59,63,67,70,73,74,76,78,81,83,],[14,14,14,-34,-15,14,14,14,14,14,14,14,-35,-16,14,14,14,14,14,14,14,14,14,14,14,14,14,14,-14,14,14,81,14,-33,]),'LAMBDA':([0,2,3,5,6,9,10,11,12,13,14,25,27,29,30,31,32,33,34,36,43,44,53,58,59,63,67,70,73,74,76,81,83,],[15,15,15,-34,-15,15,15,15,15,15,15,15,-35,-16,15,15,15,15,15,15,15,15,15,15,15,15,15,15,-14,15,15,15,-33,]),'FUNC':([0,2,5,27,83,],[18,18,-34,-35,-33,]),'IMPORT':([0,2,3,5,6,25,27,29,73,83,],[19,19,19,-34,-15,19,-35,-16,-14,-33,]),'IDENTIFIER':([0,2,3,5,6,7,9,10,11,12,13,14,18,19,25,27,29,30,31,32,33,34,36,43,44,53,58,59,63,64,67,70,73,74,76,81,83,],[8,8,8,-34,-15,35,8,8,8,8,8,8,45,46,8,-35,-16,8,8,8,8,8,8,8,8,8,8,8,8,73,8,8,-14,8,8,8,-33,]),'STRING':([0,2,3,5,6,9,10,11,12,13,14,25,27,29,30,31,32,33,34,36,43,44,53,58,59,63,67,70,73,74,76,81,83,],[21,21,21,-34,-15,21,21,21,21,21,21,21,-35,-16,21,21,21,21,21,21,21,21,21,21,21,21,21,21,-14,21,21,21,-33,]),'NUMBER':([0,2,3,5,6,9,10,11,12,13,14,25,27,29,30,31,32,33,34,36,43,44,53,58,59,63,67,70,73,74,76,81,83,],[22,22,22,-34,-15,22,22,22,22,22,22,22,-35,-16,22,22,22,22,22,22,22,22,22,22,22,22,22,22,-14,22,22,22,-33,]),'TRUE':([0,2,3,5,6,9,10,11,12,13,14,25,27,29,30,31,32,33,34,36,43,44,53,58,59,63,67,70,73,74,76,81,83,],[23,23,23,-34,-15,23,23,23,23,23,23,23,-35,-16,23,23,23,23,23,23,23,23,23,23,23,23,23,23,-14,23,23,23,-33,]),'FALSE':([0,2,3,5,6,9,10,11,12,13,14,25,27,29,30,31,32,33,34,36,43,44,53,58,59,63,67,70,73,74,76,81,83,],[24,24,24,-34,-15,24,24,24,24,24,24,24,-35,-16,24,24,24,24,24,24,24,24,24,24,24,24,24,24,-14,24,24,24,-33,]),'$end':([1,2,3,4,5,6,8,16,17,20,21,22,23,24,26,27,28,29,37,41,47,48,49,50,51,52,57,60,66,68,69,71,73,77,79,80,83,],[0,-5,-4,-6,-34,-15,-38,-31,-32,-19,-20,-21,-22,-23,-3,-35,-2,-16,-17,-27,-1,-8,-9,-10,-11,-30,-18,-28,-37,-24,-26,-36,-14,-29,-7,-25,-33,]),'PLUS':([4,8,16,17,20,21,22,23,24,26,28,37,38,39,40,41,42,47,48,49,50,51,52,56,57,60,65,66,68,69,71,77,79,80,82,],[30,-38,-31,-32,-19,-20,-21,-22,-23,30,30,-17,30,30,30,30,30,30,-8,-9,-10,-11,30,30,-18,-28,30,-37,30,30,-36,30,30,30,30,]),'TIMES':([4,8,16,17,20,21,22,23,24,26,28,37,38,39,40,41,42,47,48,49,50,51,52,56,57,60,65,66,68,69,71,77,79,80,82,],[32,-38,-31,-32,-19,-20,-21,-22,-23,32,32,-17,32,32,32,32,32,32,32,32,-10,-11,32,32,-18,-28,32,-37,32,32,-36,32,32,32,32,]),'DIVIDE':([4,8,16,17,20,21,22,23,24,26,28,37,38,39,40,41,42,47,48,49,50,51,52,56,57,60,65,66,68,69,71,77,79,80,82,],[33,-38,-31,-32,-19,-20,-21,-22,-23,33,33,-17,33,33,33,33,33,33,33,33,-10,-11,33,33,-18,-28,33,-37,33,33,-36,33,33,33,33,]),'PIPE':([4,8,16,17,20,21,22,23,24,26,28,37,38,39,40,41,42,47,48,49,50,51,52,56,57,60,65,66,68,69,71,77,79,80,82,],[34,-38,-31,-32,-19,-20,-21,-22,-23,34,34,-17,34,34,34,34,34,34,-8,-9,-10,-11,-30,34,-18,-28,34,-37,34,34,-36,34,34,34,34,]),'RPAREN':([8,16,17,20,21,22,23,24,36,37,38,41,43,44,48,49,50,51,52,54,55,56,57,60,61,62,63,66,68,69,71,72,75,77,79,80,],[-38,-31,-32,-19,-20,-21,-22,-23,-41,-17,57,-27,-41,-41,-8,-9,-10,-11,-30,66,-40,-42,-18,-28,70,71,-41,-37,-24,-26,-36,78,-39,-29,-7,-25,]),'DO':([8,16,17,20,21,22,23,24,37,39,41,48,49,50,51,52,57,60,66,68,69,71,77,79,80,],[-38,-31,-32,-19,-20,-21,-22,-23,-17,58,-27,-8,-9,-10,-11,-30,-18,-28,-37,-24,-26,-36,-29,-7,-25,]),'THEN':([8,16,17,20,21,22,23,24,37,40,41,48,49,50,51,52,57,60,66,68,69,71,77,79,80,],[-38,-31,-32,-19,-20,-21,-22,-23,-17,59,-27,-8,-9,-10,-11,-30,-18,-28,-37,-24,-26,-36,-29,-7,-25,]),'RCBRACE':([8,16,17,20,21,22,23,24,37,41,42,48,49,50,51,52,57,60,66,68,69,71,77,79,80,82,],[-38,-31,-32,-19,-20,-21,-22,-23,-17,-27,60,-8,-9,-10,-11,-30,-18,-28,-37,-24,-26,-36,-29,-7,-25,83,]),'COMMA':([8,16,17,20,21,22,23,24,36,37,41,43,44,48,49,50,51,52,54,55,56,57,60,61,62,63,66,68,69,71,72,75,77,79,80,],[-38,-31,-32,-19,-20,-21,-22,-23,-41,-17,-27,-41,-41,-8,-9,-10,-11,-30,67,-40,-42,-18,-28,67,67,-41,-37,-24,-26,-36,67,-39,-29,-7,-25,]),'IN':([8,16,17,20,21,22,23,24,37,41,48,49,50,51,52,57,60,65,66,68,69,71,77,79,80,],[-38,-31,-32,-19,-20,-21,-22,-23,-17,-27,-8,-9,-10,-11,-30,-18,-28,74,-37,-24,-26,-36,-29,-7,-25,]),'ELSE':([8,16,17,20,21,22,23,24,37,41,48,49,50,51,52,57,60,66,68,69,71,77,79,80,],[-38,-31,-32,-19,-20,-21,-22,-23,-17,-27,-8,-9,-10,-11,-30,-18,-28,-37,-24,76,-36,-29,-7,-25,]),'EQUALS':([35,],[53,]),'AS':([46,],[64,]),}
+_lr_action_items = {'IDENTIFIER':([0,2,4,6,7,8,9,10,11,15,24,25,26,27,28,29,30,31,32,33,34,35,42,43,45,58,60,61,67,74,76,77,78,79,],[5,5,-4,36,5,5,5,5,5,44,-5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,76,5,-3,5,5,5,]),'LET':([0,2,4,7,8,9,10,11,24,25,26,27,28,29,30,31,32,33,34,35,42,43,45,58,60,61,74,76,77,78,79,],[6,6,-4,6,6,6,6,6,-5,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,-3,6,6,6,]),'MINUS':([0,2,3,4,5,7,8,9,10,11,12,13,14,17,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,37,38,39,40,41,42,43,45,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,63,65,69,70,71,72,73,74,75,76,77,78,79,81,82,83,],[7,7,26,-4,-37,7,7,7,7,7,-31,-32,-33,-19,-20,-21,-22,-23,26,-5,7,7,7,7,7,7,7,7,7,7,7,26,26,26,26,26,7,7,7,-8,-9,-10,26,26,26,26,26,-16,26,26,7,-18,7,7,-35,26,-28,26,26,26,-34,7,-36,-3,7,7,7,26,26,26,]),'LPAREN':([0,2,4,5,7,8,9,10,11,12,13,14,16,17,19,20,21,22,24,25,26,27,28,29,30,31,32,33,34,35,37,41,42,43,45,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,63,69,71,72,73,74,75,76,77,78,79,81,82,83,],[8,8,-4,-37,8,8,8,8,8,42,43,-33,45,-19,-20,-21,-22,-23,-5,8,8,8,8,8,8,8,8,8,8,8,-17,-27,8,8,8,-8,-9,-10,-11,-12,-13,-14,-15,-16,-30,-6,8,-18,8,8,-35,-28,-24,-26,-34,8,-36,-3,8,8,8,-29,-7,-25,]),'WHILE':([0,2,4,7,8,9,10,11,24,25,26,27,28,29,30,31,32,33,34,35,42,43,45,58,60,61,74,76,77,78,79,],[9,9,-4,9,9,9,9,9,-5,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,-3,9,9,9,]),'IF':([0,2,4,7,8,9,10,11,24,25,26,27,28,29,30,31,32,33,34,35,42,43,45,58,60,61,74,76,77,78,79,],[10,10,-4,10,10,10,10,10,-5,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,-3,10,10,10,]),'LAZY':([0,2,4,7,8,9,10,11,24,25,26,27,28,29,30,31,32,33,34,35,42,43,45,58,60,61,74,76,77,78,79,],[11,11,-4,11,11,11,11,11,-5,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,-3,11,11,11,]),'IMPORT':([0,2,4,24,76,],[15,15,-4,-5,-3,]),'LAMBDA':([0,2,4,7,8,9,10,11,24,25,26,27,28,29,30,31,32,33,34,35,42,43,45,58,60,61,74,76,77,78,79,],[16,16,-4,16,16,16,16,16,-5,16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,-3,16,16,16,]),'LCBRACE':([0,2,4,7,8,9,10,11,18,24,25,26,27,28,29,30,31,32,33,34,35,42,43,45,58,60,61,74,76,77,78,79,],[18,18,-4,18,18,18,18,18,18,-5,18,18,18,18,18,18,18,18,18,18,18,18,18,18,18,18,18,18,-3,18,18,18,]),'STRING':([0,2,4,7,8,9,10,11,18,24,25,26,27,28,29,30,31,32,33,34,35,42,43,45,58,60,61,74,76,77,78,79,],[19,19,-4,19,19,19,19,19,19,-5,19,19,19,19,19,19,19,19,19,19,19,19,19,19,19,19,19,19,-3,19,19,19,]),'NUMBER':([0,2,4,7,8,9,10,11,18,24,25,26,27,28,29,30,31,32,33,34,35,42,43,45,58,60,61,74,76,77,78,79,],[20,20,-4,20,20,20,20,20,20,-5,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,-3,20,20,20,]),'TRUE':([0,2,4,7,8,9,10,11,18,24,25,26,27,28,29,30,31,32,33,34,35,42,43,45,58,60,61,74,76,77,78,79,],[21,21,-4,21,21,21,21,21,21,-5,21,21,21,21,21,21,21,21,21,21,21,21,21,21,21,21,21,21,-3,21,21,21,]),'FALSE':([0,2,4,7,8,9,10,11,18,24,25,26,27,28,29,30,31,32,33,34,35,42,43,45,58,60,61,74,76,77,78,79,],[22,22,-4,22,22,22,22,22,22,-5,22,22,22,22,22,22,22,22,22,22,22,22,22,22,22,22,22,22,-3,22,22,22,]),'$end':([1,3,5,12,13,14,17,19,20,21,22,23,37,41,47,48,49,50,51,52,53,54,55,56,57,59,63,69,71,72,73,75,81,82,83,],[0,-2,-37,-31,-32,-33,-19,-20,-21,-22,-23,-1,-17,-27,-8,-9,-10,-11,-12,-13,-14,-15,-16,-30,-6,-18,-35,-28,-24,-26,-34,-36,-29,-7,-25,]),'PLUS':([3,5,12,13,14,17,19,20,21,22,23,37,38,39,40,41,47,48,49,50,51,52,53,54,55,56,57,59,63,65,69,70,71,72,73,75,81,82,83,],[25,-37,-31,-32,-33,-19,-20,-21,-22,-23,25,25,25,25,25,25,-8,-9,-10,25,25,25,25,25,-16,25,25,-18,-35,25,-28,25,25,25,-34,-36,25,25,25,]),'TIMES':([3,5,12,13,14,17,19,20,21,22,23,37,38,39,40,41,47,48,49,50,51,52,53,54,55,56,57,59,63,65,69,70,71,72,73,75,81,82,83,],[27,-37,-31,-32,-33,-19,-20,-21,-22,-23,27,27,27,27,27,27,27,27,-10,27,27,27,27,27,-16,27,27,-18,-35,27,-28,27,27,27,-34,-36,27,27,27,]),'EQUALITY':([3,5,12,13,14,17,19,20,21,22,23,37,38,39,40,41,47,48,49,50,51,52,53,54,55,56,57,59,63,65,69,70,71,72,73,75,81,82,83,],[28,-37,-31,-32,-33,-19,-20,-21,-22,-23,28,-17,28,28,28,28,-8,-9,-10,None,None,None,None,None,-16,28,28,-18,-35,28,-28,28,28,28,-34,-36,28,28,28,]),'GREATER':([3,5,12,13,14,17,19,20,21,22,23,37,38,39,40,41,47,48,49,50,51,52,53,54,55,56,57,59,63,65,69,70,71,72,73,75,81,82,83,],[29,-37,-31,-32,-33,-19,-20,-21,-22,-23,29,-17,29,29,29,29,-8,-9,-10,None,None,None,None,None,-16,29,29,-18,-35,29,-28,29,29,29,-34,-36,29,29,29,]),'LESS':([3,5,12,13,14,17,19,20,21,22,23,37,38,39,40,41,47,48,49,50,51,52,53,54,55,56,57,59,63,65,69,70,71,72,73,75,81,82,83,],[30,-37,-31,-32,-33,-19,-20,-21,-22,-23,30,-17,30,30,30,30,-8,-9,-10,None,None,None,None,None,-16,30,30,-18,-35,30,-28,30,30,30,-34,-36,30,30,30,]),'GREATEREQUAL':([3,5,12,13,14,17,19,20,21,22,23,37,38,39,40,41,47,48,49,50,51,52,53,54,55,56,57,59,63,65,69,70,71,72,73,75,81,82,83,],[31,-37,-31,-32,-33,-19,-20,-21,-22,-23,31,-17,31,31,31,31,-8,-9,-10,None,None,None,None,None,-16,31,31,-18,-35,31,-28,31,31,31,-34,-36,31,31,31,]),'LESSEQUAL':([3,5,12,13,14,17,19,20,21,22,23,37,38,39,40,41,47,48,49,50,51,52,53,54,55,56,57,59,63,65,69,70,71,72,73,75,81,82,83,],[32,-37,-31,-32,-33,-19,-20,-21,-22,-23,32,-17,32,32,32,32,-8,-9,-10,None,None,None,None,None,-16,32,32,-18,-35,32,-28,32,32,32,-34,-36,32,32,32,]),'DIVIDE':([3,5,12,13,14,17,19,20,21,22,23,37,38,39,40,41,47,48,49,50,51,52,53,54,55,56,57,59,63,65,69,70,71,72,73,75,81,82,83,],[33,-37,-31,-32,-33,-19,-20,-21,-22,-23,33,33,33,33,33,33,33,33,-10,33,33,33,33,33,-16,33,33,-18,-35,33,-28,33,33,33,-34,-36,33,33,33,]),'PIPE':([3,5,12,13,14,17,19,20,21,22,23,37,38,39,40,41,47,48,49,50,51,52,53,54,55,56,57,59,63,65,69,70,71,72,73,75,81,82,83,],[34,-37,-31,-32,-33,-19,-20,-21,-22,-23,34,-17,34,34,34,34,-8,-9,-10,-11,-12,-13,-14,-15,-16,-30,34,-18,-35,34,-28,34,34,34,-34,-36,34,34,34,]),'EQUALS':([5,36,],[35,58,]),'RPAREN':([5,12,13,14,17,19,20,21,22,37,38,41,42,43,45,47,48,49,50,51,52,53,54,55,56,57,59,62,63,64,65,66,68,69,71,72,73,75,80,81,82,83,],[-37,-31,-32,-33,-19,-20,-21,-22,-23,-17,59,-27,63,-40,-40,-8,-9,-10,-11,-12,-13,-14,-15,-16,-30,-6,-18,73,-35,-39,-41,75,77,-28,-24,-26,-34,-36,-38,-29,-7,-25,]),'DO':([5,12,13,14,17,19,20,21,22,37,39,41,47,48,49,50,51,52,53,54,55,56,57,59,63,69,71,72,73,75,81,82,83,],[-37,-31,-32,-33,-19,-20,-21,-22,-23,-17,60,-27,-8,-9,-10,-11,-12,-13,-14,-15,-16,-30,-6,-18,-35,-28,-24,-26,-34,-36,-29,-7,-25,]),'THEN':([5,12,13,14,17,19,20,21,22,37,40,41,47,48,49,50,51,52,53,54,55,56,57,59,63,69,71,72,73,75,81,82,83,],[-37,-31,-32,-33,-19,-20,-21,-22,-23,-17,61,-27,-8,-9,-10,-11,-12,-13,-14,-15,-16,-30,-6,-18,-35,-28,-24,-26,-34,-36,-29,-7,-25,]),'COMMA':([5,12,13,14,17,19,20,21,22,37,41,42,43,45,47,48,49,50,51,52,53,54,55,56,57,59,62,63,64,65,66,68,69,71,72,73,75,80,81,82,83,],[-37,-31,-32,-33,-19,-20,-21,-22,-23,-17,-27,-40,-40,-40,-8,-9,-10,-11,-12,-13,-14,-15,-16,-30,-6,-18,74,-35,-39,-41,74,74,-28,-24,-26,-34,-36,-38,-29,-7,-25,]),'IN':([5,12,13,14,17,19,20,21,22,37,41,47,48,49,50,51,52,53,54,55,56,57,59,63,69,70,71,72,73,75,81,82,83,],[-37,-31,-32,-33,-19,-20,-21,-22,-23,-17,-27,-8,-9,-10,-11,-12,-13,-14,-15,-16,-30,-6,-18,-35,-28,78,-24,-26,-34,-36,-29,-7,-25,]),'ELSE':([5,12,13,14,17,19,20,21,22,37,41,47,48,49,50,51,52,53,54,55,56,57,59,63,69,71,72,73,75,81,82,83,],[-37,-31,-32,-33,-19,-20,-21,-22,-23,-17,-27,-8,-9,-10,-11,-12,-13,-14,-15,-16,-30,-6,-18,-35,-28,-24,79,-34,-36,-29,-7,-25,]),'RCBRACE':([17,19,20,21,22,46,69,],[-19,-20,-21,-22,-23,69,-28,]),'AS':([44,],[67,]),}
 
 _lr_action = {}
 for _k, _v in _lr_action_items.items():
    for _x,_y in zip(_v[0],_v[1]):
       if not _x in _lr_action:  _lr_action[_x] = {}
       _lr_action[_x][_k] = _y
 del _lr_action_items
 
-_lr_goto_items = {'program':([0,],[1,]),'definitions':([0,],[2,]),'imports':([0,2,],[3,25,]),'expression':([0,2,3,9,10,11,12,13,14,25,30,31,32,33,34,36,43,44,53,58,59,63,67,70,74,76,81,],[4,26,28,37,38,39,40,41,42,47,48,49,50,51,52,56,56,56,65,68,69,56,56,77,79,80,82,]),'function_definition':([0,2,],[5,27,]),'import':([0,2,3,25,],[6,6,29,29,]),'function_call':([0,2,3,9,10,11,12,13,14,25,30,31,32,33,34,36,43,44,53,58,59,63,67,70,74,76,81,],[16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,16,]),'term':([0,2,3,9,10,11,12,13,14,25,30,31,32,33,34,36,43,44,53,58,59,63,67,70,74,76,81,],[17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,]),'factor':([0,2,3,9,10,11,12,13,14,25,30,31,32,33,34,36,43,44,53,58,59,63,67,70,74,76,81,],[20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,20,]),'args':([36,43,44,63,],[54,61,62,72,]),'arg':([36,43,44,63,67,],[55,55,55,55,75,]),}
+_lr_goto_items = {'program':([0,],[1,]),'imports':([0,],[2,]),'expression':([0,2,7,8,9,10,11,25,26,27,28,29,30,31,32,33,34,35,42,43,45,58,60,61,74,77,78,79,],[3,23,37,38,39,40,41,47,48,49,50,51,52,53,54,55,56,57,65,65,65,70,71,72,65,81,82,83,]),'import':([0,2,],[4,24,]),'function_call':([0,2,7,8,9,10,11,25,26,27,28,29,30,31,32,33,34,35,42,43,45,58,60,61,74,77,78,79,],[12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,]),'lambda':([0,2,7,8,9,10,11,25,26,27,28,29,30,31,32,33,34,35,42,43,45,58,60,61,74,77,78,79,],[13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,]),'term':([0,2,7,8,9,10,11,18,25,26,27,28,29,30,31,32,33,34,35,42,43,45,58,60,61,74,77,78,79,],[14,14,14,14,14,14,14,46,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,]),'factor':([0,2,7,8,9,10,11,18,25,26,27,28,29,30,31,32,33,34,35,42,43,45,58,60,61,74,77,78,79,],[17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,17,]),'args':([42,43,45,],[62,66,68,]),'arg':([42,43,45,74,],[64,64,64,80,]),}
 
 _lr_goto = {}
 for _k, _v in _lr_goto_items.items():
    for _x, _y in zip(_v[0], _v[1]):
        if not _x in _lr_goto: _lr_goto[_x] = {}
        _lr_goto[_x][_k] = _y
 del _lr_goto_items
 _lr_productions = [
   ("S' -> program","S'",1,None,None,None),
-  ('program -> definitions imports expression','program',3,'p_program','maryChain.py',261),
-  ('program -> imports expression','program',2,'p_program','maryChain.py',262),
-  ('program -> definitions expression','program',2,'p_program','maryChain.py',263),
-  ('program -> imports','program',1,'p_program','maryChain.py',264),
-  ('program -> definitions','program',1,'p_program','maryChain.py',265),
-  ('program -> expression','program',1,'p_program','maryChain.py',266),
-  ('expression -> LET IDENTIFIER EQUALS expression IN expression','expression',6,'p_expression_let_in','maryChain.py',313),
-  ('expression -> expression PLUS expression','expression',3,'p_expression_binop','maryChain.py',336),
-  ('expression -> expression MINUS expression','expression',3,'p_expression_binop','maryChain.py',337),
-  ('expression -> expression TIMES expression','expression',3,'p_expression_binop','maryChain.py',338),
-  ('expression -> expression DIVIDE expression','expression',3,'p_expression_binop','maryChain.py',339),
-  ('namespace -> IDENTIFIER','namespace',1,'p_namespace','maryChain.py',360),
-  ('namespace -> namespace DOT IDENTIFIER','namespace',3,'p_namespace','maryChain.py',361),
-  ('import -> IMPORT IDENTIFIER AS IDENTIFIER','import',4,'p_import','maryChain.py',371),
-  ('imports -> import','imports',1,'p_imports','maryChain.py',377),
-  ('imports -> imports import','imports',2,'p_imports','maryChain.py',378),
-  ('expression -> MINUS expression','expression',2,'p_expression_uminus','maryChain.py',391),
-  ('expression -> LPAREN expression RPAREN','expression',3,'p_expression_paren','maryChain.py',395),
-  ('term -> factor','term',1,'p_term_factor','maryChain.py',399),
-  ('factor -> STRING','factor',1,'p_factor_string','maryChain.py',403),
-  ('factor -> NUMBER','factor',1,'p_factor_num','maryChain.py',407),
-  ('factor -> TRUE','factor',1,'p_factor_boolean','maryChain.py',411),
-  ('factor -> FALSE','factor',1,'p_factor_boolean','maryChain.py',412),
-  ('expression -> WHILE expression DO expression','expression',4,'p_expression_while','maryChain.py',419),
-  ('expression -> IF expression THEN expression ELSE expression','expression',6,'p_expression_if_then_else','maryChain.py',426),
-  ('expression -> IF expression THEN expression','expression',4,'p_expression_if_then','maryChain.py',446),
-  ('expression -> LAZY expression','expression',2,'p_lazy_expr','maryChain.py',468),
-  ('expression -> LCBRACE expression RCBRACE','expression',3,'p_expression_braces','maryChain.py',486),
-  ('expression -> LAMBDA LPAREN args RPAREN expression','expression',5,'p_expression_lambda','maryChain.py',504),
-  ('expression -> expression PIPE expression','expression',3,'p_expression_pipe','maryChain.py',522),
-  ('expression -> function_call','expression',1,'p_expression_func_call','maryChain.py',539),
-  ('expression -> term','expression',1,'p_expression_term','maryChain.py',557),
-  ('function_definition -> FUNC IDENTIFIER LPAREN args RPAREN LCBRACE expression RCBRACE','function_definition',8,'p_function_definition','maryChain.py',609),
-  ('definitions -> function_definition','definitions',1,'p_definitions','maryChain.py',634),
-  ('definitions -> definitions function_definition','definitions',2,'p_definitions','maryChain.py',635),
-  ('function_call -> function_call LPAREN args RPAREN','function_call',4,'p_function_call','maryChain.py',676),
-  ('function_call -> IDENTIFIER LPAREN args RPAREN','function_call',4,'p_function_call','maryChain.py',677),
-  ('function_call -> IDENTIFIER','function_call',1,'p_function_call','maryChain.py',678),
-  ('args -> args COMMA arg','args',3,'p_args','maryChain.py',696),
-  ('args -> arg','args',1,'p_args','maryChain.py',697),
-  ('args -> <empty>','args',0,'p_args','maryChain.py',698),
-  ('arg -> expression','arg',1,'p_arg','maryChain.py',725),
+  ('program -> imports expression','program',2,'p_program','maryChain.py',242),
+  ('program -> expression','program',1,'p_program','maryChain.py',243),
+  ('import -> IMPORT IDENTIFIER AS IDENTIFIER','import',4,'p_import','maryChain.py',283),
+  ('imports -> import','imports',1,'p_imports','maryChain.py',289),
+  ('imports -> imports import','imports',2,'p_imports','maryChain.py',290),
+  ('expression -> IDENTIFIER EQUALS expression','expression',3,'p_expression_assignment','maryChain.py',301),
+  ('expression -> LET IDENTIFIER EQUALS expression IN expression','expression',6,'p_expression_let_in','maryChain.py',306),
+  ('expression -> expression PLUS expression','expression',3,'p_expression_binop','maryChain.py',327),
+  ('expression -> expression MINUS expression','expression',3,'p_expression_binop','maryChain.py',328),
+  ('expression -> expression TIMES expression','expression',3,'p_expression_binop','maryChain.py',329),
+  ('expression -> expression EQUALITY expression','expression',3,'p_expression_binop','maryChain.py',330),
+  ('expression -> expression GREATER expression','expression',3,'p_expression_binop','maryChain.py',331),
+  ('expression -> expression LESS expression','expression',3,'p_expression_binop','maryChain.py',332),
+  ('expression -> expression GREATEREQUAL expression','expression',3,'p_expression_binop','maryChain.py',333),
+  ('expression -> expression LESSEQUAL expression','expression',3,'p_expression_binop','maryChain.py',334),
+  ('expression -> expression DIVIDE expression','expression',3,'p_expression_binop','maryChain.py',335),
+  ('expression -> MINUS expression','expression',2,'p_expression_uminus','maryChain.py',355),
+  ('expression -> LPAREN expression RPAREN','expression',3,'p_expression_paren','maryChain.py',359),
+  ('term -> factor','term',1,'p_term_factor','maryChain.py',363),
+  ('factor -> STRING','factor',1,'p_factor_string','maryChain.py',367),
+  ('factor -> NUMBER','factor',1,'p_factor_num','maryChain.py',371),
+  ('factor -> TRUE','factor',1,'p_factor_boolean','maryChain.py',375),
+  ('factor -> FALSE','factor',1,'p_factor_boolean','maryChain.py',376),
+  ('expression -> WHILE expression DO expression','expression',4,'p_expression_while','maryChain.py',383),
+  ('expression -> IF expression THEN expression ELSE expression','expression',6,'p_expression_if_then_else','maryChain.py',390),
+  ('expression -> IF expression THEN expression','expression',4,'p_expression_if_then','maryChain.py',410),
+  ('expression -> LAZY expression','expression',2,'p_lazy_expr','maryChain.py',432),
+  ('term -> LCBRACE term RCBRACE','term',3,'p_expression_braces','maryChain.py',450),
+  ('lambda -> LAMBDA LPAREN args RPAREN expression','lambda',5,'p_expression_lambda','maryChain.py',468),
+  ('expression -> expression PIPE expression','expression',3,'p_expression_pipe','maryChain.py',486),
+  ('expression -> function_call','expression',1,'p_expression_func_call','maryChain.py',503),
+  ('expression -> lambda','expression',1,'p_expression_func_call','maryChain.py',504),
+  ('expression -> term','expression',1,'p_expression_term','maryChain.py',522),
+  ('function_call -> function_call LPAREN args RPAREN','function_call',4,'p_function_call','maryChain.py',574),
+  ('function_call -> function_call LPAREN RPAREN','function_call',3,'p_function_call','maryChain.py',575),
+  ('function_call -> lambda LPAREN args RPAREN','function_call',4,'p_function_call','maryChain.py',576),
+  ('function_call -> IDENTIFIER','function_call',1,'p_function_call','maryChain.py',577),
+  ('args -> args COMMA arg','args',3,'p_args','maryChain.py',598),
+  ('args -> arg','args',1,'p_args','maryChain.py',599),
+  ('args -> <empty>','args',0,'p_args','maryChain.py',600),
+  ('arg -> expression','arg',1,'p_arg','maryChain.py',627),
 ]
```

### Comparing `maryChain-0.0.2/setup.py` & `maryChain-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='maryChain',                           # should match the package folder
-    version='0.0.2',                                # important for updates
+    version='0.0.3',                                # important for updates
     license='MIT',                                  # should match your chosen license
     description='maryChain - lightweight programming functional language for LLM',
     long_description=long_description,              # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='Alessio Ricco',
     author_email='alessio.ricco@gmail.com',
     url='https://github.com/alessioricco/maryChain', 
@@ -27,9 +27,9 @@
         'Programming Language :: Python :: 3',
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
         "ply",
     ],   
-    download_url="https://github.com/alessioricco/maryChain",
+    download_url="https://github.com/alessioricco/maryChain/releases/tag/v0.0.3",
 )
```

