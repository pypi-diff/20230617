# Comparing `tmp/foc-0.1.2.tar.gz` & `tmp/foc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foc-0.1.2.tar", last modified: Mon Jun 12 00:48:24 2023, max compression
+gzip compressed data, was "foc-0.1.3.tar", last modified: Sat Jun 17 16:46:10 2023, max compression
```

## Comparing `foc-0.1.2.tar` & `foc-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-12 00:48:24.984709 foc-0.1.2/
--rw-r--r--   0 thyeem     (501) staff       (20)      164 2023-06-12 00:47:08.000000 foc-0.1.2/ChangeLog.md
--rw-r--r--   0 thyeem     (501) staff       (20)     1068 2023-05-15 21:22:31.000000 foc-0.1.2/LICENSE
--rw-r--r--   0 thyeem     (501) staff       (20)       55 2023-06-06 23:18:02.000000 foc-0.1.2/MANIFEST.in
--rw-r--r--   0 thyeem     (501) staff       (20)      420 2023-06-12 00:48:24.984821 foc-0.1.2/PKG-INFO
--rw-r--r--   0 thyeem     (501) staff       (20)    16522 2023-06-11 21:45:18.000000 foc-0.1.2/README.md
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-12 00:48:24.982955 foc-0.1.2/foc/
--rw-r--r--   0 thyeem     (501) staff       (20)    16576 2023-06-11 21:33:00.000000 foc-0.1.2/foc/__init__.py
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-12 00:48:24.984035 foc-0.1.2/foc.egg-info/
--rw-r--r--   0 thyeem     (501) staff       (20)      420 2023-06-12 00:48:24.000000 foc-0.1.2/foc.egg-info/PKG-INFO
--rw-r--r--   0 thyeem     (501) staff       (20)      221 2023-06-12 00:48:24.000000 foc-0.1.2/foc.egg-info/SOURCES.txt
--rw-r--r--   0 thyeem     (501) staff       (20)        1 2023-06-12 00:48:24.000000 foc-0.1.2/foc.egg-info/dependency_links.txt
--rw-r--r--   0 thyeem     (501) staff       (20)       10 2023-06-12 00:48:24.000000 foc-0.1.2/foc.egg-info/top_level.txt
--rw-r--r--   0 thyeem     (501) staff       (20)      102 2023-06-12 00:48:24.985543 foc-0.1.2/setup.cfg
--rw-r--r--   0 thyeem     (501) staff       (20)      696 2023-06-12 00:43:14.000000 foc-0.1.2/setup.py
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-12 00:48:24.984484 foc-0.1.2/tests/
--rw-r--r--   0 thyeem     (501) staff       (20)        0 2023-06-11 20:28:50.000000 foc-0.1.2/tests/__init__.py
--rw-r--r--   0 thyeem     (501) staff       (20)     7973 2023-06-11 21:43:33.000000 foc-0.1.2/tests/test_foc.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-17 16:46:10.717319 foc-0.1.3/
+-rw-r--r--   0 thyeem     (501) staff       (20)      313 2023-06-17 16:43:38.000000 foc-0.1.3/ChangeLog.md
+-rw-r--r--   0 thyeem     (501) staff       (20)     1068 2023-05-15 21:22:31.000000 foc-0.1.3/LICENSE
+-rw-r--r--   0 thyeem     (501) staff       (20)       55 2023-06-06 23:18:02.000000 foc-0.1.3/MANIFEST.in
+-rw-r--r--   0 thyeem     (501) staff       (20)      420 2023-06-17 16:46:10.717432 foc-0.1.3/PKG-INFO
+-rw-r--r--   0 thyeem     (501) staff       (20)    16885 2023-06-17 16:37:04.000000 foc-0.1.3/README.md
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-17 16:46:10.715128 foc-0.1.3/foc/
+-rw-r--r--   0 thyeem     (501) staff       (20)    18551 2023-06-17 16:37:04.000000 foc-0.1.3/foc/__init__.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-17 16:46:10.716466 foc-0.1.3/foc.egg-info/
+-rw-r--r--   0 thyeem     (501) staff       (20)      420 2023-06-17 16:46:10.000000 foc-0.1.3/foc.egg-info/PKG-INFO
+-rw-r--r--   0 thyeem     (501) staff       (20)      221 2023-06-17 16:46:10.000000 foc-0.1.3/foc.egg-info/SOURCES.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)        1 2023-06-17 16:46:10.000000 foc-0.1.3/foc.egg-info/dependency_links.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)       10 2023-06-17 16:46:10.000000 foc-0.1.3/foc.egg-info/top_level.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)      102 2023-06-17 16:46:10.717896 foc-0.1.3/setup.cfg
+-rw-r--r--   0 thyeem     (501) staff       (20)      696 2023-06-17 16:37:59.000000 foc-0.1.3/setup.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-17 16:46:10.717048 foc-0.1.3/tests/
+-rw-r--r--   0 thyeem     (501) staff       (20)        0 2023-06-11 20:28:50.000000 foc-0.1.3/tests/__init__.py
+-rw-r--r--   0 thyeem     (501) staff       (20)     8030 2023-06-16 13:26:37.000000 foc-0.1.3/tests/test_foc.py
```

### Comparing `foc-0.1.2/LICENSE` & `foc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `foc-0.1.2/README.md` & `foc-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -82,14 +82,17 @@
 
 >>> even(3)
 False
 
 >>> null([]) == null(()) == null({}) == null("")
 True
 
+>>> elem(5, range(10))
+True
+
 >>> words("fun on functions")
 ['fun', 'on', 'functions']
 
 >>> unwords(['fun', 'on', 'functions'])
 'fun on functions'
 
 >>> lines("fun\non\nfunctions")
@@ -120,27 +123,25 @@
 > When using `ff_`, passing arguments in reverse order for a long-args function is painful.
 >
 > `ff_` takes arguments _in order_ by default (`sgra=False`). It will take args _in reverse order_ when the `sgra` keyword is on.
 >
 > _`_` in function names indicates that it is a partial application (not-fully-evaluated function) builder._
 
 ```python
-import operator as op
+>>> f_("+", 5)(2)    # the same as `(5+) 2` in Haskell
+7                    # 5 + 2
 
->>> f_(op.add, 5)(2)    # the same as `(5+) 2` in Haskell
-7                       # 5 + 2
+>>> ff_("+", 5)(2)   # the same as `(+5) 2 in Haskell`
+7                    # 2 + 5
 
->>> ff_(op.add, 5)(2)   # the same as `(+5) 2 in Haskell`
-7                       # 2 + 5
+>>> f_("-", 5)(2)    # the same as `(5-) 2`
+3                    # 5 - 2
 
->>> f_(op.sub, 5)(2)    # the same as `(5-) 2`
-3                       # 5 - 2
-
->>> ff_(op.sub, 5)(2)   # the same as `(subtract 5) 2`
--3                      # 2 - 5
+>>> ff_("-", 5)(2)   # the same as `(subtract 5) 2`
+-3                   # 2 - 5
 
 # with N-ary function
 >>> def print_args(a, b, c, d): print(f"{a}-{b}-{c}-{d}")
 
 >>> f_(print_args, 1, 2)(3, 4)                # partial-eval from the left
 1-2-3-4                                       # print_args(1, 2, 3, 4)
 
@@ -156,25 +157,25 @@
 
 #### Build curried functions: `c_` and `cc_`
 When currying a given function, `c_` takes arguments _from the left_ while `cc_` takes them _from the right_.
 > _`_` in function names indicates that it is a partial application (not-fully-evaluated function) builder._
 
 ```python
 # currying from the left args
->>> c_(op.add)(5)(2)    # 5 + 2
+>>> c_("+")(5)(2)    # 5 + 2
 7
 
->>> c_(op.sub)(5)(2)    # 5 - 2
+>>> c_("-")(5)(2)    # 5 - 2
 3
 
 # currying from the right args
->>> cc_(op.add)(5)(2)   # 2 + 5
+>>> cc_("+")(5)(2)   # 2 + 5
 7
 
->>> cc_(op.sub)(5)(2)   # 2 - 5
+>>> cc_("-")(5)(2)   # 2 - 5
 -3
 
 # with N-ary function
 >>> c_(print_args)(1)(2)(3)(4)    # print_args(1, 2, 3, 4)
 1-2-3-4
 
 >>> cc_(print_args)(1)(2)(3)(4)   # print_args(4, 3, 2, 1)
@@ -183,34 +184,35 @@
 
 #### Build composition of functions: `cf_` and `cfd`
 `cf_` (_composition of function_) composes functions using the given list of functions. On the other hand, `cfd` (_composing-function decorator_) decorates a function with the given list of functions.
 
 > _`_` in function names indicates that it is a partial application (not-fully-evaluated function) builder._
 
 ```python
->>> pow3 = f_(op.pow, 3)      # the same as (3^) in Haskell
->>> add5 = f_(op.add, 5)      # the same as (5+)
->>> mul7 = f_(op.mul, 7)      # the same as (7*)
+>>> square = ff_("**", 2)     # the same as (^2) in Haskell
+>>> add_by_5 = ff_("+", 5)    # the same as (+5)
+>>> mul_by_7 = ff_("*", 7)    # the same as (*7)
 
->>> cf_(mul7, add5, pow3)(2)  # (7*) . (5+) . (3^) $ 2
-98                            # mul7(add5(pow3(2))) = 7 * (5 + (3 ^ 2))
+>>> cf_(mul_by_7, add_by_5, square)(3)   # (*7) . (+5) . (^2) $ 2
+98                            # mul_by_7(add_by_5(square(2))) = ((3 ^ 2) + 5) * 7
 
->>> @cfd(mul7, add5, pow3)
+>>> @cfd(mul_by_7, add_by_5, square)
 ... def even_num_less_than(x):
 ...     return len(list(filter(even, range(x))))
 
 >>> even_num_less_than(7)     # even numbers less than 7 = len({0, 2, 4, 6}) = 4
-602                           # mul7(add5(pow3(even_num_less_than(7)))) = 7 * (5 + (3 ^ 4))
+147                           # mul_by_7(add_by_5(square(4))) = ((4 ^ 2) + 5) * 7
+
+# the meaning of decorating a function with a composition of functions
+g = cfd(a, b, c, d)(f)   # g = (a . b . c . d)(f)
 
 # the same
->>> cf_(mul7, add5, pow3, even_num_less_than)(7)
-602
+cfd(a, b, c, d)(f)(x)    # g(x) = a(b(c(d(f(x)))))
 
->>> cfd(mul7, add5, pow3)(even_num_less_than)(7)
-602
+cf_(a, b, c, d, f)(x)    # (a . b . c . d . f)(x) = a(b(c(d(f(x))))) = g(x)
 ```
 
 `cfd` is very handy and useful to recreate previously defined functions by composing functions. All you need is to write a basic functions to do fundamental things.
 
 #### Partial application of `map`: `m_` and `mm_`
 `m_` builds partial application of `map` (left-associative) while `mm_` builds partial application from right to left (right-associative).
 
@@ -233,24 +235,24 @@
 
 # so 'm_' and 'mm_' do
 >>> ml_ = cfd(list)(m_)
 >>> mml_ = cfd(list)(mm_)
 ```
 
 ```python
->>> list(map(f_(op.mul, 8), range(1, 6)))   # (8*) <$> [1..5]
+>>> list(map(f_("*", 8), range(1, 6)))   # (8*) <$> [1..5]
 [8, 16, 24, 32, 40]                         # [ (lambda x: 8*x)(x) for x in range(1, 6) ]
 
->>> mapl(f_(op.mul, 8), range(1, 6))        # (8*) <$> [1..5]
+>>> mapl(f_("*", 8), range(1, 6))        # (8*) <$> [1..5]
 [8, 16, 24, 32, 40]
 
->>> ml_(f_(op.mul, 8))(range(1, 6))         # ((8*) <$>) [1..5]
+>>> ml_(f_("*", 8))(range(1, 6))         # ((8*) <$>) [1..5]
 [8, 16, 24, 32, 40]
 
->>> mml_(range(1, 6))(f_(op.mul, 8))        # (<$> [1..5]) (8*)
+>>> mml_(range(1, 6))(f_("*", 8))        # (<$> [1..5]) (8*)
 [8, 16, 24, 32, 40]
 ```
 
 #### Partial application of `filter`: `v_` and `vv_`
 `v_` builds partial application of `filter` (left-associative) while `vv_` builds partial application from right to left (right-associative).
 
 The same as `map` (mapping functions over iterables) except for filtering iterables using predicate function.
@@ -275,35 +277,35 @@
 [0, 2, 4, 6, 8]
 
 >>> even_nums({2, 3, 5, 7, 11, 13, 17, 19, 23})
 [2]
 
 >>> primes_lt_50 = vvl_([2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47])
 
->>> primes_lt_50(ff_(op.gt, 20))    # (> 20)
+>>> primes_lt_50(ff_(">", 20))    # (> 20)
 [23, 29, 31, 37, 41, 43, 47]
 
 >>> primes_lt_50(lambda x: x % 3 == 2)
 [2, 5, 11, 17, 23, 29, 41, 47]
 
->>> primes_lt_50(cf_(ff_(op.eq, 2), ff_(op.mod, 3)))    # ((== 2) . (% 3))
+>>> primes_lt_50(cf_(ff_("==", 2), ff_("%", 3)))    # ((== 2) . (% 3))
 [2, 5, 11, 17, 23, 29, 41, 47]
 ```
 
 #### Other higher-order functions
 > To see all available functions, use `flist()` to print to `stdout` or `usage = flist(True)`.
 
 ```python
->>> bimap(f_(op.add, 3), f_(op.mul, 7), (5, 7))    # bimap (3+) (7*) (5, 7)
+>>> bimap(f_("+", 3), f_("*", 7), (5, 7))    # bimap (3+) (7*) (5, 7)
 (8, 49)                                            # (3+5, 7*7)
 
->>> first(f_(op.add, 3), (5, 7))                   # first (3+) (5, 7)
+>>> first(f_("+", 3), (5, 7))                   # first (3+) (5, 7)
 (8, 7)                                             # (3+5, 7)
 
->>> second(f_(op.mul, 7), (5, 7))                  # second (7*) (5, 7)
+>>> second(f_("*", 7), (5, 7))                  # second (7*) (5, 7)
 (5, 49)                                            # (5, 7*7)
 
 >>> take(5, iterate(lambda x: x**2, 2))            # [2, 2**2, (2**2)**2, ((2**2)**2)**2, ...]
 [2, 4, 16, 256, 65536]
 
 >>> [* takewhile(even, [2, 4, 6, 1, 3, 5]) ]       # `takewhile` returns a generator
 [2, 4, 6]
@@ -314,43 +316,43 @@
 >>> [* dropwhile(even, [2, 4, 6, 1, 3, 5]) ]       # `dropwhile` returns a generator
 [1, 3, 5]
 
 >>> dropwhilel(even, [2, 4, 6, 1, 3, 5])
 [1, 3, 5]
 
 # fold with a given initial value from the left
->>> foldl(op.sub, 10, range(1, 5))                 # foldl (-) 10 [1..4]
+>>> foldl("-", 10, range(1, 5))                 # foldl (-) 10 [1..4]
 0
 
 # fold with a given initial value from the right
->>> foldr(op.sub, 10, range(1, 5))                 # foldr (-) 10 [1..4]
+>>> foldr("-", 10, range(1, 5))                 # foldr (-) 10 [1..4]
 8
 
 # `foldl` without an initial value (used first item instead)
->>> foldl1(op.sub, range(1, 5))                    # foldl1 (-) [1..4]
+>>> foldl1("-", range(1, 5))                    # foldl1 (-) [1..4]
 -8
 
 # `foldr` without an initial value (used first item instead)
->>> foldr1(op.sub, range(1, 5))                    # foldr1 (-) [1..4]
+>>> foldr1("-", range(1, 5))                    # foldr1 (-) [1..4]
 -2
 
 # accumulate reduced values from the left
->>> scanl(op.sub, 10, range(1, 5))                 # scanl (-) 10 [1..4]
+>>> scanl("-", 10, range(1, 5))                 # scanl (-) 10 [1..4]
 [10, 9, 7, 4, 0]
 
 # accumulate reduced values from the right
->>> scanr(op.sub, 10, range(1, 5))                 # scanr (-) 10 [1..4]
+>>> scanr("-", 10, range(1, 5))                 # scanr (-) 10 [1..4]
 [8, -7, 9, -6, 10]
 
 # `scanl` but no starting value
->>> scanl1(op.sub, range(1, 5))                    # scanl1 (-) [1..4]
+>>> scanl1("-", range(1, 5))                    # scanl1 (-) [1..4]
 [1, -1, -4, -8]
 
 # `scanr` but no starting value
->>> scanr1(op.sub, range(1, 5))                    # scanr1 (-) [1..4]
+>>> scanr1("-", range(1, 5))                    # scanr1 (-) [1..4]
 [-2, 3, -1, 4]
 
 # See also 'concat' that returns a generator
 >>> concatl(["sofia", "maria"])
 ['s', 'o', 'f', 'i', 'a', 'm', 'a', 'r', 'i', 'a']
 
 # See also 'concatmap' that returns a generator
@@ -429,51 +431,41 @@
 ```
 
 #### Dot-accessible dictionary: `dmap`
 `dmap` is a _yet another_ `dict`. It's exactly the same as `dict` but it enables to access its nested structure with '_dot notations_'.
 
 ```python
 >>> d = dmap(name="yunchan lim", age=19, profession="pianist")
-{'name': 'yunchan lim', 'age': 19, 'profession': 'pianist'}
-
->>> d.cliburn.semifinal.mozart.concerto = "No.22"
->>> d.cliburn.final.rachmaninoff = "crazy!"
-
-# pretty-printer
->>> import json
->>> pprint = cf_(print, ff_(json.dumps, indent=2)
-
->>> pprint(d)
-{
-  "name": "yunchan lim",
-  "age": 19,
-  "profession": "pianist",
-  "cliburn": {
-    "semifinal": {
-      "mozart": {
-        "concerto": "No.22"
-      }
-    },
-    "final": {
-      "rachmaninoff": "crazy!"
-    }
-  }
-}
+>>> nprint(d)    # neatly print 'dict' or 'dict-items'
+        name  |  yunchan lim
+         age  |  19
+  profession  |  pianist
+
+# just put the value in the desired key path
+>>> d.cliburn.semifinal.mozart = "piano concerto no.22"
+>>> d.cliburn.semifinal.liszt = "12 transcendental etudes"
+>>> d.cliburn.final.beethoven = "piano concerto no.3"
+>>> d.cliburn.final.rachmaninoff = "piano concerto no.3"
+>>> nprint(d)
+        name  |  yunchan lim
+         age  |  19
+  profession  |  pianist
+     cliburn  |   semifinal  |   mozart  |  piano concerto no.22
+              |              |    liszt  |  12 transcendental etudes
+              |       final  |      beethoven  |  piano concerto no.3
+              |              |   rachmaninoff  |  piano concerto no.3
 
 >>> del d.cliburn
 >>> d.profession = "one-in-a-million talent"
+>>> nprint(d)
+        name  |  yunchan lim
+         age  |  19
+  profession  |  one-in-a-million talent
 
->>> pprint(d)
-{
-  "name": "yunchan lim",
-  "age": 19,
-  "profession": "one-in-a-million talent"
-}
-
-# No such path of keys
+# No such key path
 >>> d.bach.chopin.beethoven
 {}
 ```
 
 
 #### `raise` with a function(_expression_): `error`
 
@@ -518,11 +510,11 @@
             ff_(torch.Tensor.view, B, S, E),  # (B, S, N, H) -> (B, S, E)
             torch.Tensor.contiguous,  # contiguos in-memory tensor
             ff_(torch.transpose, 1, 2),  # (B, S, N, H)
             ff_(torch.matmul, v),  # (B, N, S, S) x (B, N, S, H) -> (B, N, S, H)
             self.attn_dropout,  # attention dropout
             ff_(F.softmax, dim=-1),  # softmax
             ff_(torch.masked_fill, self.mask[:,:,:S,:S] == 0, float("-inf")),  # mask
-            ff_(op.truediv, math.sqrt(k.size(-1))),  # / sqrt(d_k)
+            ff_("/", math.sqrt(k.size(-1))),  # / sqrt(d_k)
             ff_(torch.matmul, k.transpose(-2, -1)),  # Q @ K^T -> (B, N, S, S)
         )(q)
 ```
```

### Comparing `foc-0.1.2/foc/__init__.py` & `foc-0.1.3/foc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,16 @@
 from inspect import signature
 from itertools import count, cycle, dropwhile, takewhile, tee
 from shutil import rmtree
 from textwrap import fill
 
 __all__ = [
     "flist",
-    "op",
     "deque",
     "safe",
-    "not_",
     "id",
     "fst",
     "snd",
     "nth",
     "take",
     "drop",
     "head",
@@ -32,14 +30,15 @@
     "odd",
     "even",
     "null",
     "words",
     "unwords",
     "lines",
     "unlines",
+    "elem",
     "repeat",
     "replicate",
     "cycle",
     "count",
     "tee",
     "product",
     "flip",
@@ -65,14 +64,22 @@
     "enumeratel",
     "reverse",
     "sort",
     "takewhile",
     "takewhilel",
     "dropwhile",
     "dropwhilel",
+    "tup",
+    "not_",
+    "and_",
+    "or_",
+    "in_",
+    "is_",
+    "is_not_",
+    "bop",
     "bimap",
     "first",
     "second",
     "iterate",
     "foldl",
     "foldl1",
     "foldr",
@@ -101,14 +108,15 @@
     "fwrite",
     "split_at",
     "chunk_of",
     "capture",
     "captures",
     "error",
     "HOME",
+    "cd",
     "pwd",
     "normpath",
     "exists",
     "dirname",
     "basename",
     "mkdir",
     "rmdir",
@@ -133,18 +141,14 @@
             return f(*args, **kwargs)
         except:
             return
 
     return wrapper
 
 
-# `not` as a function
-not_ = op.not_
-
-
 def id(x):
     return x
 
 
 @safe
 def fst(x):
     return nth(1, x)
@@ -224,14 +228,18 @@
     return x.split("\n")
 
 
 def unlines(x):
     return "\n".join(x)
 
 
+def elem(x, xs):
+    return x in xs
+
+
 def repeat(x):
     return (x for _ in it.count())
 
 
 def replicate(n, x):
     return take(n, repeat(x))
 
@@ -247,81 +255,84 @@
     @wraps(f)
     def wrapper(*args, **kwargs):
         return f(*args[::-1], **kwargs)
 
     return wrapper
 
 
-# for decreasing verbosity
-f_ = partial
+def f_(f, *args, **kwargs):
+    """build left-associative partial application,
+    where the given function's arguments partially evaluation from the left"""
+
+    return partial(bop(f), *args, **kwargs)
 
 
 def ff_(f, *args, sgra=False, **kwargs):
-    """build partial application after getting a function flipped:
-    'flipped' means the original funtion is partially applied from the right.
+    """build left-associative partial application,
+    where the given function's arguments partially evaluation from the right
 
     Passing arguments in reverse order for a function is painful.
     `ff_` takes arguments _in order_ by default (`sgra=False`).
     When 'sgra=True', it will take arguments in reverse order.
 
     naming: 'sgra' == 'args'[::-1]
     """
     if sgra:
-        return f_(flip(f), *args, **kwargs)
+        return f_(flip(bop(f)), *args, **kwargs)
     else:
-        return flip(f_(flip(f), *args[::-1], **kwargs))
+        return flip(f_(flip(bop(f)), *args[::-1], **kwargs))
 
 
 def curry(f, n=None):
     """build curried function that takes arguments from the left.
     The currying result is simply a nested unary function.
 
     This function takes positional arguments only when currying.
     Use partial application `f_` before currying if you need to change kwargs"""
+    f = bop(f)
     n = n if n else len(fn_args(f))
 
     @wraps(f)
     def wrapper(x):
         return f(x) if n <= 1 else curry(f_(f, x), n=pred(n))
 
     return wrapper
 
 
 # for decreasing verbosity
 c_ = curry
 
 
-def cc_(f, *args, **kwargs):
+def cc_(f):
     """build curried function that takes arguments from the right"""
-    return c_(flip(f), *args, **kwargs)
+    return c_(flip(bop(f)))
 
 
 def cf_(*fs, rep=None):
     """compose a given list of functions then return the composed function"""
 
-    def wrapper(f, g):
+    def compose(f, g):
         return lambda x: f(g(x))
 
-    args = fs * rep if rep else fs
-    return reduce(wrapper, args, id)
+    return reduce(compose, fs * rep if rep else fs)
 
 
 def cfd(*fs, rep=None):
     """decorator using the composition of functions:
     decorate a function using the composition of the given functions.
     """
 
-    def comp(g):
-        @wraps(g)
+    def cfdeco(f):
+        @wraps(f)
         def wrapper(*args, **kwargs):
-            return cf_(*fs, rep=rep)(g(*args, *kwargs))
+            return cf_(*fs, rep=rep)(f(*args, *kwargs))
 
         return wrapper
 
-    return comp
+    return cfdeco
 
 
 def m_(f):
     """builds partial application of `map` (left-associative)
     map(f, xs) == f <$> xs
 
     (f <$>) == map(f,)  == f_(map, f) == m_(f)
@@ -405,14 +416,74 @@
 takewhilel.__doc__ = "unpacks the result in list after `takewhile`"
 
 
 dropwhilel = cfd(list)(dropwhile)
 dropwhilel.__doc__ = "unpacks the result in list after `dropwhile`"
 
 
+def tup(*args):
+    """construct tuple with given arguments: this mirros `dict(**kwargs)`"""
+    return args
+
+
+def not_(x):
+    """`not` as a function"""
+    return not x
+
+
+def and_(a, b):
+    """`and` as a function"""
+    return a and b
+
+
+def or_(a, b):
+    """`and` as a function"""
+    return a or b
+
+
+# `in` as a function
+in_ = op.contains
+
+
+# `is` as a function
+is_ = op.is_
+
+
+# `is not` as a function
+is_not_ = op.is_not
+
+
+@cache
+def bop(f):
+    """symbolic binary operators"""
+    return {
+        "+": op.add,
+        "-": op.sub,
+        "*": op.mul,
+        "/": op.truediv,
+        "//": op.floordiv,
+        "**": op.pow,
+        "@": op.matmul,
+        "%": op.mod,
+        "&": op.and_,
+        "|": op.or_,
+        "^": op.xor,
+        "<<": op.lshift,
+        ">>": op.rshift,
+        "==": op.eq,
+        "!=": op.ne,
+        ">": op.gt,
+        ">=": op.ge,
+        "<": op.lt,
+        "<=": op.le,
+        "[]": op.getitem,
+        ",": lambda a, b: (a, b),
+    }.get(f, f)
+
+
 def bimap(f, g, x):
     """map over both 'first' and 'second' arguments at the same time
     bimap(f, g) == first(f) . second(g)
     """
     return cf_(f_(first, f), f_(second, g))(x)
 
 
@@ -430,56 +501,56 @@
     while True:
         yield x
         x = f(x)
 
 
 def foldl(f, initial, xs):
     """left-associative fold of an iterable. The same as 'foldl' in Haskell"""
-    return reduce(f, xs, initial)
+    return reduce(bop(f), xs, initial)
 
 
 def foldl1(f, xs):
     """`foldl` without initial value. The same as 'foldl1' in Haskell"""
-    return reduce(f, xs)
+    return reduce(bop(f), xs)
 
 
 def foldr(f, inital, xs):
     """right-associative fold of an iterable. The same as 'foldr' in Haskell"""
-    return reduce(flip(f), xs[::-1], inital)
+    return reduce(flip(bop(f)), xs[::-1], inital)
 
 
 def foldr1(f, xs):
     """`foldr` without initial value. The same as 'foldr1' in Haskell"""
-    return reduce(flip(f), xs[::-1])
+    return reduce(flip(bop(f)), xs[::-1])
 
 
 @cfd(list)
 def scanl(f, initial, xs):
     """returns a list of successive reduced values from the left
     The same as `scanl` in Haskell"""
-    return it.accumulate(xs, f, initial=initial)
+    return it.accumulate(xs, bop(f), initial=initial)
 
 
 @cfd(list)
 def scanl1(f, xs):
     """`scanl` without starting value. The same as 'scanl1' in Haskell"""
-    return it.accumulate(xs, f)
+    return it.accumulate(xs, bop(f))
 
 
 @cfd(reverse)
 def scanr(f, initial, xs):
     """returns a list of successive reduced values from the right
     The same as `scanr` in Haskell"""
-    return it.accumulate(xs[::-1], flip(f), initial=initial)
+    return it.accumulate(xs[::-1], flip(bop(f)), initial=initial)
 
 
 @cfd(reverse)
 def scanr1(f, xs):
     """`scanr` without starting value. The same as 'scanr1' in Haskell"""
-    return it.accumulate(xs[::-1], flip(f))
+    return it.accumulate(xs[::-1], flip(bop(f)))
 
 
 def permutation(x, r, rep=False):
     return it.product(x, repeat=r) if rep else it.permutations(x, r)
 
 
 def combination(x, r, rep=False):
@@ -509,14 +580,16 @@
 concatmapl = cfd(list)(concatmap)
 concatmapl.__doc__ = "unpacks the result in list after `concatmap`"
 
 
 def lazy(f, *args, **kwargs):
     """delays the evaluation of a function(or expression) using generator"""
 
+    f = bop(f)
+
     def g(*a, **k):
         yield f(*a, **k) if callable(f) else f
 
     return cfd(next)(f_(g, *args, **kwargs))
 
 
 def force(x, *args, **kwargs):
@@ -613,14 +686,22 @@
     raise e(str)
 
 
 def HOME():
     return os.getenv("HOME")
 
 
+def cd(path=None):
+    if path:
+        os.chdir(normpath(path, abs=True))
+    else:
+        os.chdir(HOME())
+    return pwd()
+
+
 def pwd():
     return os.getcwd()
 
 
 def normpath(path, abs=False):
     return cf_(
         os.path.abspath if abs else id,
@@ -739,48 +820,66 @@
             instances[cls] = cls(*args, **kwargs)
         return instances[cls]
 
     return wrapper
 
 
 def polling(f, sec, args=None, kwargs=None):
-    def wrapper():
+    def go():
         polling(f, sec, args, kwargs)
         if args and kwargs:
             f(*args, **kwargs)
         elif kwargs:
             f(**kwargs)
         elif args:
             f(*args)
         else:
             f()
 
-    t = threading.Timer(sec, wrapper, args, kwargs)
+    t = threading.Timer(sec, go, args, kwargs)
     t.start()
     return t
 
 
-def neatly(_width=100, _indent=12, **kwargs):
-    """generate justified string using the given **kwargs"""
+def neatly(x={}, _width=100, _indent=None, **kwargs):
+    """generate justified string of 'dict' or 'dict-items'"""
+    d = {**x, **kwargs}
+    _indent = _indent or max(map(len, d.keys())) + 1
+    if _width < _indent:
+        error(f"Error, neatly print with invalid width: {_width}")
+
+    def go(x):
+        if isinstance(x, dict):
+            return neatly(**x, _width=_width - _indent - 6)
+        else:
+            return x
+
+    def lf(k, v):
+        return [
+            (" ", v) if i else (k, v)
+            for i, v in enumerate(filter(cf_(not_, null), lines(f"{v}")))
+        ]
+
     return "\n".join(
         fill(
             f"{v}",
             width=_width,
             break_on_hyphens=False,
             drop_whitespace=False,
-            initial_indent=f"{k:>{_indent}}  |  ",
+            initial_indent=f"{k.replace('_','-'):>{_indent}}  |  ",
             subsequent_indent=f"{' ':>{_indent}}  |  ",
         )
-        for k, v in kwargs.items()
+        for k, v in d.items()
+        for k, v in lf(k, go(v))
     )
 
 
-def nprint(x, **kwargs):
+def nprint(x={}, _width=100, _indent=None, **kwargs):
     """neatly print dictionary using `neatly` formatter"""
-    print(neatly(**x, **kwargs))
+    print(neatly(**x, _width=_width, _indent=_indent, **kwargs))
 
 
 def timestamp(
     origin=None,
     w=0,
     d=0,
     h=0,
@@ -810,15 +909,15 @@
 def __sig__():
     def sig(o):
         try:
             return signature(o).__str__()
         except:
             return " is valid, but live-inspect not available"
 
-    return dmap({x: x + sig(eval(x)) for x in __all__[3:]})
+    return dmap({x: x + sig(eval(x)) for x in __all__[2:]})
 
 
 def flist(to_dict=False):
     if to_dict:
         return __sig__()
     else:
         nprint(__sig__(), _indent=14)
```

### Comparing `foc-0.1.2/setup.py` & `foc-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_decription = f.read()
 
 setuptools.setup(
     name="foc",
-    version="0.1.2",
+    version="0.1.3",
     author="Francis Lim",
     author_email="thyeem@gmail.com",
     description="A collection of python functions for somebody's sanity",
     long_decription=long_decription,
     long_decription_content_type="text/markdown",
     install_requires=[],
     url="https://github.com/thyeem/foc",
```

### Comparing `foc-0.1.2/tests/test_foc.py` & `foc-0.1.3/tests/test_foc.py`

 * *Files 12% similar despite different names*

```diff
@@ -102,14 +102,20 @@
     assert null({})
     assert null("")
     assert null(deque([]))
     assert null(range(3, 3))
     assert not null(range(1, 5))
 
 
+def test_elem():
+    assert elem("f", "francis")
+    assert elem(5, range(10))
+    assert elem("sofia", dict(sofia="painter", maria="ballerina"))
+
+
 def test_words():
     assert words("fun on functions") == ["fun", "on", "functions"]
 
 
 def test_unwords():
     assert unwords(["fun", "on", "functions"]) == "fun on functions"
 
@@ -131,61 +137,61 @@
 
 
 def test_flip():
     assert fn(4, 3, 2, 1) == flip(fn)(1, 2, 3, 4)
 
 
 def test_ff_():
-    assert f_(op.add, 5)(2) == 7
-    assert ff_(op.add, 5)(2) == 7
-    assert f_(op.sub, 5)(2) == 3
-    assert ff_(op.sub, 5)(2) == -3
+    assert f_("+", 5)(2) == 7
+    assert ff_("+", 5)(2) == 7
+    assert f_("-", 5)(2) == 3
+    assert ff_("-", 5)(2) == -3
     assert f_(fn, 1, 2)(3, 4) == "1-2-3-4"
     assert f_(fn, 1, 2, 3)(4) == "1-2-3-4"
     assert ff_(fn, 1, 2)(3, 4) == "3-4-1-2"
     assert ff_(fn, 1, 2, sgra=True)(3, 4) == "4-3-2-1"
 
 
 def test_curry():
-    assert c_(op.add)(5)(2) == 7
-    assert c_(op.add)(2)(5) == 7
-    assert c_(op.sub)(5)(2) == 3
-    assert c_(op.sub)(2)(5) == -3
-    assert c_(op.sub)(5)(2) == cc_(op.sub)(2)(5)
+    assert c_("+")(5)(2) == 7
+    assert c_("+")(2)(5) == 7
+    assert c_("-")(5)(2) == 3
+    assert c_("-")(2)(5) == -3
+    assert c_("-")(5)(2) == cc_("-")(2)(5)
     assert c_(fn)(1)(2)(3)(4) == "1-2-3-4"
     assert c_(fn)(4)(3)(2)(1) == "4-3-2-1"
     assert c_(fn)(4)(3)(2)(1) == cc_(fn)(1)(2)(3)(4)
 
 
 def test_cf_():
-    assert cf_(f_(op.mul, 7), f_(op.add, 5), f_(op.pow, 3))(2) == 98
+    assert cf_(f_("*", 7), f_("+", 5), f_("**", 3))(2) == 98
 
 
 def test_cfd():
-    @cfd(f_(op.mul, 7), f_(op.add, 5), ff_(op.pow, 3))
+    @cfd(f_("*", 7), f_("+", 5), ff_("**", 3))
     def f(x, y):
         return x**2 + y**2
 
     assert f(3, 4) == 109410
 
 
 def test_mapl():
-    fn = f_(op.mul, 8)
+    fn = f_("*", 8)
     assert mapl(fn, range(1, 6)) == [8, 16, 24, 32, 40]
     assert list(map(fn, range(1, 6))) == mapl(fn, range(1, 6))
 
 
 def test_ml():
-    fn = f_(op.mul, 8)
+    fn = f_("*", 8)
     assert ml_(fn)(range(1, 6)) == [8, 16, 24, 32, 40]
     assert list(m_(fn)(range(1, 6))) == ml_(fn)(range(1, 6))
 
 
 def test_mml():
-    fn = f_(op.mul, 8)
+    fn = f_("*", 8)
     assert mml_(range(1, 6))(fn) == [8, 16, 24, 32, 40]
     assert list(mm_(range(1, 6))(fn)) == mml_(range(1, 6))(fn)
 
 
 def test_filterl():
     assert filterl(even, range(10)) == [0, 2, 4, 6, 8]
     assert list(filter(even, range(10))) == filterl(even, range(10))
@@ -213,59 +219,59 @@
 
 
 def test_dropwhilel():
     assert dropwhilel(even, [2, 4, 6, 1, 3, 5]) == [1, 3, 5]
 
 
 def test_bimap():
-    assert bimap(f_(op.add, 3), f_(op.mul, 7), (5, 7)) == (8, 49)
+    assert bimap(f_("+", 3), f_("*", 7), (5, 7)) == (8, 49)
 
 
 def test_first():
-    assert first(f_(op.add, 3), (5, 7)) == (8, 7)
+    assert first(f_("+", 3), (5, 7)) == (8, 7)
 
 
 def test_second():
-    assert second(f_(op.mul, 7), (5, 7)) == (5, 49)
+    assert second(f_("*", 7), (5, 7)) == (5, 49)
 
 
 def test_iterate():
     assert take(5, iterate(lambda x: x**2, 2)) == [2, 4, 16, 256, 65536]
 
 
 def test_foldl():
-    assert foldl(op.sub, 10, range(1, 5)) == 0
+    assert foldl("-", 10, range(1, 5)) == 0
 
 
 def test_foldr():
-    assert foldr(op.sub, 10, range(1, 5)) == 8
+    assert foldr("-", 10, range(1, 5)) == 8
 
 
 def test_foldl1():
-    assert foldl1(op.sub, range(1, 5)) == -8
+    assert foldl1("-", range(1, 5)) == -8
 
 
 def test_foldr1():
-    assert foldr1(op.sub, range(1, 5)) == -2
+    assert foldr1("-", range(1, 5)) == -2
 
 
 def test_scanl():
-    assert scanl(op.sub, 10, range(1, 5)) == [10, 9, 7, 4, 0]
+    assert scanl("-", 10, range(1, 5)) == [10, 9, 7, 4, 0]
 
 
 def test_scanr():
-    assert scanr(op.sub, 10, range(1, 5)) == [8, -7, 9, -6, 10]
+    assert scanr("-", 10, range(1, 5)) == [8, -7, 9, -6, 10]
 
 
 def test_scanl1():
-    assert scanl1(op.sub, range(1, 5)) == [1, -1, -4, -8]
+    assert scanl1("-", range(1, 5)) == [1, -1, -4, -8]
 
 
 def test_scanr1():
-    assert scanr1(op.sub, range(1, 5)) == [-2, 3, -1, 4]
+    assert scanr1("-", range(1, 5)) == [-2, 3, -1, 4]
 
 
 def test_concatl():
     assert concatl(["sofia", "maria"]) == [
         "s",
         "o",
         "f",
```

