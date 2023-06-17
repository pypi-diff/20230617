# Comparing `tmp/xtuples-0.0.4.tar.gz` & `tmp/xtuples-0.0.5.tar.gz`

## Comparing `xtuples-0.0.4.tar` & `xtuples-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,16 @@
--rw-r--r--   0        0        0   115930 2020-02-02 00:00:00.000000 xtuples-0.0.4/docs/index.html
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 xtuples-0.0.4/src/xtuples/__about__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 xtuples-0.0.4/src/xtuples/__init__.py
--rw-r--r--   0        0        0    23963 2020-02-02 00:00:00.000000 xtuples-0.0.4/src/xtuples/xtuples.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 xtuples-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 xtuples-0.0.4/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 xtuples-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 xtuples-0.0.4/README.md
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 xtuples-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 xtuples-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 xtuples-0.0.5/docs/index.html
+-rw-r--r--   0        0        0   240844 2020-02-02 00:00:00.000000 xtuples-0.0.5/docs/search.js
+-rw-r--r--   0        0        0    36104 2020-02-02 00:00:00.000000 xtuples-0.0.5/docs/xtuples.html
+-rw-r--r--   0        0        0    35654 2020-02-02 00:00:00.000000 xtuples-0.0.5/docs/xtuples/__about__.html
+-rw-r--r--   0        0        0    94700 2020-02-02 00:00:00.000000 xtuples-0.0.5/docs/xtuples/json.html
+-rw-r--r--   0        0        0   541716 2020-02-02 00:00:00.000000 xtuples-0.0.5/docs/xtuples/xtuples.html
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 xtuples-0.0.5/src/xtuples/__about__.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 xtuples-0.0.5/src/xtuples/__init__.py
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 xtuples-0.0.5/src/xtuples/json.py
+-rw-r--r--   0        0        0    19708 2020-02-02 00:00:00.000000 xtuples-0.0.5/src/xtuples/xtuples.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 xtuples-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 xtuples-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 xtuples-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 xtuples-0.0.5/README.md
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 xtuples-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 xtuples-0.0.5/PKG-INFO
```

### Comparing `xtuples-0.0.4/src/xtuples/xtuples.py` & `xtuples-0.0.5/src/xtuples/xtuples.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 
 # ---------------------------------------------------------------
 
-import json
-
 import abc
 import typing
 import dataclasses
 import collections
 
 import operator
 import itertools
@@ -22,28 +20,53 @@
 
 # ---------------------------------------------------------------
 
 REGISTRY = {}
 
 # ---------------------------------------------------------------
 
+def pipe(f, obj, *args, at = None, **kwargs):
+    if at is None:
+        return f(obj, *args, **kwargs)
+    elif isinstance(at, int):
+        return f(*args[:at], obj, *args[at:], **kwargs)
+    elif isinstance(at, str):
+        return f(*args, **{at: obj}, **kwargs)
+    else:
+        assert False, at
+
+# ---------------------------------------------------------------
+
+
 # TODO: some kind of validation placeholder?
 # called in init, eg. quarter in [1 .. 4]
 
 class nTuple(abc.ABC):
 
     @abc.abstractmethod
     def __abstract__(self):
         # NOTE: here to prevent initialise instances of this
         # but rather use the decorator and typing.NamedTuple
         return
 
     @staticmethod
-    def pipe(obj, f, *args, **kwargs):
-        return f(obj, *args, **kwargs)
+    def pipe(obj, f, *args, at = None, **kwargs):
+        """
+        >>> example = Example(1, "a")
+        >>> example.pipe(lambda a, b: a, None)
+        Example(x=1, s='a', it=iTuple())
+        >>> example.pipe(lambda a, b: a, None, at = 1)
+        >>> example.pipe(lambda a, b: a, None, at = 'b')
+        >>> example.pipe(lambda a, b: a, a=None, at = 'b')
+        >>> example.pipe(lambda a, b: a, b=None, at = 'a')
+        Example(x=1, s='a', it=iTuple())
+        >>> example.pipe(lambda a, b: a, None, at = 0)
+        Example(x=1, s='a', it=iTuple())
+        """
+        return pipe(f, obj, *args, at = at, **kwargs)
 
     @staticmethod
     def partial(obj, f, *args, **kwargs):
         return functools.partial(f, obj, *args, **kwargs)
 
     @classmethod
     def is_subclass(cls, t):
@@ -98,44 +121,14 @@
         >>> ex = Example(1, "a")
         >>> ex.pipe(ex.cls.as_dict)
         {'x': 1, 's': 'a', 'it': iTuple()}
         """
         return fDict(obj._asdict())
 
     @classmethod
-    def cast_json(cls, obj):
-        """
-        >>> ex = Example(1, "a")
-        >>> ex.pipe(ex.cls.cast_json)
-        {'x': 1, 's': 'a', 'it': {'__t__': 'iTuple', 'data': []}, '__t__': 'Example'}
-        """
-        d = {
-            k: cast_json(v)
-            for k, v in obj._asdict().items()
-            #
-        }
-        d["__t__"] = type(obj).__name__
-        return d
-
-    @classmethod
-    def uncast_json(meta, obj):
-        """
-        >>> ex = Example(1, "a")
-        >>> ex.cls.uncast_json(ex.pipe(ex.cls.cast_json))
-        Example(x=1, s='a', it=iTuple())
-        """
-        cls = REGISTRY[obj["__t__"]]
-        return cls(
-            *(
-                uncast_json(v)
-                for k, v in obj.items() if k != "__t__"
-            )
-        )
-
-    @classmethod
     def decorate(meta, cls):
         assert cls.__name__ not in REGISTRY
         cls.pipe = meta.pipe
         cls.partial = meta.partial
         cls.cls = meta
         REGISTRY[cls.__name__] = cls
         return cls
@@ -143,22 +136,22 @@
 # ---------------------------------------------------------------
 
 class fDict(collections.UserDict):
     __slots__ = ()
 
     data: dict
 
-    def pipe(self, f, *args, **kwargs):
+    def pipe(self, f, *args, at=None, **kwargs):
         """
         >>> fDict({0: 1}).pipe(lambda d: d.map_values(
         ...     lambda v: v + 1
         ... ))
         {0: 2}
         """
-        res = f(self, *args, **kwargs)
+        res = pipe(f, self, *args, at = at, **kwargs)
         if isinstance(res, dict):
             return fDict(res)
         return res
 
     def partial(self, f, *args, **kwargs):
         """
         >>> f = fDict({0: 1}).partial(
@@ -273,35 +266,14 @@
     def decorate(meta, cls):
         assert cls.__name__ not in REGISTRY
         REGISTRY[cls.__name__] = cls
         return cls
 
     # -----
 
-    def cast_json(self):
-        """
-        >>> iTuple.range(1).cast_json()
-        {'__t__': 'iTuple', 'data': [0]}
-        """
-        return dict(
-            __t__ = type(self).__name__,
-            data = list(self.map(cast_json)),
-        )
-
-    @classmethod
-    def uncast_json(cls, obj):
-        """
-        >>> iTuple.uncast_json(iTuple.range(1).cast_json())
-        iTuple(0)
-        """
-        assert obj["__t__"] == cls.__name__
-        return cls(data=obj["data"])
-
-    # -----
-
     @classmethod
     def range(cls, *args, **kwargs):
         """
         >>> iTuple.range(3)
         iTuple(0, 1, 2)
         """
         return cls(range(*args, **kwargs))
@@ -328,24 +300,24 @@
         >>> iTuple.from_items({i: i + 1 for i in range(2)})
         iTuple((0, 1), (1, 2))
         """
         return cls(d.items())
 
     # -----
 
-    def pipe(self, f, *args, **kwargs):
+    def pipe(self, f, *args, at = None, **kwargs):
         """
         >>> iTuple.range(2).pipe(lambda it: it)
         iTuple(0, 1)
         >>> iTuple.range(2).pipe(
         ...     lambda it, v: it.map(lambda x: x * v), 2
         ... )
         iTuple(0, 2)
         """
-        return f(self, *args, **kwargs)
+        return pipe(f, self, *args, at = at, **kwargs)
 
     def partial(self, f, *args, **kwargs):
         """
         >>> f = iTuple.range(2).partial(
         ...     lambda it, v: it.map(lambda x: x * v)
         ... )
         >>> f(2)
@@ -732,189 +704,29 @@
     s: str
     it: iTuple = iTuple([])
 
     @property
     def cls(self):
         ...
 
-    def pipe(self, f, *args, **kwargs):
+    def pipe(self, f, *args, at = None, **kwargs):
         ...
 
-    def partial(self, f, *args, **kwargs):
+    def partial(self, f, *args, at = None, **kwargs):
         ...
 
 # ---------------------------------------------------------------
 
 # TODO: context manager to control
 # if we add the type information when writing to json or not
 
 # TODO: context mananger to control
 # lazy default behaviour (ie. default to lazy or not)
 
-# ---------------------------------------------------------------
-
-class JSONEncoder(json.JSONEncoder):
-
-    def iterencode(self, o, *args, **kwargs):
-        for chunk in super().iterencode(
-            cast_json(o), *args, **kwargs
-        ):
-            yield chunk
-
-    # def meta_default(self, obj):
-    #     return json.JSONEncoder.default(self, obj)
-
-    # def default(self, obj):
-    #     if isinstance(obj, fDict):
-    #         return self.meta_default(obj.data)
-    #     return cast_json(obj, default=self.meta_default)
-
-# -----
-
-class JSONDecoder(json.JSONDecoder):
-
-    def __init__(self, *args, **kwargs):
-        json.JSONDecoder.__init__(
-            self,
-            object_hook=self.object_hook,
-            *args,
-            **kwargs
-            #
-        )
-
-    @classmethod
-    def xtuple_object_hook(cls, d):
-        return uncast_json(d)
-
-    def object_hook(self, d):
-        return self.xtuple_object_hook(d)
-
-# -----
-
-def cast_json(obj, default = lambda obj: obj):
-    if nTuple.is_instance(obj):
-        return nTuple.cast_json(obj)
-    try:
-        return obj.cast_json()
-    except:
-        return default(obj)
-
-def uncast_json(obj):
-    if not isinstance(obj, dict):
-        return obj
-    __t__ = obj.get("__t__", None)
-    if __t__ is None:
-        return obj
-    cls = iTuple if __t__ == "iTuple" else REGISTRY[__t__]
-    if hasattr(cls, "uncast_json"):
-        return cls.uncast_json(obj)
-    return cls(
-        *(v for k, v in obj.items() if k != "__t__")
-    )
-
-# -----
-
-# TODO: fString so can do .pipe ?
-def to_json(v, **kwargs):
-    """
-    >>> print(iTuple([Example(1, "a")]).pipe(to_json, indent=2))
-    {
-      "__t__": "iTuple",
-      "data": [
-        {
-          "x": 1,
-          "s": "a",
-          "it": {
-            "__t__": "iTuple",
-            "data": []
-          },
-          "__t__": "Example"
-        }
-      ]
-    }
-    >>> print(iTuple([
-    ...     iTuple([Example(1, "a")])
-    ... ]).pipe(to_json, indent=2))
-    {
-      "__t__": "iTuple",
-      "data": [
-        {
-          "__t__": "iTuple",
-          "data": [
-            {
-              "x": 1,
-              "s": "a",
-              "it": {
-                "__t__": "iTuple",
-                "data": []
-              },
-              "__t__": "Example"
-            }
-          ]
-        }
-      ]
-    }
-    >>> print(Example(2, "b", iTuple([
-    ...     iTuple([Example(1, "a")])
-    ... ])).pipe(to_json, indent=2))
-    {
-      "x": 2,
-      "s": "b",
-      "it": {
-        "__t__": "iTuple",
-        "data": [
-          {
-            "__t__": "iTuple",
-            "data": [
-              {
-                "x": 1,
-                "s": "a",
-                "it": {
-                  "__t__": "iTuple",
-                  "data": []
-                },
-                "__t__": "Example"
-              }
-            ]
-          }
-        ]
-      },
-      "__t__": "Example"
-    }
-    """
-    return json.dumps(v, cls=JSONEncoder, **kwargs)
-
-def from_json(v: str, **kwargs):
-    """
-    >>> ex = iTuple([Example(1, "a")])
-    >>> from_json(ex.pipe(to_json))
-    iTuple(Example(x=1, s='a', it=iTuple()))
-    >>> from_json(
-    ...     iTuple([iTuple([Example(1, "a")])]).pipe(to_json)
-    ... )
-    iTuple(iTuple(Example(x=1, s='a', it=iTuple())))
-    >>> from_json(
-    ...     Example(2, "b", iTuple([
-    ...         iTuple([Example(1, "a")])
-    ...     ])).pipe(to_json)
-    ... )
-    Example(x=2, s='b', it=iTuple(iTuple(Example(x=1, s='a', it=iTuple()))))
-    """
-    return json.loads(v, cls=JSONDecoder, **kwargs)
-
-def load_json(f):
-    return json.load(f, cls=JSONDecoder)
-
-def dump_json(f, v):
-    return json.dump(f, v, cls=JSONEncoder)
-
-# ---------------------------------------------------------------
-
 __all__ = [
     "iTuple",
     "nTuple",
     "fDict",
-    "JSONDecoder",
-    "JSONEncoder",
+    "Example",
 ]
 
 # ---------------------------------------------------------------
```

### Comparing `xtuples-0.0.4/.gitignore` & `xtuples-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.4/LICENSE.txt` & `xtuples-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.4/pyproject.toml` & `xtuples-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   "- coverage combine",
   "coverage report",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
-docs = "python -m pdoc --output-dir ./public ./"
+docs = "python -m pdoc --output-dir ./docs ./src/xtuples"
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.9"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
```

