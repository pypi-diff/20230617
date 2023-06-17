# Comparing `tmp/xtuples-0.0.3.tar.gz` & `tmp/xtuples-0.0.4.tar.gz`

## Comparing `xtuples-0.0.3.tar` & `xtuples-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0   130688 2020-02-02 00:00:00.000000 xtuples-0.0.3/docs/xtuples.html
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 xtuples-0.0.3/src/xtuples/__about__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 xtuples-0.0.3/src/xtuples/__init__.py
--rw-r--r--   0        0        0    26321 2020-02-02 00:00:00.000000 xtuples-0.0.3/src/xtuples/xtuples.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 xtuples-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 xtuples-0.0.3/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 xtuples-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 xtuples-0.0.3/README.md
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 xtuples-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 xtuples-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0   115930 2020-02-02 00:00:00.000000 xtuples-0.0.4/docs/index.html
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 xtuples-0.0.4/src/xtuples/__about__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 xtuples-0.0.4/src/xtuples/__init__.py
+-rw-r--r--   0        0        0    23963 2020-02-02 00:00:00.000000 xtuples-0.0.4/src/xtuples/xtuples.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 xtuples-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 xtuples-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 xtuples-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 xtuples-0.0.4/README.md
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 xtuples-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 xtuples-0.0.4/PKG-INFO
```

### Comparing `xtuples-0.0.3/docs/xtuples.html` & `xtuples-0.0.4/docs/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -49,179 +49,14 @@
 
 # ---------------------------------------------------------------
 
 REGISTRY = {}
 
 # ---------------------------------------------------------------
 
-# TODO: context manager to control
-# if we add the type information when writing to json or not
-
-# TODO: context mananger to control
-# lazy default behaviour (ie. default to lazy or not)
-
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
-    __t__ = obj.get(&#34;__t__&#34;, None)
-    if __t__ is None:
-        return obj
-    cls = iTuple if __t__ == &#34;iTuple&#34; else REGISTRY[__t__]
-    if hasattr(cls, &#34;uncast_json&#34;):
-        return cls.uncast_json(obj)
-    return cls(
-        *(v for k, v in obj.items() if k != &#34;__t__&#34;)
-    )
-
-# -----
-
-# TODO: fString so can do .pipe ?
-def to_json(v, **kwargs):
-    &#34;&#34;&#34;
-    &gt;&gt;&gt; print(iTuple([Example(1, &#34;a&#34;)]).pipe(to_json, indent=2))
-    {
-      &#34;__t__&#34;: &#34;iTuple&#34;,
-      &#34;data&#34;: [
-        {
-          &#34;x&#34;: 1,
-          &#34;s&#34;: &#34;a&#34;,
-          &#34;it&#34;: {
-            &#34;__t__&#34;: &#34;iTuple&#34;,
-            &#34;data&#34;: []
-          },
-          &#34;__t__&#34;: &#34;Example&#34;
-        }
-      ]
-    }
-    &gt;&gt;&gt; print(iTuple([
-    ...     iTuple([Example(1, &#34;a&#34;)])
-    ... ]).pipe(to_json, indent=2))
-    {
-      &#34;__t__&#34;: &#34;iTuple&#34;,
-      &#34;data&#34;: [
-        {
-          &#34;__t__&#34;: &#34;iTuple&#34;,
-          &#34;data&#34;: [
-            {
-              &#34;x&#34;: 1,
-              &#34;s&#34;: &#34;a&#34;,
-              &#34;it&#34;: {
-                &#34;__t__&#34;: &#34;iTuple&#34;,
-                &#34;data&#34;: []
-              },
-              &#34;__t__&#34;: &#34;Example&#34;
-            }
-          ]
-        }
-      ]
-    }
-    &gt;&gt;&gt; print(Example(2, &#34;b&#34;, iTuple([
-    ...     iTuple([Example(1, &#34;a&#34;)])
-    ... ])).pipe(to_json, indent=2))
-    {
-      &#34;x&#34;: 2,
-      &#34;s&#34;: &#34;b&#34;,
-      &#34;it&#34;: {
-        &#34;__t__&#34;: &#34;iTuple&#34;,
-        &#34;data&#34;: [
-          {
-            &#34;__t__&#34;: &#34;iTuple&#34;,
-            &#34;data&#34;: [
-              {
-                &#34;x&#34;: 1,
-                &#34;s&#34;: &#34;a&#34;,
-                &#34;it&#34;: {
-                  &#34;__t__&#34;: &#34;iTuple&#34;,
-                  &#34;data&#34;: []
-                },
-                &#34;__t__&#34;: &#34;Example&#34;
-              }
-            ]
-          }
-        ]
-      },
-      &#34;__t__&#34;: &#34;Example&#34;
-    }
-    &#34;&#34;&#34;
-    return json.dumps(v, cls=JSONEncoder, **kwargs)
-
-def from_json(v: str, **kwargs):
-    &#34;&#34;&#34;
-    &gt;&gt;&gt; ex = iTuple([Example(1, &#34;a&#34;)])
-    &gt;&gt;&gt; from_json(ex.pipe(to_json))
-    iTuple(Example(x=1, s=&#39;a&#39;, it=iTuple()))
-    &gt;&gt;&gt; from_json(
-    ...     iTuple([iTuple([Example(1, &#34;a&#34;)])]).pipe(to_json)
-    ... )
-    iTuple(iTuple(Example(x=1, s=&#39;a&#39;, it=iTuple())))
-    &gt;&gt;&gt; from_json(
-    ...     Example(2, &#34;b&#34;, iTuple([
-    ...         iTuple([Example(1, &#34;a&#34;)])
-    ...     ])).pipe(to_json)
-    ... )
-    Example(x=2, s=&#39;b&#39;, it=iTuple(iTuple(Example(x=1, s=&#39;a&#39;, it=iTuple()))))
-    &#34;&#34;&#34;
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
 # TODO: some kind of validation placeholder?
 # called in init, eg. quarter in [1 .. 4]
 
 class nTuple(abc.ABC):
 
     @abc.abstractmethod
     def __abstract__(self):
@@ -932,297 +767,85 @@
         ...
 
     def partial(self, f, *args, **kwargs):
         ...
 
 # ---------------------------------------------------------------
 
-# import misc.perfmon
+# TODO: context manager to control
+# if we add the type information when writing to json or not
 
-# def int_memory_gen(cum=False):
-#     i = 0
-#     while True:
-#         yield i
-#     return
-
-# def dict_memory_gen(cum=False):
-#     i = 0
-#     if cum:
-#         while True:
-#             yield {ii: ii for ii in range(i)}
-#             i += 1
-#     else:
-#         while True:
-#             yield {i: i}
-#             i += 1
-#     return
-
-# def list_memory_gen(cum=False):
-#     i = 0
-#     if cum:
-#         while True:
-#             yield list(range(i))
-#             i += 1
-#     else:
-#         while True:
-#             yield [i]
-#             i += 1
-#     return
-
-# def iTuple_memory_gen(cum=False):
-#     i = 0
-#     if cum:
-#         while True:
-#             yield iTuple(range(i))
-#             i += 1
-#     else:
-#         while True:
-#             yield iTuple([i])
-#             i += 1
-#     return
-
-# print(&#34;int&#34;, misc.perfmon.profile_memory(
-#     int_memory_gen
-# ))
-
-# print(&#34;list&#34;, misc.perfmon.profile_memory(
-#     list_memory_gen
-# ))
-
-# print(&#34;iTuple&#34;, misc.perfmon.profile_memory(
-#     iTuple_memory_gen
-# ))
-
-# print(&#34;list cum&#34;, misc.perfmon.profile_memory(
-#     list_memory_gen, cum=True,
-# ))
-
-# print(&#34;iTuple cum&#34;, misc.perfmon.profile_memory(
-#     iTuple_memory_gen, cum=True,
-# ))
+# TODO: context mananger to control
+# lazy default behaviour (ie. default to lazy or not)
 
 # ---------------------------------------------------------------
 
-# s = S(1)
-# s_parent = S_Parent(s)
-
-# print(s.cls.annotations(s))
-
-# print(s.cls)
-
-# print(s_parent.cast_json())
-
-# print(iTuple([s_parent]).cast_json())
-
-# # ---------------------------------------------------------------
-
-# l = iTuple([s])
-
-# print(l.extend([2]))
-
-# print(l.append(1))
-
-# print(l.map(print))
-
-# # ---------------------------------------------------------------
-
-# print(s.cls)
-
-# print(&#34;Should be true:&#34;, nTuple.is_instance(s))
-# print(&#34;Should be false:&#34;, nTuple.is_subclass(s))
+class JSONEncoder(json.JSONEncoder):
 
-# print(&#34;Should be true:&#34;, nTuple.is_subclass(S))
-# print(&#34;Should be false:&#34;, nTuple.is_instance(S))
+    def iterencode(self, o, *args, **kwargs):
+        for chunk in super().iterencode(
+            cast_json(o), *args, **kwargs
+        ):
+            yield chunk
 
-# ---------------------------------------------------------------
+    # def meta_default(self, obj):
+    #     return json.JSONEncoder.default(self, obj)
 
-# NOTE: i coudl in theory generate sqlalchemy tables
+    # def default(self, obj):
+    #     if isinstance(obj, fDict):
+    #         return self.meta_default(obj.data)
+    #     return cast_json(obj, default=self.meta_default)
 
-# based on the struct definition
+# -----
 
-# joins presumably are then manual?
+class JSONDecoder(json.JSONDecoder):
 
-# with standardised eg. persist methods based on unique keys, etc.
+    def __init__(self, *args, **kwargs):
+        json.JSONDecoder.__init__(
+            self,
+            object_hook=self.object_hook,
+            *args,
+            **kwargs
+            #
+        )
 
-# but any point?
+    @classmethod
+    def xtuple_object_hook(cls, d):
+        return uncast_json(d)
 
-# handle dates as tiny structs?
-# surely prohibitively expensive
+    def object_hook(self, d):
+        return self.xtuple_object_hook(d)
 
-# tuples perhaps not? but still a bit, and all the datetime methods suddenly wouldn&#39;t work.
+# -----
 
-# ---------------------------------------------------------------</code></pre>
-</details>
-</section>
-<section>
-</section>
-<section>
-</section>
-<section>
-<h2 class="section-title" id="header-functions">Functions</h2>
-<dl>
-<dt id="xtuples.cast_json"><code class="name flex">
-<span>def <span class="ident">cast_json</span></span>(<span>obj, default=&lt;function &lt;lambda&gt;&gt;)</span>
-</code></dt>
-<dd>
-<div class="desc"></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def cast_json(obj, default = lambda obj: obj):
+def cast_json(obj, default = lambda obj: obj):
     if nTuple.is_instance(obj):
         return nTuple.cast_json(obj)
     try:
         return obj.cast_json()
     except:
-        return default(obj)</code></pre>
-</details>
-</dd>
-<dt id="xtuples.dump_json"><code class="name flex">
-<span>def <span class="ident">dump_json</span></span>(<span>f, v)</span>
-</code></dt>
-<dd>
-<div class="desc"></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def dump_json(f, v):
-    return json.dump(f, v, cls=JSONEncoder)</code></pre>
-</details>
-</dd>
-<dt id="xtuples.from_json"><code class="name flex">
-<span>def <span class="ident">from_json</span></span>(<span>v: str, **kwargs)</span>
-</code></dt>
-<dd>
-<div class="desc"><pre><code class="language-python-repl">&gt;&gt;&gt; ex = iTuple([Example(1, &quot;a&quot;)])
-&gt;&gt;&gt; from_json(ex.pipe(to_json))
-iTuple(Example(x=1, s='a', it=iTuple()))
-&gt;&gt;&gt; from_json(
-...     iTuple([iTuple([Example(1, &quot;a&quot;)])]).pipe(to_json)
-... )
-iTuple(iTuple(Example(x=1, s='a', it=iTuple())))
-&gt;&gt;&gt; from_json(
-...     Example(2, &quot;b&quot;, iTuple([
-...         iTuple([Example(1, &quot;a&quot;)])
-...     ])).pipe(to_json)
-... )
-Example(x=2, s='b', it=iTuple(iTuple(Example(x=1, s='a', it=iTuple()))))
-</code></pre></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def from_json(v: str, **kwargs):
-    &#34;&#34;&#34;
-    &gt;&gt;&gt; ex = iTuple([Example(1, &#34;a&#34;)])
-    &gt;&gt;&gt; from_json(ex.pipe(to_json))
-    iTuple(Example(x=1, s=&#39;a&#39;, it=iTuple()))
-    &gt;&gt;&gt; from_json(
-    ...     iTuple([iTuple([Example(1, &#34;a&#34;)])]).pipe(to_json)
-    ... )
-    iTuple(iTuple(Example(x=1, s=&#39;a&#39;, it=iTuple())))
-    &gt;&gt;&gt; from_json(
-    ...     Example(2, &#34;b&#34;, iTuple([
-    ...         iTuple([Example(1, &#34;a&#34;)])
-    ...     ])).pipe(to_json)
-    ... )
-    Example(x=2, s=&#39;b&#39;, it=iTuple(iTuple(Example(x=1, s=&#39;a&#39;, it=iTuple()))))
-    &#34;&#34;&#34;
-    return json.loads(v, cls=JSONDecoder, **kwargs)</code></pre>
-</details>
-</dd>
-<dt id="xtuples.load_json"><code class="name flex">
-<span>def <span class="ident">load_json</span></span>(<span>f)</span>
-</code></dt>
-<dd>
-<div class="desc"></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def load_json(f):
-    return json.load(f, cls=JSONDecoder)</code></pre>
-</details>
-</dd>
-<dt id="xtuples.to_json"><code class="name flex">
-<span>def <span class="ident">to_json</span></span>(<span>v, **kwargs)</span>
-</code></dt>
-<dd>
-<div class="desc"><pre><code class="language-python-repl">&gt;&gt;&gt; print(iTuple([Example(1, &quot;a&quot;)]).pipe(to_json, indent=2))
-{
-  &quot;__t__&quot;: &quot;iTuple&quot;,
-  &quot;data&quot;: [
-    {
-      &quot;x&quot;: 1,
-      &quot;s&quot;: &quot;a&quot;,
-      &quot;it&quot;: {
-        &quot;__t__&quot;: &quot;iTuple&quot;,
-        &quot;data&quot;: []
-      },
-      &quot;__t__&quot;: &quot;Example&quot;
-    }
-  ]
-}
-&gt;&gt;&gt; print(iTuple([
-...     iTuple([Example(1, &quot;a&quot;)])
-... ]).pipe(to_json, indent=2))
-{
-  &quot;__t__&quot;: &quot;iTuple&quot;,
-  &quot;data&quot;: [
-    {
-      &quot;__t__&quot;: &quot;iTuple&quot;,
-      &quot;data&quot;: [
-        {
-          &quot;x&quot;: 1,
-          &quot;s&quot;: &quot;a&quot;,
-          &quot;it&quot;: {
-            &quot;__t__&quot;: &quot;iTuple&quot;,
-            &quot;data&quot;: []
-          },
-          &quot;__t__&quot;: &quot;Example&quot;
-        }
-      ]
-    }
-  ]
-}
-&gt;&gt;&gt; print(Example(2, &quot;b&quot;, iTuple([
-...     iTuple([Example(1, &quot;a&quot;)])
-... ])).pipe(to_json, indent=2))
-{
-  &quot;x&quot;: 2,
-  &quot;s&quot;: &quot;b&quot;,
-  &quot;it&quot;: {
-    &quot;__t__&quot;: &quot;iTuple&quot;,
-    &quot;data&quot;: [
-      {
-        &quot;__t__&quot;: &quot;iTuple&quot;,
-        &quot;data&quot;: [
-          {
-            &quot;x&quot;: 1,
-            &quot;s&quot;: &quot;a&quot;,
-            &quot;it&quot;: {
-              &quot;__t__&quot;: &quot;iTuple&quot;,
-              &quot;data&quot;: []
-            },
-            &quot;__t__&quot;: &quot;Example&quot;
-          }
-        ]
-      }
-    ]
-  },
-  &quot;__t__&quot;: &quot;Example&quot;
-}
-</code></pre></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def to_json(v, **kwargs):
+        return default(obj)
+
+def uncast_json(obj):
+    if not isinstance(obj, dict):
+        return obj
+    __t__ = obj.get(&#34;__t__&#34;, None)
+    if __t__ is None:
+        return obj
+    cls = iTuple if __t__ == &#34;iTuple&#34; else REGISTRY[__t__]
+    if hasattr(cls, &#34;uncast_json&#34;):
+        return cls.uncast_json(obj)
+    return cls(
+        *(v for k, v in obj.items() if k != &#34;__t__&#34;)
+    )
+
+# -----
+
+# TODO: fString so can do .pipe ?
+def to_json(v, **kwargs):
     &#34;&#34;&#34;
     &gt;&gt;&gt; print(iTuple([Example(1, &#34;a&#34;)]).pipe(to_json, indent=2))
     {
       &#34;__t__&#34;: &#34;iTuple&#34;,
       &#34;data&#34;: [
         {
           &#34;x&#34;: 1,
@@ -1281,158 +904,62 @@
             ]
           }
         ]
       },
       &#34;__t__&#34;: &#34;Example&#34;
     }
     &#34;&#34;&#34;
-    return json.dumps(v, cls=JSONEncoder, **kwargs)</code></pre>
-</details>
-</dd>
-<dt id="xtuples.uncast_json"><code class="name flex">
-<span>def <span class="ident">uncast_json</span></span>(<span>obj)</span>
-</code></dt>
-<dd>
-<div class="desc"></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def uncast_json(obj):
-    if not isinstance(obj, dict):
-        return obj
-    __t__ = obj.get(&#34;__t__&#34;, None)
-    if __t__ is None:
-        return obj
-    cls = iTuple if __t__ == &#34;iTuple&#34; else REGISTRY[__t__]
-    if hasattr(cls, &#34;uncast_json&#34;):
-        return cls.uncast_json(obj)
-    return cls(
-        *(v for k, v in obj.items() if k != &#34;__t__&#34;)
-    )</code></pre>
-</details>
-</dd>
-</dl>
-</section>
-<section>
-<h2 class="section-title" id="header-classes">Classes</h2>
-<dl>
-<dt id="xtuples.Example"><code class="flex name class">
-<span>class <span class="ident">Example</span></span>
-<span>(</span><span>x: int, s: str, it: <a title="xtuples.iTuple" href="#xtuples.iTuple">iTuple</a> = iTuple())</span>
-</code></dt>
-<dd>
-<div class="desc"><pre><code class="language-python-repl">&gt;&gt;&gt; ex = Example(1, &quot;a&quot;)
-&gt;&gt;&gt; ex
-Example(x=1, s='a', it=iTuple())
-&gt;&gt;&gt; ex.cls
-&lt;class 'xtuples.xtuples.nTuple'&gt;
-&gt;&gt;&gt; ex.pipe(lambda nt: nt.x)
-1
-&gt;&gt;&gt; f = ex.partial(lambda nt, v: nt.x * v)
-&gt;&gt;&gt; f(2)
-2
-&gt;&gt;&gt; f(3)
-3
-</code></pre></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">@nTuple.decorate
-class Example(typing.NamedTuple):
+    return json.dumps(v, cls=JSONEncoder, **kwargs)
+
+def from_json(v: str, **kwargs):
     &#34;&#34;&#34;
-    &gt;&gt;&gt; ex = Example(1, &#34;a&#34;)
-    &gt;&gt;&gt; ex
-    Example(x=1, s=&#39;a&#39;, it=iTuple())
-    &gt;&gt;&gt; ex.cls
-    &lt;class &#39;xtuples.xtuples.nTuple&#39;&gt;
-    &gt;&gt;&gt; ex.pipe(lambda nt: nt.x)
-    1
-    &gt;&gt;&gt; f = ex.partial(lambda nt, v: nt.x * v)
-    &gt;&gt;&gt; f(2)
-    2
-    &gt;&gt;&gt; f(3)
-    3
+    &gt;&gt;&gt; ex = iTuple([Example(1, &#34;a&#34;)])
+    &gt;&gt;&gt; from_json(ex.pipe(to_json))
+    iTuple(Example(x=1, s=&#39;a&#39;, it=iTuple()))
+    &gt;&gt;&gt; from_json(
+    ...     iTuple([iTuple([Example(1, &#34;a&#34;)])]).pipe(to_json)
+    ... )
+    iTuple(iTuple(Example(x=1, s=&#39;a&#39;, it=iTuple())))
+    &gt;&gt;&gt; from_json(
+    ...     Example(2, &#34;b&#34;, iTuple([
+    ...         iTuple([Example(1, &#34;a&#34;)])
+    ...     ])).pipe(to_json)
+    ... )
+    Example(x=2, s=&#39;b&#39;, it=iTuple(iTuple(Example(x=1, s=&#39;a&#39;, it=iTuple()))))
     &#34;&#34;&#34;
-    # NOTE: cls, pipe, partial are mandatory boilerplate
+    return json.loads(v, cls=JSONDecoder, **kwargs)
 
-    x: int
-    s: str
-    it: iTuple = iTuple([])
+def load_json(f):
+    return json.load(f, cls=JSONDecoder)
 
-    @property
-    def cls(self):
-        ...
+def dump_json(f, v):
+    return json.dump(f, v, cls=JSONEncoder)
 
-    def pipe(self, f, *args, **kwargs):
-        ...
+# ---------------------------------------------------------------
 
-    def partial(self, f, *args, **kwargs):
-        ...</code></pre>
+__all__ = [
+    &#34;iTuple&#34;,
+    &#34;nTuple&#34;,
+    &#34;fDict&#34;,
+    &#34;JSONDecoder&#34;,
+    &#34;JSONEncoder&#34;,
+]
+
+# ---------------------------------------------------------------</code></pre>
 </details>
-<h3>Ancestors</h3>
-<ul class="hlist">
-<li>builtins.tuple</li>
-</ul>
-<h3>Class variables</h3>
-<dl>
-<dt id="xtuples.Example.cls"><code class="name">var <span class="ident">cls</span></code></dt>
-<dd>
-<div class="desc"><p>Helper class that provides a standard way to create an ABC using
-inheritance.</p></div>
-</dd>
-</dl>
-<h3>Instance variables</h3>
-<dl>
-<dt id="xtuples.Example.it"><code class="name">var <span class="ident">it</span> : <a title="xtuples.iTuple" href="#xtuples.iTuple">iTuple</a></code></dt>
-<dd>
-<div class="desc"><p>Alias for field number 2</p></div>
-</dd>
-<dt id="xtuples.Example.s"><code class="name">var <span class="ident">s</span> : str</code></dt>
-<dd>
-<div class="desc"><p>Alias for field number 1</p></div>
-</dd>
-<dt id="xtuples.Example.x"><code class="name">var <span class="ident">x</span> : int</code></dt>
-<dd>
-<div class="desc"><p>Alias for field number 0</p></div>
-</dd>
-</dl>
-<h3>Methods</h3>
+</section>
+<section>
+</section>
+<section>
+</section>
+<section>
+</section>
+<section>
+<h2 class="section-title" id="header-classes">Classes</h2>
 <dl>
-<dt id="xtuples.Example.partial"><code class="name flex">
-<span>def <span class="ident">partial</span></span>(<span>obj, f, *args, **kwargs)</span>
-</code></dt>
-<dd>
-<div class="desc"></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">@staticmethod
-def partial(obj, f, *args, **kwargs):
-    return functools.partial(f, obj, *args, **kwargs)</code></pre>
-</details>
-</dd>
-<dt id="xtuples.Example.pipe"><code class="name flex">
-<span>def <span class="ident">pipe</span></span>(<span>obj, f, *args, **kwargs)</span>
-</code></dt>
-<dd>
-<div class="desc"></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">@staticmethod
-def pipe(obj, f, *args, **kwargs):
-    return f(obj, *args, **kwargs)</code></pre>
-</details>
-</dd>
-</dl>
-</dd>
 <dt id="xtuples.JSONDecoder"><code class="flex name class">
 <span>class <span class="ident">JSONDecoder</span></span>
 <span>(</span><span>*args, **kwargs)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Simple JSON <a href="http://json.org">http://json.org</a> decoder</p>
 <p>Performs the following translations in decoding by default:</p>
@@ -3805,38 +3332,17 @@
 </article>
 <nav id="sidebar">
 <h1>Index</h1>
 <div class="toc">
 <ul></ul>
 </div>
 <ul id="index">
-<li><h3><a href="#header-functions">Functions</a></h3>
-<ul class="two-column">
-<li><code><a title="xtuples.cast_json" href="#xtuples.cast_json">cast_json</a></code></li>
-<li><code><a title="xtuples.dump_json" href="#xtuples.dump_json">dump_json</a></code></li>
-<li><code><a title="xtuples.from_json" href="#xtuples.from_json">from_json</a></code></li>
-<li><code><a title="xtuples.load_json" href="#xtuples.load_json">load_json</a></code></li>
-<li><code><a title="xtuples.to_json" href="#xtuples.to_json">to_json</a></code></li>
-<li><code><a title="xtuples.uncast_json" href="#xtuples.uncast_json">uncast_json</a></code></li>
-</ul>
-</li>
 <li><h3><a href="#header-classes">Classes</a></h3>
 <ul>
 <li>
-<h4><code><a title="xtuples.Example" href="#xtuples.Example">Example</a></code></h4>
-<ul class="two-column">
-<li><code><a title="xtuples.Example.cls" href="#xtuples.Example.cls">cls</a></code></li>
-<li><code><a title="xtuples.Example.it" href="#xtuples.Example.it">it</a></code></li>
-<li><code><a title="xtuples.Example.partial" href="#xtuples.Example.partial">partial</a></code></li>
-<li><code><a title="xtuples.Example.pipe" href="#xtuples.Example.pipe">pipe</a></code></li>
-<li><code><a title="xtuples.Example.s" href="#xtuples.Example.s">s</a></code></li>
-<li><code><a title="xtuples.Example.x" href="#xtuples.Example.x">x</a></code></li>
-</ul>
-</li>
-<li>
 <h4><code><a title="xtuples.JSONDecoder" href="#xtuples.JSONDecoder">JSONDecoder</a></code></h4>
 <ul class="">
 <li><code><a title="xtuples.JSONDecoder.object_hook" href="#xtuples.JSONDecoder.object_hook">object_hook</a></code></li>
 <li><code><a title="xtuples.JSONDecoder.xtuple_object_hook" href="#xtuples.JSONDecoder.xtuple_object_hook">xtuple_object_hook</a></code></li>
 </ul>
 </li>
 <li>
```

#### html2text {}

```diff
@@ -30,179 +30,14 @@
 
 # ---------------------------------------------------------------
 
 REGISTRY = {}
 
 # ---------------------------------------------------------------
 
-# TODO: context manager to control
-# if we add the type information when writing to json or not
-
-# TODO: context mananger to control
-# lazy default behaviour (ie. default to lazy or not)
-
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
 # TODO: some kind of validation placeholder?
 # called in init, eg. quarter in [1 .. 4]
 
 class nTuple(abc.ABC):
 
     @abc.abstractmethod
     def __abstract__(self):
@@ -915,401 +750,190 @@
         ...
 
     def partial(self, f, *args, **kwargs):
         ...
 
 # ---------------------------------------------------------------
 
-# import misc.perfmon
+# TODO: context manager to control
+# if we add the type information when writing to json or not
 
-# def int_memory_gen(cum=False):
-#     i = 0
-#     while True:
-#         yield i
-#     return
-
-# def dict_memory_gen(cum=False):
-#     i = 0
-#     if cum:
-#         while True:
-#             yield {ii: ii for ii in range(i)}
-#             i += 1
-#     else:
-#         while True:
-#             yield {i: i}
-#             i += 1
-#     return
-
-# def list_memory_gen(cum=False):
-#     i = 0
-#     if cum:
-#         while True:
-#             yield list(range(i))
-#             i += 1
-#     else:
-#         while True:
-#             yield [i]
-#             i += 1
-#     return
-
-# def iTuple_memory_gen(cum=False):
-#     i = 0
-#     if cum:
-#         while True:
-#             yield iTuple(range(i))
-#             i += 1
-#     else:
-#         while True:
-#             yield iTuple([i])
-#             i += 1
-#     return
-
-# print("int", misc.perfmon.profile_memory(
-#     int_memory_gen
-# ))
-
-# print("list", misc.perfmon.profile_memory(
-#     list_memory_gen
-# ))
-
-# print("iTuple", misc.perfmon.profile_memory(
-#     iTuple_memory_gen
-# ))
-
-# print("list cum", misc.perfmon.profile_memory(
-#     list_memory_gen, cum=True,
-# ))
-
-# print("iTuple cum", misc.perfmon.profile_memory(
-#     iTuple_memory_gen, cum=True,
-# ))
+# TODO: context mananger to control
+# lazy default behaviour (ie. default to lazy or not)
 
 # ---------------------------------------------------------------
 
-# s = S(1)
-# s_parent = S_Parent(s)
-
-# print(s.cls.annotations(s))
-
-# print(s.cls)
-
-# print(s_parent.cast_json())
-
-# print(iTuple([s_parent]).cast_json())
-
-# # ---------------------------------------------------------------
-
-# l = iTuple([s])
-
-# print(l.extend([2]))
-
-# print(l.append(1))
-
-# print(l.map(print))
-
-# # ---------------------------------------------------------------
+class JSONEncoder(json.JSONEncoder):
 
-# print(s.cls)
+    def iterencode(self, o, *args, **kwargs):
+        for chunk in super().iterencode(
+            cast_json(o), *args, **kwargs
+        ):
+            yield chunk
 
-# print("Should be true:", nTuple.is_instance(s))
-# print("Should be false:", nTuple.is_subclass(s))
+    # def meta_default(self, obj):
+    #     return json.JSONEncoder.default(self, obj)
 
-# print("Should be true:", nTuple.is_subclass(S))
-# print("Should be false:", nTuple.is_instance(S))
+    # def default(self, obj):
+    #     if isinstance(obj, fDict):
+    #         return self.meta_default(obj.data)
+    #     return cast_json(obj, default=self.meta_default)
 
-# ---------------------------------------------------------------
+# -----
 
-# NOTE: i coudl in theory generate sqlalchemy tables
+class JSONDecoder(json.JSONDecoder):
 
-# based on the struct definition
+    def __init__(self, *args, **kwargs):
+        json.JSONDecoder.__init__(
+            self,
+            object_hook=self.object_hook,
+            *args,
+            **kwargs
+            #
+        )
 
-# joins presumably are then manual?
+    @classmethod
+    def xtuple_object_hook(cls, d):
+        return uncast_json(d)
 
-# with standardised eg. persist methods based on unique keys, etc.
+    def object_hook(self, d):
+        return self.xtuple_object_hook(d)
 
-# but any point?
+# -----
 
-# handle dates as tiny structs?
-# surely prohibitively expensive
+def cast_json(obj, default = lambda obj: obj):
+    if nTuple.is_instance(obj):
+        return nTuple.cast_json(obj)
+    try:
+        return obj.cast_json()
+    except:
+        return default(obj)
 
-# tuples perhaps not? but still a bit, and all the datetime methods suddenly
-wouldn't work.
+def uncast_json(obj):
+    if not isinstance(obj, dict):
+        return obj
+    __t__ = obj.get("__t__", None)
+    if __t__ is None:
+        return obj
+    cls = iTuple if __t__ == "iTuple" else REGISTRY[__t__]
+    if hasattr(cls, "uncast_json"):
+        return cls.uncast_json(obj)
+    return cls(
+        *(v for k, v in obj.items() if k != "__t__")
+    )
 
-# ---------------------------------------------------------------
+# -----
 
-***** Functions *****
-  def cast_json(obj, default=<function <lambda>>)
-        Expand source code
-      def cast_json(obj, default = lambda obj: obj):
-          if nTuple.is_instance(obj):
-              return nTuple.cast_json(obj)
-          try:
-              return obj.cast_json()
-          except:
-              return default(obj)
-  def dump_json(f, v)
-        Expand source code
-      def dump_json(f, v):
-          return json.dump(f, v, cls=JSONEncoder)
-  def from_json(v:Â str, **kwargs)
-      >>> ex = iTuple([Example(1, "a")])
-      >>> from_json(ex.pipe(to_json))
-      iTuple(Example(x=1, s='a', it=iTuple()))
-      >>> from_json(
-      ...     iTuple([iTuple([Example(1, "a")])]).pipe(to_json)
-      ... )
-      iTuple(iTuple(Example(x=1, s='a', it=iTuple())))
-      >>> from_json(
-      ...     Example(2, "b", iTuple([
-      ...         iTuple([Example(1, "a")])
-      ...     ])).pipe(to_json)
-      ... )
-      Example(x=2, s='b', it=iTuple(iTuple(Example(x=1, s='a', it=iTuple()))))
-        Expand source code
-      def from_json(v: str, **kwargs):
-          """
-          >>> ex = iTuple([Example(1, "a")])
-          >>> from_json(ex.pipe(to_json))
-          iTuple(Example(x=1, s='a', it=iTuple()))
-          >>> from_json(
-          ...     iTuple([iTuple([Example(1, "a")])]).pipe(to_json)
-          ... )
-          iTuple(iTuple(Example(x=1, s='a', it=iTuple())))
-          >>> from_json(
-          ...     Example(2, "b", iTuple([
-          ...         iTuple([Example(1, "a")])
-          ...     ])).pipe(to_json)
-          ... )
-          Example(x=2, s='b', it=iTuple(iTuple(Example(x=1, s='a', it=iTuple
-      ()))))
-          """
-          return json.loads(v, cls=JSONDecoder, **kwargs)
-  def load_json(f)
-        Expand source code
-      def load_json(f):
-          return json.load(f, cls=JSONDecoder)
-  def to_json(v, **kwargs)
-      >>> print(iTuple([Example(1, "a")]).pipe(to_json, indent=2))
-      {
-        "__t__": "iTuple",
-        "data": [
-          {
-            "x": 1,
-            "s": "a",
-            "it": {
-              "__t__": "iTuple",
-              "data": []
-            },
-            "__t__": "Example"
-          }
-        ]
-      }
-      >>> print(iTuple([
-      ...     iTuple([Example(1, "a")])
-      ... ]).pipe(to_json, indent=2))
-      {
-        "__t__": "iTuple",
-        "data": [
-          {
+# TODO: fString so can do .pipe ?
+def to_json(v, **kwargs):
+    """
+    >>> print(iTuple([Example(1, "a")]).pipe(to_json, indent=2))
+    {
+      "__t__": "iTuple",
+      "data": [
+        {
+          "x": 1,
+          "s": "a",
+          "it": {
             "__t__": "iTuple",
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
-      }
-      >>> print(Example(2, "b", iTuple([
-      ...     iTuple([Example(1, "a")])
-      ... ])).pipe(to_json, indent=2))
-      {
-        "x": 2,
-        "s": "b",
-        "it": {
+            "data": []
+          },
+          "__t__": "Example"
+        }
+      ]
+    }
+    >>> print(iTuple([
+    ...     iTuple([Example(1, "a")])
+    ... ]).pipe(to_json, indent=2))
+    {
+      "__t__": "iTuple",
+      "data": [
+        {
           "__t__": "iTuple",
           "data": [
             {
-              "__t__": "iTuple",
-              "data": [
-                {
-                  "x": 1,
-                  "s": "a",
-                  "it": {
-                    "__t__": "iTuple",
-                    "data": []
-                  },
-                  "__t__": "Example"
-                }
-              ]
+              "x": 1,
+              "s": "a",
+              "it": {
+                "__t__": "iTuple",
+                "data": []
+              },
+              "__t__": "Example"
             }
           ]
-        },
-        "__t__": "Example"
-      }
-        Expand source code
-      def to_json(v, **kwargs):
-          """
-          >>> print(iTuple([Example(1, "a")]).pipe(to_json, indent=2))
+        }
+      ]
+    }
+    >>> print(Example(2, "b", iTuple([
+    ...     iTuple([Example(1, "a")])
+    ... ])).pipe(to_json, indent=2))
+    {
+      "x": 2,
+      "s": "b",
+      "it": {
+        "__t__": "iTuple",
+        "data": [
           {
             "__t__": "iTuple",
             "data": [
               {
                 "x": 1,
                 "s": "a",
                 "it": {
                   "__t__": "iTuple",
                   "data": []
                 },
                 "__t__": "Example"
               }
             ]
           }
-          >>> print(iTuple([
-          ...     iTuple([Example(1, "a")])
-          ... ]).pipe(to_json, indent=2))
-          {
-            "__t__": "iTuple",
-            "data": [
-              {
-                "__t__": "iTuple",
-                "data": [
-                  {
-                    "x": 1,
-                    "s": "a",
-                    "it": {
-                      "__t__": "iTuple",
-                      "data": []
-                    },
-                    "__t__": "Example"
-                  }
-                ]
-              }
-            ]
-          }
-          >>> print(Example(2, "b", iTuple([
-          ...     iTuple([Example(1, "a")])
-          ... ])).pipe(to_json, indent=2))
-          {
-            "x": 2,
-            "s": "b",
-            "it": {
-              "__t__": "iTuple",
-              "data": [
-                {
-                  "__t__": "iTuple",
-                  "data": [
-                    {
-                      "x": 1,
-                      "s": "a",
-                      "it": {
-                        "__t__": "iTuple",
-                        "data": []
-                      },
-                      "__t__": "Example"
-                    }
-                  ]
-                }
-              ]
-            },
-            "__t__": "Example"
-          }
-          """
-          return json.dumps(v, cls=JSONEncoder, **kwargs)
-  def uncast_json(obj)
-        Expand source code
-      def uncast_json(obj):
-          if not isinstance(obj, dict):
-              return obj
-          __t__ = obj.get("__t__", None)
-          if __t__ is None:
-              return obj
-          cls = iTuple if __t__ == "iTuple" else REGISTRY[__t__]
-          if hasattr(cls, "uncast_json"):
-              return cls.uncast_json(obj)
-          return cls(
-              *(v for k, v in obj.items() if k != "__t__")
-          )
+        ]
+      },
+      "__t__": "Example"
+    }
+    """
+    return json.dumps(v, cls=JSONEncoder, **kwargs)
 
-***** Classes *****
-  class Example (x:Â int, s:Â str, it:Â iTupleÂ =Â iTuple())
-      >>> ex = Example(1, "a")
-      >>> ex
-      Example(x=1, s='a', it=iTuple())
-      >>> ex.cls
-      <class 'xtuples.xtuples.nTuple'>
-      >>> ex.pipe(lambda nt: nt.x)
-      1
-      >>> f = ex.partial(lambda nt, v: nt.x * v)
-      >>> f(2)
-      2
-      >>> f(3)
-      3
-        Expand source code
-      @nTuple.decorate
-      class Example(typing.NamedTuple):
-          """
-          >>> ex = Example(1, "a")
-          >>> ex
-          Example(x=1, s='a', it=iTuple())
-          >>> ex.cls
-          <class 'xtuples.xtuples.nTuple'>
-          >>> ex.pipe(lambda nt: nt.x)
-          1
-          >>> f = ex.partial(lambda nt, v: nt.x * v)
-          >>> f(2)
-          2
-          >>> f(3)
-          3
-          """
-          # NOTE: cls, pipe, partial are mandatory boilerplate
-
-          x: int
-          s: str
-          it: iTuple = iTuple([])
-
-          @property
-          def cls(self):
-              ...
+def from_json(v: str, **kwargs):
+    """
+    >>> ex = iTuple([Example(1, "a")])
+    >>> from_json(ex.pipe(to_json))
+    iTuple(Example(x=1, s='a', it=iTuple()))
+    >>> from_json(
+    ...     iTuple([iTuple([Example(1, "a")])]).pipe(to_json)
+    ... )
+    iTuple(iTuple(Example(x=1, s='a', it=iTuple())))
+    >>> from_json(
+    ...     Example(2, "b", iTuple([
+    ...         iTuple([Example(1, "a")])
+    ...     ])).pipe(to_json)
+    ... )
+    Example(x=2, s='b', it=iTuple(iTuple(Example(x=1, s='a', it=iTuple()))))
+    """
+    return json.loads(v, cls=JSONDecoder, **kwargs)
 
-          def pipe(self, f, *args, **kwargs):
-              ...
+def load_json(f):
+    return json.load(f, cls=JSONDecoder)
 
-          def partial(self, f, *args, **kwargs):
-              ...
-      **** Ancestors ****
-          * builtins.tuple
-      **** Class variables ****
-        var cls
-            Helper class that provides a standard way to create an ABC using
-            inheritance.
-      **** Instance variables ****
-        var it :Â iTuple
-            Alias for field number 2
-        var s :Â str
-            Alias for field number 1
-        var x :Â int
-            Alias for field number 0
-      **** Methods ****
-        def partial(obj, f, *args, **kwargs)
-              Expand source code
-            @staticmethod
-            def partial(obj, f, *args, **kwargs):
-                return functools.partial(f, obj, *args, **kwargs)
-        def pipe(obj, f, *args, **kwargs)
-              Expand source code
-            @staticmethod
-            def pipe(obj, f, *args, **kwargs):
-                return f(obj, *args, **kwargs)
+def dump_json(f, v):
+    return json.dump(f, v, cls=JSONEncoder)
+
+# ---------------------------------------------------------------
+
+__all__ = [
+    "iTuple",
+    "nTuple",
+    "fDict",
+    "JSONDecoder",
+    "JSONEncoder",
+]
+
+# ---------------------------------------------------------------
+
+***** Classes *****
   class JSONDecoder (*args, **kwargs)
       Simple JSON http://json.org decoder
       Performs the following translations in decoding by default:
       +---------------+-------------------+ | JSON | Python |
       +===============+===================+ | object | dict | +---------------
       +-------------------+ | array | list | +---------------+-----------------
       --+ | string | str | +---------------+-------------------+ | number (int)
@@ -2995,29 +2619,15 @@
                     *(
                         uncast_json(v)
                         for k, v in obj.items() if k != "__t__"
                     )
                 )
 
 ****** Index ******
-    * **** Functions ****
-          o cast_json
-          o dump_json
-          o from_json
-          o load_json
-          o to_json
-          o uncast_json
     * **** Classes ****
-          o *** Example ***
-                # cls
-                # it
-                # partial
-                # pipe
-                # s
-                # x
           o *** JSONDecoder ***
                 # object_hook
                 # xtuple_object_hook
           o *** JSONEncoder ***
                 # iterencode
           o *** fDict ***
                 # data
```

### Comparing `xtuples-0.0.3/src/xtuples/xtuples.py` & `xtuples-0.0.4/src/xtuples/xtuples.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,1612 +35,1464 @@
 00000220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000230: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a 5245  ----------....RE
 00000240: 4749 5354 5259 203d 207b 7d0d 0a0d 0a23  GISTRY = {}....#
 00000250: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
 00000260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000290: 0d0a 0d0a 2320 544f 444f 3a20 636f 6e74  ....# TODO: cont
-000002a0: 6578 7420 6d61 6e61 6765 7220 746f 2063  ext manager to c
-000002b0: 6f6e 7472 6f6c 0d0a 2320 6966 2077 6520  ontrol..# if we 
-000002c0: 6164 6420 7468 6520 7479 7065 2069 6e66  add the type inf
-000002d0: 6f72 6d61 7469 6f6e 2077 6865 6e20 7772  ormation when wr
-000002e0: 6974 696e 6720 746f 206a 736f 6e20 6f72  iting to json or
-000002f0: 206e 6f74 0d0a 0d0a 2320 544f 444f 3a20   not....# TODO: 
-00000300: 636f 6e74 6578 7420 6d61 6e61 6e67 6572  context mananger
-00000310: 2074 6f20 636f 6e74 726f 6c0d 0a23 206c   to control..# l
-00000320: 617a 7920 6465 6661 756c 7420 6265 6861  azy default beha
-00000330: 7669 6f75 7220 2869 652e 2064 6566 6175  viour (ie. defau
-00000340: 6c74 2074 6f20 6c61 7a79 206f 7220 6e6f  lt to lazy or no
-00000350: 7429 0d0a 0d0a 2320 2d2d 2d2d 2d2d 2d2d  t)....# --------
-00000360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000390: 2d2d 2d2d 2d2d 2d0d 0a0d 0a63 6c61 7373  -------....class
-000003a0: 204a 534f 4e45 6e63 6f64 6572 286a 736f   JSONEncoder(jso
-000003b0: 6e2e 4a53 4f4e 456e 636f 6465 7229 3a0d  n.JSONEncoder):.
-000003c0: 0a0d 0a20 2020 2064 6566 2069 7465 7265  ...    def itere
-000003d0: 6e63 6f64 6528 7365 6c66 2c20 6f2c 202a  ncode(self, o, *
-000003e0: 6172 6773 2c20 2a2a 6b77 6172 6773 293a  args, **kwargs):
-000003f0: 0d0a 2020 2020 2020 2020 666f 7220 6368  ..        for ch
-00000400: 756e 6b20 696e 2073 7570 6572 2829 2e69  unk in super().i
-00000410: 7465 7265 6e63 6f64 6528 0d0a 2020 2020  terencode(..    
-00000420: 2020 2020 2020 2020 6361 7374 5f6a 736f          cast_jso
-00000430: 6e28 6f29 2c20 2a61 7267 732c 202a 2a6b  n(o), *args, **k
-00000440: 7761 7267 730d 0a20 2020 2020 2020 2029  wargs..        )
-00000450: 3a0d 0a20 2020 2020 2020 2020 2020 2079  :..            y
-00000460: 6965 6c64 2063 6875 6e6b 0d0a 0d0a 2020  ield chunk....  
-00000470: 2020 2320 6465 6620 6d65 7461 5f64 6566    # def meta_def
-00000480: 6175 6c74 2873 656c 662c 206f 626a 293a  ault(self, obj):
-00000490: 0d0a 2020 2020 2320 2020 2020 7265 7475  ..    #     retu
-000004a0: 726e 206a 736f 6e2e 4a53 4f4e 456e 636f  rn json.JSONEnco
-000004b0: 6465 722e 6465 6661 756c 7428 7365 6c66  der.default(self
-000004c0: 2c20 6f62 6a29 0d0a 0d0a 2020 2020 2320  , obj)....    # 
-000004d0: 6465 6620 6465 6661 756c 7428 7365 6c66  def default(self
-000004e0: 2c20 6f62 6a29 3a0d 0a20 2020 2023 2020  , obj):..    #  
-000004f0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00000500: 286f 626a 2c20 6644 6963 7429 3a0d 0a20  (obj, fDict):.. 
-00000510: 2020 2023 2020 2020 2020 2020 2072 6574     #         ret
-00000520: 7572 6e20 7365 6c66 2e6d 6574 615f 6465  urn self.meta_de
-00000530: 6661 756c 7428 6f62 6a2e 6461 7461 290d  fault(obj.data).
-00000540: 0a20 2020 2023 2020 2020 2072 6574 7572  .    #     retur
-00000550: 6e20 6361 7374 5f6a 736f 6e28 6f62 6a2c  n cast_json(obj,
-00000560: 2064 6566 6175 6c74 3d73 656c 662e 6d65   default=self.me
-00000570: 7461 5f64 6566 6175 6c74 290d 0a0d 0a23  ta_default)....#
-00000580: 202d 2d2d 2d2d 0d0a 0d0a 636c 6173 7320   -----....class 
-00000590: 4a53 4f4e 4465 636f 6465 7228 6a73 6f6e  JSONDecoder(json
-000005a0: 2e4a 534f 4e44 6563 6f64 6572 293a 0d0a  .JSONDecoder):..
-000005b0: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-000005c0: 5f5f 2873 656c 662c 202a 6172 6773 2c20  __(self, *args, 
-000005d0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
-000005e0: 2020 2020 6a73 6f6e 2e4a 534f 4e44 6563      json.JSONDec
-000005f0: 6f64 6572 2e5f 5f69 6e69 745f 5f28 0d0a  oder.__init__(..
-00000600: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00000610: 2c0d 0a20 2020 2020 2020 2020 2020 206f  ,..            o
-00000620: 626a 6563 745f 686f 6f6b 3d73 656c 662e  bject_hook=self.
-00000630: 6f62 6a65 6374 5f68 6f6f 6b2c 0d0a 2020  object_hook,..  
-00000640: 2020 2020 2020 2020 2020 2a61 7267 732c            *args,
-00000650: 0d0a 2020 2020 2020 2020 2020 2020 2a2a  ..            **
-00000660: 6b77 6172 6773 0d0a 2020 2020 2020 2020  kwargs..        
-00000670: 2020 2020 230d 0a20 2020 2020 2020 2029      #..        )
-00000680: 0d0a 0d0a 2020 2020 4063 6c61 7373 6d65  ....    @classme
-00000690: 7468 6f64 0d0a 2020 2020 6465 6620 7874  thod..    def xt
-000006a0: 7570 6c65 5f6f 626a 6563 745f 686f 6f6b  uple_object_hook
-000006b0: 2863 6c73 2c20 6429 3a0d 0a20 2020 2020  (cls, d):..     
-000006c0: 2020 2072 6574 7572 6e20 756e 6361 7374     return uncast
-000006d0: 5f6a 736f 6e28 6429 0d0a 0d0a 2020 2020  _json(d)....    
-000006e0: 6465 6620 6f62 6a65 6374 5f68 6f6f 6b28  def object_hook(
-000006f0: 7365 6c66 2c20 6429 3a0d 0a20 2020 2020  self, d):..     
-00000700: 2020 2072 6574 7572 6e20 7365 6c66 2e78     return self.x
-00000710: 7475 706c 655f 6f62 6a65 6374 5f68 6f6f  tuple_object_hoo
-00000720: 6b28 6429 0d0a 0d0a 2320 2d2d 2d2d 2d0d  k(d)....# -----.
-00000730: 0a0d 0a64 6566 2063 6173 745f 6a73 6f6e  ...def cast_json
-00000740: 286f 626a 2c20 6465 6661 756c 7420 3d20  (obj, default = 
-00000750: 6c61 6d62 6461 206f 626a 3a20 6f62 6a29  lambda obj: obj)
-00000760: 3a0d 0a20 2020 2069 6620 6e54 7570 6c65  :..    if nTuple
-00000770: 2e69 735f 696e 7374 616e 6365 286f 626a  .is_instance(obj
-00000780: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
-00000790: 726e 206e 5475 706c 652e 6361 7374 5f6a  rn nTuple.cast_j
-000007a0: 736f 6e28 6f62 6a29 0d0a 2020 2020 7472  son(obj)..    tr
-000007b0: 793a 0d0a 2020 2020 2020 2020 7265 7475  y:..        retu
-000007c0: 726e 206f 626a 2e63 6173 745f 6a73 6f6e  rn obj.cast_json
-000007d0: 2829 0d0a 2020 2020 6578 6365 7074 3a0d  ()..    except:.
-000007e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000007f0: 6465 6661 756c 7428 6f62 6a29 0d0a 0d0a  default(obj)....
-00000800: 6465 6620 756e 6361 7374 5f6a 736f 6e28  def uncast_json(
-00000810: 6f62 6a29 3a0d 0a20 2020 2069 6620 6e6f  obj):..    if no
-00000820: 7420 6973 696e 7374 616e 6365 286f 626a  t isinstance(obj
-00000830: 2c20 6469 6374 293a 0d0a 2020 2020 2020  , dict):..      
-00000840: 2020 7265 7475 726e 206f 626a 0d0a 2020    return obj..  
-00000850: 2020 5f5f 745f 5f20 3d20 6f62 6a2e 6765    __t__ = obj.ge
-00000860: 7428 225f 5f74 5f5f 222c 204e 6f6e 6529  t("__t__", None)
-00000870: 0d0a 2020 2020 6966 205f 5f74 5f5f 2069  ..    if __t__ i
-00000880: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00000890: 2072 6574 7572 6e20 6f62 6a0d 0a20 2020   return obj..   
-000008a0: 2063 6c73 203d 2069 5475 706c 6520 6966   cls = iTuple if
-000008b0: 205f 5f74 5f5f 203d 3d20 2269 5475 706c   __t__ == "iTupl
-000008c0: 6522 2065 6c73 6520 5245 4749 5354 5259  e" else REGISTRY
-000008d0: 5b5f 5f74 5f5f 5d0d 0a20 2020 2069 6620  [__t__]..    if 
-000008e0: 6861 7361 7474 7228 636c 732c 2022 756e  hasattr(cls, "un
-000008f0: 6361 7374 5f6a 736f 6e22 293a 0d0a 2020  cast_json"):..  
-00000900: 2020 2020 2020 7265 7475 726e 2063 6c73        return cls
-00000910: 2e75 6e63 6173 745f 6a73 6f6e 286f 626a  .uncast_json(obj
-00000920: 290d 0a20 2020 2072 6574 7572 6e20 636c  )..    return cl
-00000930: 7328 0d0a 2020 2020 2020 2020 2a28 7620  s(..        *(v 
-00000940: 666f 7220 6b2c 2076 2069 6e20 6f62 6a2e  for k, v in obj.
-00000950: 6974 656d 7328 2920 6966 206b 2021 3d20  items() if k != 
-00000960: 225f 5f74 5f5f 2229 0d0a 2020 2020 290d  "__t__")..    ).
-00000970: 0a0d 0a23 202d 2d2d 2d2d 0d0a 0d0a 2320  ...# -----....# 
-00000980: 544f 444f 3a20 6653 7472 696e 6720 736f  TODO: fString so
-00000990: 2063 616e 2064 6f20 2e70 6970 6520 3f0d   can do .pipe ?.
-000009a0: 0a64 6566 2074 6f5f 6a73 6f6e 2876 2c20  .def to_json(v, 
-000009b0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
-000009c0: 2222 220d 0a20 2020 203e 3e3e 2070 7269  """..    >>> pri
-000009d0: 6e74 2869 5475 706c 6528 5b45 7861 6d70  nt(iTuple([Examp
-000009e0: 6c65 2831 2c20 2261 2229 5d29 2e70 6970  le(1, "a")]).pip
-000009f0: 6528 746f 5f6a 736f 6e2c 2069 6e64 656e  e(to_json, inden
-00000a00: 743d 3229 290d 0a20 2020 207b 0d0a 2020  t=2))..    {..  
-00000a10: 2020 2020 225f 5f74 5f5f 223a 2022 6954      "__t__": "iT
-00000a20: 7570 6c65 222c 0d0a 2020 2020 2020 2264  uple",..      "d
-00000a30: 6174 6122 3a20 5b0d 0a20 2020 2020 2020  ata": [..       
-00000a40: 207b 0d0a 2020 2020 2020 2020 2020 2278   {..          "x
-00000a50: 223a 2031 2c0d 0a20 2020 2020 2020 2020  ": 1,..         
-00000a60: 2022 7322 3a20 2261 222c 0d0a 2020 2020   "s": "a",..    
-00000a70: 2020 2020 2020 2269 7422 3a20 7b0d 0a20        "it": {.. 
-00000a80: 2020 2020 2020 2020 2020 2022 5f5f 745f             "__t_
-00000a90: 5f22 3a20 2269 5475 706c 6522 2c0d 0a20  _": "iTuple",.. 
-00000aa0: 2020 2020 2020 2020 2020 2022 6461 7461             "data
-00000ab0: 223a 205b 5d0d 0a20 2020 2020 2020 2020  ": []..         
-00000ac0: 207d 2c0d 0a20 2020 2020 2020 2020 2022   },..          "
-00000ad0: 5f5f 745f 5f22 3a20 2245 7861 6d70 6c65  __t__": "Example
-00000ae0: 220d 0a20 2020 2020 2020 207d 0d0a 2020  "..        }..  
-00000af0: 2020 2020 5d0d 0a20 2020 207d 0d0a 2020      ]..    }..  
-00000b00: 2020 3e3e 3e20 7072 696e 7428 6954 7570    >>> print(iTup
-00000b10: 6c65 285b 0d0a 2020 2020 2e2e 2e20 2020  le([..    ...   
-00000b20: 2020 6954 7570 6c65 285b 4578 616d 706c    iTuple([Exampl
-00000b30: 6528 312c 2022 6122 295d 290d 0a20 2020  e(1, "a")])..   
-00000b40: 202e 2e2e 205d 292e 7069 7065 2874 6f5f   ... ]).pipe(to_
-00000b50: 6a73 6f6e 2c20 696e 6465 6e74 3d32 2929  json, indent=2))
-00000b60: 0d0a 2020 2020 7b0d 0a20 2020 2020 2022  ..    {..      "
-00000b70: 5f5f 745f 5f22 3a20 2269 5475 706c 6522  __t__": "iTuple"
-00000b80: 2c0d 0a20 2020 2020 2022 6461 7461 223a  ,..      "data":
-00000b90: 205b 0d0a 2020 2020 2020 2020 7b0d 0a20   [..        {.. 
-00000ba0: 2020 2020 2020 2020 2022 5f5f 745f 5f22           "__t__"
-00000bb0: 3a20 2269 5475 706c 6522 2c0d 0a20 2020  : "iTuple",..   
-00000bc0: 2020 2020 2020 2022 6461 7461 223a 205b         "data": [
-00000bd0: 0d0a 2020 2020 2020 2020 2020 2020 7b0d  ..            {.
-00000be0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00000bf0: 7822 3a20 312c 0d0a 2020 2020 2020 2020  x": 1,..        
-00000c00: 2020 2020 2020 2273 223a 2022 6122 2c0d        "s": "a",.
-00000c10: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00000c20: 6974 223a 207b 0d0a 2020 2020 2020 2020  it": {..        
-00000c30: 2020 2020 2020 2020 225f 5f74 5f5f 223a          "__t__":
-00000c40: 2022 6954 7570 6c65 222c 0d0a 2020 2020   "iTuple",..    
-00000c50: 2020 2020 2020 2020 2020 2020 2264 6174              "dat
-00000c60: 6122 3a20 5b5d 0d0a 2020 2020 2020 2020  a": []..        
-00000c70: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
-00000c80: 2020 2020 2020 2020 225f 5f74 5f5f 223a          "__t__":
-00000c90: 2022 4578 616d 706c 6522 0d0a 2020 2020   "Example"..    
-00000ca0: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-00000cb0: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
-00000cc0: 7d0d 0a20 2020 2020 205d 0d0a 2020 2020  }..      ]..    
-00000cd0: 7d0d 0a20 2020 203e 3e3e 2070 7269 6e74  }..    >>> print
-00000ce0: 2845 7861 6d70 6c65 2832 2c20 2262 222c  (Example(2, "b",
-00000cf0: 2069 5475 706c 6528 5b0d 0a20 2020 202e   iTuple([..    .
-00000d00: 2e2e 2020 2020 2069 5475 706c 6528 5b45  ..     iTuple([E
-00000d10: 7861 6d70 6c65 2831 2c20 2261 2229 5d29  xample(1, "a")])
-00000d20: 0d0a 2020 2020 2e2e 2e20 5d29 292e 7069  ..    ... ])).pi
-00000d30: 7065 2874 6f5f 6a73 6f6e 2c20 696e 6465  pe(to_json, inde
-00000d40: 6e74 3d32 2929 0d0a 2020 2020 7b0d 0a20  nt=2))..    {.. 
-00000d50: 2020 2020 2022 7822 3a20 322c 0d0a 2020       "x": 2,..  
-00000d60: 2020 2020 2273 223a 2022 6222 2c0d 0a20      "s": "b",.. 
-00000d70: 2020 2020 2022 6974 223a 207b 0d0a 2020       "it": {..  
-00000d80: 2020 2020 2020 225f 5f74 5f5f 223a 2022        "__t__": "
-00000d90: 6954 7570 6c65 222c 0d0a 2020 2020 2020  iTuple",..      
-00000da0: 2020 2264 6174 6122 3a20 5b0d 0a20 2020    "data": [..   
-00000db0: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00000dc0: 2020 2020 2020 225f 5f74 5f5f 223a 2022        "__t__": "
-00000dd0: 6954 7570 6c65 222c 0d0a 2020 2020 2020  iTuple",..      
-00000de0: 2020 2020 2020 2264 6174 6122 3a20 5b0d        "data": [.
-00000df0: 0a20 2020 2020 2020 2020 2020 2020 207b  .              {
-00000e00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000e10: 2020 2278 223a 2031 2c0d 0a20 2020 2020    "x": 1,..     
-00000e20: 2020 2020 2020 2020 2020 2022 7322 3a20             "s": 
-00000e30: 2261 222c 0d0a 2020 2020 2020 2020 2020  "a",..          
-00000e40: 2020 2020 2020 2269 7422 3a20 7b0d 0a20        "it": {.. 
-00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e60: 2022 5f5f 745f 5f22 3a20 2269 5475 706c   "__t__": "iTupl
-00000e70: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
-00000e80: 2020 2020 2020 2022 6461 7461 223a 205b         "data": [
-00000e90: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00000ea0: 2020 207d 2c0d 0a20 2020 2020 2020 2020     },..         
-00000eb0: 2020 2020 2020 2022 5f5f 745f 5f22 3a20         "__t__": 
-00000ec0: 2245 7861 6d70 6c65 220d 0a20 2020 2020  "Example"..     
-00000ed0: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-00000ee0: 2020 2020 2020 2020 5d0d 0a20 2020 2020          ]..     
-00000ef0: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00000f00: 5d0d 0a20 2020 2020 207d 2c0d 0a20 2020  ]..      },..   
-00000f10: 2020 2022 5f5f 745f 5f22 3a20 2245 7861     "__t__": "Exa
-00000f20: 6d70 6c65 220d 0a20 2020 207d 0d0a 2020  mple"..    }..  
-00000f30: 2020 2222 220d 0a20 2020 2072 6574 7572    """..    retur
-00000f40: 6e20 6a73 6f6e 2e64 756d 7073 2876 2c20  n json.dumps(v, 
-00000f50: 636c 733d 4a53 4f4e 456e 636f 6465 722c  cls=JSONEncoder,
-00000f60: 202a 2a6b 7761 7267 7329 0d0a 0d0a 6465   **kwargs)....de
-00000f70: 6620 6672 6f6d 5f6a 736f 6e28 763a 2073  f from_json(v: s
-00000f80: 7472 2c20 2a2a 6b77 6172 6773 293a 0d0a  tr, **kwargs):..
-00000f90: 2020 2020 2222 220d 0a20 2020 203e 3e3e      """..    >>>
-00000fa0: 2065 7820 3d20 6954 7570 6c65 285b 4578   ex = iTuple([Ex
-00000fb0: 616d 706c 6528 312c 2022 6122 295d 290d  ample(1, "a")]).
-00000fc0: 0a20 2020 203e 3e3e 2066 726f 6d5f 6a73  .    >>> from_js
-00000fd0: 6f6e 2865 782e 7069 7065 2874 6f5f 6a73  on(ex.pipe(to_js
-00000fe0: 6f6e 2929 0d0a 2020 2020 6954 7570 6c65  on))..    iTuple
-00000ff0: 2845 7861 6d70 6c65 2878 3d31 2c20 733d  (Example(x=1, s=
-00001000: 2761 272c 2069 743d 6954 7570 6c65 2829  'a', it=iTuple()
-00001010: 2929 0d0a 2020 2020 3e3e 3e20 6672 6f6d  ))..    >>> from
-00001020: 5f6a 736f 6e28 0d0a 2020 2020 2e2e 2e20  _json(..    ... 
-00001030: 2020 2020 6954 7570 6c65 285b 6954 7570      iTuple([iTup
-00001040: 6c65 285b 4578 616d 706c 6528 312c 2022  le([Example(1, "
-00001050: 6122 295d 295d 292e 7069 7065 2874 6f5f  a")])]).pipe(to_
-00001060: 6a73 6f6e 290d 0a20 2020 202e 2e2e 2029  json)..    ... )
-00001070: 0d0a 2020 2020 6954 7570 6c65 2869 5475  ..    iTuple(iTu
-00001080: 706c 6528 4578 616d 706c 6528 783d 312c  ple(Example(x=1,
-00001090: 2073 3d27 6127 2c20 6974 3d69 5475 706c   s='a', it=iTupl
-000010a0: 6528 2929 2929 0d0a 2020 2020 3e3e 3e20  e())))..    >>> 
-000010b0: 6672 6f6d 5f6a 736f 6e28 0d0a 2020 2020  from_json(..    
-000010c0: 2e2e 2e20 2020 2020 4578 616d 706c 6528  ...     Example(
-000010d0: 322c 2022 6222 2c20 6954 7570 6c65 285b  2, "b", iTuple([
-000010e0: 0d0a 2020 2020 2e2e 2e20 2020 2020 2020  ..    ...       
-000010f0: 2020 6954 7570 6c65 285b 4578 616d 706c    iTuple([Exampl
-00001100: 6528 312c 2022 6122 295d 290d 0a20 2020  e(1, "a")])..   
-00001110: 202e 2e2e 2020 2020 205d 2929 2e70 6970   ...     ])).pip
-00001120: 6528 746f 5f6a 736f 6e29 0d0a 2020 2020  e(to_json)..    
-00001130: 2e2e 2e20 290d 0a20 2020 2045 7861 6d70  ... )..    Examp
-00001140: 6c65 2878 3d32 2c20 733d 2762 272c 2069  le(x=2, s='b', i
-00001150: 743d 6954 7570 6c65 2869 5475 706c 6528  t=iTuple(iTuple(
-00001160: 4578 616d 706c 6528 783d 312c 2073 3d27  Example(x=1, s='
-00001170: 6127 2c20 6974 3d69 5475 706c 6528 2929  a', it=iTuple())
-00001180: 2929 290d 0a20 2020 2022 2222 0d0a 2020  )))..    """..  
-00001190: 2020 7265 7475 726e 206a 736f 6e2e 6c6f    return json.lo
-000011a0: 6164 7328 762c 2063 6c73 3d4a 534f 4e44  ads(v, cls=JSOND
-000011b0: 6563 6f64 6572 2c20 2a2a 6b77 6172 6773  ecoder, **kwargs
-000011c0: 290d 0a0d 0a64 6566 206c 6f61 645f 6a73  )....def load_js
-000011d0: 6f6e 2866 293a 0d0a 2020 2020 7265 7475  on(f):..    retu
-000011e0: 726e 206a 736f 6e2e 6c6f 6164 2866 2c20  rn json.load(f, 
-000011f0: 636c 733d 4a53 4f4e 4465 636f 6465 7229  cls=JSONDecoder)
-00001200: 0d0a 0d0a 6465 6620 6475 6d70 5f6a 736f  ....def dump_jso
-00001210: 6e28 662c 2076 293a 0d0a 2020 2020 7265  n(f, v):..    re
-00001220: 7475 726e 206a 736f 6e2e 6475 6d70 2866  turn json.dump(f
-00001230: 2c20 762c 2063 6c73 3d4a 534f 4e45 6e63  , v, cls=JSONEnc
-00001240: 6f64 6572 290d 0a0d 0a23 202d 2d2d 2d2d  oder)....# -----
-00001250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001280: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a 2320  ----------....# 
-00001290: 544f 444f 3a20 736f 6d65 206b 696e 6420  TODO: some kind 
-000012a0: 6f66 2076 616c 6964 6174 696f 6e20 706c  of validation pl
-000012b0: 6163 6568 6f6c 6465 723f 0d0a 2320 6361  aceholder?..# ca
-000012c0: 6c6c 6564 2069 6e20 696e 6974 2c20 6567  lled in init, eg
-000012d0: 2e20 7175 6172 7465 7220 696e 205b 3120  . quarter in [1 
-000012e0: 2e2e 2034 5d0d 0a0d 0a63 6c61 7373 206e  .. 4]....class n
-000012f0: 5475 706c 6528 6162 632e 4142 4329 3a0d  Tuple(abc.ABC):.
-00001300: 0a0d 0a20 2020 2040 6162 632e 6162 7374  ...    @abc.abst
-00001310: 7261 6374 6d65 7468 6f64 0d0a 2020 2020  ractmethod..    
-00001320: 6465 6620 5f5f 6162 7374 7261 6374 5f5f  def __abstract__
-00001330: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00001340: 2023 204e 4f54 453a 2068 6572 6520 746f   # NOTE: here to
-00001350: 2070 7265 7665 6e74 2069 6e69 7469 616c   prevent initial
-00001360: 6973 6520 696e 7374 616e 6365 7320 6f66  ise instances of
-00001370: 2074 6869 730d 0a20 2020 2020 2020 2023   this..        #
-00001380: 2062 7574 2072 6174 6865 7220 7573 6520   but rather use 
-00001390: 7468 6520 6465 636f 7261 746f 7220 616e  the decorator an
-000013a0: 6420 7479 7069 6e67 2e4e 616d 6564 5475  d typing.NamedTu
-000013b0: 706c 650d 0a20 2020 2020 2020 2072 6574  ple..        ret
-000013c0: 7572 6e0d 0a0d 0a20 2020 2040 7374 6174  urn....    @stat
-000013d0: 6963 6d65 7468 6f64 0d0a 2020 2020 6465  icmethod..    de
-000013e0: 6620 7069 7065 286f 626a 2c20 662c 202a  f pipe(obj, f, *
-000013f0: 6172 6773 2c20 2a2a 6b77 6172 6773 293a  args, **kwargs):
-00001400: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00001410: 2066 286f 626a 2c20 2a61 7267 732c 202a   f(obj, *args, *
-00001420: 2a6b 7761 7267 7329 0d0a 0d0a 2020 2020  *kwargs)....    
-00001430: 4073 7461 7469 636d 6574 686f 640d 0a20  @staticmethod.. 
-00001440: 2020 2064 6566 2070 6172 7469 616c 286f     def partial(o
-00001450: 626a 2c20 662c 202a 6172 6773 2c20 2a2a  bj, f, *args, **
-00001460: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
-00001470: 2020 7265 7475 726e 2066 756e 6374 6f6f    return functoo
-00001480: 6c73 2e70 6172 7469 616c 2866 2c20 6f62  ls.partial(f, ob
-00001490: 6a2c 202a 6172 6773 2c20 2a2a 6b77 6172  j, *args, **kwar
-000014a0: 6773 290d 0a0d 0a20 2020 2040 636c 6173  gs)....    @clas
-000014b0: 736d 6574 686f 640d 0a20 2020 2064 6566  smethod..    def
-000014c0: 2069 735f 7375 6263 6c61 7373 2863 6c73   is_subclass(cls
-000014d0: 2c20 7429 3a0d 0a20 2020 2020 2020 2022  , t):..        "
-000014e0: 2222 0d0a 2020 2020 2020 2020 3e3e 3e20  ""..        >>> 
-000014f0: 6e54 7570 6c65 2e69 735f 7375 6263 6c61  nTuple.is_subcla
-00001500: 7373 2874 7570 6c65 290d 0a20 2020 2020  ss(tuple)..     
-00001510: 2020 2046 616c 7365 0d0a 2020 2020 2020     False..      
-00001520: 2020 3e3e 3e20 6e54 7570 6c65 2e69 735f    >>> nTuple.is_
-00001530: 7375 6263 6c61 7373 2845 7861 6d70 6c65  subclass(Example
-00001540: 2831 2c20 2261 2229 290d 0a20 2020 2020  (1, "a"))..     
-00001550: 2020 2046 616c 7365 0d0a 2020 2020 2020     False..      
-00001560: 2020 3e3e 3e20 6e54 7570 6c65 2e69 735f    >>> nTuple.is_
-00001570: 7375 6263 6c61 7373 2845 7861 6d70 6c65  subclass(Example
-00001580: 290d 0a20 2020 2020 2020 2054 7275 650d  )..        True.
-00001590: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-000015a0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-000015b0: 2020 2020 2020 2020 6973 5f73 7562 203d          is_sub =
-000015c0: 2069 7373 7562 636c 6173 7328 742c 2074   issubclass(t, t
-000015d0: 7570 6c65 290d 0a20 2020 2020 2020 2065  uple)..        e
-000015e0: 7863 6570 743a 0d0a 2020 2020 2020 2020  xcept:..        
-000015f0: 2020 2020 6973 5f73 7562 203d 2046 616c      is_sub = Fal
-00001600: 7365 0d0a 2020 2020 2020 2020 7265 7475  se..        retu
-00001610: 726e 2028 0d0a 2020 2020 2020 2020 2020  rn (..          
-00001620: 2020 6973 5f73 7562 2061 6e64 0d0a 2020    is_sub and..  
-00001630: 2020 2020 2020 2020 2020 6861 7361 7474            hasatt
-00001640: 7228 742c 2022 636c 7322 2920 616e 640d  r(t, "cls") and.
-00001650: 0a20 2020 2020 2020 2020 2020 2068 6173  .            has
-00001660: 6174 7472 2874 2c20 2270 6970 6522 2920  attr(t, "pipe") 
-00001670: 616e 640d 0a20 2020 2020 2020 2020 2020  and..           
-00001680: 2068 6173 6174 7472 2874 2c20 2270 6172   hasattr(t, "par
-00001690: 7469 616c 2229 0d0a 2020 2020 2020 2020  tial")..        
-000016a0: 290d 0a0d 0a20 2020 2040 636c 6173 736d  )....    @classm
-000016b0: 6574 686f 640d 0a20 2020 2064 6566 2069  ethod..    def i
-000016c0: 735f 696e 7374 616e 6365 2863 6c73 2c20  s_instance(cls, 
-000016d0: 6f62 6a29 3a0d 0a20 2020 2020 2020 2022  obj):..        "
-000016e0: 2222 0d0a 2020 2020 2020 2020 3e3e 3e20  ""..        >>> 
-000016f0: 6e54 7570 6c65 2e69 735f 696e 7374 616e  nTuple.is_instan
-00001700: 6365 2874 7570 6c65 290d 0a20 2020 2020  ce(tuple)..     
-00001710: 2020 2046 616c 7365 0d0a 2020 2020 2020     False..      
-00001720: 2020 3e3e 3e20 6e54 7570 6c65 2e69 735f    >>> nTuple.is_
-00001730: 696e 7374 616e 6365 2845 7861 6d70 6c65  instance(Example
-00001740: 290d 0a20 2020 2020 2020 2046 616c 7365  )..        False
-00001750: 0d0a 2020 2020 2020 2020 3e3e 3e20 6e54  ..        >>> nT
-00001760: 7570 6c65 2e69 735f 696e 7374 616e 6365  uple.is_instance
-00001770: 2845 7861 6d70 6c65 2831 2c20 2261 2229  (Example(1, "a")
-00001780: 290d 0a20 2020 2020 2020 2054 7275 650d  )..        True.
-00001790: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-000017a0: 2020 2020 2020 7265 7475 726e 2028 0d0a        return (..
-000017b0: 2020 2020 2020 2020 2020 2020 636c 732e              cls.
-000017c0: 6973 5f73 7562 636c 6173 7328 7479 7065  is_subclass(type
-000017d0: 286f 626a 2929 2061 6e64 0d0a 2020 2020  (obj)) and..    
-000017e0: 2020 2020 2020 2020 6861 7361 7474 7228          hasattr(
-000017f0: 6f62 6a2c 2027 5f61 7364 6963 7427 2920  obj, '_asdict') 
-00001800: 616e 640d 0a20 2020 2020 2020 2020 2020  and..           
-00001810: 2068 6173 6174 7472 286f 626a 2c20 275f   hasattr(obj, '_
-00001820: 6669 656c 6473 2729 0d0a 2020 2020 2020  fields')..      
-00001830: 2020 290d 0a0d 0a0d 0a20 2020 2040 7374    )......    @st
-00001840: 6174 6963 6d65 7468 6f64 0d0a 2020 2020  aticmethod..    
-00001850: 6465 6620 616e 6e6f 7461 7469 6f6e 7328  def annotations(
-00001860: 6f62 6a29 3a0d 0a20 2020 2020 2020 2022  obj):..        "
-00001870: 2222 0d0a 2020 2020 2020 2020 3e3e 3e20  ""..        >>> 
-00001880: 6578 203d 2045 7861 6d70 6c65 2831 2c20  ex = Example(1, 
-00001890: 2261 2229 0d0a 2020 2020 2020 2020 3e3e  "a")..        >>
-000018a0: 3e20 6578 2e70 6970 6528 6578 2e63 6c73  > ex.pipe(ex.cls
-000018b0: 2e61 6e6e 6f74 6174 696f 6e73 290d 0a20  .annotations).. 
-000018c0: 2020 2020 2020 207b 2778 273a 203c 636c         {'x': <cl
-000018d0: 6173 7320 2769 6e74 273e 2c20 2773 273a  ass 'int'>, 's':
-000018e0: 203c 636c 6173 7320 2773 7472 273e 2c20   <class 'str'>, 
-000018f0: 2769 7427 3a20 3c63 6c61 7373 2027 7874  'it': <class 'xt
-00001900: 7570 6c65 732e 7874 7570 6c65 732e 6954  uples.xtuples.iT
-00001910: 7570 6c65 273e 7d0d 0a20 2020 2020 2020  uple'>}..       
-00001920: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
-00001930: 7475 726e 2066 4469 6374 286f 626a 2e5f  turn fDict(obj._
-00001940: 5f61 6e6e 6f74 6174 696f 6e73 5f5f 290d  _annotations__).
-00001950: 0a0d 0a20 2020 2040 636c 6173 736d 6574  ...    @classmet
-00001960: 686f 640d 0a20 2020 2064 6566 2061 735f  hod..    def as_
-00001970: 6469 6374 2863 6c73 2c20 6f62 6a29 3a0d  dict(cls, obj):.
-00001980: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00001990: 2020 2020 2020 3e3e 3e20 6578 203d 2045        >>> ex = E
-000019a0: 7861 6d70 6c65 2831 2c20 2261 2229 0d0a  xample(1, "a")..
-000019b0: 2020 2020 2020 2020 3e3e 3e20 6578 2e70          >>> ex.p
-000019c0: 6970 6528 6578 2e63 6c73 2e61 735f 6469  ipe(ex.cls.as_di
-000019d0: 6374 290d 0a20 2020 2020 2020 207b 2778  ct)..        {'x
-000019e0: 273a 2031 2c20 2773 273a 2027 6127 2c20  ': 1, 's': 'a', 
-000019f0: 2769 7427 3a20 6954 7570 6c65 2829 7d0d  'it': iTuple()}.
-00001a00: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00001a10: 2020 2020 2020 7265 7475 726e 2066 4469        return fDi
-00001a20: 6374 286f 626a 2e5f 6173 6469 6374 2829  ct(obj._asdict()
-00001a30: 290d 0a0d 0a20 2020 2040 636c 6173 736d  )....    @classm
-00001a40: 6574 686f 640d 0a20 2020 2064 6566 2063  ethod..    def c
-00001a50: 6173 745f 6a73 6f6e 2863 6c73 2c20 6f62  ast_json(cls, ob
-00001a60: 6a29 3a0d 0a20 2020 2020 2020 2022 2222  j):..        """
-00001a70: 0d0a 2020 2020 2020 2020 3e3e 3e20 6578  ..        >>> ex
-00001a80: 203d 2045 7861 6d70 6c65 2831 2c20 2261   = Example(1, "a
-00001a90: 2229 0d0a 2020 2020 2020 2020 3e3e 3e20  ")..        >>> 
-00001aa0: 6578 2e70 6970 6528 6578 2e63 6c73 2e63  ex.pipe(ex.cls.c
-00001ab0: 6173 745f 6a73 6f6e 290d 0a20 2020 2020  ast_json)..     
-00001ac0: 2020 207b 2778 273a 2031 2c20 2773 273a     {'x': 1, 's':
-00001ad0: 2027 6127 2c20 2769 7427 3a20 7b27 5f5f   'a', 'it': {'__
-00001ae0: 745f 5f27 3a20 2769 5475 706c 6527 2c20  t__': 'iTuple', 
-00001af0: 2764 6174 6127 3a20 5b5d 7d2c 2027 5f5f  'data': []}, '__
-00001b00: 745f 5f27 3a20 2745 7861 6d70 6c65 277d  t__': 'Example'}
-00001b10: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00001b20: 2020 2020 2020 2064 203d 207b 0d0a 2020         d = {..  
-00001b30: 2020 2020 2020 2020 2020 6b3a 2063 6173            k: cas
-00001b40: 745f 6a73 6f6e 2876 290d 0a20 2020 2020  t_json(v)..     
-00001b50: 2020 2020 2020 2066 6f72 206b 2c20 7620         for k, v 
-00001b60: 696e 206f 626a 2e5f 6173 6469 6374 2829  in obj._asdict()
-00001b70: 2e69 7465 6d73 2829 0d0a 2020 2020 2020  .items()..      
-00001b80: 2020 2020 2020 230d 0a20 2020 2020 2020        #..       
-00001b90: 207d 0d0a 2020 2020 2020 2020 645b 225f   }..        d["_
-00001ba0: 5f74 5f5f 225d 203d 2074 7970 6528 6f62  _t__"] = type(ob
-00001bb0: 6a29 2e5f 5f6e 616d 655f 5f0d 0a20 2020  j).__name__..   
-00001bc0: 2020 2020 2072 6574 7572 6e20 640d 0a0d       return d...
-00001bd0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00001be0: 640d 0a20 2020 2064 6566 2075 6e63 6173  d..    def uncas
-00001bf0: 745f 6a73 6f6e 286d 6574 612c 206f 626a  t_json(meta, obj
-00001c00: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
-00001c10: 0a20 2020 2020 2020 203e 3e3e 2065 7820  .        >>> ex 
-00001c20: 3d20 4578 616d 706c 6528 312c 2022 6122  = Example(1, "a"
-00001c30: 290d 0a20 2020 2020 2020 203e 3e3e 2065  )..        >>> e
-00001c40: 782e 636c 732e 756e 6361 7374 5f6a 736f  x.cls.uncast_jso
-00001c50: 6e28 6578 2e70 6970 6528 6578 2e63 6c73  n(ex.pipe(ex.cls
-00001c60: 2e63 6173 745f 6a73 6f6e 2929 0d0a 2020  .cast_json))..  
-00001c70: 2020 2020 2020 4578 616d 706c 6528 783d        Example(x=
-00001c80: 312c 2073 3d27 6127 2c20 6974 3d69 5475  1, s='a', it=iTu
-00001c90: 706c 6528 2929 0d0a 2020 2020 2020 2020  ple())..        
-00001ca0: 2222 220d 0a20 2020 2020 2020 2063 6c73  """..        cls
-00001cb0: 203d 2052 4547 4953 5452 595b 6f62 6a5b   = REGISTRY[obj[
-00001cc0: 225f 5f74 5f5f 225d 5d0d 0a20 2020 2020  "__t__"]]..     
-00001cd0: 2020 2072 6574 7572 6e20 636c 7328 0d0a     return cls(..
-00001ce0: 2020 2020 2020 2020 2020 2020 2a28 0d0a              *(..
-00001cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d00: 756e 6361 7374 5f6a 736f 6e28 7629 0d0a  uncast_json(v)..
-00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d20: 666f 7220 6b2c 2076 2069 6e20 6f62 6a2e  for k, v in obj.
-00001d30: 6974 656d 7328 2920 6966 206b 2021 3d20  items() if k != 
-00001d40: 225f 5f74 5f5f 220d 0a20 2020 2020 2020  "__t__"..       
-00001d50: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00001d60: 290d 0a0d 0a20 2020 2040 636c 6173 736d  )....    @classm
-00001d70: 6574 686f 640d 0a20 2020 2064 6566 2064  ethod..    def d
-00001d80: 6563 6f72 6174 6528 6d65 7461 2c20 636c  ecorate(meta, cl
-00001d90: 7329 3a0d 0a20 2020 2020 2020 2061 7373  s):..        ass
-00001da0: 6572 7420 636c 732e 5f5f 6e61 6d65 5f5f  ert cls.__name__
-00001db0: 206e 6f74 2069 6e20 5245 4749 5354 5259   not in REGISTRY
-00001dc0: 0d0a 2020 2020 2020 2020 636c 732e 7069  ..        cls.pi
-00001dd0: 7065 203d 206d 6574 612e 7069 7065 0d0a  pe = meta.pipe..
-00001de0: 2020 2020 2020 2020 636c 732e 7061 7274          cls.part
-00001df0: 6961 6c20 3d20 6d65 7461 2e70 6172 7469  ial = meta.parti
-00001e00: 616c 0d0a 2020 2020 2020 2020 636c 732e  al..        cls.
-00001e10: 636c 7320 3d20 6d65 7461 0d0a 2020 2020  cls = meta..    
-00001e20: 2020 2020 5245 4749 5354 5259 5b63 6c73      REGISTRY[cls
-00001e30: 2e5f 5f6e 616d 655f 5f5d 203d 2063 6c73  .__name__] = cls
-00001e40: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00001e50: 2063 6c73 0d0a 0d0a 2320 2d2d 2d2d 2d2d   cls....# ------
-00001e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001e90: 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a63 6c61  ---------....cla
-00001ea0: 7373 2066 4469 6374 2863 6f6c 6c65 6374  ss fDict(collect
-00001eb0: 696f 6e73 2e55 7365 7244 6963 7429 3a0d  ions.UserDict):.
-00001ec0: 0a20 2020 205f 5f73 6c6f 7473 5f5f 203d  .    __slots__ =
-00001ed0: 2028 290d 0a0d 0a20 2020 2064 6174 613a   ()....    data:
-00001ee0: 2064 6963 740d 0a0d 0a20 2020 2064 6566   dict....    def
-00001ef0: 2070 6970 6528 7365 6c66 2c20 662c 202a   pipe(self, f, *
-00001f00: 6172 6773 2c20 2a2a 6b77 6172 6773 293a  args, **kwargs):
-00001f10: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00001f20: 2020 2020 2020 203e 3e3e 2066 4469 6374         >>> fDict
-00001f30: 287b 303a 2031 7d29 2e70 6970 6528 6c61  ({0: 1}).pipe(la
-00001f40: 6d62 6461 2064 3a20 642e 6d61 705f 7661  mbda d: d.map_va
-00001f50: 6c75 6573 280d 0a20 2020 2020 2020 202e  lues(..        .
-00001f60: 2e2e 2020 2020 206c 616d 6264 6120 763a  ..     lambda v:
-00001f70: 2076 202b 2031 0d0a 2020 2020 2020 2020   v + 1..        
-00001f80: 2e2e 2e20 2929 0d0a 2020 2020 2020 2020  ... ))..        
-00001f90: 7b30 3a20 327d 0d0a 2020 2020 2020 2020  {0: 2}..        
-00001fa0: 2222 220d 0a20 2020 2020 2020 2072 6573  """..        res
-00001fb0: 203d 2066 2873 656c 662c 202a 6172 6773   = f(self, *args
-00001fc0: 2c20 2a2a 6b77 6172 6773 290d 0a20 2020  , **kwargs)..   
-00001fd0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00001fe0: 6365 2872 6573 2c20 6469 6374 293a 0d0a  ce(res, dict):..
-00001ff0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00002000: 726e 2066 4469 6374 2872 6573 290d 0a20  rn fDict(res).. 
-00002010: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00002020: 730d 0a0d 0a20 2020 2064 6566 2070 6172  s....    def par
-00002030: 7469 616c 2873 656c 662c 2066 2c20 2a61  tial(self, f, *a
-00002040: 7267 732c 202a 2a6b 7761 7267 7329 3a0d  rgs, **kwargs):.
-00002050: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00002060: 2020 2020 2020 3e3e 3e20 6620 3d20 6644        >>> f = fD
-00002070: 6963 7428 7b30 3a20 317d 292e 7061 7274  ict({0: 1}).part
-00002080: 6961 6c28 0d0a 2020 2020 2020 2020 2e2e  ial(..        ..
-00002090: 2e20 2020 2020 6c61 6d62 6461 2064 2c20  .     lambda d, 
-000020a0: 6e3a 2064 2e6d 6170 5f76 616c 7565 7328  n: d.map_values(
-000020b0: 6c61 6d62 6461 2076 3a20 7620 2b20 6e29  lambda v: v + n)
-000020c0: 0d0a 2020 2020 2020 2020 2e2e 2e20 290d  ..        ... ).
-000020d0: 0a20 2020 2020 2020 203e 3e3e 2066 2831  .        >>> f(1
-000020e0: 290d 0a20 2020 2020 2020 207b 303a 2032  )..        {0: 2
-000020f0: 7d0d 0a20 2020 2020 2020 203e 3e3e 2066  }..        >>> f
-00002100: 2832 290d 0a20 2020 2020 2020 207b 303a  (2)..        {0:
-00002110: 2033 7d0d 0a20 2020 2020 2020 2022 2222   3}..        """
-00002120: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00002130: 2066 756e 6374 6f6f 6c73 2e70 6172 7469   functools.parti
-00002140: 616c 2866 2c20 7365 6c66 2c20 2a61 7267  al(f, self, *arg
-00002150: 732c 202a 2a6b 7761 7267 7329 0d0a 0d0a  s, **kwargs)....
-00002160: 2020 2020 6465 6620 6b65 7973 5f74 7570      def keys_tup
-00002170: 6c65 2873 656c 6629 3a0d 0a20 2020 2020  le(self):..     
-00002180: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00002190: 3e3e 3e20 6644 6963 7428 7b30 3a20 317d  >>> fDict({0: 1}
-000021a0: 292e 6b65 7973 5f74 7570 6c65 2829 0d0a  ).keys_tuple()..
-000021b0: 2020 2020 2020 2020 6954 7570 6c65 2830          iTuple(0
-000021c0: 290d 0a20 2020 2020 2020 2022 2222 0d0a  )..        """..
-000021d0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-000021e0: 5475 706c 652e 6672 6f6d 5f6b 6579 7328  Tuple.from_keys(
-000021f0: 7365 6c66 290d 0a0d 0a20 2020 2064 6566  self)....    def
-00002200: 2076 616c 7565 735f 7475 706c 6528 7365   values_tuple(se
-00002210: 6c66 293a 0d0a 2020 2020 2020 2020 2222  lf):..        ""
-00002220: 220d 0a20 2020 2020 2020 203e 3e3e 2066  "..        >>> f
-00002230: 4469 6374 287b 303a 2031 7d29 2e76 616c  Dict({0: 1}).val
-00002240: 7565 735f 7475 706c 6528 290d 0a20 2020  ues_tuple()..   
-00002250: 2020 2020 2069 5475 706c 6528 3129 0d0a       iTuple(1)..
-00002260: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00002270: 2020 2020 2072 6574 7572 6e20 6954 7570       return iTup
-00002280: 6c65 2e66 726f 6d5f 7661 6c75 6573 2873  le.from_values(s
-00002290: 656c 6629 0d0a 2020 2020 0d0a 2020 2020  elf)..    ..    
-000022a0: 6465 6620 6974 656d 735f 7475 706c 6528  def items_tuple(
-000022b0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-000022c0: 2222 220d 0a20 2020 2020 2020 203e 3e3e  """..        >>>
-000022d0: 2066 4469 6374 287b 303a 2031 7d29 2e69   fDict({0: 1}).i
-000022e0: 7465 6d73 5f74 7570 6c65 2829 0d0a 2020  tems_tuple()..  
-000022f0: 2020 2020 2020 6954 7570 6c65 2828 302c        iTuple((0,
-00002300: 2031 2929 0d0a 2020 2020 2020 2020 2222   1))..        ""
-00002310: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-00002320: 6e20 6954 7570 6c65 2e66 726f 6d5f 6974  n iTuple.from_it
-00002330: 656d 7328 7365 6c66 290d 0a0d 0a20 2020  ems(self)....   
-00002340: 2023 204e 4f54 453a 2077 6520 6861 7665   # NOTE: we have
-00002350: 2073 6570 6172 6174 6520 6d61 7020 696d   separate map im
-00002360: 706c 656d 656e 7461 7469 6f6e 7320 0d0a  plementations ..
-00002370: 2020 2020 2320 6173 2074 6865 7920 6172      # as they ar
-00002380: 6520 636f 6e73 7461 6e74 2073 697a 652c  e constant size,
-00002390: 2064 6963 7420 746f 2064 6963 740d 0a20   dict to dict.. 
-000023a0: 2020 2023 206f 7468 6572 2069 7465 7261     # other itera
-000023b0: 746f 7220 6675 6e63 7469 6f6e 7320 7368  tor functions sh
-000023c0: 6f75 6c64 2075 7365 2069 5475 706c 6520  ould use iTuple 
-000023d0: 2866 726f 6d20 7468 6520 6162 6f76 6529  (from the above)
-000023e0: 0d0a 0d0a 2020 2020 6465 6620 6d61 705f  ....    def map_
-000023f0: 6b65 7973 2873 656c 662c 2066 2c20 2a61  keys(self, f, *a
-00002400: 7267 732c 202a 2a6b 7761 7267 7329 3a0d  rgs, **kwargs):.
-00002410: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00002420: 2020 2020 2020 3e3e 3e20 6644 6963 7428        >>> fDict(
-00002430: 7b30 3a20 317d 292e 6d61 705f 6b65 7973  {0: 1}).map_keys
-00002440: 286c 616d 6264 6120 763a 2076 202b 2031  (lambda v: v + 1
-00002450: 290d 0a20 2020 2020 2020 207b 313a 2031  )..        {1: 1
-00002460: 7d0d 0a20 2020 2020 2020 2022 2222 0d0a  }..        """..
-00002470: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-00002480: 4469 6374 280d 0a20 2020 2020 2020 2020  Dict(..         
-00002490: 2020 2028 6628 6b2c 202a 6172 6773 2c20     (f(k, *args, 
-000024a0: 2a2a 6b77 6172 6773 292c 2076 2920 666f  **kwargs), v) fo
-000024b0: 7220 6b2c 2076 2069 6e20 7365 6c66 2e69  r k, v in self.i
-000024c0: 7465 6d73 2829 0d0a 2020 2020 2020 2020  tems()..        
-000024d0: 290d 0a0d 0a20 2020 2064 6566 206d 6170  )....    def map
-000024e0: 5f76 616c 7565 7328 7365 6c66 2c20 662c  _values(self, f,
-000024f0: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-00002500: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
-00002510: 0a20 2020 2020 2020 203e 3e3e 2066 4469  .        >>> fDi
-00002520: 6374 287b 303a 2031 7d29 2e6d 6170 5f76  ct({0: 1}).map_v
-00002530: 616c 7565 7328 6c61 6d62 6461 2076 3a20  alues(lambda v: 
-00002540: 7620 2b20 3129 0d0a 2020 2020 2020 2020  v + 1)..        
-00002550: 7b30 3a20 327d 0d0a 2020 2020 2020 2020  {0: 2}..        
-00002560: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
-00002570: 7572 6e20 6644 6963 7428 0d0a 2020 2020  urn fDict(..    
-00002580: 2020 2020 2020 2020 286b 2c20 6628 762c          (k, f(v,
-00002590: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-000025a0: 2929 2066 6f72 206b 2c20 7620 696e 2073  )) for k, v in s
-000025b0: 656c 662e 6974 656d 7328 290d 0a20 2020  elf.items()..   
-000025c0: 2020 2020 2029 0d0a 0d0a 2020 2020 6465       )....    de
-000025d0: 6620 6d61 705f 6974 656d 7328 7365 6c66  f map_items(self
-000025e0: 2c20 662c 202a 6172 6773 2c20 2a2a 6b77  , f, *args, **kw
-000025f0: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
-00002600: 2222 220d 0a20 2020 2020 2020 203e 3e3e  """..        >>>
-00002610: 2066 4469 6374 287b 303a 2031 7d29 2e6d   fDict({0: 1}).m
-00002620: 6170 5f69 7465 6d73 286c 616d 6264 6120  ap_items(lambda 
-00002630: 6b2c 2076 3a20 2876 2c20 6b29 290d 0a20  k, v: (v, k)).. 
-00002640: 2020 2020 2020 207b 313a 2030 7d0d 0a20         {1: 0}.. 
-00002650: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00002660: 2020 2020 7265 7475 726e 2066 4469 6374      return fDict
-00002670: 280d 0a20 2020 2020 2020 2020 2020 2066  (..            f
-00002680: 286b 2c20 762c 202a 6172 6773 2c20 2a2a  (k, v, *args, **
-00002690: 6b77 6172 6773 2920 666f 7220 6b2c 2076  kwargs) for k, v
-000026a0: 2069 6e20 7365 6c66 2e69 7465 6d73 2829   in self.items()
-000026b0: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
-000026c0: 2020 2064 6566 2069 6e76 6572 7428 7365     def invert(se
-000026d0: 6c66 293a 0d0a 2020 2020 2020 2020 2222  lf):..        ""
-000026e0: 220d 0a20 2020 2020 2020 203e 3e3e 2066  "..        >>> f
-000026f0: 4469 6374 287b 303a 2031 7d29 2e69 6e76  Dict({0: 1}).inv
-00002700: 6572 7428 290d 0a20 2020 2020 2020 207b  ert()..        {
-00002710: 313a 2030 7d0d 0a20 2020 2020 2020 2022  1: 0}..        "
-00002720: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
-00002730: 726e 2066 4469 6374 2828 762c 206b 2920  rn fDict((v, k) 
-00002740: 666f 7220 6b2c 2076 2069 6e20 7365 6c66  for k, v in self
-00002750: 2e69 7465 6d73 2829 290d 0a0d 0a23 202d  .items())....# -
-00002760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a  --------------..
-000027a0: 0d0a 4064 6174 6163 6c61 7373 6573 2e64  ..@dataclasses.d
-000027b0: 6174 6163 6c61 7373 2869 6e69 7420 3d20  ataclass(init = 
-000027c0: 4661 6c73 652c 2072 6570 723d 5472 7565  False, repr=True
-000027d0: 290d 0a63 6c61 7373 2069 5475 706c 6528  )..class iTuple(
-000027e0: 636f 6c6c 6563 7469 6f6e 732e 5573 6572  collections.User
-000027f0: 4c69 7374 2c20 7475 706c 6529 3a20 2320  List, tuple): # 
-00002800: 7479 7065 3a20 6967 6e6f 7265 0d0a 2020  type: ignore..  
-00002810: 2020 5f5f 736c 6f74 735f 5f20 3d20 2829    __slots__ = ()
-00002820: 0d0a 0d0a 2020 2020 6461 7461 3a20 7475  ....    data: tu
-00002830: 706c 6520 2320 7479 7065 3a20 6967 6e6f  ple # type: igno
-00002840: 7265 0d0a 0d0a 2020 2020 2320 2d2d 2d2d  re....    # ----
-00002850: 2d0d 0a0d 0a20 2020 2040 7374 6174 6963  -....    @static
-00002860: 6d65 7468 6f64 0d0a 2020 2020 6465 6620  method..    def 
-00002870: 5f5f 6e65 775f 5f28 636c 732c 2064 6174  __new__(cls, dat
-00002880: 6120 3d20 4e6f 6e65 293a 0d0a 2020 2020  a = None):..    
-00002890: 2020 2020 2320 4e4f 5445 3a20 7765 2075      # NOTE: we u
-000028a0: 7365 2063 6c73 206e 6f74 2061 7272 6179  se cls not array
-000028b0: 0d0a 2020 2020 2020 2020 2320 736f 2073  ..        # so s
-000028c0: 7562 2d63 6c61 7373 696e 6720 2a64 6f65  ub-classing *doe
-000028d0: 732a 2063 6861 6e67 6520 6964 656e 7469  s* change identi
-000028e0: 7479 0d0a 2020 2020 2020 2020 6966 2069  ty..        if i
-000028f0: 7369 6e73 7461 6e63 6528 6461 7461 2c20  sinstance(data, 
-00002900: 636c 7329 3a0d 0a20 2020 2020 2020 2020  cls):..         
-00002910: 2020 2072 6574 7572 6e20 6461 7461 0d0a     return data..
-00002920: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002930: 7570 6572 2829 2e5f 5f6e 6577 5f5f 2863  uper().__new__(c
-00002940: 6c73 2c20 6461 7461 3d64 6174 6129 0d0a  ls, data=data)..
-00002950: 0d0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-00002960: 686f 640d 0a20 2020 2064 6566 2077 7261  hod..    def wra
-00002970: 705f 7475 706c 6528 6461 7461 293a 0d0a  p_tuple(data):..
-00002980: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00002990: 6174 6120 6966 2069 7369 6e73 7461 6e63  ata if isinstanc
-000029a0: 6528 6461 7461 2c20 7475 706c 6529 2065  e(data, tuple) e
-000029b0: 6c73 6520 7475 706c 6528 6461 7461 290d  lse tuple(data).
-000029c0: 0a20 2020 200d 0a20 2020 2064 6566 205f  .    ..    def _
-000029d0: 5f69 6e69 745f 5f28 7365 6c66 2c20 6461  _init__(self, da
-000029e0: 7461 203d 204e 6f6e 6529 3a0d 0a20 2020  ta = None):..   
-000029f0: 2020 2020 2023 2054 4f44 4f3a 206f 7074       # TODO: opt
-00002a00: 696f 6e20 666f 7220 6c61 7a79 2069 6e69  ion for lazy ini
-00002a10: 743f 0d0a 2020 2020 2020 2020 7365 6c66  t?..        self
-00002a20: 2e64 6174 6120 3d20 280d 0a20 2020 2020  .data = (..     
-00002a30: 2020 2020 2020 2074 7570 6c65 2829 2069         tuple() i
-00002a40: 6620 6461 7461 2069 7320 4e6f 6e65 0d0a  f data is None..
-00002a50: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00002a60: 2073 656c 662e 7772 6170 5f74 7570 6c65   self.wrap_tuple
-00002a70: 2864 6174 6129 0d0a 2020 2020 2020 2020  (data)..        
-00002a80: 290d 0a0d 0a20 2020 2064 6566 205f 5f72  )....    def __r
-00002a90: 6570 725f 5f28 7365 6c66 293a 0d0a 2020  epr__(self):..  
-00002aa0: 2020 2020 2020 7320 3d20 7375 7065 7228        s = super(
-00002ab0: 292e 5f5f 7265 7072 5f5f 2829 0d0a 2020  ).__repr__()..  
-00002ac0: 2020 2020 2020 7265 7475 726e 2022 7b7d        return "{}
-00002ad0: 287b 7d29 222e 666f 726d 6174 280d 0a20  ({})".format(.. 
-00002ae0: 2020 2020 2020 2020 2020 2074 7970 6528             type(
-00002af0: 7365 6c66 292e 5f5f 6e61 6d65 5f5f 2c0d  self).__name__,.
-00002b00: 0a20 2020 2020 2020 2020 2020 2073 5b31  .            s[1
-00002b10: 3a2d 3220 6966 2073 5b2d 325d 203d 3d20  :-2 if s[-2] == 
-00002b20: 222c 2220 656c 7365 202d 315d 2c0d 0a20  "," else -1],.. 
-00002b30: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
-00002b40: 6465 6620 5f5f 6861 7368 5f5f 2873 656c  def __hash__(sel
-00002b50: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
-00002b60: 7572 6e20 6861 7368 2873 656c 662e 6461  urn hash(self.da
-00002b70: 7461 290d 0a0d 0a20 2020 2040 636c 6173  ta)....    @clas
-00002b80: 736d 6574 686f 640d 0a20 2020 2064 6566  smethod..    def
-00002b90: 2064 6563 6f72 6174 6528 6d65 7461 2c20   decorate(meta, 
-00002ba0: 636c 7329 3a0d 0a20 2020 2020 2020 2061  cls):..        a
-00002bb0: 7373 6572 7420 636c 732e 5f5f 6e61 6d65  ssert cls.__name
-00002bc0: 5f5f 206e 6f74 2069 6e20 5245 4749 5354  __ not in REGIST
-00002bd0: 5259 0d0a 2020 2020 2020 2020 5245 4749  RY..        REGI
-00002be0: 5354 5259 5b63 6c73 2e5f 5f6e 616d 655f  STRY[cls.__name_
-00002bf0: 5f5d 203d 2063 6c73 0d0a 2020 2020 2020  _] = cls..      
-00002c00: 2020 7265 7475 726e 2063 6c73 0d0a 0d0a    return cls....
-00002c10: 2020 2020 2320 2d2d 2d2d 2d0d 0a0d 0a20      # -----.... 
-00002c20: 2020 2064 6566 2063 6173 745f 6a73 6f6e     def cast_json
-00002c30: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00002c40: 2022 2222 0d0a 2020 2020 2020 2020 3e3e   """..        >>
-00002c50: 3e20 6954 7570 6c65 2e72 616e 6765 2831  > iTuple.range(1
-00002c60: 292e 6361 7374 5f6a 736f 6e28 290d 0a20  ).cast_json().. 
-00002c70: 2020 2020 2020 207b 275f 5f74 5f5f 273a         {'__t__':
-00002c80: 2027 6954 7570 6c65 272c 2027 6461 7461   'iTuple', 'data
-00002c90: 273a 205b 305d 7d0d 0a20 2020 2020 2020  ': [0]}..       
-00002ca0: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
-00002cb0: 7475 726e 2064 6963 7428 0d0a 2020 2020  turn dict(..    
-00002cc0: 2020 2020 2020 2020 5f5f 745f 5f20 3d20          __t__ = 
-00002cd0: 7479 7065 2873 656c 6629 2e5f 5f6e 616d  type(self).__nam
-00002ce0: 655f 5f2c 0d0a 2020 2020 2020 2020 2020  e__,..          
-00002cf0: 2020 6461 7461 203d 206c 6973 7428 7365    data = list(se
-00002d00: 6c66 2e6d 6170 2863 6173 745f 6a73 6f6e  lf.map(cast_json
-00002d10: 2929 2c0d 0a20 2020 2020 2020 2029 0d0a  )),..        )..
-00002d20: 0d0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-00002d30: 6f64 0d0a 2020 2020 6465 6620 756e 6361  od..    def unca
-00002d40: 7374 5f6a 736f 6e28 636c 732c 206f 626a  st_json(cls, obj
-00002d50: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
-00002d60: 0a20 2020 2020 2020 203e 3e3e 2069 5475  .        >>> iTu
-00002d70: 706c 652e 756e 6361 7374 5f6a 736f 6e28  ple.uncast_json(
-00002d80: 6954 7570 6c65 2e72 616e 6765 2831 292e  iTuple.range(1).
-00002d90: 6361 7374 5f6a 736f 6e28 2929 0d0a 2020  cast_json())..  
-00002da0: 2020 2020 2020 6954 7570 6c65 2830 290d        iTuple(0).
-00002db0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00002dc0: 2020 2020 2020 6173 7365 7274 206f 626a        assert obj
-00002dd0: 5b22 5f5f 745f 5f22 5d20 3d3d 2063 6c73  ["__t__"] == cls
-00002de0: 2e5f 5f6e 616d 655f 5f0d 0a20 2020 2020  .__name__..     
-00002df0: 2020 2072 6574 7572 6e20 636c 7328 6461     return cls(da
-00002e00: 7461 3d6f 626a 5b22 6461 7461 225d 290d  ta=obj["data"]).
-00002e10: 0a0d 0a20 2020 2023 202d 2d2d 2d2d 0d0a  ...    # -----..
-00002e20: 0d0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-00002e30: 6f64 0d0a 2020 2020 6465 6620 7261 6e67  od..    def rang
-00002e40: 6528 636c 732c 202a 6172 6773 2c20 2a2a  e(cls, *args, **
-00002e50: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
-00002e60: 2020 2222 220d 0a20 2020 2020 2020 203e    """..        >
-00002e70: 3e3e 2069 5475 706c 652e 7261 6e67 6528  >> iTuple.range(
-00002e80: 3329 0d0a 2020 2020 2020 2020 6954 7570  3)..        iTup
-00002e90: 6c65 2830 2c20 312c 2032 290d 0a20 2020  le(0, 1, 2)..   
-00002ea0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00002eb0: 2020 7265 7475 726e 2063 6c73 2872 616e    return cls(ran
-00002ec0: 6765 282a 6172 6773 2c20 2a2a 6b77 6172  ge(*args, **kwar
-00002ed0: 6773 2929 0d0a 0d0a 2020 2020 4063 6c61  gs))....    @cla
-00002ee0: 7373 6d65 7468 6f64 0d0a 2020 2020 6465  ssmethod..    de
-00002ef0: 6620 6672 6f6d 5f6b 6579 7328 636c 732c  f from_keys(cls,
-00002f00: 2064 293a 0d0a 2020 2020 2020 2020 2222   d):..        ""
-00002f10: 220d 0a20 2020 2020 2020 203e 3e3e 2069  "..        >>> i
-00002f20: 5475 706c 652e 6672 6f6d 5f6b 6579 7328  Tuple.from_keys(
-00002f30: 7b69 3a20 6920 2b20 3120 666f 7220 6920  {i: i + 1 for i 
-00002f40: 696e 2072 616e 6765 2832 297d 290d 0a20  in range(2)}).. 
-00002f50: 2020 2020 2020 2069 5475 706c 6528 302c         iTuple(0,
-00002f60: 2031 290d 0a20 2020 2020 2020 2022 2222   1)..        """
-00002f70: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00002f80: 2063 6c73 2864 2e6b 6579 7328 2929 0d0a   cls(d.keys())..
-00002f90: 2020 2020 2020 2020 0d0a 2020 2020 4063          ..    @c
-00002fa0: 6c61 7373 6d65 7468 6f64 0d0a 2020 2020  lassmethod..    
-00002fb0: 6465 6620 6672 6f6d 5f76 616c 7565 7328  def from_values(
-00002fc0: 636c 732c 2064 293a 0d0a 2020 2020 2020  cls, d):..      
-00002fd0: 2020 2222 220d 0a20 2020 2020 2020 203e    """..        >
-00002fe0: 3e3e 2069 5475 706c 652e 6672 6f6d 5f76  >> iTuple.from_v
-00002ff0: 616c 7565 7328 7b69 3a20 6920 2b20 3120  alues({i: i + 1 
-00003000: 666f 7220 6920 696e 2072 616e 6765 2832  for i in range(2
-00003010: 297d 290d 0a20 2020 2020 2020 2069 5475  )})..        iTu
-00003020: 706c 6528 312c 2032 290d 0a20 2020 2020  ple(1, 2)..     
-00003030: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00003040: 7265 7475 726e 2063 6c73 2864 2e76 616c  return cls(d.val
-00003050: 7565 7328 2929 0d0a 2020 2020 2020 2020  ues())..        
-00003060: 0d0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-00003070: 6f64 0d0a 2020 2020 6465 6620 6672 6f6d  od..    def from
-00003080: 5f69 7465 6d73 2863 6c73 2c20 6429 3a0d  _items(cls, d):.
-00003090: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-000030a0: 2020 2020 2020 3e3e 3e20 6954 7570 6c65        >>> iTuple
-000030b0: 2e66 726f 6d5f 6974 656d 7328 7b69 3a20  .from_items({i: 
-000030c0: 6920 2b20 3120 666f 7220 6920 696e 2072  i + 1 for i in r
-000030d0: 616e 6765 2832 297d 290d 0a20 2020 2020  ange(2)})..     
-000030e0: 2020 2069 5475 706c 6528 2830 2c20 3129     iTuple((0, 1)
-000030f0: 2c20 2831 2c20 3229 290d 0a20 2020 2020  , (1, 2))..     
-00003100: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00003110: 7265 7475 726e 2063 6c73 2864 2e69 7465  return cls(d.ite
-00003120: 6d73 2829 290d 0a0d 0a20 2020 2023 202d  ms())....    # -
-00003130: 2d2d 2d2d 0d0a 0d0a 2020 2020 6465 6620  ----....    def 
-00003140: 7069 7065 2873 656c 662c 2066 2c20 2a61  pipe(self, f, *a
-00003150: 7267 732c 202a 2a6b 7761 7267 7329 3a0d  rgs, **kwargs):.
-00003160: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00003170: 2020 2020 2020 3e3e 3e20 6954 7570 6c65        >>> iTuple
-00003180: 2e72 616e 6765 2832 292e 7069 7065 286c  .range(2).pipe(l
-00003190: 616d 6264 6120 6974 3a20 6974 290d 0a20  ambda it: it).. 
-000031a0: 2020 2020 2020 2069 5475 706c 6528 302c         iTuple(0,
-000031b0: 2031 290d 0a20 2020 2020 2020 203e 3e3e   1)..        >>>
-000031c0: 2069 5475 706c 652e 7261 6e67 6528 3229   iTuple.range(2)
-000031d0: 2e70 6970 6528 0d0a 2020 2020 2020 2020  .pipe(..        
-000031e0: 2e2e 2e20 2020 2020 6c61 6d62 6461 2069  ...     lambda i
-000031f0: 742c 2076 3a20 6974 2e6d 6170 286c 616d  t, v: it.map(lam
-00003200: 6264 6120 783a 2078 202a 2076 292c 2032  bda x: x * v), 2
-00003210: 0d0a 2020 2020 2020 2020 2e2e 2e20 290d  ..        ... ).
-00003220: 0a20 2020 2020 2020 2069 5475 706c 6528  .        iTuple(
-00003230: 302c 2032 290d 0a20 2020 2020 2020 2022  0, 2)..        "
-00003240: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
-00003250: 726e 2066 2873 656c 662c 202a 6172 6773  rn f(self, *args
-00003260: 2c20 2a2a 6b77 6172 6773 290d 0a0d 0a20  , **kwargs).... 
-00003270: 2020 2064 6566 2070 6172 7469 616c 2873     def partial(s
-00003280: 656c 662c 2066 2c20 2a61 7267 732c 202a  elf, f, *args, *
-00003290: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
-000032a0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000032b0: 3e3e 3e20 6620 3d20 6954 7570 6c65 2e72  >>> f = iTuple.r
-000032c0: 616e 6765 2832 292e 7061 7274 6961 6c28  ange(2).partial(
-000032d0: 0d0a 2020 2020 2020 2020 2e2e 2e20 2020  ..        ...   
-000032e0: 2020 6c61 6d62 6461 2069 742c 2076 3a20    lambda it, v: 
-000032f0: 6974 2e6d 6170 286c 616d 6264 6120 783a  it.map(lambda x:
-00003300: 2078 202a 2076 290d 0a20 2020 2020 2020   x * v)..       
-00003310: 202e 2e2e 2029 0d0a 2020 2020 2020 2020   ... )..        
-00003320: 3e3e 3e20 6628 3229 0d0a 2020 2020 2020  >>> f(2)..      
-00003330: 2020 6954 7570 6c65 2830 2c20 3229 0d0a    iTuple(0, 2)..
-00003340: 2020 2020 2020 2020 3e3e 3e20 6628 3329          >>> f(3)
-00003350: 0d0a 2020 2020 2020 2020 6954 7570 6c65  ..        iTuple
-00003360: 2830 2c20 3329 0d0a 2020 2020 2020 2020  (0, 3)..        
-00003370: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
-00003380: 7572 6e20 6675 6e63 746f 6f6c 732e 7061  urn functools.pa
-00003390: 7274 6961 6c28 662c 2073 656c 662c 202a  rtial(f, self, *
-000033a0: 6172 6773 2c20 2a2a 6b77 6172 6773 290d  args, **kwargs).
-000033b0: 0a0d 0a20 2020 2023 202d 2d2d 2d2d 0d0a  ...    # -----..
-000033c0: 0d0a 2020 2020 6465 6620 6c65 6e28 7365  ..    def len(se
-000033d0: 6c66 293a 0d0a 2020 2020 2020 2020 2222  lf):..        ""
-000033e0: 220d 0a20 2020 2020 2020 203e 3e3e 2069  "..        >>> i
-000033f0: 5475 706c 652e 7261 6e67 6528 3329 2e6c  Tuple.range(3).l
-00003400: 656e 2829 0d0a 2020 2020 2020 2020 330d  en()..        3.
-00003410: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00003420: 2020 2020 2020 7265 7475 726e 206c 656e        return len
-00003430: 2873 656c 6629 0d0a 0d0a 2020 2020 6465  (self)....    de
-00003440: 6620 6170 7065 6e64 2873 656c 662c 2076  f append(self, v
-00003450: 616c 7565 2c20 2a76 616c 7565 7329 3a0d  alue, *values):.
-00003460: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00003470: 2020 2020 2020 3e3e 3e20 6954 7570 6c65        >>> iTuple
-00003480: 2e72 616e 6765 2831 292e 6170 7065 6e64  .range(1).append
-00003490: 2831 290d 0a20 2020 2020 2020 2069 5475  (1)..        iTu
-000034a0: 706c 6528 302c 2031 290d 0a20 2020 2020  ple(0, 1)..     
-000034b0: 2020 203e 3e3e 2069 5475 706c 652e 7261     >>> iTuple.ra
-000034c0: 6e67 6528 3129 2e61 7070 656e 6428 312c  nge(1).append(1,
-000034d0: 2032 290d 0a20 2020 2020 2020 2069 5475   2)..        iTu
-000034e0: 706c 6528 302c 2031 2c20 3229 0d0a 2020  ple(0, 1, 2)..  
-000034f0: 2020 2020 2020 3e3e 3e20 6954 7570 6c65        >>> iTuple
-00003500: 2e72 616e 6765 2831 292e 6170 7065 6e64  .range(1).append
-00003510: 2831 2c20 322c 2033 290d 0a20 2020 2020  (1, 2, 3)..     
-00003520: 2020 2069 5475 706c 6528 302c 2031 2c20     iTuple(0, 1, 
-00003530: 322c 2033 290d 0a20 2020 2020 2020 203e  2, 3)..        >
-00003540: 3e3e 2069 5475 706c 652e 7261 6e67 6528  >> iTuple.range(
-00003550: 3129 2e61 7070 656e 6428 312c 2028 322c  1).append(1, (2,
-00003560: 2929 0d0a 2020 2020 2020 2020 6954 7570  ))..        iTup
-00003570: 6c65 2830 2c20 312c 2028 322c 2929 0d0a  le(0, 1, (2,))..
-00003580: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00003590: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000035a0: 202b 2028 7661 6c75 652c 202a 7661 6c75   + (value, *valu
-000035b0: 6573 290d 0a0d 0a20 2020 2064 6566 2070  es)....    def p
-000035c0: 7265 7065 6e64 2873 656c 662c 2076 616c  repend(self, val
-000035d0: 7565 2c20 2a76 616c 7565 7329 3a0d 0a20  ue, *values):.. 
-000035e0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-000035f0: 2020 2020 3e3e 3e20 6954 7570 6c65 2e72      >>> iTuple.r
-00003600: 616e 6765 2831 292e 7072 6570 656e 6428  ange(1).prepend(
-00003610: 3129 0d0a 2020 2020 2020 2020 6954 7570  1)..        iTup
-00003620: 6c65 2831 2c20 3029 0d0a 2020 2020 2020  le(1, 0)..      
-00003630: 2020 3e3e 3e20 6954 7570 6c65 2e72 616e    >>> iTuple.ran
-00003640: 6765 2831 292e 7072 6570 656e 6428 312c  ge(1).prepend(1,
-00003650: 2032 290d 0a20 2020 2020 2020 2069 5475   2)..        iTu
-00003660: 706c 6528 312c 2032 2c20 3029 0d0a 2020  ple(1, 2, 0)..  
-00003670: 2020 2020 2020 3e3e 3e20 6954 7570 6c65        >>> iTuple
-00003680: 2e72 616e 6765 2831 292e 7072 6570 656e  .range(1).prepen
-00003690: 6428 312c 2032 2c20 3329 0d0a 2020 2020  d(1, 2, 3)..    
-000036a0: 2020 2020 6954 7570 6c65 2831 2c20 322c      iTuple(1, 2,
-000036b0: 2033 2c20 3029 0d0a 2020 2020 2020 2020   3, 0)..        
-000036c0: 3e3e 3e20 6954 7570 6c65 2e72 616e 6765  >>> iTuple.range
-000036d0: 2831 292e 7072 6570 656e 6428 312c 2028  (1).prepend(1, (
-000036e0: 322c 2929 0d0a 2020 2020 2020 2020 6954  2,))..        iT
-000036f0: 7570 6c65 2831 2c20 2832 2c29 2c20 3029  uple(1, (2,), 0)
-00003700: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00003710: 2020 2020 2020 2072 6574 7572 6e20 2876         return (v
-00003720: 616c 7565 2c20 2a76 616c 7565 7329 202b  alue, *values) +
-00003730: 2073 656c 660d 0a0d 0a20 2020 2064 6566   self....    def
-00003740: 207a 6970 2873 656c 662c 202a 6974 7273   zip(self, *itrs
-00003750: 2c20 6c61 7a79 203d 2046 616c 7365 293a  , lazy = False):
-00003760: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00003770: 2020 2020 2020 203e 3e3e 2069 5475 706c         >>> iTupl
-00003780: 6528 5b5b 312c 2031 5d2c 205b 322c 2032  e([[1, 1], [2, 2
-00003790: 5d2c 205b 332c 2033 5d5d 292e 7a69 7028  ], [3, 3]]).zip(
-000037a0: 290d 0a20 2020 2020 2020 2069 5475 706c  )..        iTupl
-000037b0: 6528 2831 2c20 322c 2033 292c 2028 312c  e((1, 2, 3), (1,
-000037c0: 2032 2c20 3329 290d 0a20 2020 2020 2020   2, 3))..       
-000037d0: 203e 3e3e 2069 5475 706c 6528 5b69 5475   >>> iTuple([iTu
-000037e0: 706c 652e 7261 6e67 6528 3329 2c20 6954  ple.range(3), iT
-000037f0: 7570 6c65 2e72 616e 6765 2831 2c20 3429  uple.range(1, 4)
-00003800: 5d29 2e7a 6970 2829 0d0a 2020 2020 2020  ]).zip()..      
-00003810: 2020 6954 7570 6c65 2828 302c 2031 292c    iTuple((0, 1),
-00003820: 2028 312c 2032 292c 2028 322c 2033 2929   (1, 2), (2, 3))
-00003830: 0d0a 2020 2020 2020 2020 3e3e 3e20 6954  ..        >>> iT
-00003840: 7570 6c65 2e72 616e 6765 2833 292e 7a69  uple.range(3).zi
-00003850: 7028 6954 7570 6c65 2e72 616e 6765 2831  p(iTuple.range(1
-00003860: 2c20 3429 290d 0a20 2020 2020 2020 2069  , 4))..        i
-00003870: 5475 706c 6528 2830 2c20 3129 2c20 2831  Tuple((0, 1), (1
-00003880: 2c20 3229 2c20 2832 2c20 3329 290d 0a20  , 2), (2, 3)).. 
-00003890: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-000038a0: 2020 2020 6966 206c 656e 2869 7472 7329      if len(itrs)
-000038b0: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
-000038c0: 2020 2020 7265 7320 3d20 7a69 7028 2a73      res = zip(*s
-000038d0: 656c 6629 0d0a 2020 2020 2020 2020 656c  elf)..        el
-000038e0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-000038f0: 2072 6573 203d 207a 6970 2873 656c 662c   res = zip(self,
-00003900: 202a 6974 7273 290d 0a20 2020 2020 2020   *itrs)..       
-00003910: 2072 6574 7572 6e20 7265 7320 6966 206c   return res if l
-00003920: 617a 7920 656c 7365 2069 5475 706c 6528  azy else iTuple(
-00003930: 6461 7461 3d72 6573 290d 0a0d 0a20 2020  data=res)....   
-00003940: 2064 6566 2066 6c61 7474 656e 2873 656c   def flatten(sel
-00003950: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
-00003960: 0d0a 2020 2020 2020 2020 3e3e 3e20 6954  ..        >>> iT
-00003970: 7570 6c65 2e72 616e 6765 2833 292e 6d61  uple.range(3).ma
-00003980: 7028 6c61 6d62 6461 2078 3a20 5b78 5d29  p(lambda x: [x])
-00003990: 2e66 6c61 7474 656e 2829 0d0a 2020 2020  .flatten()..    
-000039a0: 2020 2020 6954 7570 6c65 2830 2c20 312c      iTuple(0, 1,
-000039b0: 2032 290d 0a20 2020 2020 2020 2022 2222   2)..        """
-000039c0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000039d0: 2069 5475 706c 6528 6974 6572 746f 6f6c   iTuple(itertool
-000039e0: 732e 6368 6169 6e28 2a73 656c 6629 290d  s.chain(*self)).
-000039f0: 0a0d 0a20 2020 2064 6566 2065 7874 656e  ...    def exten
-00003a00: 6428 7365 6c66 2c20 7661 6c75 652c 202a  d(self, value, *
-00003a10: 7661 6c75 6573 293a 0d0a 2020 2020 2020  values):..      
-00003a20: 2020 2222 220d 0a20 2020 2020 2020 203e    """..        >
-00003a30: 3e3e 2069 5475 706c 652e 7261 6e67 6528  >> iTuple.range(
-00003a40: 3129 2e65 7874 656e 6428 2831 2c29 290d  1).extend((1,)).
-00003a50: 0a20 2020 2020 2020 2069 5475 706c 6528  .        iTuple(
-00003a60: 302c 2031 290d 0a20 2020 2020 2020 203e  0, 1)..        >
-00003a70: 3e3e 2069 5475 706c 652e 7261 6e67 6528  >> iTuple.range(
-00003a80: 3129 2e65 7874 656e 6428 5b31 5d29 0d0a  1).extend([1])..
-00003a90: 2020 2020 2020 2020 6954 7570 6c65 2830          iTuple(0
-00003aa0: 2c20 3129 0d0a 2020 2020 2020 2020 3e3e  , 1)..        >>
-00003ab0: 3e20 6954 7570 6c65 2e72 616e 6765 2831  > iTuple.range(1
-00003ac0: 292e 6578 7465 6e64 285b 315d 2c20 5b32  ).extend([1], [2
-00003ad0: 5d29 0d0a 2020 2020 2020 2020 6954 7570  ])..        iTup
-00003ae0: 6c65 2830 2c20 312c 2032 290d 0a20 2020  le(0, 1, 2)..   
-00003af0: 2020 2020 203e 3e3e 2069 5475 706c 652e       >>> iTuple.
-00003b00: 7261 6e67 6528 3129 2e65 7874 656e 6428  range(1).extend(
-00003b10: 5b31 5d2c 205b 5b32 5d5d 290d 0a20 2020  [1], [[2]])..   
-00003b20: 2020 2020 2069 5475 706c 6528 302c 2031       iTuple(0, 1
-00003b30: 2c20 5b32 5d29 0d0a 2020 2020 2020 2020  , [2])..        
-00003b40: 3e3e 3e20 6954 7570 6c65 2e72 616e 6765  >>> iTuple.range
-00003b50: 2831 292e 6578 7465 6e64 285b 315d 2c20  (1).extend([1], 
-00003b60: 5b5b 325d 5d2c 205b 325d 290d 0a20 2020  [[2]], [2])..   
-00003b70: 2020 2020 2069 5475 706c 6528 302c 2031       iTuple(0, 1
-00003b80: 2c20 5b32 5d2c 2032 290d 0a20 2020 2020  , [2], 2)..     
-00003b90: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00003ba0: 7265 7475 726e 2069 5475 706c 6528 6974  return iTuple(it
-00003bb0: 6572 746f 6f6c 732e 6368 6169 6e2e 6672  ertools.chain.fr
-00003bc0: 6f6d 5f69 7465 7261 626c 6528 0d0a 2020  om_iterable(..  
-00003bd0: 2020 2020 2020 2020 2020 2873 656c 662c            (self,
-00003be0: 2076 616c 7565 2c20 2a76 616c 7565 7329   value, *values)
-00003bf0: 0d0a 2020 2020 2020 2020 2929 0d0a 0d0a  ..        ))....
-00003c00: 2020 2020 6465 6620 7072 6574 656e 6428      def pretend(
-00003c10: 7365 6c66 2c20 7661 6c75 652c 202a 7661  self, value, *va
-00003c20: 6c75 6573 293a 0d0a 2020 2020 2020 2020  lues):..        
-00003c30: 2222 220d 0a20 2020 2020 2020 203e 3e3e  """..        >>>
-00003c40: 2069 5475 706c 652e 7261 6e67 6528 3129   iTuple.range(1)
-00003c50: 2e70 7265 7465 6e64 2828 312c 2929 0d0a  .pretend((1,))..
-00003c60: 2020 2020 2020 2020 6954 7570 6c65 2831          iTuple(1
-00003c70: 2c20 3029 0d0a 2020 2020 2020 2020 3e3e  , 0)..        >>
-00003c80: 3e20 6954 7570 6c65 2e72 616e 6765 2831  > iTuple.range(1
-00003c90: 292e 7072 6574 656e 6428 5b31 5d29 0d0a  ).pretend([1])..
-00003ca0: 2020 2020 2020 2020 6954 7570 6c65 2831          iTuple(1
-00003cb0: 2c20 3029 0d0a 2020 2020 2020 2020 3e3e  , 0)..        >>
-00003cc0: 3e20 6954 7570 6c65 2e72 616e 6765 2831  > iTuple.range(1
-00003cd0: 292e 7072 6574 656e 6428 5b31 5d2c 205b  ).pretend([1], [
-00003ce0: 325d 290d 0a20 2020 2020 2020 2069 5475  2])..        iTu
-00003cf0: 706c 6528 312c 2032 2c20 3029 0d0a 2020  ple(1, 2, 0)..  
-00003d00: 2020 2020 2020 3e3e 3e20 6954 7570 6c65        >>> iTuple
-00003d10: 2e72 616e 6765 2831 292e 7072 6574 656e  .range(1).preten
-00003d20: 6428 5b31 5d2c 205b 5b32 5d5d 290d 0a20  d([1], [[2]]).. 
-00003d30: 2020 2020 2020 2069 5475 706c 6528 312c         iTuple(1,
-00003d40: 205b 325d 2c20 3029 0d0a 2020 2020 2020   [2], 0)..      
-00003d50: 2020 3e3e 3e20 6954 7570 6c65 2e72 616e    >>> iTuple.ran
-00003d60: 6765 2831 292e 7072 6574 656e 6428 5b31  ge(1).pretend([1
-00003d70: 5d2c 205b 5b32 5d5d 2c20 5b32 5d29 0d0a  ], [[2]], [2])..
-00003d80: 2020 2020 2020 2020 6954 7570 6c65 2831          iTuple(1
-00003d90: 2c20 5b32 5d2c 2032 2c20 3029 0d0a 2020  , [2], 2, 0)..  
-00003da0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00003db0: 2020 2072 6574 7572 6e20 6954 7570 6c65     return iTuple
-00003dc0: 2869 7465 7274 6f6f 6c73 2e63 6861 696e  (itertools.chain
-00003dd0: 2e66 726f 6d5f 6974 6572 6162 6c65 280d  .from_iterable(.
-00003de0: 0a20 2020 2020 2020 2020 2020 2028 7661  .            (va
-00003df0: 6c75 652c 202a 7661 6c75 6573 2c20 7365  lue, *values, se
-00003e00: 6c66 290d 0a20 2020 2020 2020 2029 290d  lf)..        )).
-00003e10: 0a0d 0a20 2020 2064 6566 2066 696c 7465  ...    def filte
-00003e20: 725f 6571 2873 656c 662c 2076 2c20 6620  r_eq(self, v, f 
-00003e30: 3d20 4e6f 6e65 2c20 6571 203d 204e 6f6e  = None, eq = Non
-00003e40: 652c 206c 617a 7920 3d20 4661 6c73 6529  e, lazy = False)
-00003e50: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00003e60: 2020 2020 2020 2020 3e3e 3e20 6954 7570          >>> iTup
-00003e70: 6c65 2e72 616e 6765 2833 292e 6669 6c74  le.range(3).filt
-00003e80: 6572 5f65 7128 3129 0d0a 2020 2020 2020  er_eq(1)..      
-00003e90: 2020 6954 7570 6c65 2831 290d 0a20 2020    iTuple(1)..   
-00003ea0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00003eb0: 2020 6966 2066 2069 7320 4e6f 6e65 2061    if f is None a
-00003ec0: 6e64 2065 7120 6973 204e 6f6e 653a 0d0a  nd eq is None:..
-00003ed0: 2020 2020 2020 2020 2020 2020 7265 7320              res 
-00003ee0: 3d20 6669 6c74 6572 286c 616d 6264 6120  = filter(lambda 
-00003ef0: 783a 2078 203d 3d20 762c 2073 656c 6629  x: x == v, self)
-00003f00: 0d0a 2020 2020 2020 2020 656c 6966 2066  ..        elif f
-00003f10: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-00003f20: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-00003f30: 2066 696c 7465 7228 6c61 6d62 6461 2078   filter(lambda x
-00003f40: 3a20 6628 7829 203d 3d20 762c 2073 656c  : f(x) == v, sel
-00003f50: 6629 0d0a 2020 2020 2020 2020 656c 6966  f)..        elif
-00003f60: 2065 7120 6973 206e 6f74 204e 6f6e 653a   eq is not None:
-00003f70: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00003f80: 7320 3d20 6669 6c74 6572 286c 616d 6264  s = filter(lambd
-00003f90: 6120 783a 2065 7128 782c 2076 292c 2073  a x: eq(x, v), s
-00003fa0: 656c 6629 0d0a 2020 2020 2020 2020 656c  elf)..        el
-00003fb0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00003fc0: 2072 6573 203d 2066 696c 7465 7228 6c61   res = filter(la
-00003fd0: 6d62 6461 2078 3a20 6571 2866 2878 292c  mbda x: eq(f(x),
-00003fe0: 2076 292c 2073 656c 6629 0d0a 2020 2020   v), self)..    
-00003ff0: 2020 2020 7265 7475 726e 2072 6573 2069      return res i
-00004000: 6620 6c61 7a79 2065 6c73 6520 7479 7065  f lazy else type
-00004010: 2873 656c 6629 2864 6174 613d 7265 7329  (self)(data=res)
-00004020: 0d0a 0d0a 2020 2020 6465 6620 6669 6c74  ....    def filt
-00004030: 6572 2873 656c 662c 2066 2c20 6571 203d  er(self, f, eq =
-00004040: 204e 6f6e 652c 206c 617a 7920 3d20 4661   None, lazy = Fa
-00004050: 6c73 6529 3a0d 0a20 2020 2020 2020 2022  lse):..        "
-00004060: 2222 0d0a 2020 2020 2020 2020 3e3e 3e20  ""..        >>> 
-00004070: 6954 7570 6c65 2e72 616e 6765 2833 292e  iTuple.range(3).
-00004080: 6669 6c74 6572 286c 616d 6264 6120 783a  filter(lambda x:
-00004090: 2078 203e 2031 290d 0a20 2020 2020 2020   x > 1)..       
-000040a0: 2069 5475 706c 6528 3229 0d0a 2020 2020   iTuple(2)..    
-000040b0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-000040c0: 2072 6574 7572 6e20 7365 6c66 2e66 696c   return self.fil
-000040d0: 7465 725f 6571 2854 7275 652c 2066 203d  ter_eq(True, f =
-000040e0: 2066 2c20 6571 203d 2065 712c 206c 617a   f, eq = eq, laz
-000040f0: 7920 3d20 6c61 7a79 290d 0a0d 0a20 2020  y = lazy)....   
-00004100: 2064 6566 206d 6170 2873 656c 662c 2066   def map(self, f
-00004110: 2c20 2a69 7465 7261 626c 6573 2c20 6c61  , *iterables, la
-00004120: 7a79 203d 2046 616c 7365 293a 0d0a 2020  zy = False):..  
-00004130: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00004140: 2020 203e 3e3e 2069 5475 706c 652e 7261     >>> iTuple.ra
-00004150: 6e67 6528 3329 2e6d 6170 286c 616d 6264  nge(3).map(lambd
-00004160: 6120 783a 2078 202a 2032 290d 0a20 2020  a x: x * 2)..   
-00004170: 2020 2020 2069 5475 706c 6528 302c 2032       iTuple(0, 2
-00004180: 2c20 3429 0d0a 2020 2020 2020 2020 2222  , 4)..        ""
-00004190: 220d 0a20 2020 2020 2020 2072 6573 203d  "..        res =
-000041a0: 206d 6170 2866 2c20 7365 6c66 2c20 2a69   map(f, self, *i
-000041b0: 7465 7261 626c 6573 290d 0a20 2020 2020  terables)..     
-000041c0: 2020 2072 6574 7572 6e20 7265 7320 6966     return res if
-000041d0: 206c 617a 7920 656c 7365 2069 5475 706c   lazy else iTupl
-000041e0: 6528 6461 7461 3d72 6573 290d 0a0d 0a20  e(data=res).... 
-000041f0: 2020 2064 6566 2065 6e75 6d65 7261 7465     def enumerate
-00004200: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00004210: 2022 2222 0d0a 2020 2020 2020 2020 3e3e   """..        >>
-00004220: 3e20 6954 7570 6c65 2e72 616e 6765 2833  > iTuple.range(3
-00004230: 292e 656e 756d 6572 6174 6528 290d 0a20  ).enumerate().. 
-00004240: 2020 2020 2020 2069 5475 706c 6528 2830         iTuple((0
-00004250: 2c20 3029 2c20 2831 2c20 3129 2c20 2832  , 0), (1, 1), (2
-00004260: 2c20 3229 290d 0a20 2020 2020 2020 2022  , 2))..        "
-00004270: 2222 0d0a 2020 2020 2020 2020 2320 544f  ""..        # TO
-00004280: 444f 3a20 616c 6c6f 7720 6c61 7a79 0d0a  DO: allow lazy..
-00004290: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-000042a0: 5475 706c 6528 656e 756d 6572 6174 6528  Tuple(enumerate(
-000042b0: 7365 6c66 2929 0d0a 0d0a 2020 2020 6465  self))....    de
-000042c0: 6620 6772 6f75 7062 7928 0d0a 2020 2020  f groupby(..    
-000042d0: 2020 2020 7365 6c66 2c20 0d0a 2020 2020      self, ..    
-000042e0: 2020 2020 662c 200d 0a20 2020 2020 2020      f, ..       
-000042f0: 206c 617a 7920 3d20 4661 6c73 652c 200d   lazy = False, .
-00004300: 0a20 2020 2020 2020 206b 6579 7320 3d20  .        keys = 
-00004310: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-00004320: 7069 7065 3d20 4e6f 6e65 2c0d 0a20 2020  pipe= None,..   
-00004330: 2029 3a0d 0a20 2020 2020 2020 2022 2222   ):..        """
-00004340: 0d0a 2020 2020 2020 2020 3e3e 3e20 6954  ..        >>> iT
-00004350: 7570 6c65 2e72 616e 6765 2833 292e 6772  uple.range(3).gr
-00004360: 6f75 7062 7928 6c61 6d62 6461 2078 3a20  oupby(lambda x: 
-00004370: 7820 3c20 3229 0d0a 2020 2020 2020 2020  x < 2)..        
-00004380: 6954 7570 6c65 2828 302c 2031 292c 2028  iTuple((0, 1), (
-00004390: 322c 2929 0d0a 2020 2020 2020 2020 3e3e  2,))..        >>
-000043a0: 3e20 6954 7570 6c65 2e72 616e 6765 2833  > iTuple.range(3
-000043b0: 292e 6772 6f75 7062 7928 0d0a 2020 2020  ).groupby(..    
-000043c0: 2020 2020 2e2e 2e20 2020 206c 616d 6264      ...    lambd
-000043d0: 6120 783a 2078 203c 2032 2c20 6b65 7973  a x: x < 2, keys
-000043e0: 3d54 7275 652c 2070 6970 653d 6644 6963  =True, pipe=fDic
-000043f0: 740d 0a20 2020 2020 2020 202e 2e2e 2029  t..        ... )
-00004400: 0d0a 2020 2020 2020 2020 7b54 7275 653a  ..        {True:
-00004410: 2028 302c 2031 292c 2046 616c 7365 3a20   (0, 1), False: 
-00004420: 2832 2c29 7d0d 0a20 2020 2020 2020 2022  (2,)}..        "
-00004430: 2222 0d0a 2020 2020 2020 2020 2320 544f  ""..        # TO
-00004440: 444f 3a20 6c61 7a79 206e 6f20 6b65 7973  DO: lazy no keys
-00004450: 0d0a 2020 2020 2020 2020 7265 7320 3d20  ..        res = 
-00004460: 6974 6572 746f 6f6c 732e 6772 6f75 7062  itertools.groupb
-00004470: 7928 7365 6c66 2c20 6b65 793d 6629 0d0a  y(self, key=f)..
-00004480: 2020 2020 2020 2020 6966 206c 617a 7920          if lazy 
-00004490: 616e 6420 6b65 7973 2061 6e64 2070 6970  and keys and pip
-000044a0: 6520 6973 204e 6f6e 653a 0d0a 2020 2020  e is None:..    
-000044b0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-000044c0: 6573 0d0a 2020 2020 2020 2020 6966 2070  es..        if p
-000044d0: 6970 6520 6973 204e 6f6e 653a 0d0a 2020  ipe is None:..  
-000044e0: 2020 2020 2020 2020 2020 7069 7065 203d            pipe =
-000044f0: 2069 5475 706c 650d 0a20 2020 2020 2020   iTuple..       
-00004500: 2069 6620 6b65 7973 3a0d 0a20 2020 2020   if keys:..     
-00004510: 2020 2020 2020 2072 6574 7572 6e20 7069         return pi
-00004520: 7065 2828 6b2c 2074 7570 6c65 2867 292c  pe((k, tuple(g),
-00004530: 2920 666f 7220 6b2c 2067 2069 6e20 7265  ) for k, g in re
-00004540: 7329 0d0a 2020 2020 2020 2020 656c 7365  s)..        else
-00004550: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00004560: 6574 7572 6e20 7069 7065 2874 7570 6c65  eturn pipe(tuple
-00004570: 2867 2920 666f 7220 6b2c 2067 2069 6e20  (g) for k, g in 
-00004580: 7265 7329 0d0a 0d0a 2020 2020 6465 6620  res)....    def 
-00004590: 6669 7273 7428 7365 6c66 293a 0d0a 2020  first(self):..  
-000045a0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-000045b0: 2020 203e 3e3e 2069 5475 706c 652e 7261     >>> iTuple.ra
-000045c0: 6e67 6528 3329 2e66 6972 7374 2829 0d0a  nge(3).first()..
-000045d0: 2020 2020 2020 2020 300d 0a20 2020 2020          0..     
-000045e0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000045f0: 7265 7475 726e 2073 656c 665b 305d 0d0a  return self[0]..
-00004600: 2020 2020 0d0a 2020 2020 6465 6620 6c61      ..    def la
-00004610: 7374 2873 656c 6629 3a0d 0a20 2020 2020  st(self):..     
-00004620: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00004630: 3e3e 3e20 6954 7570 6c65 2e72 616e 6765  >>> iTuple.range
-00004640: 2833 292e 6c61 7374 2829 0d0a 2020 2020  (3).last()..    
-00004650: 2020 2020 320d 0a20 2020 2020 2020 2022      2..        "
-00004660: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
-00004670: 726e 2073 656c 665b 2d31 5d0d 0a0d 0a20  rn self[-1].... 
-00004680: 2020 2064 6566 2066 6972 7374 5f77 6865     def first_whe
-00004690: 7265 2873 656c 662c 2066 293a 0d0a 2020  re(self, f):..  
-000046a0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-000046b0: 2020 203e 3e3e 2069 5475 706c 652e 7261     >>> iTuple.ra
-000046c0: 6e67 6528 3329 2e66 6972 7374 5f77 6865  nge(3).first_whe
-000046d0: 7265 286c 616d 6264 6120 763a 2076 203e  re(lambda v: v >
-000046e0: 2030 290d 0a20 2020 2020 2020 2031 0d0a   0)..        1..
-000046f0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00004700: 2020 2020 2066 6f72 2076 2069 6e20 7365       for v in se
-00004710: 6c66 3a0d 0a20 2020 2020 2020 2020 2020  lf:..           
-00004720: 2069 6620 6628 7629 3a0d 0a20 2020 2020   if f(v):..     
-00004730: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00004740: 6e20 760d 0a20 2020 2020 2020 2072 6574  n v..        ret
-00004750: 7572 6e20 4e6f 6e65 0d0a 0d0a 2020 2020  urn None....    
-00004760: 6465 6620 6c61 7374 5f77 6865 7265 2873  def last_where(s
-00004770: 656c 662c 2066 293a 0d0a 2020 2020 2020  elf, f):..      
-00004780: 2020 2222 220d 0a20 2020 2020 2020 203e    """..        >
-00004790: 3e3e 2069 5475 706c 652e 7261 6e67 6528  >> iTuple.range(
-000047a0: 3329 2e6c 6173 745f 7768 6572 6528 6c61  3).last_where(la
-000047b0: 6d62 6461 2076 3a20 7620 3c20 3229 0d0a  mbda v: v < 2)..
-000047c0: 2020 2020 2020 2020 310d 0a20 2020 2020          1..     
-000047d0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000047e0: 666f 7220 7620 696e 2072 6576 6572 7365  for v in reverse
-000047f0: 6428 7365 6c66 293a 0d0a 2020 2020 2020  d(self):..      
-00004800: 2020 2020 2020 6966 2066 2876 293a 0d0a        if f(v):..
-00004810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004820: 7265 7475 726e 2076 0d0a 2020 2020 2020  return v..      
-00004830: 2020 7265 7475 726e 204e 6f6e 650d 0a0d    return None...
-00004840: 0a20 2020 2064 6566 2074 616b 6528 7365  .    def take(se
-00004850: 6c66 2c20 6e29 3a0d 0a20 2020 2020 2020  lf, n):..       
-00004860: 2022 2222 0d0a 2020 2020 2020 2020 3e3e   """..        >>
-00004870: 3e20 6954 7570 6c65 2e72 616e 6765 2833  > iTuple.range(3
-00004880: 292e 7461 6b65 2832 290d 0a20 2020 2020  ).take(2)..     
-00004890: 2020 2069 5475 706c 6528 302c 2031 290d     iTuple(0, 1).
-000048a0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-000048b0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000048c0: 665b 3a6e 5d0d 0a0d 0a20 2020 2064 6566  f[:n]....    def
-000048d0: 2074 6169 6c28 7365 6c66 2c20 6e29 3a0d   tail(self, n):.
-000048e0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-000048f0: 2020 2020 2020 3e3e 3e20 6954 7570 6c65        >>> iTuple
-00004900: 2e72 616e 6765 2833 292e 7461 696c 2832  .range(3).tail(2
-00004910: 290d 0a20 2020 2020 2020 2069 5475 706c  )..        iTupl
-00004920: 6528 312c 2032 290d 0a20 2020 2020 2020  e(1, 2)..       
-00004930: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
-00004940: 7475 726e 2073 656c 665b 2d6e 3a5d 0d0a  turn self[-n:]..
-00004950: 0d0a 2020 2020 6465 6620 7265 7665 7273  ..    def revers
-00004960: 6528 7365 6c66 2c20 6c61 7a79 203d 2046  e(self, lazy = F
-00004970: 616c 7365 293a 0d0a 2020 2020 2020 2020  alse):..        
-00004980: 2222 220d 0a20 2020 2020 2020 203e 3e3e  """..        >>>
-00004990: 2069 5475 706c 652e 7261 6e67 6528 3329   iTuple.range(3)
-000049a0: 2e72 6576 6572 7365 2829 0d0a 2020 2020  .reverse()..    
-000049b0: 2020 2020 6954 7570 6c65 2832 2c20 312c      iTuple(2, 1,
-000049c0: 2030 290d 0a20 2020 2020 2020 2022 2222   0)..        """
-000049d0: 0d0a 2020 2020 2020 2020 6966 206c 617a  ..        if laz
-000049e0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-000049f0: 7265 7475 726e 2072 6576 6572 7365 6428  return reversed(
-00004a00: 7365 6c66 290d 0a20 2020 2020 2020 2072  self)..        r
-00004a10: 6574 7572 6e20 7479 7065 2873 656c 6629  eturn type(self)
-00004a20: 2864 6174 613d 7265 7665 7273 6564 2873  (data=reversed(s
-00004a30: 656c 6629 290d 0a0d 0a20 2020 2064 6566  elf))....    def
-00004a40: 2074 616b 655f 7768 696c 6528 7365 6c66   take_while(self
-00004a50: 2c20 662c 206e 203d 204e 6f6e 652c 206c  , f, n = None, l
-00004a60: 617a 7920 3d20 4661 6c73 6529 3a0d 0a20  azy = False):.. 
-00004a70: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00004a80: 2020 2020 3e3e 3e20 6954 7570 6c65 2e72      >>> iTuple.r
-00004a90: 616e 6765 2833 292e 7461 6b65 5f77 6869  ange(3).take_whi
-00004aa0: 6c65 286c 616d 6264 6120 763a 2076 203c  le(lambda v: v <
-00004ab0: 2031 290d 0a20 2020 2020 2020 2069 5475   1)..        iTu
-00004ac0: 706c 6528 3029 0d0a 2020 2020 2020 2020  ple(0)..        
-00004ad0: 2222 220d 0a20 2020 2020 2020 2064 6566  """..        def
-00004ae0: 2069 7465 7228 293a 0d0a 2020 2020 2020   iter():..      
-00004af0: 2020 2020 2020 6920 3d20 300d 0a20 2020        i = 0..   
-00004b00: 2020 2020 2020 2020 2066 6f72 2076 2069           for v i
-00004b10: 6e20 7365 6c66 3a0d 0a20 2020 2020 2020  n self:..       
-00004b20: 2020 2020 2020 2020 2069 6620 6628 7629           if f(v)
-00004b30: 2061 6e64 2028 6e20 6973 204e 6f6e 6520   and (n is None 
-00004b40: 6f72 2069 203c 206e 293a 0d0a 2020 2020  or i < n):..    
-00004b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b60: 7969 656c 6420 760d 0a20 2020 2020 2020  yield v..       
-00004b70: 2020 2020 2020 2020 2020 2020 2069 202b               i +
-00004b80: 3d20 310d 0a20 2020 2020 2020 2020 2020  = 1..           
-00004b90: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00004ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bb0: 7265 7475 726e 0d0a 2020 2020 2020 2020  return..        
-00004bc0: 7265 7320 3d20 6974 6572 2829 0d0a 2020  res = iter()..  
-00004bd0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00004be0: 2069 6620 6c61 7a79 2065 6c73 6520 7479   if lazy else ty
-00004bf0: 7065 2873 656c 6629 2864 6174 613d 7265  pe(self)(data=re
-00004c00: 7329 0d0a 0d0a 2020 2020 6465 6620 7461  s)....    def ta
-00004c10: 696c 5f77 6869 6c65 2873 656c 662c 2066  il_while(self, f
-00004c20: 2c20 6e20 3d20 4e6f 6e65 293a 0d0a 2020  , n = None):..  
-00004c30: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00004c40: 2020 203e 3e3e 2069 5475 706c 652e 7261     >>> iTuple.ra
-00004c50: 6e67 6528 3329 2e74 6169 6c5f 7768 696c  nge(3).tail_whil
-00004c60: 6528 6c61 6d62 6461 2076 3a20 7620 3e20  e(lambda v: v > 
-00004c70: 3129 0d0a 2020 2020 2020 2020 6954 7570  1)..        iTup
-00004c80: 6c65 2832 290d 0a20 2020 2020 2020 2022  le(2)..        "
-00004c90: 2222 0d0a 2020 2020 2020 2020 6920 3d20  ""..        i = 
-00004ca0: 300d 0a20 2020 2020 2020 2066 6f72 2076  0..        for v
-00004cb0: 2069 6e20 7265 7665 7273 6564 2873 656c   in reversed(sel
-00004cc0: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
-00004cd0: 2069 6620 6628 7629 2061 6e64 2028 6e20   if f(v) and (n 
-00004ce0: 6973 204e 6f6e 6520 6f72 2069 203c 206e  is None or i < n
-00004cf0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00004d00: 2020 2020 6920 2b3d 2031 0d0a 2020 2020      i += 1..    
-00004d10: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00004d20: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00004d30: 7265 616b 0d0a 2020 2020 2020 2020 7265  reak..        re
-00004d40: 7475 726e 2073 656c 662e 7461 696c 2869  turn self.tail(i
-00004d50: 290d 0a0d 0a20 2020 2023 204e 4f54 453a  )....    # NOTE:
-00004d60: 2066 726f 6d20 6173 2069 6e2c 2073 7461   from as in, sta
-00004d70: 7274 696e 6720 6672 6f6d 2066 6972 7374  rting from first
-00004d80: 2074 7275 650d 0a20 2020 2023 2076 6572   true..    # ver
-00004d90: 7375 7320 6162 6f76 652c 2077 6869 6368  sus above, which
-00004da0: 2069 7320 756e 7469 6c20 6669 7273 7420   is until first 
-00004db0: 6661 6c73 650d 0a20 2020 2064 6566 2074  false..    def t
-00004dc0: 616b 655f 6166 7465 7228 7365 6c66 2c20  ake_after(self, 
-00004dd0: 662c 206e 203d 204e 6f6e 652c 206c 617a  f, n = None, laz
-00004de0: 7920 3d20 4661 6c73 6529 3a0d 0a20 2020  y = False):..   
-00004df0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00004e00: 2020 3e3e 3e20 6954 7570 6c65 2e72 616e    >>> iTuple.ran
-00004e10: 6765 2833 292e 7461 6b65 5f61 6674 6572  ge(3).take_after
-00004e20: 286c 616d 6264 6120 763a 2076 203c 2031  (lambda v: v < 1
-00004e30: 290d 0a20 2020 2020 2020 2069 5475 706c  )..        iTupl
-00004e40: 6528 312c 2032 290d 0a20 2020 2020 2020  e(1, 2)..       
-00004e50: 203e 3e3e 2069 5475 706c 652e 7261 6e67   >>> iTuple.rang
-00004e60: 6528 3329 2e74 616b 655f 6166 7465 7228  e(3).take_after(
-00004e70: 6c61 6d62 6461 2076 3a20 7620 3c20 312c  lambda v: v < 1,
-00004e80: 206e 203d 2031 290d 0a20 2020 2020 2020   n = 1)..       
-00004e90: 2069 5475 706c 6528 3129 0d0a 2020 2020   iTuple(1)..    
-00004ea0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00004eb0: 2064 6566 2069 7465 7228 293a 0d0a 2020   def iter():..  
-00004ec0: 2020 2020 2020 2020 2020 6920 3d20 300d            i = 0.
-00004ed0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00004ee0: 2076 2069 6e20 7365 6c66 3a0d 0a20 2020   v in self:..   
-00004ef0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004f00: 6628 7629 3a0d 0a20 2020 2020 2020 2020  f(v):..         
-00004f10: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
-00004f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004f30: 2065 6c69 6620 6e20 6973 204e 6f6e 6520   elif n is None 
-00004f40: 6f72 2069 203c 206e 3a0d 0a20 2020 2020  or i < n:..     
-00004f50: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-00004f60: 6965 6c64 2076 0d0a 2020 2020 2020 2020  ield v..        
-00004f70: 2020 2020 2020 2020 2020 2020 6920 2b3d              i +=
-00004f80: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-00004f90: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00004fa0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00004fb0: 6574 7572 6e0d 0a20 2020 2020 2020 2072  eturn..        r
-00004fc0: 6573 203d 2069 7465 7228 290d 0a20 2020  es = iter()..   
-00004fd0: 2020 2020 2072 6574 7572 6e20 7265 7320       return res 
-00004fe0: 6966 206c 617a 7920 656c 7365 2074 7970  if lazy else typ
-00004ff0: 6528 7365 6c66 2928 6461 7461 3d72 6573  e(self)(data=res
-00005000: 290d 0a0d 0a20 2020 2064 6566 2074 6169  )....    def tai
-00005010: 6c5f 6166 7465 7228 7365 6c66 2c20 662c  l_after(self, f,
-00005020: 206e 203d 204e 6f6e 6529 3a0d 0a20 2020   n = None):..   
-00005030: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00005040: 2020 3e3e 3e20 6954 7570 6c65 2e72 616e    >>> iTuple.ran
-00005050: 6765 2833 292e 7461 696c 5f61 6674 6572  ge(3).tail_after
-00005060: 286c 616d 6264 6120 763a 2076 203c 2032  (lambda v: v < 2
-00005070: 290d 0a20 2020 2020 2020 2069 5475 706c  )..        iTupl
-00005080: 6528 302c 2031 290d 0a20 2020 2020 2020  e(0, 1)..       
-00005090: 203e 3e3e 2069 5475 706c 652e 7261 6e67   >>> iTuple.rang
-000050a0: 6528 3329 2e74 6169 6c5f 6166 7465 7228  e(3).tail_after(
-000050b0: 6c61 6d62 6461 2076 3a20 7620 3c20 322c  lambda v: v < 2,
-000050c0: 2031 290d 0a20 2020 2020 2020 2069 5475   1)..        iTu
-000050d0: 706c 6528 3129 0d0a 2020 2020 2020 2020  ple(1)..        
-000050e0: 2222 220d 0a20 2020 2020 2020 206c 203d  """..        l =
-000050f0: 2030 0d0a 2020 2020 2020 2020 7220 3d20   0..        r = 
-00005100: 300d 0a20 2020 2020 2020 2066 6f72 2076  0..        for v
-00005110: 2069 6e20 7265 7665 7273 6564 2873 656c   in reversed(sel
-00005120: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
-00005130: 2069 6620 6e6f 7420 6628 7629 3a0d 0a20   if not f(v):.. 
-00005140: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00005150: 202b 3d20 310d 0a20 2020 2020 2020 2020   += 1..         
-00005160: 2020 2065 6c69 6620 6e20 6973 204e 6f6e     elif n is Non
-00005170: 6520 6f72 2072 203c 206e 3a0d 0a20 2020  e or r < n:..   
-00005180: 2020 2020 2020 2020 2020 2020 2072 202b               r +
-00005190: 3d20 310d 0a20 2020 2020 2020 2020 2020  = 1..           
-000051a0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-000051b0: 2020 2020 2020 2020 6272 6561 6b0d 0a20          break.. 
-000051c0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000051d0: 6c66 2e74 6169 6c28 6c20 2b20 7229 2e74  lf.tail(l + r).t
-000051e0: 616b 6528 7229 0d0a 0d0a 2020 2020 6465  ake(r)....    de
-000051f0: 6620 6973 6c69 6365 2873 656c 662c 206c  f islice(self, l
-00005200: 6566 7420 3d20 4e6f 6e65 2c20 7269 6768  eft = None, righ
-00005210: 7420 3d20 4e6f 6e65 293a 0d0a 2020 2020  t = None):..    
-00005220: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00005230: 203e 3e3e 2069 5475 706c 652e 7261 6e67   >>> iTuple.rang
-00005240: 6528 3529 2e69 736c 6963 6528 312c 2033  e(5).islice(1, 3
-00005250: 290d 0a20 2020 2020 2020 2069 5475 706c  )..        iTupl
-00005260: 6528 312c 2032 290d 0a20 2020 2020 2020  e(1, 2)..       
-00005270: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
-00005280: 7475 726e 2073 656c 665b 6c65 6674 3a72  turn self[left:r
-00005290: 6967 6874 5d0d 0a0d 0a20 2020 2064 6566  ight]....    def
-000052a0: 2075 6e69 7175 6528 7365 6c66 293a 0d0a   unique(self):..
-000052b0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-000052c0: 2020 2020 203e 3e3e 2069 5475 706c 6528       >>> iTuple(
-000052d0: 5b31 2c20 312c 2033 2c20 322c 2034 2c20  [1, 1, 3, 2, 4, 
-000052e0: 322c 2033 5d29 2e75 6e69 7175 6528 290d  2, 3]).unique().
-000052f0: 0a20 2020 2020 2020 2069 5475 706c 6528  .        iTuple(
-00005300: 312c 2033 2c20 322c 2034 290d 0a20 2020  1, 3, 2, 4)..   
-00005310: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00005320: 2020 6465 6620 6974 6572 2829 3a0d 0a20    def iter():.. 
-00005330: 2020 2020 2020 2020 2020 2073 6565 6e20             seen 
-00005340: 3d20 7365 7428 290d 0a20 2020 2020 2020  = set()..       
-00005350: 2020 2020 2073 6565 6e5f 6164 6420 3d20       seen_add = 
-00005360: 7365 656e 2e61 6464 0d0a 2020 2020 2020  seen.add..      
-00005370: 2020 2020 2020 7365 656e 5f63 6f6e 7461        seen_conta
-00005380: 696e 7320 3d20 7365 656e 2e5f 5f63 6f6e  ins = seen.__con
-00005390: 7461 696e 735f 5f0d 0a20 2020 2020 2020  tains__..       
-000053a0: 2020 2020 2066 6f72 2076 2069 6e20 6974       for v in it
-000053b0: 6572 746f 6f6c 732e 6669 6c74 6572 6661  ertools.filterfa
-000053c0: 6c73 6528 7365 656e 5f63 6f6e 7461 696e  lse(seen_contain
-000053d0: 732c 2073 656c 6629 3a0d 0a20 2020 2020  s, self):..     
-000053e0: 2020 2020 2020 2020 2020 2073 6565 6e5f             seen_
-000053f0: 6164 6428 7629 0d0a 2020 2020 2020 2020  add(v)..        
-00005400: 2020 2020 2020 2020 7969 656c 6420 760d          yield v.
-00005410: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00005420: 7479 7065 2873 656c 6629 2864 6174 613d  type(self)(data=
-00005430: 6974 6572 2829 290d 0a20 2020 200d 0a20  iter())..    .. 
-00005440: 2020 2064 6566 2073 6f72 7428 7365 6c66     def sort(self
-00005450: 2c20 6620 3d20 6c61 6d62 6461 2076 3a20  , f = lambda v: 
-00005460: 7629 3a0d 0a20 2020 2020 2020 2022 2222  v):..        """
-00005470: 0d0a 2020 2020 2020 2020 3e3e 3e20 6954  ..        >>> iT
-00005480: 7570 6c65 2e72 616e 6765 2833 292e 7265  uple.range(3).re
-00005490: 7665 7273 6528 292e 736f 7274 2829 0d0a  verse().sort()..
-000054a0: 2020 2020 2020 2020 6954 7570 6c65 2830          iTuple(0
-000054b0: 2c20 312c 2032 290d 0a20 2020 2020 2020  , 1, 2)..       
-000054c0: 203e 3e3e 2069 5475 706c 652e 7261 6e67   >>> iTuple.rang
-000054d0: 6528 3329 2e73 6f72 7428 290d 0a20 2020  e(3).sort()..   
-000054e0: 2020 2020 2069 5475 706c 6528 302c 2031       iTuple(0, 1
-000054f0: 2c20 3229 0d0a 2020 2020 2020 2020 2222  , 2)..        ""
-00005500: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-00005510: 6e20 7479 7065 2873 656c 6629 2864 6174  n type(self)(dat
-00005520: 613d 736f 7274 6564 2873 656c 662c 206b  a=sorted(self, k
-00005530: 6579 203d 2066 2929 0d0a 0d0a 2020 2020  ey = f))....    
-00005540: 6465 6620 6163 6375 6d75 6c61 7465 2873  def accumulate(s
-00005550: 656c 662c 2066 2c20 696e 6974 6961 6c20  elf, f, initial 
-00005560: 3d20 4e6f 6e65 2c20 6c61 7a79 203d 2046  = None, lazy = F
-00005570: 616c 7365 293a 0d0a 2020 2020 2020 2020  alse):..        
-00005580: 2222 220d 0a20 2020 2020 2020 203e 3e3e  """..        >>>
-00005590: 2069 5475 706c 652e 7261 6e67 6528 3329   iTuple.range(3)
-000055a0: 2e61 6363 756d 756c 6174 6528 6c61 6d62  .accumulate(lamb
-000055b0: 6461 2061 6363 2c20 763a 2076 290d 0a20  da acc, v: v).. 
-000055c0: 2020 2020 2020 2069 5475 706c 6528 302c         iTuple(0,
-000055d0: 2031 2c20 3229 0d0a 2020 2020 2020 2020   1, 2)..        
-000055e0: 3e3e 3e20 6954 7570 6c65 2e72 616e 6765  >>> iTuple.range
-000055f0: 2833 292e 6163 6375 6d75 6c61 7465 286c  (3).accumulate(l
-00005600: 616d 6264 6120 6163 632c 2076 3a20 762c  ambda acc, v: v,
-00005610: 2069 6e69 7469 616c 3d30 290d 0a20 2020   initial=0)..   
-00005620: 2020 2020 2069 5475 706c 6528 302c 2030       iTuple(0, 0
-00005630: 2c20 312c 2032 290d 0a20 2020 2020 2020  , 1, 2)..       
-00005640: 203e 3e3e 2069 5475 706c 652e 7261 6e67   >>> iTuple.rang
-00005650: 6528 3329 2e61 6363 756d 756c 6174 6528  e(3).accumulate(
-00005660: 6f70 6572 6174 6f72 2e61 6464 290d 0a20  operator.add).. 
-00005670: 2020 2020 2020 2069 5475 706c 6528 302c         iTuple(0,
-00005680: 2031 2c20 3329 0d0a 2020 2020 2020 2020   1, 3)..        
-00005690: 2222 220d 0a20 2020 2020 2020 2072 6573  """..        res
-000056a0: 203d 2069 7465 7274 6f6f 6c73 2e61 6363   = itertools.acc
-000056b0: 756d 756c 6174 6528 7365 6c66 2c20 6675  umulate(self, fu
-000056c0: 6e63 3d66 2c20 696e 6974 6961 6c3d 696e  nc=f, initial=in
-000056d0: 6974 6961 6c29 0d0a 2020 2020 2020 2020  itial)..        
-000056e0: 7265 7475 726e 2072 6573 2069 6620 6c61  return res if la
-000056f0: 7a79 2065 6c73 6520 6954 7570 6c65 2864  zy else iTuple(d
-00005700: 6174 613d 7265 7329 0d0a 0d0a 2020 2020  ata=res)....    
-00005710: 6465 6620 666f 6c64 6375 6d28 7365 6c66  def foldcum(self
-00005720: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
-00005730: 7329 3a0d 0a20 2020 2020 2020 2022 2222  s):..        """
-00005740: 0d0a 2020 2020 2020 2020 3e3e 3e20 6954  ..        >>> iT
-00005750: 7570 6c65 2e72 616e 6765 2833 292e 666f  uple.range(3).fo
-00005760: 6c64 6375 6d28 6c61 6d62 6461 2061 6363  ldcum(lambda acc
-00005770: 2c20 763a 2076 290d 0a20 2020 2020 2020  , v: v)..       
-00005780: 2069 5475 706c 6528 302c 2031 2c20 3229   iTuple(0, 1, 2)
-00005790: 0d0a 2020 2020 2020 2020 3e3e 3e20 6954  ..        >>> iT
-000057a0: 7570 6c65 2e72 616e 6765 2833 292e 666f  uple.range(3).fo
-000057b0: 6c64 6375 6d28 6f70 6572 6174 6f72 2e61  ldcum(operator.a
-000057c0: 6464 290d 0a20 2020 2020 2020 2069 5475  dd)..        iTu
-000057d0: 706c 6528 302c 2031 2c20 3329 0d0a 2020  ple(0, 1, 3)..  
-000057e0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-000057f0: 2020 2072 6574 7572 6e20 7365 6c66 2e61     return self.a
-00005800: 6363 756d 756c 6174 6528 2a61 7267 732c  ccumulate(*args,
-00005810: 202a 2a6b 7761 7267 7329 0d0a 0d0a 2020   **kwargs)....  
-00005820: 2020 6465 6620 666f 6c64 2873 656c 662c    def fold(self,
-00005830: 2066 2c20 696e 6974 6961 6c3d 4e6f 6e65   f, initial=None
-00005840: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
-00005850: 0a20 2020 2020 2020 203e 3e3e 2069 5475  .        >>> iTu
-00005860: 706c 652e 7261 6e67 6528 3329 2e66 6f6c  ple.range(3).fol
-00005870: 6428 6c61 6d62 6461 2061 6363 2c20 763a  d(lambda acc, v:
-00005880: 2076 290d 0a20 2020 2020 2020 2032 0d0a   v)..        2..
-00005890: 2020 2020 2020 2020 3e3e 3e20 6954 7570          >>> iTup
-000058a0: 6c65 2e72 616e 6765 2833 292e 666f 6c64  le.range(3).fold
-000058b0: 286c 616d 6264 6120 6163 632c 2076 3a20  (lambda acc, v: 
-000058c0: 762c 2069 6e69 7469 616c 3d30 290d 0a20  v, initial=0).. 
-000058d0: 2020 2020 2020 2032 0d0a 2020 2020 2020         2..      
-000058e0: 2020 3e3e 3e20 6954 7570 6c65 2e72 616e    >>> iTuple.ran
-000058f0: 6765 2833 292e 666f 6c64 286f 7065 7261  ge(3).fold(opera
-00005900: 746f 722e 6164 6429 0d0a 2020 2020 2020  tor.add)..      
-00005910: 2020 330d 0a20 2020 2020 2020 2022 2222    3..        """
-00005920: 0d0a 2020 2020 2020 2020 6966 2069 6e69  ..        if ini
-00005930: 7469 616c 2069 7320 6e6f 7420 4e6f 6e65  tial is not None
-00005940: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00005950: 6573 203d 2066 756e 6374 6f6f 6c73 2e72  es = functools.r
-00005960: 6564 7563 6528 662c 2073 656c 662c 2069  educe(f, self, i
-00005970: 6e69 7469 616c 290d 0a20 2020 2020 2020  nitial)..       
-00005980: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00005990: 2020 2020 7265 7320 3d20 6675 6e63 746f      res = functo
-000059a0: 6f6c 732e 7265 6475 6365 2866 2c20 7365  ols.reduce(f, se
-000059b0: 6c66 290d 0a20 2020 2020 2020 2072 6574  lf)..        ret
-000059c0: 7572 6e20 7265 730d 0a0d 0a20 2020 2023  urn res....    #
-000059d0: 202d 2d2d 2d2d 0d0a 0d0a 2020 2020 2320   -----....    # 
-000059e0: 636f 6d62 696e 6174 6f72 6963 730d 0a0d  combinatorics...
-000059f0: 0a20 2020 2023 202d 2d2d 2d2d 0d0a 0d0a  .    # -----....
-00005a00: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  # --------------
-00005a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005a40: 2d0d 0a0d 0a40 6e54 7570 6c65 2e64 6563  -....@nTuple.dec
-00005a50: 6f72 6174 650d 0a63 6c61 7373 2045 7861  orate..class Exa
-00005a60: 6d70 6c65 2874 7970 696e 672e 4e61 6d65  mple(typing.Name
-00005a70: 6454 7570 6c65 293a 0d0a 2020 2020 2222  dTuple):..    ""
-00005a80: 220d 0a20 2020 203e 3e3e 2065 7820 3d20  "..    >>> ex = 
-00005a90: 4578 616d 706c 6528 312c 2022 6122 290d  Example(1, "a").
-00005aa0: 0a20 2020 203e 3e3e 2065 780d 0a20 2020  .    >>> ex..   
-00005ab0: 2045 7861 6d70 6c65 2878 3d31 2c20 733d   Example(x=1, s=
-00005ac0: 2761 272c 2069 743d 6954 7570 6c65 2829  'a', it=iTuple()
-00005ad0: 290d 0a20 2020 203e 3e3e 2065 782e 636c  )..    >>> ex.cl
-00005ae0: 730d 0a20 2020 203c 636c 6173 7320 2778  s..    <class 'x
-00005af0: 7475 706c 6573 2e78 7475 706c 6573 2e6e  tuples.xtuples.n
-00005b00: 5475 706c 6527 3e0d 0a20 2020 203e 3e3e  Tuple'>..    >>>
-00005b10: 2065 782e 7069 7065 286c 616d 6264 6120   ex.pipe(lambda 
-00005b20: 6e74 3a20 6e74 2e78 290d 0a20 2020 2031  nt: nt.x)..    1
-00005b30: 0d0a 2020 2020 3e3e 3e20 6620 3d20 6578  ..    >>> f = ex
-00005b40: 2e70 6172 7469 616c 286c 616d 6264 6120  .partial(lambda 
-00005b50: 6e74 2c20 763a 206e 742e 7820 2a20 7629  nt, v: nt.x * v)
-00005b60: 0d0a 2020 2020 3e3e 3e20 6628 3229 0d0a  ..    >>> f(2)..
-00005b70: 2020 2020 320d 0a20 2020 203e 3e3e 2066      2..    >>> f
-00005b80: 2833 290d 0a20 2020 2033 0d0a 2020 2020  (3)..    3..    
-00005b90: 2222 220d 0a20 2020 2023 204e 4f54 453a  """..    # NOTE:
-00005ba0: 2063 6c73 2c20 7069 7065 2c20 7061 7274   cls, pipe, part
-00005bb0: 6961 6c20 6172 6520 6d61 6e64 6174 6f72  ial are mandator
-00005bc0: 7920 626f 696c 6572 706c 6174 650d 0a0d  y boilerplate...
-00005bd0: 0a20 2020 2078 3a20 696e 740d 0a20 2020  .    x: int..   
-00005be0: 2073 3a20 7374 720d 0a20 2020 2069 743a   s: str..    it:
-00005bf0: 2069 5475 706c 6520 3d20 6954 7570 6c65   iTuple = iTuple
-00005c00: 285b 5d29 0d0a 0d0a 2020 2020 4070 726f  ([])....    @pro
-00005c10: 7065 7274 790d 0a20 2020 2064 6566 2063  perty..    def c
-00005c20: 6c73 2873 656c 6629 3a0d 0a20 2020 2020  ls(self):..     
-00005c30: 2020 202e 2e2e 0d0a 0d0a 2020 2020 6465     .......    de
-00005c40: 6620 7069 7065 2873 656c 662c 2066 2c20  f pipe(self, f, 
-00005c50: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
-00005c60: 3a0d 0a20 2020 2020 2020 202e 2e2e 0d0a  :..        .....
-00005c70: 0d0a 2020 2020 6465 6620 7061 7274 6961  ..    def partia
-00005c80: 6c28 7365 6c66 2c20 662c 202a 6172 6773  l(self, f, *args
-00005c90: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
-00005ca0: 2020 2020 2020 2e2e 2e0d 0a0d 0a23 202d        .......# -
+00000290: 0d0a 0d0a 2320 544f 444f 3a20 736f 6d65  ....# TODO: some
+000002a0: 206b 696e 6420 6f66 2076 616c 6964 6174   kind of validat
+000002b0: 696f 6e20 706c 6163 6568 6f6c 6465 723f  ion placeholder?
+000002c0: 0d0a 2320 6361 6c6c 6564 2069 6e20 696e  ..# called in in
+000002d0: 6974 2c20 6567 2e20 7175 6172 7465 7220  it, eg. quarter 
+000002e0: 696e 205b 3120 2e2e 2034 5d0d 0a0d 0a63  in [1 .. 4]....c
+000002f0: 6c61 7373 206e 5475 706c 6528 6162 632e  lass nTuple(abc.
+00000300: 4142 4329 3a0d 0a0d 0a20 2020 2040 6162  ABC):....    @ab
+00000310: 632e 6162 7374 7261 6374 6d65 7468 6f64  c.abstractmethod
+00000320: 0d0a 2020 2020 6465 6620 5f5f 6162 7374  ..    def __abst
+00000330: 7261 6374 5f5f 2873 656c 6629 3a0d 0a20  ract__(self):.. 
+00000340: 2020 2020 2020 2023 204e 4f54 453a 2068         # NOTE: h
+00000350: 6572 6520 746f 2070 7265 7665 6e74 2069  ere to prevent i
+00000360: 6e69 7469 616c 6973 6520 696e 7374 616e  nitialise instan
+00000370: 6365 7320 6f66 2074 6869 730d 0a20 2020  ces of this..   
+00000380: 2020 2020 2023 2062 7574 2072 6174 6865       # but rathe
+00000390: 7220 7573 6520 7468 6520 6465 636f 7261  r use the decora
+000003a0: 746f 7220 616e 6420 7479 7069 6e67 2e4e  tor and typing.N
+000003b0: 616d 6564 5475 706c 650d 0a20 2020 2020  amedTuple..     
+000003c0: 2020 2072 6574 7572 6e0d 0a0d 0a20 2020     return....   
+000003d0: 2040 7374 6174 6963 6d65 7468 6f64 0d0a   @staticmethod..
+000003e0: 2020 2020 6465 6620 7069 7065 286f 626a      def pipe(obj
+000003f0: 2c20 662c 202a 6172 6773 2c20 2a2a 6b77  , f, *args, **kw
+00000400: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
+00000410: 7265 7475 726e 2066 286f 626a 2c20 2a61  return f(obj, *a
+00000420: 7267 732c 202a 2a6b 7761 7267 7329 0d0a  rgs, **kwargs)..
+00000430: 0d0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+00000440: 686f 640d 0a20 2020 2064 6566 2070 6172  hod..    def par
+00000450: 7469 616c 286f 626a 2c20 662c 202a 6172  tial(obj, f, *ar
+00000460: 6773 2c20 2a2a 6b77 6172 6773 293a 0d0a  gs, **kwargs):..
+00000470: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00000480: 756e 6374 6f6f 6c73 2e70 6172 7469 616c  unctools.partial
+00000490: 2866 2c20 6f62 6a2c 202a 6172 6773 2c20  (f, obj, *args, 
+000004a0: 2a2a 6b77 6172 6773 290d 0a0d 0a20 2020  **kwargs)....   
+000004b0: 2040 636c 6173 736d 6574 686f 640d 0a20   @classmethod.. 
+000004c0: 2020 2064 6566 2069 735f 7375 6263 6c61     def is_subcla
+000004d0: 7373 2863 6c73 2c20 7429 3a0d 0a20 2020  ss(cls, t):..   
+000004e0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000004f0: 2020 3e3e 3e20 6e54 7570 6c65 2e69 735f    >>> nTuple.is_
+00000500: 7375 6263 6c61 7373 2874 7570 6c65 290d  subclass(tuple).
+00000510: 0a20 2020 2020 2020 2046 616c 7365 0d0a  .        False..
+00000520: 2020 2020 2020 2020 3e3e 3e20 6e54 7570          >>> nTup
+00000530: 6c65 2e69 735f 7375 6263 6c61 7373 2845  le.is_subclass(E
+00000540: 7861 6d70 6c65 2831 2c20 2261 2229 290d  xample(1, "a")).
+00000550: 0a20 2020 2020 2020 2046 616c 7365 0d0a  .        False..
+00000560: 2020 2020 2020 2020 3e3e 3e20 6e54 7570          >>> nTup
+00000570: 6c65 2e69 735f 7375 6263 6c61 7373 2845  le.is_subclass(E
+00000580: 7861 6d70 6c65 290d 0a20 2020 2020 2020  xample)..       
+00000590: 2054 7275 650d 0a20 2020 2020 2020 2022   True..        "
+000005a0: 2222 0d0a 2020 2020 2020 2020 7472 793a  ""..        try:
+000005b0: 0d0a 2020 2020 2020 2020 2020 2020 6973  ..            is
+000005c0: 5f73 7562 203d 2069 7373 7562 636c 6173  _sub = issubclas
+000005d0: 7328 742c 2074 7570 6c65 290d 0a20 2020  s(t, tuple)..   
+000005e0: 2020 2020 2065 7863 6570 743a 0d0a 2020       except:..  
+000005f0: 2020 2020 2020 2020 2020 6973 5f73 7562            is_sub
+00000600: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
+00000610: 2020 7265 7475 726e 2028 0d0a 2020 2020    return (..    
+00000620: 2020 2020 2020 2020 6973 5f73 7562 2061          is_sub a
+00000630: 6e64 0d0a 2020 2020 2020 2020 2020 2020  nd..            
+00000640: 6861 7361 7474 7228 742c 2022 636c 7322  hasattr(t, "cls"
+00000650: 2920 616e 640d 0a20 2020 2020 2020 2020  ) and..         
+00000660: 2020 2068 6173 6174 7472 2874 2c20 2270     hasattr(t, "p
+00000670: 6970 6522 2920 616e 640d 0a20 2020 2020  ipe") and..     
+00000680: 2020 2020 2020 2068 6173 6174 7472 2874         hasattr(t
+00000690: 2c20 2270 6172 7469 616c 2229 0d0a 2020  , "partial")..  
+000006a0: 2020 2020 2020 290d 0a0d 0a20 2020 2040        )....    @
+000006b0: 636c 6173 736d 6574 686f 640d 0a20 2020  classmethod..   
+000006c0: 2064 6566 2069 735f 696e 7374 616e 6365   def is_instance
+000006d0: 2863 6c73 2c20 6f62 6a29 3a0d 0a20 2020  (cls, obj):..   
+000006e0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000006f0: 2020 3e3e 3e20 6e54 7570 6c65 2e69 735f    >>> nTuple.is_
+00000700: 696e 7374 616e 6365 2874 7570 6c65 290d  instance(tuple).
+00000710: 0a20 2020 2020 2020 2046 616c 7365 0d0a  .        False..
+00000720: 2020 2020 2020 2020 3e3e 3e20 6e54 7570          >>> nTup
+00000730: 6c65 2e69 735f 696e 7374 616e 6365 2845  le.is_instance(E
+00000740: 7861 6d70 6c65 290d 0a20 2020 2020 2020  xample)..       
+00000750: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+00000760: 3e3e 3e20 6e54 7570 6c65 2e69 735f 696e  >>> nTuple.is_in
+00000770: 7374 616e 6365 2845 7861 6d70 6c65 2831  stance(Example(1
+00000780: 2c20 2261 2229 290d 0a20 2020 2020 2020  , "a"))..       
+00000790: 2054 7275 650d 0a20 2020 2020 2020 2022   True..        "
+000007a0: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
+000007b0: 726e 2028 0d0a 2020 2020 2020 2020 2020  rn (..          
+000007c0: 2020 636c 732e 6973 5f73 7562 636c 6173    cls.is_subclas
+000007d0: 7328 7479 7065 286f 626a 2929 2061 6e64  s(type(obj)) and
+000007e0: 0d0a 2020 2020 2020 2020 2020 2020 6861  ..            ha
+000007f0: 7361 7474 7228 6f62 6a2c 2027 5f61 7364  sattr(obj, '_asd
+00000800: 6963 7427 2920 616e 640d 0a20 2020 2020  ict') and..     
+00000810: 2020 2020 2020 2068 6173 6174 7472 286f         hasattr(o
+00000820: 626a 2c20 275f 6669 656c 6473 2729 0d0a  bj, '_fields')..
+00000830: 2020 2020 2020 2020 290d 0a0d 0a0d 0a20          )...... 
+00000840: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+00000850: 0d0a 2020 2020 6465 6620 616e 6e6f 7461  ..    def annota
+00000860: 7469 6f6e 7328 6f62 6a29 3a0d 0a20 2020  tions(obj):..   
+00000870: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00000880: 2020 3e3e 3e20 6578 203d 2045 7861 6d70    >>> ex = Examp
+00000890: 6c65 2831 2c20 2261 2229 0d0a 2020 2020  le(1, "a")..    
+000008a0: 2020 2020 3e3e 3e20 6578 2e70 6970 6528      >>> ex.pipe(
+000008b0: 6578 2e63 6c73 2e61 6e6e 6f74 6174 696f  ex.cls.annotatio
+000008c0: 6e73 290d 0a20 2020 2020 2020 207b 2778  ns)..        {'x
+000008d0: 273a 203c 636c 6173 7320 2769 6e74 273e  ': <class 'int'>
+000008e0: 2c20 2773 273a 203c 636c 6173 7320 2773  , 's': <class 's
+000008f0: 7472 273e 2c20 2769 7427 3a20 3c63 6c61  tr'>, 'it': <cla
+00000900: 7373 2027 7874 7570 6c65 732e 7874 7570  ss 'xtuples.xtup
+00000910: 6c65 732e 6954 7570 6c65 273e 7d0d 0a20  les.iTuple'>}.. 
+00000920: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00000930: 2020 2020 7265 7475 726e 2066 4469 6374      return fDict
+00000940: 286f 626a 2e5f 5f61 6e6e 6f74 6174 696f  (obj.__annotatio
+00000950: 6e73 5f5f 290d 0a0d 0a20 2020 2040 636c  ns__)....    @cl
+00000960: 6173 736d 6574 686f 640d 0a20 2020 2064  assmethod..    d
+00000970: 6566 2061 735f 6469 6374 2863 6c73 2c20  ef as_dict(cls, 
+00000980: 6f62 6a29 3a0d 0a20 2020 2020 2020 2022  obj):..        "
+00000990: 2222 0d0a 2020 2020 2020 2020 3e3e 3e20  ""..        >>> 
+000009a0: 6578 203d 2045 7861 6d70 6c65 2831 2c20  ex = Example(1, 
+000009b0: 2261 2229 0d0a 2020 2020 2020 2020 3e3e  "a")..        >>
+000009c0: 3e20 6578 2e70 6970 6528 6578 2e63 6c73  > ex.pipe(ex.cls
+000009d0: 2e61 735f 6469 6374 290d 0a20 2020 2020  .as_dict)..     
+000009e0: 2020 207b 2778 273a 2031 2c20 2773 273a     {'x': 1, 's':
+000009f0: 2027 6127 2c20 2769 7427 3a20 6954 7570   'a', 'it': iTup
+00000a00: 6c65 2829 7d0d 0a20 2020 2020 2020 2022  le()}..        "
+00000a10: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
+00000a20: 726e 2066 4469 6374 286f 626a 2e5f 6173  rn fDict(obj._as
+00000a30: 6469 6374 2829 290d 0a0d 0a20 2020 2040  dict())....    @
+00000a40: 636c 6173 736d 6574 686f 640d 0a20 2020  classmethod..   
+00000a50: 2064 6566 2063 6173 745f 6a73 6f6e 2863   def cast_json(c
+00000a60: 6c73 2c20 6f62 6a29 3a0d 0a20 2020 2020  ls, obj):..     
+00000a70: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00000a80: 3e3e 3e20 6578 203d 2045 7861 6d70 6c65  >>> ex = Example
+00000a90: 2831 2c20 2261 2229 0d0a 2020 2020 2020  (1, "a")..      
+00000aa0: 2020 3e3e 3e20 6578 2e70 6970 6528 6578    >>> ex.pipe(ex
+00000ab0: 2e63 6c73 2e63 6173 745f 6a73 6f6e 290d  .cls.cast_json).
+00000ac0: 0a20 2020 2020 2020 207b 2778 273a 2031  .        {'x': 1
+00000ad0: 2c20 2773 273a 2027 6127 2c20 2769 7427  , 's': 'a', 'it'
+00000ae0: 3a20 7b27 5f5f 745f 5f27 3a20 2769 5475  : {'__t__': 'iTu
+00000af0: 706c 6527 2c20 2764 6174 6127 3a20 5b5d  ple', 'data': []
+00000b00: 7d2c 2027 5f5f 745f 5f27 3a20 2745 7861  }, '__t__': 'Exa
+00000b10: 6d70 6c65 277d 0d0a 2020 2020 2020 2020  mple'}..        
+00000b20: 2222 220d 0a20 2020 2020 2020 2064 203d  """..        d =
+00000b30: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00000b40: 6b3a 2063 6173 745f 6a73 6f6e 2876 290d  k: cast_json(v).
+00000b50: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00000b60: 206b 2c20 7620 696e 206f 626a 2e5f 6173   k, v in obj._as
+00000b70: 6469 6374 2829 2e69 7465 6d73 2829 0d0a  dict().items()..
+00000b80: 2020 2020 2020 2020 2020 2020 230d 0a20              #.. 
+00000b90: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+00000ba0: 2020 645b 225f 5f74 5f5f 225d 203d 2074    d["__t__"] = t
+00000bb0: 7970 6528 6f62 6a29 2e5f 5f6e 616d 655f  ype(obj).__name_
+00000bc0: 5f0d 0a20 2020 2020 2020 2072 6574 7572  _..        retur
+00000bd0: 6e20 640d 0a0d 0a20 2020 2040 636c 6173  n d....    @clas
+00000be0: 736d 6574 686f 640d 0a20 2020 2064 6566  smethod..    def
+00000bf0: 2075 6e63 6173 745f 6a73 6f6e 286d 6574   uncast_json(met
+00000c00: 612c 206f 626a 293a 0d0a 2020 2020 2020  a, obj):..      
+00000c10: 2020 2222 220d 0a20 2020 2020 2020 203e    """..        >
+00000c20: 3e3e 2065 7820 3d20 4578 616d 706c 6528  >> ex = Example(
+00000c30: 312c 2022 6122 290d 0a20 2020 2020 2020  1, "a")..       
+00000c40: 203e 3e3e 2065 782e 636c 732e 756e 6361   >>> ex.cls.unca
+00000c50: 7374 5f6a 736f 6e28 6578 2e70 6970 6528  st_json(ex.pipe(
+00000c60: 6578 2e63 6c73 2e63 6173 745f 6a73 6f6e  ex.cls.cast_json
+00000c70: 2929 0d0a 2020 2020 2020 2020 4578 616d  ))..        Exam
+00000c80: 706c 6528 783d 312c 2073 3d27 6127 2c20  ple(x=1, s='a', 
+00000c90: 6974 3d69 5475 706c 6528 2929 0d0a 2020  it=iTuple())..  
+00000ca0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00000cb0: 2020 2063 6c73 203d 2052 4547 4953 5452     cls = REGISTR
+00000cc0: 595b 6f62 6a5b 225f 5f74 5f5f 225d 5d0d  Y[obj["__t__"]].
+00000cd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000ce0: 636c 7328 0d0a 2020 2020 2020 2020 2020  cls(..          
+00000cf0: 2020 2a28 0d0a 2020 2020 2020 2020 2020    *(..          
+00000d00: 2020 2020 2020 756e 6361 7374 5f6a 736f        uncast_jso
+00000d10: 6e28 7629 0d0a 2020 2020 2020 2020 2020  n(v)..          
+00000d20: 2020 2020 2020 666f 7220 6b2c 2076 2069        for k, v i
+00000d30: 6e20 6f62 6a2e 6974 656d 7328 2920 6966  n obj.items() if
+00000d40: 206b 2021 3d20 225f 5f74 5f5f 220d 0a20   k != "__t__".. 
+00000d50: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00000d60: 2020 2020 2020 290d 0a0d 0a20 2020 2040        )....    @
+00000d70: 636c 6173 736d 6574 686f 640d 0a20 2020  classmethod..   
+00000d80: 2064 6566 2064 6563 6f72 6174 6528 6d65   def decorate(me
+00000d90: 7461 2c20 636c 7329 3a0d 0a20 2020 2020  ta, cls):..     
+00000da0: 2020 2061 7373 6572 7420 636c 732e 5f5f     assert cls.__
+00000db0: 6e61 6d65 5f5f 206e 6f74 2069 6e20 5245  name__ not in RE
+00000dc0: 4749 5354 5259 0d0a 2020 2020 2020 2020  GISTRY..        
+00000dd0: 636c 732e 7069 7065 203d 206d 6574 612e  cls.pipe = meta.
+00000de0: 7069 7065 0d0a 2020 2020 2020 2020 636c  pipe..        cl
+00000df0: 732e 7061 7274 6961 6c20 3d20 6d65 7461  s.partial = meta
+00000e00: 2e70 6172 7469 616c 0d0a 2020 2020 2020  .partial..      
+00000e10: 2020 636c 732e 636c 7320 3d20 6d65 7461    cls.cls = meta
+00000e20: 0d0a 2020 2020 2020 2020 5245 4749 5354  ..        REGIST
+00000e30: 5259 5b63 6c73 2e5f 5f6e 616d 655f 5f5d  RY[cls.__name__]
+00000e40: 203d 2063 6c73 0d0a 2020 2020 2020 2020   = cls..        
+00000e50: 7265 7475 726e 2063 6c73 0d0a 0d0a 2320  return cls....# 
+00000e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d  ---------------.
+00000ea0: 0a0d 0a63 6c61 7373 2066 4469 6374 2863  ...class fDict(c
+00000eb0: 6f6c 6c65 6374 696f 6e73 2e55 7365 7244  ollections.UserD
+00000ec0: 6963 7429 3a0d 0a20 2020 205f 5f73 6c6f  ict):..    __slo
+00000ed0: 7473 5f5f 203d 2028 290d 0a0d 0a20 2020  ts__ = ()....   
+00000ee0: 2064 6174 613a 2064 6963 740d 0a0d 0a20   data: dict.... 
+00000ef0: 2020 2064 6566 2070 6970 6528 7365 6c66     def pipe(self
+00000f00: 2c20 662c 202a 6172 6773 2c20 2a2a 6b77  , f, *args, **kw
+00000f10: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
+00000f20: 2222 220d 0a20 2020 2020 2020 203e 3e3e  """..        >>>
+00000f30: 2066 4469 6374 287b 303a 2031 7d29 2e70   fDict({0: 1}).p
+00000f40: 6970 6528 6c61 6d62 6461 2064 3a20 642e  ipe(lambda d: d.
+00000f50: 6d61 705f 7661 6c75 6573 280d 0a20 2020  map_values(..   
+00000f60: 2020 2020 202e 2e2e 2020 2020 206c 616d       ...     lam
+00000f70: 6264 6120 763a 2076 202b 2031 0d0a 2020  bda v: v + 1..  
+00000f80: 2020 2020 2020 2e2e 2e20 2929 0d0a 2020        ... ))..  
+00000f90: 2020 2020 2020 7b30 3a20 327d 0d0a 2020        {0: 2}..  
+00000fa0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00000fb0: 2020 2072 6573 203d 2066 2873 656c 662c     res = f(self,
+00000fc0: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
+00000fd0: 290d 0a20 2020 2020 2020 2069 6620 6973  )..        if is
+00000fe0: 696e 7374 616e 6365 2872 6573 2c20 6469  instance(res, di
+00000ff0: 6374 293a 0d0a 2020 2020 2020 2020 2020  ct):..          
+00001000: 2020 7265 7475 726e 2066 4469 6374 2872    return fDict(r
+00001010: 6573 290d 0a20 2020 2020 2020 2072 6574  es)..        ret
+00001020: 7572 6e20 7265 730d 0a0d 0a20 2020 2064  urn res....    d
+00001030: 6566 2070 6172 7469 616c 2873 656c 662c  ef partial(self,
+00001040: 2066 2c20 2a61 7267 732c 202a 2a6b 7761   f, *args, **kwa
+00001050: 7267 7329 3a0d 0a20 2020 2020 2020 2022  rgs):..        "
+00001060: 2222 0d0a 2020 2020 2020 2020 3e3e 3e20  ""..        >>> 
+00001070: 6620 3d20 6644 6963 7428 7b30 3a20 317d  f = fDict({0: 1}
+00001080: 292e 7061 7274 6961 6c28 0d0a 2020 2020  ).partial(..    
+00001090: 2020 2020 2e2e 2e20 2020 2020 6c61 6d62      ...     lamb
+000010a0: 6461 2064 2c20 6e3a 2064 2e6d 6170 5f76  da d, n: d.map_v
+000010b0: 616c 7565 7328 6c61 6d62 6461 2076 3a20  alues(lambda v: 
+000010c0: 7620 2b20 6e29 0d0a 2020 2020 2020 2020  v + n)..        
+000010d0: 2e2e 2e20 290d 0a20 2020 2020 2020 203e  ... )..        >
+000010e0: 3e3e 2066 2831 290d 0a20 2020 2020 2020  >> f(1)..       
+000010f0: 207b 303a 2032 7d0d 0a20 2020 2020 2020   {0: 2}..       
+00001100: 203e 3e3e 2066 2832 290d 0a20 2020 2020   >>> f(2)..     
+00001110: 2020 207b 303a 2033 7d0d 0a20 2020 2020     {0: 3}..     
+00001120: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00001130: 7265 7475 726e 2066 756e 6374 6f6f 6c73  return functools
+00001140: 2e70 6172 7469 616c 2866 2c20 7365 6c66  .partial(f, self
+00001150: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
+00001160: 7329 0d0a 0d0a 2020 2020 6465 6620 6b65  s)....    def ke
+00001170: 7973 5f74 7570 6c65 2873 656c 6629 3a0d  ys_tuple(self):.
+00001180: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00001190: 2020 2020 2020 3e3e 3e20 6644 6963 7428        >>> fDict(
+000011a0: 7b30 3a20 317d 292e 6b65 7973 5f74 7570  {0: 1}).keys_tup
+000011b0: 6c65 2829 0d0a 2020 2020 2020 2020 6954  le()..        iT
+000011c0: 7570 6c65 2830 290d 0a20 2020 2020 2020  uple(0)..       
+000011d0: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
+000011e0: 7475 726e 2069 5475 706c 652e 6672 6f6d  turn iTuple.from
+000011f0: 5f6b 6579 7328 7365 6c66 290d 0a0d 0a20  _keys(self).... 
+00001200: 2020 2064 6566 2076 616c 7565 735f 7475     def values_tu
+00001210: 706c 6528 7365 6c66 293a 0d0a 2020 2020  ple(self):..    
+00001220: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00001230: 203e 3e3e 2066 4469 6374 287b 303a 2031   >>> fDict({0: 1
+00001240: 7d29 2e76 616c 7565 735f 7475 706c 6528  }).values_tuple(
+00001250: 290d 0a20 2020 2020 2020 2069 5475 706c  )..        iTupl
+00001260: 6528 3129 0d0a 2020 2020 2020 2020 2222  e(1)..        ""
+00001270: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+00001280: 6e20 6954 7570 6c65 2e66 726f 6d5f 7661  n iTuple.from_va
+00001290: 6c75 6573 2873 656c 6629 0d0a 2020 2020  lues(self)..    
+000012a0: 0d0a 2020 2020 6465 6620 6974 656d 735f  ..    def items_
+000012b0: 7475 706c 6528 7365 6c66 293a 0d0a 2020  tuple(self):..  
+000012c0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+000012d0: 2020 203e 3e3e 2066 4469 6374 287b 303a     >>> fDict({0:
+000012e0: 2031 7d29 2e69 7465 6d73 5f74 7570 6c65   1}).items_tuple
+000012f0: 2829 0d0a 2020 2020 2020 2020 6954 7570  ()..        iTup
+00001300: 6c65 2828 302c 2031 2929 0d0a 2020 2020  le((0, 1))..    
+00001310: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00001320: 2072 6574 7572 6e20 6954 7570 6c65 2e66   return iTuple.f
+00001330: 726f 6d5f 6974 656d 7328 7365 6c66 290d  rom_items(self).
+00001340: 0a0d 0a20 2020 2023 204e 4f54 453a 2077  ...    # NOTE: w
+00001350: 6520 6861 7665 2073 6570 6172 6174 6520  e have separate 
+00001360: 6d61 7020 696d 706c 656d 656e 7461 7469  map implementati
+00001370: 6f6e 7320 0d0a 2020 2020 2320 6173 2074  ons ..    # as t
+00001380: 6865 7920 6172 6520 636f 6e73 7461 6e74  hey are constant
+00001390: 2073 697a 652c 2064 6963 7420 746f 2064   size, dict to d
+000013a0: 6963 740d 0a20 2020 2023 206f 7468 6572  ict..    # other
+000013b0: 2069 7465 7261 746f 7220 6675 6e63 7469   iterator functi
+000013c0: 6f6e 7320 7368 6f75 6c64 2075 7365 2069  ons should use i
+000013d0: 5475 706c 6520 2866 726f 6d20 7468 6520  Tuple (from the 
+000013e0: 6162 6f76 6529 0d0a 0d0a 2020 2020 6465  above)....    de
+000013f0: 6620 6d61 705f 6b65 7973 2873 656c 662c  f map_keys(self,
+00001400: 2066 2c20 2a61 7267 732c 202a 2a6b 7761   f, *args, **kwa
+00001410: 7267 7329 3a0d 0a20 2020 2020 2020 2022  rgs):..        "
+00001420: 2222 0d0a 2020 2020 2020 2020 3e3e 3e20  ""..        >>> 
+00001430: 6644 6963 7428 7b30 3a20 317d 292e 6d61  fDict({0: 1}).ma
+00001440: 705f 6b65 7973 286c 616d 6264 6120 763a  p_keys(lambda v:
+00001450: 2076 202b 2031 290d 0a20 2020 2020 2020   v + 1)..       
+00001460: 207b 313a 2031 7d0d 0a20 2020 2020 2020   {1: 1}..       
+00001470: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
+00001480: 7475 726e 2066 4469 6374 280d 0a20 2020  turn fDict(..   
+00001490: 2020 2020 2020 2020 2028 6628 6b2c 202a           (f(k, *
+000014a0: 6172 6773 2c20 2a2a 6b77 6172 6773 292c  args, **kwargs),
+000014b0: 2076 2920 666f 7220 6b2c 2076 2069 6e20   v) for k, v in 
+000014c0: 7365 6c66 2e69 7465 6d73 2829 0d0a 2020  self.items()..  
+000014d0: 2020 2020 2020 290d 0a0d 0a20 2020 2064        )....    d
+000014e0: 6566 206d 6170 5f76 616c 7565 7328 7365  ef map_values(se
+000014f0: 6c66 2c20 662c 202a 6172 6773 2c20 2a2a  lf, f, *args, **
+00001500: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
+00001510: 2020 2222 220d 0a20 2020 2020 2020 203e    """..        >
+00001520: 3e3e 2066 4469 6374 287b 303a 2031 7d29  >> fDict({0: 1})
+00001530: 2e6d 6170 5f76 616c 7565 7328 6c61 6d62  .map_values(lamb
+00001540: 6461 2076 3a20 7620 2b20 3129 0d0a 2020  da v: v + 1)..  
+00001550: 2020 2020 2020 7b30 3a20 327d 0d0a 2020        {0: 2}..  
+00001560: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00001570: 2020 2072 6574 7572 6e20 6644 6963 7428     return fDict(
+00001580: 0d0a 2020 2020 2020 2020 2020 2020 286b  ..            (k
+00001590: 2c20 6628 762c 202a 6172 6773 2c20 2a2a  , f(v, *args, **
+000015a0: 6b77 6172 6773 2929 2066 6f72 206b 2c20  kwargs)) for k, 
+000015b0: 7620 696e 2073 656c 662e 6974 656d 7328  v in self.items(
+000015c0: 290d 0a20 2020 2020 2020 2029 0d0a 0d0a  )..        )....
+000015d0: 2020 2020 6465 6620 6d61 705f 6974 656d      def map_item
+000015e0: 7328 7365 6c66 2c20 662c 202a 6172 6773  s(self, f, *args
+000015f0: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
+00001600: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00001610: 2020 203e 3e3e 2066 4469 6374 287b 303a     >>> fDict({0:
+00001620: 2031 7d29 2e6d 6170 5f69 7465 6d73 286c   1}).map_items(l
+00001630: 616d 6264 6120 6b2c 2076 3a20 2876 2c20  ambda k, v: (v, 
+00001640: 6b29 290d 0a20 2020 2020 2020 207b 313a  k))..        {1:
+00001650: 2030 7d0d 0a20 2020 2020 2020 2022 2222   0}..        """
+00001660: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00001670: 2066 4469 6374 280d 0a20 2020 2020 2020   fDict(..       
+00001680: 2020 2020 2066 286b 2c20 762c 202a 6172       f(k, v, *ar
+00001690: 6773 2c20 2a2a 6b77 6172 6773 2920 666f  gs, **kwargs) fo
+000016a0: 7220 6b2c 2076 2069 6e20 7365 6c66 2e69  r k, v in self.i
+000016b0: 7465 6d73 2829 0d0a 2020 2020 2020 2020  tems()..        
+000016c0: 290d 0a0d 0a20 2020 2064 6566 2069 6e76  )....    def inv
+000016d0: 6572 7428 7365 6c66 293a 0d0a 2020 2020  ert(self):..    
+000016e0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000016f0: 203e 3e3e 2066 4469 6374 287b 303a 2031   >>> fDict({0: 1
+00001700: 7d29 2e69 6e76 6572 7428 290d 0a20 2020  }).invert()..   
+00001710: 2020 2020 207b 313a 2030 7d0d 0a20 2020       {1: 0}..   
+00001720: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00001730: 2020 7265 7475 726e 2066 4469 6374 2828    return fDict((
+00001740: 762c 206b 2920 666f 7220 6b2c 2076 2069  v, k) for k, v i
+00001750: 6e20 7365 6c66 2e69 7465 6d73 2829 290d  n self.items()).
+00001760: 0a0d 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d  ...# -----------
+00001770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000017a0: 2d2d 2d2d 0d0a 0d0a 4064 6174 6163 6c61  ----....@datacla
+000017b0: 7373 6573 2e64 6174 6163 6c61 7373 2869  sses.dataclass(i
+000017c0: 6e69 7420 3d20 4661 6c73 652c 2072 6570  nit = False, rep
+000017d0: 723d 5472 7565 290d 0a63 6c61 7373 2069  r=True)..class i
+000017e0: 5475 706c 6528 636f 6c6c 6563 7469 6f6e  Tuple(collection
+000017f0: 732e 5573 6572 4c69 7374 2c20 7475 706c  s.UserList, tupl
+00001800: 6529 3a20 2320 7479 7065 3a20 6967 6e6f  e): # type: igno
+00001810: 7265 0d0a 2020 2020 5f5f 736c 6f74 735f  re..    __slots_
+00001820: 5f20 3d20 2829 0d0a 0d0a 2020 2020 6461  _ = ()....    da
+00001830: 7461 3a20 7475 706c 6520 2320 7479 7065  ta: tuple # type
+00001840: 3a20 6967 6e6f 7265 0d0a 0d0a 2020 2020  : ignore....    
+00001850: 2320 2d2d 2d2d 2d0d 0a0d 0a20 2020 2040  # -----....    @
+00001860: 7374 6174 6963 6d65 7468 6f64 0d0a 2020  staticmethod..  
+00001870: 2020 6465 6620 5f5f 6e65 775f 5f28 636c    def __new__(cl
+00001880: 732c 2064 6174 6120 3d20 4e6f 6e65 293a  s, data = None):
+00001890: 0d0a 2020 2020 2020 2020 2320 4e4f 5445  ..        # NOTE
+000018a0: 3a20 7765 2075 7365 2063 6c73 206e 6f74  : we use cls not
+000018b0: 2061 7272 6179 0d0a 2020 2020 2020 2020   array..        
+000018c0: 2320 736f 2073 7562 2d63 6c61 7373 696e  # so sub-classin
+000018d0: 6720 2a64 6f65 732a 2063 6861 6e67 6520  g *does* change 
+000018e0: 6964 656e 7469 7479 0d0a 2020 2020 2020  identity..      
+000018f0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00001900: 6461 7461 2c20 636c 7329 3a0d 0a20 2020  data, cls):..   
+00001910: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001920: 6461 7461 0d0a 2020 2020 2020 2020 7265  data..        re
+00001930: 7475 726e 2073 7570 6572 2829 2e5f 5f6e  turn super().__n
+00001940: 6577 5f5f 2863 6c73 2c20 6461 7461 3d64  ew__(cls, data=d
+00001950: 6174 6129 0d0a 0d0a 2020 2020 4073 7461  ata)....    @sta
+00001960: 7469 636d 6574 686f 640d 0a20 2020 2064  ticmethod..    d
+00001970: 6566 2077 7261 705f 7475 706c 6528 6461  ef wrap_tuple(da
+00001980: 7461 293a 0d0a 2020 2020 2020 2020 7265  ta):..        re
+00001990: 7475 726e 2064 6174 6120 6966 2069 7369  turn data if isi
+000019a0: 6e73 7461 6e63 6528 6461 7461 2c20 7475  nstance(data, tu
+000019b0: 706c 6529 2065 6c73 6520 7475 706c 6528  ple) else tuple(
+000019c0: 6461 7461 290d 0a20 2020 200d 0a20 2020  data)..    ..   
+000019d0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+000019e0: 6c66 2c20 6461 7461 203d 204e 6f6e 6529  lf, data = None)
+000019f0: 3a0d 0a20 2020 2020 2020 2023 2054 4f44  :..        # TOD
+00001a00: 4f3a 206f 7074 696f 6e20 666f 7220 6c61  O: option for la
+00001a10: 7a79 2069 6e69 743f 0d0a 2020 2020 2020  zy init?..      
+00001a20: 2020 7365 6c66 2e64 6174 6120 3d20 280d    self.data = (.
+00001a30: 0a20 2020 2020 2020 2020 2020 2074 7570  .            tup
+00001a40: 6c65 2829 2069 6620 6461 7461 2069 7320  le() if data is 
+00001a50: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
+00001a60: 2020 656c 7365 2073 656c 662e 7772 6170    else self.wrap
+00001a70: 5f74 7570 6c65 2864 6174 6129 0d0a 2020  _tuple(data)..  
+00001a80: 2020 2020 2020 290d 0a0d 0a20 2020 2064        )....    d
+00001a90: 6566 205f 5f72 6570 725f 5f28 7365 6c66  ef __repr__(self
+00001aa0: 293a 0d0a 2020 2020 2020 2020 7320 3d20  ):..        s = 
+00001ab0: 7375 7065 7228 292e 5f5f 7265 7072 5f5f  super().__repr__
+00001ac0: 2829 0d0a 2020 2020 2020 2020 7265 7475  ()..        retu
+00001ad0: 726e 2022 7b7d 287b 7d29 222e 666f 726d  rn "{}({})".form
+00001ae0: 6174 280d 0a20 2020 2020 2020 2020 2020  at(..           
+00001af0: 2074 7970 6528 7365 6c66 292e 5f5f 6e61   type(self).__na
+00001b00: 6d65 5f5f 2c0d 0a20 2020 2020 2020 2020  me__,..         
+00001b10: 2020 2073 5b31 3a2d 3220 6966 2073 5b2d     s[1:-2 if s[-
+00001b20: 325d 203d 3d20 222c 2220 656c 7365 202d  2] == "," else -
+00001b30: 315d 2c0d 0a20 2020 2020 2020 2029 0d0a  1],..        )..
+00001b40: 0d0a 2020 2020 6465 6620 5f5f 6861 7368  ..    def __hash
+00001b50: 5f5f 2873 656c 6629 3a0d 0a20 2020 2020  __(self):..     
+00001b60: 2020 2072 6574 7572 6e20 6861 7368 2873     return hash(s
+00001b70: 656c 662e 6461 7461 290d 0a0d 0a20 2020  elf.data)....   
+00001b80: 2040 636c 6173 736d 6574 686f 640d 0a20   @classmethod.. 
+00001b90: 2020 2064 6566 2064 6563 6f72 6174 6528     def decorate(
+00001ba0: 6d65 7461 2c20 636c 7329 3a0d 0a20 2020  meta, cls):..   
+00001bb0: 2020 2020 2061 7373 6572 7420 636c 732e       assert cls.
+00001bc0: 5f5f 6e61 6d65 5f5f 206e 6f74 2069 6e20  __name__ not in 
+00001bd0: 5245 4749 5354 5259 0d0a 2020 2020 2020  REGISTRY..      
+00001be0: 2020 5245 4749 5354 5259 5b63 6c73 2e5f    REGISTRY[cls._
+00001bf0: 5f6e 616d 655f 5f5d 203d 2063 6c73 0d0a  _name__] = cls..
+00001c00: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00001c10: 6c73 0d0a 0d0a 2020 2020 2320 2d2d 2d2d  ls....    # ----
+00001c20: 2d0d 0a0d 0a20 2020 2064 6566 2063 6173  -....    def cas
+00001c30: 745f 6a73 6f6e 2873 656c 6629 3a0d 0a20  t_json(self):.. 
+00001c40: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00001c50: 2020 2020 3e3e 3e20 6954 7570 6c65 2e72      >>> iTuple.r
+00001c60: 616e 6765 2831 292e 6361 7374 5f6a 736f  ange(1).cast_jso
+00001c70: 6e28 290d 0a20 2020 2020 2020 207b 275f  n()..        {'_
+00001c80: 5f74 5f5f 273a 2027 6954 7570 6c65 272c  _t__': 'iTuple',
+00001c90: 2027 6461 7461 273a 205b 305d 7d0d 0a20   'data': [0]}.. 
+00001ca0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00001cb0: 2020 2020 7265 7475 726e 2064 6963 7428      return dict(
+00001cc0: 0d0a 2020 2020 2020 2020 2020 2020 5f5f  ..            __
+00001cd0: 745f 5f20 3d20 7479 7065 2873 656c 6629  t__ = type(self)
+00001ce0: 2e5f 5f6e 616d 655f 5f2c 0d0a 2020 2020  .__name__,..    
+00001cf0: 2020 2020 2020 2020 6461 7461 203d 206c          data = l
+00001d00: 6973 7428 7365 6c66 2e6d 6170 2863 6173  ist(self.map(cas
+00001d10: 745f 6a73 6f6e 2929 2c0d 0a20 2020 2020  t_json)),..     
+00001d20: 2020 2029 0d0a 0d0a 2020 2020 4063 6c61     )....    @cla
+00001d30: 7373 6d65 7468 6f64 0d0a 2020 2020 6465  ssmethod..    de
+00001d40: 6620 756e 6361 7374 5f6a 736f 6e28 636c  f uncast_json(cl
+00001d50: 732c 206f 626a 293a 0d0a 2020 2020 2020  s, obj):..      
+00001d60: 2020 2222 220d 0a20 2020 2020 2020 203e    """..        >
+00001d70: 3e3e 2069 5475 706c 652e 756e 6361 7374  >> iTuple.uncast
+00001d80: 5f6a 736f 6e28 6954 7570 6c65 2e72 616e  _json(iTuple.ran
+00001d90: 6765 2831 292e 6361 7374 5f6a 736f 6e28  ge(1).cast_json(
+00001da0: 2929 0d0a 2020 2020 2020 2020 6954 7570  ))..        iTup
+00001db0: 6c65 2830 290d 0a20 2020 2020 2020 2022  le(0)..        "
+00001dc0: 2222 0d0a 2020 2020 2020 2020 6173 7365  ""..        asse
+00001dd0: 7274 206f 626a 5b22 5f5f 745f 5f22 5d20  rt obj["__t__"] 
+00001de0: 3d3d 2063 6c73 2e5f 5f6e 616d 655f 5f0d  == cls.__name__.
+00001df0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001e00: 636c 7328 6461 7461 3d6f 626a 5b22 6461  cls(data=obj["da
+00001e10: 7461 225d 290d 0a0d 0a20 2020 2023 202d  ta"])....    # -
+00001e20: 2d2d 2d2d 0d0a 0d0a 2020 2020 4063 6c61  ----....    @cla
+00001e30: 7373 6d65 7468 6f64 0d0a 2020 2020 6465  ssmethod..    de
+00001e40: 6620 7261 6e67 6528 636c 732c 202a 6172  f range(cls, *ar
+00001e50: 6773 2c20 2a2a 6b77 6172 6773 293a 0d0a  gs, **kwargs):..
+00001e60: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00001e70: 2020 2020 203e 3e3e 2069 5475 706c 652e       >>> iTuple.
+00001e80: 7261 6e67 6528 3329 0d0a 2020 2020 2020  range(3)..      
+00001e90: 2020 6954 7570 6c65 2830 2c20 312c 2032    iTuple(0, 1, 2
+00001ea0: 290d 0a20 2020 2020 2020 2022 2222 0d0a  )..        """..
+00001eb0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00001ec0: 6c73 2872 616e 6765 282a 6172 6773 2c20  ls(range(*args, 
+00001ed0: 2a2a 6b77 6172 6773 2929 0d0a 0d0a 2020  **kwargs))....  
+00001ee0: 2020 4063 6c61 7373 6d65 7468 6f64 0d0a    @classmethod..
+00001ef0: 2020 2020 6465 6620 6672 6f6d 5f6b 6579      def from_key
+00001f00: 7328 636c 732c 2064 293a 0d0a 2020 2020  s(cls, d):..    
+00001f10: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00001f20: 203e 3e3e 2069 5475 706c 652e 6672 6f6d   >>> iTuple.from
+00001f30: 5f6b 6579 7328 7b69 3a20 6920 2b20 3120  _keys({i: i + 1 
+00001f40: 666f 7220 6920 696e 2072 616e 6765 2832  for i in range(2
+00001f50: 297d 290d 0a20 2020 2020 2020 2069 5475  )})..        iTu
+00001f60: 706c 6528 302c 2031 290d 0a20 2020 2020  ple(0, 1)..     
+00001f70: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00001f80: 7265 7475 726e 2063 6c73 2864 2e6b 6579  return cls(d.key
+00001f90: 7328 2929 0d0a 2020 2020 2020 2020 0d0a  s())..        ..
+00001fa0: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+00001fb0: 0d0a 2020 2020 6465 6620 6672 6f6d 5f76  ..    def from_v
+00001fc0: 616c 7565 7328 636c 732c 2064 293a 0d0a  alues(cls, d):..
+00001fd0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00001fe0: 2020 2020 203e 3e3e 2069 5475 706c 652e       >>> iTuple.
+00001ff0: 6672 6f6d 5f76 616c 7565 7328 7b69 3a20  from_values({i: 
+00002000: 6920 2b20 3120 666f 7220 6920 696e 2072  i + 1 for i in r
+00002010: 616e 6765 2832 297d 290d 0a20 2020 2020  ange(2)})..     
+00002020: 2020 2069 5475 706c 6528 312c 2032 290d     iTuple(1, 2).
+00002030: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00002040: 2020 2020 2020 7265 7475 726e 2063 6c73        return cls
+00002050: 2864 2e76 616c 7565 7328 2929 0d0a 2020  (d.values())..  
+00002060: 2020 2020 2020 0d0a 2020 2020 4063 6c61        ..    @cla
+00002070: 7373 6d65 7468 6f64 0d0a 2020 2020 6465  ssmethod..    de
+00002080: 6620 6672 6f6d 5f69 7465 6d73 2863 6c73  f from_items(cls
+00002090: 2c20 6429 3a0d 0a20 2020 2020 2020 2022  , d):..        "
+000020a0: 2222 0d0a 2020 2020 2020 2020 3e3e 3e20  ""..        >>> 
+000020b0: 6954 7570 6c65 2e66 726f 6d5f 6974 656d  iTuple.from_item
+000020c0: 7328 7b69 3a20 6920 2b20 3120 666f 7220  s({i: i + 1 for 
+000020d0: 6920 696e 2072 616e 6765 2832 297d 290d  i in range(2)}).
+000020e0: 0a20 2020 2020 2020 2069 5475 706c 6528  .        iTuple(
+000020f0: 2830 2c20 3129 2c20 2831 2c20 3229 290d  (0, 1), (1, 2)).
+00002100: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00002110: 2020 2020 2020 7265 7475 726e 2063 6c73        return cls
+00002120: 2864 2e69 7465 6d73 2829 290d 0a0d 0a20  (d.items()).... 
+00002130: 2020 2023 202d 2d2d 2d2d 0d0a 0d0a 2020     # -----....  
+00002140: 2020 6465 6620 7069 7065 2873 656c 662c    def pipe(self,
+00002150: 2066 2c20 2a61 7267 732c 202a 2a6b 7761   f, *args, **kwa
+00002160: 7267 7329 3a0d 0a20 2020 2020 2020 2022  rgs):..        "
+00002170: 2222 0d0a 2020 2020 2020 2020 3e3e 3e20  ""..        >>> 
+00002180: 6954 7570 6c65 2e72 616e 6765 2832 292e  iTuple.range(2).
+00002190: 7069 7065 286c 616d 6264 6120 6974 3a20  pipe(lambda it: 
+000021a0: 6974 290d 0a20 2020 2020 2020 2069 5475  it)..        iTu
+000021b0: 706c 6528 302c 2031 290d 0a20 2020 2020  ple(0, 1)..     
+000021c0: 2020 203e 3e3e 2069 5475 706c 652e 7261     >>> iTuple.ra
+000021d0: 6e67 6528 3229 2e70 6970 6528 0d0a 2020  nge(2).pipe(..  
+000021e0: 2020 2020 2020 2e2e 2e20 2020 2020 6c61        ...     la
+000021f0: 6d62 6461 2069 742c 2076 3a20 6974 2e6d  mbda it, v: it.m
+00002200: 6170 286c 616d 6264 6120 783a 2078 202a  ap(lambda x: x *
+00002210: 2076 292c 2032 0d0a 2020 2020 2020 2020   v), 2..        
+00002220: 2e2e 2e20 290d 0a20 2020 2020 2020 2069  ... )..        i
+00002230: 5475 706c 6528 302c 2032 290d 0a20 2020  Tuple(0, 2)..   
+00002240: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00002250: 2020 7265 7475 726e 2066 2873 656c 662c    return f(self,
+00002260: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
+00002270: 290d 0a0d 0a20 2020 2064 6566 2070 6172  )....    def par
+00002280: 7469 616c 2873 656c 662c 2066 2c20 2a61  tial(self, f, *a
+00002290: 7267 732c 202a 2a6b 7761 7267 7329 3a0d  rgs, **kwargs):.
+000022a0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000022b0: 2020 2020 2020 3e3e 3e20 6620 3d20 6954        >>> f = iT
+000022c0: 7570 6c65 2e72 616e 6765 2832 292e 7061  uple.range(2).pa
+000022d0: 7274 6961 6c28 0d0a 2020 2020 2020 2020  rtial(..        
+000022e0: 2e2e 2e20 2020 2020 6c61 6d62 6461 2069  ...     lambda i
+000022f0: 742c 2076 3a20 6974 2e6d 6170 286c 616d  t, v: it.map(lam
+00002300: 6264 6120 783a 2078 202a 2076 290d 0a20  bda x: x * v).. 
+00002310: 2020 2020 2020 202e 2e2e 2029 0d0a 2020         ... )..  
+00002320: 2020 2020 2020 3e3e 3e20 6628 3229 0d0a        >>> f(2)..
+00002330: 2020 2020 2020 2020 6954 7570 6c65 2830          iTuple(0
+00002340: 2c20 3229 0d0a 2020 2020 2020 2020 3e3e  , 2)..        >>
+00002350: 3e20 6628 3329 0d0a 2020 2020 2020 2020  > f(3)..        
+00002360: 6954 7570 6c65 2830 2c20 3329 0d0a 2020  iTuple(0, 3)..  
+00002370: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00002380: 2020 2072 6574 7572 6e20 6675 6e63 746f     return functo
+00002390: 6f6c 732e 7061 7274 6961 6c28 662c 2073  ols.partial(f, s
+000023a0: 656c 662c 202a 6172 6773 2c20 2a2a 6b77  elf, *args, **kw
+000023b0: 6172 6773 290d 0a0d 0a20 2020 2023 202d  args)....    # -
+000023c0: 2d2d 2d2d 0d0a 0d0a 2020 2020 6465 6620  ----....    def 
+000023d0: 6c65 6e28 7365 6c66 293a 0d0a 2020 2020  len(self):..    
+000023e0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000023f0: 203e 3e3e 2069 5475 706c 652e 7261 6e67   >>> iTuple.rang
+00002400: 6528 3329 2e6c 656e 2829 0d0a 2020 2020  e(3).len()..    
+00002410: 2020 2020 330d 0a20 2020 2020 2020 2022      3..        "
+00002420: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
+00002430: 726e 206c 656e 2873 656c 6629 0d0a 0d0a  rn len(self)....
+00002440: 2020 2020 6465 6620 6170 7065 6e64 2873      def append(s
+00002450: 656c 662c 2076 616c 7565 2c20 2a76 616c  elf, value, *val
+00002460: 7565 7329 3a0d 0a20 2020 2020 2020 2022  ues):..        "
+00002470: 2222 0d0a 2020 2020 2020 2020 3e3e 3e20  ""..        >>> 
+00002480: 6954 7570 6c65 2e72 616e 6765 2831 292e  iTuple.range(1).
+00002490: 6170 7065 6e64 2831 290d 0a20 2020 2020  append(1)..     
+000024a0: 2020 2069 5475 706c 6528 302c 2031 290d     iTuple(0, 1).
+000024b0: 0a20 2020 2020 2020 203e 3e3e 2069 5475  .        >>> iTu
+000024c0: 706c 652e 7261 6e67 6528 3129 2e61 7070  ple.range(1).app
+000024d0: 656e 6428 312c 2032 290d 0a20 2020 2020  end(1, 2)..     
+000024e0: 2020 2069 5475 706c 6528 302c 2031 2c20     iTuple(0, 1, 
+000024f0: 3229 0d0a 2020 2020 2020 2020 3e3e 3e20  2)..        >>> 
+00002500: 6954 7570 6c65 2e72 616e 6765 2831 292e  iTuple.range(1).
+00002510: 6170 7065 6e64 2831 2c20 322c 2033 290d  append(1, 2, 3).
+00002520: 0a20 2020 2020 2020 2069 5475 706c 6528  .        iTuple(
+00002530: 302c 2031 2c20 322c 2033 290d 0a20 2020  0, 1, 2, 3)..   
+00002540: 2020 2020 203e 3e3e 2069 5475 706c 652e       >>> iTuple.
+00002550: 7261 6e67 6528 3129 2e61 7070 656e 6428  range(1).append(
+00002560: 312c 2028 322c 2929 0d0a 2020 2020 2020  1, (2,))..      
+00002570: 2020 6954 7570 6c65 2830 2c20 312c 2028    iTuple(0, 1, (
+00002580: 322c 2929 0d0a 2020 2020 2020 2020 2222  2,))..        ""
+00002590: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+000025a0: 6e20 7365 6c66 202b 2028 7661 6c75 652c  n self + (value,
+000025b0: 202a 7661 6c75 6573 290d 0a0d 0a20 2020   *values)....   
+000025c0: 2064 6566 2070 7265 7065 6e64 2873 656c   def prepend(sel
+000025d0: 662c 2076 616c 7565 2c20 2a76 616c 7565  f, value, *value
+000025e0: 7329 3a0d 0a20 2020 2020 2020 2022 2222  s):..        """
+000025f0: 0d0a 2020 2020 2020 2020 3e3e 3e20 6954  ..        >>> iT
+00002600: 7570 6c65 2e72 616e 6765 2831 292e 7072  uple.range(1).pr
+00002610: 6570 656e 6428 3129 0d0a 2020 2020 2020  epend(1)..      
+00002620: 2020 6954 7570 6c65 2831 2c20 3029 0d0a    iTuple(1, 0)..
+00002630: 2020 2020 2020 2020 3e3e 3e20 6954 7570          >>> iTup
+00002640: 6c65 2e72 616e 6765 2831 292e 7072 6570  le.range(1).prep
+00002650: 656e 6428 312c 2032 290d 0a20 2020 2020  end(1, 2)..     
+00002660: 2020 2069 5475 706c 6528 312c 2032 2c20     iTuple(1, 2, 
+00002670: 3029 0d0a 2020 2020 2020 2020 3e3e 3e20  0)..        >>> 
+00002680: 6954 7570 6c65 2e72 616e 6765 2831 292e  iTuple.range(1).
+00002690: 7072 6570 656e 6428 312c 2032 2c20 3329  prepend(1, 2, 3)
+000026a0: 0d0a 2020 2020 2020 2020 6954 7570 6c65  ..        iTuple
+000026b0: 2831 2c20 322c 2033 2c20 3029 0d0a 2020  (1, 2, 3, 0)..  
+000026c0: 2020 2020 2020 3e3e 3e20 6954 7570 6c65        >>> iTuple
+000026d0: 2e72 616e 6765 2831 292e 7072 6570 656e  .range(1).prepen
+000026e0: 6428 312c 2028 322c 2929 0d0a 2020 2020  d(1, (2,))..    
+000026f0: 2020 2020 6954 7570 6c65 2831 2c20 2832      iTuple(1, (2
+00002700: 2c29 2c20 3029 0d0a 2020 2020 2020 2020  ,), 0)..        
+00002710: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
+00002720: 7572 6e20 2876 616c 7565 2c20 2a76 616c  urn (value, *val
+00002730: 7565 7329 202b 2073 656c 660d 0a0d 0a20  ues) + self.... 
+00002740: 2020 2064 6566 207a 6970 2873 656c 662c     def zip(self,
+00002750: 202a 6974 7273 2c20 6c61 7a79 203d 2046   *itrs, lazy = F
+00002760: 616c 7365 293a 0d0a 2020 2020 2020 2020  alse):..        
+00002770: 2222 220d 0a20 2020 2020 2020 203e 3e3e  """..        >>>
+00002780: 2069 5475 706c 6528 5b5b 312c 2031 5d2c   iTuple([[1, 1],
+00002790: 205b 322c 2032 5d2c 205b 332c 2033 5d5d   [2, 2], [3, 3]]
+000027a0: 292e 7a69 7028 290d 0a20 2020 2020 2020  ).zip()..       
+000027b0: 2069 5475 706c 6528 2831 2c20 322c 2033   iTuple((1, 2, 3
+000027c0: 292c 2028 312c 2032 2c20 3329 290d 0a20  ), (1, 2, 3)).. 
+000027d0: 2020 2020 2020 203e 3e3e 2069 5475 706c         >>> iTupl
+000027e0: 6528 5b69 5475 706c 652e 7261 6e67 6528  e([iTuple.range(
+000027f0: 3329 2c20 6954 7570 6c65 2e72 616e 6765  3), iTuple.range
+00002800: 2831 2c20 3429 5d29 2e7a 6970 2829 0d0a  (1, 4)]).zip()..
+00002810: 2020 2020 2020 2020 6954 7570 6c65 2828          iTuple((
+00002820: 302c 2031 292c 2028 312c 2032 292c 2028  0, 1), (1, 2), (
+00002830: 322c 2033 2929 0d0a 2020 2020 2020 2020  2, 3))..        
+00002840: 3e3e 3e20 6954 7570 6c65 2e72 616e 6765  >>> iTuple.range
+00002850: 2833 292e 7a69 7028 6954 7570 6c65 2e72  (3).zip(iTuple.r
+00002860: 616e 6765 2831 2c20 3429 290d 0a20 2020  ange(1, 4))..   
+00002870: 2020 2020 2069 5475 706c 6528 2830 2c20       iTuple((0, 
+00002880: 3129 2c20 2831 2c20 3229 2c20 2832 2c20  1), (1, 2), (2, 
+00002890: 3329 290d 0a20 2020 2020 2020 2022 2222  3))..        """
+000028a0: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+000028b0: 2869 7472 7329 203d 3d20 303a 0d0a 2020  (itrs) == 0:..  
+000028c0: 2020 2020 2020 2020 2020 7265 7320 3d20            res = 
+000028d0: 7a69 7028 2a73 656c 6629 0d0a 2020 2020  zip(*self)..    
+000028e0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000028f0: 2020 2020 2020 2072 6573 203d 207a 6970         res = zip
+00002900: 2873 656c 662c 202a 6974 7273 290d 0a20  (self, *itrs).. 
+00002910: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00002920: 7320 6966 206c 617a 7920 656c 7365 2069  s if lazy else i
+00002930: 5475 706c 6528 6461 7461 3d72 6573 290d  Tuple(data=res).
+00002940: 0a0d 0a20 2020 2064 6566 2066 6c61 7474  ...    def flatt
+00002950: 656e 2873 656c 6629 3a0d 0a20 2020 2020  en(self):..     
+00002960: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00002970: 3e3e 3e20 6954 7570 6c65 2e72 616e 6765  >>> iTuple.range
+00002980: 2833 292e 6d61 7028 6c61 6d62 6461 2078  (3).map(lambda x
+00002990: 3a20 5b78 5d29 2e66 6c61 7474 656e 2829  : [x]).flatten()
+000029a0: 0d0a 2020 2020 2020 2020 6954 7570 6c65  ..        iTuple
+000029b0: 2830 2c20 312c 2032 290d 0a20 2020 2020  (0, 1, 2)..     
+000029c0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000029d0: 7265 7475 726e 2069 5475 706c 6528 6974  return iTuple(it
+000029e0: 6572 746f 6f6c 732e 6368 6169 6e28 2a73  ertools.chain(*s
+000029f0: 656c 6629 290d 0a0d 0a20 2020 2064 6566  elf))....    def
+00002a00: 2065 7874 656e 6428 7365 6c66 2c20 7661   extend(self, va
+00002a10: 6c75 652c 202a 7661 6c75 6573 293a 0d0a  lue, *values):..
+00002a20: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00002a30: 2020 2020 203e 3e3e 2069 5475 706c 652e       >>> iTuple.
+00002a40: 7261 6e67 6528 3129 2e65 7874 656e 6428  range(1).extend(
+00002a50: 2831 2c29 290d 0a20 2020 2020 2020 2069  (1,))..        i
+00002a60: 5475 706c 6528 302c 2031 290d 0a20 2020  Tuple(0, 1)..   
+00002a70: 2020 2020 203e 3e3e 2069 5475 706c 652e       >>> iTuple.
+00002a80: 7261 6e67 6528 3129 2e65 7874 656e 6428  range(1).extend(
+00002a90: 5b31 5d29 0d0a 2020 2020 2020 2020 6954  [1])..        iT
+00002aa0: 7570 6c65 2830 2c20 3129 0d0a 2020 2020  uple(0, 1)..    
+00002ab0: 2020 2020 3e3e 3e20 6954 7570 6c65 2e72      >>> iTuple.r
+00002ac0: 616e 6765 2831 292e 6578 7465 6e64 285b  ange(1).extend([
+00002ad0: 315d 2c20 5b32 5d29 0d0a 2020 2020 2020  1], [2])..      
+00002ae0: 2020 6954 7570 6c65 2830 2c20 312c 2032    iTuple(0, 1, 2
+00002af0: 290d 0a20 2020 2020 2020 203e 3e3e 2069  )..        >>> i
+00002b00: 5475 706c 652e 7261 6e67 6528 3129 2e65  Tuple.range(1).e
+00002b10: 7874 656e 6428 5b31 5d2c 205b 5b32 5d5d  xtend([1], [[2]]
+00002b20: 290d 0a20 2020 2020 2020 2069 5475 706c  )..        iTupl
+00002b30: 6528 302c 2031 2c20 5b32 5d29 0d0a 2020  e(0, 1, [2])..  
+00002b40: 2020 2020 2020 3e3e 3e20 6954 7570 6c65        >>> iTuple
+00002b50: 2e72 616e 6765 2831 292e 6578 7465 6e64  .range(1).extend
+00002b60: 285b 315d 2c20 5b5b 325d 5d2c 205b 325d  ([1], [[2]], [2]
+00002b70: 290d 0a20 2020 2020 2020 2069 5475 706c  )..        iTupl
+00002b80: 6528 302c 2031 2c20 5b32 5d2c 2032 290d  e(0, 1, [2], 2).
+00002b90: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00002ba0: 2020 2020 2020 7265 7475 726e 2069 5475        return iTu
+00002bb0: 706c 6528 6974 6572 746f 6f6c 732e 6368  ple(itertools.ch
+00002bc0: 6169 6e2e 6672 6f6d 5f69 7465 7261 626c  ain.from_iterabl
+00002bd0: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
+00002be0: 2873 656c 662c 2076 616c 7565 2c20 2a76  (self, value, *v
+00002bf0: 616c 7565 7329 0d0a 2020 2020 2020 2020  alues)..        
+00002c00: 2929 0d0a 0d0a 2020 2020 6465 6620 7072  ))....    def pr
+00002c10: 6574 656e 6428 7365 6c66 2c20 7661 6c75  etend(self, valu
+00002c20: 652c 202a 7661 6c75 6573 293a 0d0a 2020  e, *values):..  
+00002c30: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00002c40: 2020 203e 3e3e 2069 5475 706c 652e 7261     >>> iTuple.ra
+00002c50: 6e67 6528 3129 2e70 7265 7465 6e64 2828  nge(1).pretend((
+00002c60: 312c 2929 0d0a 2020 2020 2020 2020 6954  1,))..        iT
+00002c70: 7570 6c65 2831 2c20 3029 0d0a 2020 2020  uple(1, 0)..    
+00002c80: 2020 2020 3e3e 3e20 6954 7570 6c65 2e72      >>> iTuple.r
+00002c90: 616e 6765 2831 292e 7072 6574 656e 6428  ange(1).pretend(
+00002ca0: 5b31 5d29 0d0a 2020 2020 2020 2020 6954  [1])..        iT
+00002cb0: 7570 6c65 2831 2c20 3029 0d0a 2020 2020  uple(1, 0)..    
+00002cc0: 2020 2020 3e3e 3e20 6954 7570 6c65 2e72      >>> iTuple.r
+00002cd0: 616e 6765 2831 292e 7072 6574 656e 6428  ange(1).pretend(
+00002ce0: 5b31 5d2c 205b 325d 290d 0a20 2020 2020  [1], [2])..     
+00002cf0: 2020 2069 5475 706c 6528 312c 2032 2c20     iTuple(1, 2, 
+00002d00: 3029 0d0a 2020 2020 2020 2020 3e3e 3e20  0)..        >>> 
+00002d10: 6954 7570 6c65 2e72 616e 6765 2831 292e  iTuple.range(1).
+00002d20: 7072 6574 656e 6428 5b31 5d2c 205b 5b32  pretend([1], [[2
+00002d30: 5d5d 290d 0a20 2020 2020 2020 2069 5475  ]])..        iTu
+00002d40: 706c 6528 312c 205b 325d 2c20 3029 0d0a  ple(1, [2], 0)..
+00002d50: 2020 2020 2020 2020 3e3e 3e20 6954 7570          >>> iTup
+00002d60: 6c65 2e72 616e 6765 2831 292e 7072 6574  le.range(1).pret
+00002d70: 656e 6428 5b31 5d2c 205b 5b32 5d5d 2c20  end([1], [[2]], 
+00002d80: 5b32 5d29 0d0a 2020 2020 2020 2020 6954  [2])..        iT
+00002d90: 7570 6c65 2831 2c20 5b32 5d2c 2032 2c20  uple(1, [2], 2, 
+00002da0: 3029 0d0a 2020 2020 2020 2020 2222 220d  0)..        """.
+00002db0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002dc0: 6954 7570 6c65 2869 7465 7274 6f6f 6c73  iTuple(itertools
+00002dd0: 2e63 6861 696e 2e66 726f 6d5f 6974 6572  .chain.from_iter
+00002de0: 6162 6c65 280d 0a20 2020 2020 2020 2020  able(..         
+00002df0: 2020 2028 7661 6c75 652c 202a 7661 6c75     (value, *valu
+00002e00: 6573 2c20 7365 6c66 290d 0a20 2020 2020  es, self)..     
+00002e10: 2020 2029 290d 0a0d 0a20 2020 2064 6566     ))....    def
+00002e20: 2066 696c 7465 725f 6571 2873 656c 662c   filter_eq(self,
+00002e30: 2076 2c20 6620 3d20 4e6f 6e65 2c20 6571   v, f = None, eq
+00002e40: 203d 204e 6f6e 652c 206c 617a 7920 3d20   = None, lazy = 
+00002e50: 4661 6c73 6529 3a0d 0a20 2020 2020 2020  False):..       
+00002e60: 2022 2222 0d0a 2020 2020 2020 2020 3e3e   """..        >>
+00002e70: 3e20 6954 7570 6c65 2e72 616e 6765 2833  > iTuple.range(3
+00002e80: 292e 6669 6c74 6572 5f65 7128 3129 0d0a  ).filter_eq(1)..
+00002e90: 2020 2020 2020 2020 6954 7570 6c65 2831          iTuple(1
+00002ea0: 290d 0a20 2020 2020 2020 2022 2222 0d0a  )..        """..
+00002eb0: 2020 2020 2020 2020 6966 2066 2069 7320          if f is 
+00002ec0: 4e6f 6e65 2061 6e64 2065 7120 6973 204e  None and eq is N
+00002ed0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00002ee0: 2020 7265 7320 3d20 6669 6c74 6572 286c    res = filter(l
+00002ef0: 616d 6264 6120 783a 2078 203d 3d20 762c  ambda x: x == v,
+00002f00: 2073 656c 6629 0d0a 2020 2020 2020 2020   self)..        
+00002f10: 656c 6966 2066 2069 7320 6e6f 7420 4e6f  elif f is not No
+00002f20: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00002f30: 2072 6573 203d 2066 696c 7465 7228 6c61   res = filter(la
+00002f40: 6d62 6461 2078 3a20 6628 7829 203d 3d20  mbda x: f(x) == 
+00002f50: 762c 2073 656c 6629 0d0a 2020 2020 2020  v, self)..      
+00002f60: 2020 656c 6966 2065 7120 6973 206e 6f74    elif eq is not
+00002f70: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00002f80: 2020 2020 7265 7320 3d20 6669 6c74 6572      res = filter
+00002f90: 286c 616d 6264 6120 783a 2065 7128 782c  (lambda x: eq(x,
+00002fa0: 2076 292c 2073 656c 6629 0d0a 2020 2020   v), self)..    
+00002fb0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00002fc0: 2020 2020 2020 2072 6573 203d 2066 696c         res = fil
+00002fd0: 7465 7228 6c61 6d62 6461 2078 3a20 6571  ter(lambda x: eq
+00002fe0: 2866 2878 292c 2076 292c 2073 656c 6629  (f(x), v), self)
+00002ff0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00003000: 2072 6573 2069 6620 6c61 7a79 2065 6c73   res if lazy els
+00003010: 6520 7479 7065 2873 656c 6629 2864 6174  e type(self)(dat
+00003020: 613d 7265 7329 0d0a 0d0a 2020 2020 6465  a=res)....    de
+00003030: 6620 6669 6c74 6572 2873 656c 662c 2066  f filter(self, f
+00003040: 2c20 6571 203d 204e 6f6e 652c 206c 617a  , eq = None, laz
+00003050: 7920 3d20 4661 6c73 6529 3a0d 0a20 2020  y = False):..   
+00003060: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00003070: 2020 3e3e 3e20 6954 7570 6c65 2e72 616e    >>> iTuple.ran
+00003080: 6765 2833 292e 6669 6c74 6572 286c 616d  ge(3).filter(lam
+00003090: 6264 6120 783a 2078 203e 2031 290d 0a20  bda x: x > 1).. 
+000030a0: 2020 2020 2020 2069 5475 706c 6528 3229         iTuple(2)
+000030b0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+000030c0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000030d0: 6c66 2e66 696c 7465 725f 6571 2854 7275  lf.filter_eq(Tru
+000030e0: 652c 2066 203d 2066 2c20 6571 203d 2065  e, f = f, eq = e
+000030f0: 712c 206c 617a 7920 3d20 6c61 7a79 290d  q, lazy = lazy).
+00003100: 0a0d 0a20 2020 2064 6566 206d 6170 2873  ...    def map(s
+00003110: 656c 662c 2066 2c20 2a69 7465 7261 626c  elf, f, *iterabl
+00003120: 6573 2c20 6c61 7a79 203d 2046 616c 7365  es, lazy = False
+00003130: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
+00003140: 0a20 2020 2020 2020 203e 3e3e 2069 5475  .        >>> iTu
+00003150: 706c 652e 7261 6e67 6528 3329 2e6d 6170  ple.range(3).map
+00003160: 286c 616d 6264 6120 783a 2078 202a 2032  (lambda x: x * 2
+00003170: 290d 0a20 2020 2020 2020 2069 5475 706c  )..        iTupl
+00003180: 6528 302c 2032 2c20 3429 0d0a 2020 2020  e(0, 2, 4)..    
+00003190: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000031a0: 2072 6573 203d 206d 6170 2866 2c20 7365   res = map(f, se
+000031b0: 6c66 2c20 2a69 7465 7261 626c 6573 290d  lf, *iterables).
+000031c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000031d0: 7265 7320 6966 206c 617a 7920 656c 7365  res if lazy else
+000031e0: 2069 5475 706c 6528 6461 7461 3d72 6573   iTuple(data=res
+000031f0: 290d 0a0d 0a20 2020 2064 6566 2065 6e75  )....    def enu
+00003200: 6d65 7261 7465 2873 656c 6629 3a0d 0a20  merate(self):.. 
+00003210: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00003220: 2020 2020 3e3e 3e20 6954 7570 6c65 2e72      >>> iTuple.r
+00003230: 616e 6765 2833 292e 656e 756d 6572 6174  ange(3).enumerat
+00003240: 6528 290d 0a20 2020 2020 2020 2069 5475  e()..        iTu
+00003250: 706c 6528 2830 2c20 3029 2c20 2831 2c20  ple((0, 0), (1, 
+00003260: 3129 2c20 2832 2c20 3229 290d 0a20 2020  1), (2, 2))..   
+00003270: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00003280: 2020 2320 544f 444f 3a20 616c 6c6f 7720    # TODO: allow 
+00003290: 6c61 7a79 0d0a 2020 2020 2020 2020 7265  lazy..        re
+000032a0: 7475 726e 2069 5475 706c 6528 656e 756d  turn iTuple(enum
+000032b0: 6572 6174 6528 7365 6c66 2929 0d0a 0d0a  erate(self))....
+000032c0: 2020 2020 6465 6620 6772 6f75 7062 7928      def groupby(
+000032d0: 0d0a 2020 2020 2020 2020 7365 6c66 2c20  ..        self, 
+000032e0: 0d0a 2020 2020 2020 2020 662c 200d 0a20  ..        f, .. 
+000032f0: 2020 2020 2020 206c 617a 7920 3d20 4661         lazy = Fa
+00003300: 6c73 652c 200d 0a20 2020 2020 2020 206b  lse, ..        k
+00003310: 6579 7320 3d20 4661 6c73 652c 0d0a 2020  eys = False,..  
+00003320: 2020 2020 2020 7069 7065 3d20 4e6f 6e65        pipe= None
+00003330: 2c0d 0a20 2020 2029 3a0d 0a20 2020 2020  ,..    ):..     
+00003340: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00003350: 3e3e 3e20 6954 7570 6c65 2e72 616e 6765  >>> iTuple.range
+00003360: 2833 292e 6772 6f75 7062 7928 6c61 6d62  (3).groupby(lamb
+00003370: 6461 2078 3a20 7820 3c20 3229 0d0a 2020  da x: x < 2)..  
+00003380: 2020 2020 2020 6954 7570 6c65 2828 302c        iTuple((0,
+00003390: 2031 292c 2028 322c 2929 0d0a 2020 2020   1), (2,))..    
+000033a0: 2020 2020 3e3e 3e20 6954 7570 6c65 2e72      >>> iTuple.r
+000033b0: 616e 6765 2833 292e 6772 6f75 7062 7928  ange(3).groupby(
+000033c0: 0d0a 2020 2020 2020 2020 2e2e 2e20 2020  ..        ...   
+000033d0: 206c 616d 6264 6120 783a 2078 203c 2032   lambda x: x < 2
+000033e0: 2c20 6b65 7973 3d54 7275 652c 2070 6970  , keys=True, pip
+000033f0: 653d 6644 6963 740d 0a20 2020 2020 2020  e=fDict..       
+00003400: 202e 2e2e 2029 0d0a 2020 2020 2020 2020   ... )..        
+00003410: 7b54 7275 653a 2028 302c 2031 292c 2046  {True: (0, 1), F
+00003420: 616c 7365 3a20 2832 2c29 7d0d 0a20 2020  alse: (2,)}..   
+00003430: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00003440: 2020 2320 544f 444f 3a20 6c61 7a79 206e    # TODO: lazy n
+00003450: 6f20 6b65 7973 0d0a 2020 2020 2020 2020  o keys..        
+00003460: 7265 7320 3d20 6974 6572 746f 6f6c 732e  res = itertools.
+00003470: 6772 6f75 7062 7928 7365 6c66 2c20 6b65  groupby(self, ke
+00003480: 793d 6629 0d0a 2020 2020 2020 2020 6966  y=f)..        if
+00003490: 206c 617a 7920 616e 6420 6b65 7973 2061   lazy and keys a
+000034a0: 6e64 2070 6970 6520 6973 204e 6f6e 653a  nd pipe is None:
+000034b0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000034c0: 7475 726e 2072 6573 0d0a 2020 2020 2020  turn res..      
+000034d0: 2020 6966 2070 6970 6520 6973 204e 6f6e    if pipe is Non
+000034e0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000034f0: 7069 7065 203d 2069 5475 706c 650d 0a20  pipe = iTuple.. 
+00003500: 2020 2020 2020 2069 6620 6b65 7973 3a0d         if keys:.
+00003510: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00003520: 7572 6e20 7069 7065 2828 6b2c 2074 7570  urn pipe((k, tup
+00003530: 6c65 2867 292c 2920 666f 7220 6b2c 2067  le(g),) for k, g
+00003540: 2069 6e20 7265 7329 0d0a 2020 2020 2020   in res)..      
+00003550: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00003560: 2020 2020 2072 6574 7572 6e20 7069 7065       return pipe
+00003570: 2874 7570 6c65 2867 2920 666f 7220 6b2c  (tuple(g) for k,
+00003580: 2067 2069 6e20 7265 7329 0d0a 0d0a 2020   g in res)....  
+00003590: 2020 6465 6620 6669 7273 7428 7365 6c66    def first(self
+000035a0: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
+000035b0: 0a20 2020 2020 2020 203e 3e3e 2069 5475  .        >>> iTu
+000035c0: 706c 652e 7261 6e67 6528 3329 2e66 6972  ple.range(3).fir
+000035d0: 7374 2829 0d0a 2020 2020 2020 2020 300d  st()..        0.
+000035e0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000035f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00003600: 665b 305d 0d0a 2020 2020 0d0a 2020 2020  f[0]..    ..    
+00003610: 6465 6620 6c61 7374 2873 656c 6629 3a0d  def last(self):.
+00003620: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00003630: 2020 2020 2020 3e3e 3e20 6954 7570 6c65        >>> iTuple
+00003640: 2e72 616e 6765 2833 292e 6c61 7374 2829  .range(3).last()
+00003650: 0d0a 2020 2020 2020 2020 320d 0a20 2020  ..        2..   
+00003660: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00003670: 2020 7265 7475 726e 2073 656c 665b 2d31    return self[-1
+00003680: 5d0d 0a0d 0a20 2020 2064 6566 2066 6972  ]....    def fir
+00003690: 7374 5f77 6865 7265 2873 656c 662c 2066  st_where(self, f
+000036a0: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
+000036b0: 0a20 2020 2020 2020 203e 3e3e 2069 5475  .        >>> iTu
+000036c0: 706c 652e 7261 6e67 6528 3329 2e66 6972  ple.range(3).fir
+000036d0: 7374 5f77 6865 7265 286c 616d 6264 6120  st_where(lambda 
+000036e0: 763a 2076 203e 2030 290d 0a20 2020 2020  v: v > 0)..     
+000036f0: 2020 2031 0d0a 2020 2020 2020 2020 2222     1..        ""
+00003700: 220d 0a20 2020 2020 2020 2066 6f72 2076  "..        for v
+00003710: 2069 6e20 7365 6c66 3a0d 0a20 2020 2020   in self:..     
+00003720: 2020 2020 2020 2069 6620 6628 7629 3a0d         if f(v):.
+00003730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003740: 2072 6574 7572 6e20 760d 0a20 2020 2020   return v..     
+00003750: 2020 2072 6574 7572 6e20 4e6f 6e65 0d0a     return None..
+00003760: 0d0a 2020 2020 6465 6620 6c61 7374 5f77  ..    def last_w
+00003770: 6865 7265 2873 656c 662c 2066 293a 0d0a  here(self, f):..
+00003780: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00003790: 2020 2020 203e 3e3e 2069 5475 706c 652e       >>> iTuple.
+000037a0: 7261 6e67 6528 3329 2e6c 6173 745f 7768  range(3).last_wh
+000037b0: 6572 6528 6c61 6d62 6461 2076 3a20 7620  ere(lambda v: v 
+000037c0: 3c20 3229 0d0a 2020 2020 2020 2020 310d  < 2)..        1.
+000037d0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000037e0: 2020 2020 2020 666f 7220 7620 696e 2072        for v in r
+000037f0: 6576 6572 7365 6428 7365 6c66 293a 0d0a  eversed(self):..
+00003800: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+00003810: 2876 293a 0d0a 2020 2020 2020 2020 2020  (v):..          
+00003820: 2020 2020 2020 7265 7475 726e 2076 0d0a        return v..
+00003830: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00003840: 6f6e 650d 0a0d 0a20 2020 2064 6566 2074  one....    def t
+00003850: 616b 6528 7365 6c66 2c20 6e29 3a0d 0a20  ake(self, n):.. 
+00003860: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00003870: 2020 2020 3e3e 3e20 6954 7570 6c65 2e72      >>> iTuple.r
+00003880: 616e 6765 2833 292e 7461 6b65 2832 290d  ange(3).take(2).
+00003890: 0a20 2020 2020 2020 2069 5475 706c 6528  .        iTuple(
+000038a0: 302c 2031 290d 0a20 2020 2020 2020 2022  0, 1)..        "
+000038b0: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
+000038c0: 726e 2073 656c 665b 3a6e 5d0d 0a0d 0a20  rn self[:n].... 
+000038d0: 2020 2064 6566 2074 6169 6c28 7365 6c66     def tail(self
+000038e0: 2c20 6e29 3a0d 0a20 2020 2020 2020 2022  , n):..        "
+000038f0: 2222 0d0a 2020 2020 2020 2020 3e3e 3e20  ""..        >>> 
+00003900: 6954 7570 6c65 2e72 616e 6765 2833 292e  iTuple.range(3).
+00003910: 7461 696c 2832 290d 0a20 2020 2020 2020  tail(2)..       
+00003920: 2069 5475 706c 6528 312c 2032 290d 0a20   iTuple(1, 2).. 
+00003930: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00003940: 2020 2020 7265 7475 726e 2073 656c 665b      return self[
+00003950: 2d6e 3a5d 0d0a 0d0a 2020 2020 6465 6620  -n:]....    def 
+00003960: 7265 7665 7273 6528 7365 6c66 2c20 6c61  reverse(self, la
+00003970: 7a79 203d 2046 616c 7365 293a 0d0a 2020  zy = False):..  
+00003980: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00003990: 2020 203e 3e3e 2069 5475 706c 652e 7261     >>> iTuple.ra
+000039a0: 6e67 6528 3329 2e72 6576 6572 7365 2829  nge(3).reverse()
+000039b0: 0d0a 2020 2020 2020 2020 6954 7570 6c65  ..        iTuple
+000039c0: 2832 2c20 312c 2030 290d 0a20 2020 2020  (2, 1, 0)..     
+000039d0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000039e0: 6966 206c 617a 793a 0d0a 2020 2020 2020  if lazy:..      
+000039f0: 2020 2020 2020 7265 7475 726e 2072 6576        return rev
+00003a00: 6572 7365 6428 7365 6c66 290d 0a20 2020  ersed(self)..   
+00003a10: 2020 2020 2072 6574 7572 6e20 7479 7065       return type
+00003a20: 2873 656c 6629 2864 6174 613d 7265 7665  (self)(data=reve
+00003a30: 7273 6564 2873 656c 6629 290d 0a0d 0a20  rsed(self)).... 
+00003a40: 2020 2064 6566 2074 616b 655f 7768 696c     def take_whil
+00003a50: 6528 7365 6c66 2c20 662c 206e 203d 204e  e(self, f, n = N
+00003a60: 6f6e 652c 206c 617a 7920 3d20 4661 6c73  one, lazy = Fals
+00003a70: 6529 3a0d 0a20 2020 2020 2020 2022 2222  e):..        """
+00003a80: 0d0a 2020 2020 2020 2020 3e3e 3e20 6954  ..        >>> iT
+00003a90: 7570 6c65 2e72 616e 6765 2833 292e 7461  uple.range(3).ta
+00003aa0: 6b65 5f77 6869 6c65 286c 616d 6264 6120  ke_while(lambda 
+00003ab0: 763a 2076 203c 2031 290d 0a20 2020 2020  v: v < 1)..     
+00003ac0: 2020 2069 5475 706c 6528 3029 0d0a 2020     iTuple(0)..  
+00003ad0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00003ae0: 2020 2064 6566 2069 7465 7228 293a 0d0a     def iter():..
+00003af0: 2020 2020 2020 2020 2020 2020 6920 3d20              i = 
+00003b00: 300d 0a20 2020 2020 2020 2020 2020 2066  0..            f
+00003b10: 6f72 2076 2069 6e20 7365 6c66 3a0d 0a20  or v in self:.. 
+00003b20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00003b30: 6620 6628 7629 2061 6e64 2028 6e20 6973  f f(v) and (n is
+00003b40: 204e 6f6e 6520 6f72 2069 203c 206e 293a   None or i < n):
+00003b50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003b60: 2020 2020 2020 7969 656c 6420 760d 0a20        yield v.. 
+00003b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b80: 2020 2069 202b 3d20 310d 0a20 2020 2020     i += 1..     
+00003b90: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00003ba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003bb0: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
+00003bc0: 2020 2020 2020 7265 7320 3d20 6974 6572        res = iter
+00003bd0: 2829 0d0a 2020 2020 2020 2020 7265 7475  ()..        retu
+00003be0: 726e 2072 6573 2069 6620 6c61 7a79 2065  rn res if lazy e
+00003bf0: 6c73 6520 7479 7065 2873 656c 6629 2864  lse type(self)(d
+00003c00: 6174 613d 7265 7329 0d0a 0d0a 2020 2020  ata=res)....    
+00003c10: 6465 6620 7461 696c 5f77 6869 6c65 2873  def tail_while(s
+00003c20: 656c 662c 2066 2c20 6e20 3d20 4e6f 6e65  elf, f, n = None
+00003c30: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
+00003c40: 0a20 2020 2020 2020 203e 3e3e 2069 5475  .        >>> iTu
+00003c50: 706c 652e 7261 6e67 6528 3329 2e74 6169  ple.range(3).tai
+00003c60: 6c5f 7768 696c 6528 6c61 6d62 6461 2076  l_while(lambda v
+00003c70: 3a20 7620 3e20 3129 0d0a 2020 2020 2020  : v > 1)..      
+00003c80: 2020 6954 7570 6c65 2832 290d 0a20 2020    iTuple(2)..   
+00003c90: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00003ca0: 2020 6920 3d20 300d 0a20 2020 2020 2020    i = 0..       
+00003cb0: 2066 6f72 2076 2069 6e20 7265 7665 7273   for v in revers
+00003cc0: 6564 2873 656c 6629 3a0d 0a20 2020 2020  ed(self):..     
+00003cd0: 2020 2020 2020 2069 6620 6628 7629 2061         if f(v) a
+00003ce0: 6e64 2028 6e20 6973 204e 6f6e 6520 6f72  nd (n is None or
+00003cf0: 2069 203c 206e 293a 0d0a 2020 2020 2020   i < n):..      
+00003d00: 2020 2020 2020 2020 2020 6920 2b3d 2031            i += 1
+00003d10: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00003d20: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00003d30: 2020 2020 2062 7265 616b 0d0a 2020 2020       break..    
+00003d40: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00003d50: 7461 696c 2869 290d 0a0d 0a20 2020 2023  tail(i)....    #
+00003d60: 204e 4f54 453a 2066 726f 6d20 6173 2069   NOTE: from as i
+00003d70: 6e2c 2073 7461 7274 696e 6720 6672 6f6d  n, starting from
+00003d80: 2066 6972 7374 2074 7275 650d 0a20 2020   first true..   
+00003d90: 2023 2076 6572 7375 7320 6162 6f76 652c   # versus above,
+00003da0: 2077 6869 6368 2069 7320 756e 7469 6c20   which is until 
+00003db0: 6669 7273 7420 6661 6c73 650d 0a20 2020  first false..   
+00003dc0: 2064 6566 2074 616b 655f 6166 7465 7228   def take_after(
+00003dd0: 7365 6c66 2c20 662c 206e 203d 204e 6f6e  self, f, n = Non
+00003de0: 652c 206c 617a 7920 3d20 4661 6c73 6529  e, lazy = False)
+00003df0: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00003e00: 2020 2020 2020 2020 3e3e 3e20 6954 7570          >>> iTup
+00003e10: 6c65 2e72 616e 6765 2833 292e 7461 6b65  le.range(3).take
+00003e20: 5f61 6674 6572 286c 616d 6264 6120 763a  _after(lambda v:
+00003e30: 2076 203c 2031 290d 0a20 2020 2020 2020   v < 1)..       
+00003e40: 2069 5475 706c 6528 312c 2032 290d 0a20   iTuple(1, 2).. 
+00003e50: 2020 2020 2020 203e 3e3e 2069 5475 706c         >>> iTupl
+00003e60: 652e 7261 6e67 6528 3329 2e74 616b 655f  e.range(3).take_
+00003e70: 6166 7465 7228 6c61 6d62 6461 2076 3a20  after(lambda v: 
+00003e80: 7620 3c20 312c 206e 203d 2031 290d 0a20  v < 1, n = 1).. 
+00003e90: 2020 2020 2020 2069 5475 706c 6528 3129         iTuple(1)
+00003ea0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00003eb0: 2020 2020 2020 2064 6566 2069 7465 7228         def iter(
+00003ec0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00003ed0: 6920 3d20 300d 0a20 2020 2020 2020 2020  i = 0..         
+00003ee0: 2020 2066 6f72 2076 2069 6e20 7365 6c66     for v in self
+00003ef0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003f00: 2020 2069 6620 6628 7629 3a0d 0a20 2020     if f(v):..   
+00003f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f20: 2070 6173 730d 0a20 2020 2020 2020 2020   pass..         
+00003f30: 2020 2020 2020 2065 6c69 6620 6e20 6973         elif n is
+00003f40: 204e 6f6e 6520 6f72 2069 203c 206e 3a0d   None or i < n:.
+00003f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003f60: 2020 2020 2079 6965 6c64 2076 0d0a 2020       yield v..  
+00003f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f80: 2020 6920 2b3d 2031 0d0a 2020 2020 2020    i += 1..      
+00003f90: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00003fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003fb0: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
+00003fc0: 2020 2020 2072 6573 203d 2069 7465 7228       res = iter(
+00003fd0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00003fe0: 6e20 7265 7320 6966 206c 617a 7920 656c  n res if lazy el
+00003ff0: 7365 2074 7970 6528 7365 6c66 2928 6461  se type(self)(da
+00004000: 7461 3d72 6573 290d 0a0d 0a20 2020 2064  ta=res)....    d
+00004010: 6566 2074 6169 6c5f 6166 7465 7228 7365  ef tail_after(se
+00004020: 6c66 2c20 662c 206e 203d 204e 6f6e 6529  lf, f, n = None)
+00004030: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00004040: 2020 2020 2020 2020 3e3e 3e20 6954 7570          >>> iTup
+00004050: 6c65 2e72 616e 6765 2833 292e 7461 696c  le.range(3).tail
+00004060: 5f61 6674 6572 286c 616d 6264 6120 763a  _after(lambda v:
+00004070: 2076 203c 2032 290d 0a20 2020 2020 2020   v < 2)..       
+00004080: 2069 5475 706c 6528 302c 2031 290d 0a20   iTuple(0, 1).. 
+00004090: 2020 2020 2020 203e 3e3e 2069 5475 706c         >>> iTupl
+000040a0: 652e 7261 6e67 6528 3329 2e74 6169 6c5f  e.range(3).tail_
+000040b0: 6166 7465 7228 6c61 6d62 6461 2076 3a20  after(lambda v: 
+000040c0: 7620 3c20 322c 2031 290d 0a20 2020 2020  v < 2, 1)..     
+000040d0: 2020 2069 5475 706c 6528 3129 0d0a 2020     iTuple(1)..  
+000040e0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+000040f0: 2020 206c 203d 2030 0d0a 2020 2020 2020     l = 0..      
+00004100: 2020 7220 3d20 300d 0a20 2020 2020 2020    r = 0..       
+00004110: 2066 6f72 2076 2069 6e20 7265 7665 7273   for v in revers
+00004120: 6564 2873 656c 6629 3a0d 0a20 2020 2020  ed(self):..     
+00004130: 2020 2020 2020 2069 6620 6e6f 7420 6628         if not f(
+00004140: 7629 3a0d 0a20 2020 2020 2020 2020 2020  v):..           
+00004150: 2020 2020 206c 202b 3d20 310d 0a20 2020       l += 1..   
+00004160: 2020 2020 2020 2020 2065 6c69 6620 6e20           elif n 
+00004170: 6973 204e 6f6e 6520 6f72 2072 203c 206e  is None or r < n
+00004180: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004190: 2020 2072 202b 3d20 310d 0a20 2020 2020     r += 1..     
+000041a0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000041b0: 2020 2020 2020 2020 2020 2020 2020 6272                br
+000041c0: 6561 6b0d 0a20 2020 2020 2020 2072 6574  eak..        ret
+000041d0: 7572 6e20 7365 6c66 2e74 6169 6c28 6c20  urn self.tail(l 
+000041e0: 2b20 7229 2e74 616b 6528 7229 0d0a 0d0a  + r).take(r)....
+000041f0: 2020 2020 6465 6620 6973 6c69 6365 2873      def islice(s
+00004200: 656c 662c 206c 6566 7420 3d20 4e6f 6e65  elf, left = None
+00004210: 2c20 7269 6768 7420 3d20 4e6f 6e65 293a  , right = None):
+00004220: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00004230: 2020 2020 2020 203e 3e3e 2069 5475 706c         >>> iTupl
+00004240: 652e 7261 6e67 6528 3529 2e69 736c 6963  e.range(5).islic
+00004250: 6528 312c 2033 290d 0a20 2020 2020 2020  e(1, 3)..       
+00004260: 2069 5475 706c 6528 312c 2032 290d 0a20   iTuple(1, 2).. 
+00004270: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00004280: 2020 2020 7265 7475 726e 2073 656c 665b      return self[
+00004290: 6c65 6674 3a72 6967 6874 5d0d 0a0d 0a20  left:right].... 
+000042a0: 2020 2064 6566 2075 6e69 7175 6528 7365     def unique(se
+000042b0: 6c66 293a 0d0a 2020 2020 2020 2020 2222  lf):..        ""
+000042c0: 220d 0a20 2020 2020 2020 203e 3e3e 2069  "..        >>> i
+000042d0: 5475 706c 6528 5b31 2c20 312c 2033 2c20  Tuple([1, 1, 3, 
+000042e0: 322c 2034 2c20 322c 2033 5d29 2e75 6e69  2, 4, 2, 3]).uni
+000042f0: 7175 6528 290d 0a20 2020 2020 2020 2069  que()..        i
+00004300: 5475 706c 6528 312c 2033 2c20 322c 2034  Tuple(1, 3, 2, 4
+00004310: 290d 0a20 2020 2020 2020 2022 2222 0d0a  )..        """..
+00004320: 2020 2020 2020 2020 6465 6620 6974 6572          def iter
+00004330: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+00004340: 2073 6565 6e20 3d20 7365 7428 290d 0a20   seen = set().. 
+00004350: 2020 2020 2020 2020 2020 2073 6565 6e5f             seen_
+00004360: 6164 6420 3d20 7365 656e 2e61 6464 0d0a  add = seen.add..
+00004370: 2020 2020 2020 2020 2020 2020 7365 656e              seen
+00004380: 5f63 6f6e 7461 696e 7320 3d20 7365 656e  _contains = seen
+00004390: 2e5f 5f63 6f6e 7461 696e 735f 5f0d 0a20  .__contains__.. 
+000043a0: 2020 2020 2020 2020 2020 2066 6f72 2076             for v
+000043b0: 2069 6e20 6974 6572 746f 6f6c 732e 6669   in itertools.fi
+000043c0: 6c74 6572 6661 6c73 6528 7365 656e 5f63  lterfalse(seen_c
+000043d0: 6f6e 7461 696e 732c 2073 656c 6629 3a0d  ontains, self):.
+000043e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000043f0: 2073 6565 6e5f 6164 6428 7629 0d0a 2020   seen_add(v)..  
+00004400: 2020 2020 2020 2020 2020 2020 2020 7969                yi
+00004410: 656c 6420 760d 0a20 2020 2020 2020 2072  eld v..        r
+00004420: 6574 7572 6e20 7479 7065 2873 656c 6629  eturn type(self)
+00004430: 2864 6174 613d 6974 6572 2829 290d 0a20  (data=iter()).. 
+00004440: 2020 200d 0a20 2020 2064 6566 2073 6f72     ..    def sor
+00004450: 7428 7365 6c66 2c20 6620 3d20 6c61 6d62  t(self, f = lamb
+00004460: 6461 2076 3a20 7629 3a0d 0a20 2020 2020  da v: v):..     
+00004470: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00004480: 3e3e 3e20 6954 7570 6c65 2e72 616e 6765  >>> iTuple.range
+00004490: 2833 292e 7265 7665 7273 6528 292e 736f  (3).reverse().so
+000044a0: 7274 2829 0d0a 2020 2020 2020 2020 6954  rt()..        iT
+000044b0: 7570 6c65 2830 2c20 312c 2032 290d 0a20  uple(0, 1, 2).. 
+000044c0: 2020 2020 2020 203e 3e3e 2069 5475 706c         >>> iTupl
+000044d0: 652e 7261 6e67 6528 3329 2e73 6f72 7428  e.range(3).sort(
+000044e0: 290d 0a20 2020 2020 2020 2069 5475 706c  )..        iTupl
+000044f0: 6528 302c 2031 2c20 3229 0d0a 2020 2020  e(0, 1, 2)..    
+00004500: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00004510: 2072 6574 7572 6e20 7479 7065 2873 656c   return type(sel
+00004520: 6629 2864 6174 613d 736f 7274 6564 2873  f)(data=sorted(s
+00004530: 656c 662c 206b 6579 203d 2066 2929 0d0a  elf, key = f))..
+00004540: 0d0a 2020 2020 6465 6620 6163 6375 6d75  ..    def accumu
+00004550: 6c61 7465 2873 656c 662c 2066 2c20 696e  late(self, f, in
+00004560: 6974 6961 6c20 3d20 4e6f 6e65 2c20 6c61  itial = None, la
+00004570: 7a79 203d 2046 616c 7365 293a 0d0a 2020  zy = False):..  
+00004580: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00004590: 2020 203e 3e3e 2069 5475 706c 652e 7261     >>> iTuple.ra
+000045a0: 6e67 6528 3329 2e61 6363 756d 756c 6174  nge(3).accumulat
+000045b0: 6528 6c61 6d62 6461 2061 6363 2c20 763a  e(lambda acc, v:
+000045c0: 2076 290d 0a20 2020 2020 2020 2069 5475   v)..        iTu
+000045d0: 706c 6528 302c 2031 2c20 3229 0d0a 2020  ple(0, 1, 2)..  
+000045e0: 2020 2020 2020 3e3e 3e20 6954 7570 6c65        >>> iTuple
+000045f0: 2e72 616e 6765 2833 292e 6163 6375 6d75  .range(3).accumu
+00004600: 6c61 7465 286c 616d 6264 6120 6163 632c  late(lambda acc,
+00004610: 2076 3a20 762c 2069 6e69 7469 616c 3d30   v: v, initial=0
+00004620: 290d 0a20 2020 2020 2020 2069 5475 706c  )..        iTupl
+00004630: 6528 302c 2030 2c20 312c 2032 290d 0a20  e(0, 0, 1, 2).. 
+00004640: 2020 2020 2020 203e 3e3e 2069 5475 706c         >>> iTupl
+00004650: 652e 7261 6e67 6528 3329 2e61 6363 756d  e.range(3).accum
+00004660: 756c 6174 6528 6f70 6572 6174 6f72 2e61  ulate(operator.a
+00004670: 6464 290d 0a20 2020 2020 2020 2069 5475  dd)..        iTu
+00004680: 706c 6528 302c 2031 2c20 3329 0d0a 2020  ple(0, 1, 3)..  
+00004690: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+000046a0: 2020 2072 6573 203d 2069 7465 7274 6f6f     res = itertoo
+000046b0: 6c73 2e61 6363 756d 756c 6174 6528 7365  ls.accumulate(se
+000046c0: 6c66 2c20 6675 6e63 3d66 2c20 696e 6974  lf, func=f, init
+000046d0: 6961 6c3d 696e 6974 6961 6c29 0d0a 2020  ial=initial)..  
+000046e0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000046f0: 2069 6620 6c61 7a79 2065 6c73 6520 6954   if lazy else iT
+00004700: 7570 6c65 2864 6174 613d 7265 7329 0d0a  uple(data=res)..
+00004710: 0d0a 2020 2020 6465 6620 666f 6c64 6375  ..    def foldcu
+00004720: 6d28 7365 6c66 2c20 2a61 7267 732c 202a  m(self, *args, *
+00004730: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
+00004740: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00004750: 3e3e 3e20 6954 7570 6c65 2e72 616e 6765  >>> iTuple.range
+00004760: 2833 292e 666f 6c64 6375 6d28 6c61 6d62  (3).foldcum(lamb
+00004770: 6461 2061 6363 2c20 763a 2076 290d 0a20  da acc, v: v).. 
+00004780: 2020 2020 2020 2069 5475 706c 6528 302c         iTuple(0,
+00004790: 2031 2c20 3229 0d0a 2020 2020 2020 2020   1, 2)..        
+000047a0: 3e3e 3e20 6954 7570 6c65 2e72 616e 6765  >>> iTuple.range
+000047b0: 2833 292e 666f 6c64 6375 6d28 6f70 6572  (3).foldcum(oper
+000047c0: 6174 6f72 2e61 6464 290d 0a20 2020 2020  ator.add)..     
+000047d0: 2020 2069 5475 706c 6528 302c 2031 2c20     iTuple(0, 1, 
+000047e0: 3329 0d0a 2020 2020 2020 2020 2222 220d  3)..        """.
+000047f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00004800: 7365 6c66 2e61 6363 756d 756c 6174 6528  self.accumulate(
+00004810: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+00004820: 0d0a 0d0a 2020 2020 6465 6620 666f 6c64  ....    def fold
+00004830: 2873 656c 662c 2066 2c20 696e 6974 6961  (self, f, initia
+00004840: 6c3d 4e6f 6e65 293a 0d0a 2020 2020 2020  l=None):..      
+00004850: 2020 2222 220d 0a20 2020 2020 2020 203e    """..        >
+00004860: 3e3e 2069 5475 706c 652e 7261 6e67 6528  >> iTuple.range(
+00004870: 3329 2e66 6f6c 6428 6c61 6d62 6461 2061  3).fold(lambda a
+00004880: 6363 2c20 763a 2076 290d 0a20 2020 2020  cc, v: v)..     
+00004890: 2020 2032 0d0a 2020 2020 2020 2020 3e3e     2..        >>
+000048a0: 3e20 6954 7570 6c65 2e72 616e 6765 2833  > iTuple.range(3
+000048b0: 292e 666f 6c64 286c 616d 6264 6120 6163  ).fold(lambda ac
+000048c0: 632c 2076 3a20 762c 2069 6e69 7469 616c  c, v: v, initial
+000048d0: 3d30 290d 0a20 2020 2020 2020 2032 0d0a  =0)..        2..
+000048e0: 2020 2020 2020 2020 3e3e 3e20 6954 7570          >>> iTup
+000048f0: 6c65 2e72 616e 6765 2833 292e 666f 6c64  le.range(3).fold
+00004900: 286f 7065 7261 746f 722e 6164 6429 0d0a  (operator.add)..
+00004910: 2020 2020 2020 2020 330d 0a20 2020 2020          3..     
+00004920: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00004930: 6966 2069 6e69 7469 616c 2069 7320 6e6f  if initial is no
+00004940: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+00004950: 2020 2020 2072 6573 203d 2066 756e 6374       res = funct
+00004960: 6f6f 6c73 2e72 6564 7563 6528 662c 2073  ools.reduce(f, s
+00004970: 656c 662c 2069 6e69 7469 616c 290d 0a20  elf, initial).. 
+00004980: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00004990: 2020 2020 2020 2020 2020 7265 7320 3d20            res = 
+000049a0: 6675 6e63 746f 6f6c 732e 7265 6475 6365  functools.reduce
+000049b0: 2866 2c20 7365 6c66 290d 0a20 2020 2020  (f, self)..     
+000049c0: 2020 2072 6574 7572 6e20 7265 730d 0a0d     return res...
+000049d0: 0a20 2020 2023 202d 2d2d 2d2d 0d0a 0d0a  .    # -----....
+000049e0: 2020 2020 2320 636f 6d62 696e 6174 6f72      # combinator
+000049f0: 6963 730d 0a0d 0a20 2020 2023 202d 2d2d  ics....    # ---
+00004a00: 2d2d 0d0a 0d0a 2320 2d2d 2d2d 2d2d 2d2d  --....# --------
+00004a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004a40: 2d2d 2d2d 2d2d 2d0d 0a0d 0a40 6e54 7570  -------....@nTup
+00004a50: 6c65 2e64 6563 6f72 6174 650d 0a63 6c61  le.decorate..cla
+00004a60: 7373 2045 7861 6d70 6c65 2874 7970 696e  ss Example(typin
+00004a70: 672e 4e61 6d65 6454 7570 6c65 293a 0d0a  g.NamedTuple):..
+00004a80: 2020 2020 2222 220d 0a20 2020 203e 3e3e      """..    >>>
+00004a90: 2065 7820 3d20 4578 616d 706c 6528 312c   ex = Example(1,
+00004aa0: 2022 6122 290d 0a20 2020 203e 3e3e 2065   "a")..    >>> e
+00004ab0: 780d 0a20 2020 2045 7861 6d70 6c65 2878  x..    Example(x
+00004ac0: 3d31 2c20 733d 2761 272c 2069 743d 6954  =1, s='a', it=iT
+00004ad0: 7570 6c65 2829 290d 0a20 2020 203e 3e3e  uple())..    >>>
+00004ae0: 2065 782e 636c 730d 0a20 2020 203c 636c   ex.cls..    <cl
+00004af0: 6173 7320 2778 7475 706c 6573 2e78 7475  ass 'xtuples.xtu
+00004b00: 706c 6573 2e6e 5475 706c 6527 3e0d 0a20  ples.nTuple'>.. 
+00004b10: 2020 203e 3e3e 2065 782e 7069 7065 286c     >>> ex.pipe(l
+00004b20: 616d 6264 6120 6e74 3a20 6e74 2e78 290d  ambda nt: nt.x).
+00004b30: 0a20 2020 2031 0d0a 2020 2020 3e3e 3e20  .    1..    >>> 
+00004b40: 6620 3d20 6578 2e70 6172 7469 616c 286c  f = ex.partial(l
+00004b50: 616d 6264 6120 6e74 2c20 763a 206e 742e  ambda nt, v: nt.
+00004b60: 7820 2a20 7629 0d0a 2020 2020 3e3e 3e20  x * v)..    >>> 
+00004b70: 6628 3229 0d0a 2020 2020 320d 0a20 2020  f(2)..    2..   
+00004b80: 203e 3e3e 2066 2833 290d 0a20 2020 2033   >>> f(3)..    3
+00004b90: 0d0a 2020 2020 2222 220d 0a20 2020 2023  ..    """..    #
+00004ba0: 204e 4f54 453a 2063 6c73 2c20 7069 7065   NOTE: cls, pipe
+00004bb0: 2c20 7061 7274 6961 6c20 6172 6520 6d61  , partial are ma
+00004bc0: 6e64 6174 6f72 7920 626f 696c 6572 706c  ndatory boilerpl
+00004bd0: 6174 650d 0a0d 0a20 2020 2078 3a20 696e  ate....    x: in
+00004be0: 740d 0a20 2020 2073 3a20 7374 720d 0a20  t..    s: str.. 
+00004bf0: 2020 2069 743a 2069 5475 706c 6520 3d20     it: iTuple = 
+00004c00: 6954 7570 6c65 285b 5d29 0d0a 0d0a 2020  iTuple([])....  
+00004c10: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
+00004c20: 2064 6566 2063 6c73 2873 656c 6629 3a0d   def cls(self):.
+00004c30: 0a20 2020 2020 2020 202e 2e2e 0d0a 0d0a  .        .......
+00004c40: 2020 2020 6465 6620 7069 7065 2873 656c      def pipe(sel
+00004c50: 662c 2066 2c20 2a61 7267 732c 202a 2a6b  f, f, *args, **k
+00004c60: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
+00004c70: 202e 2e2e 0d0a 0d0a 2020 2020 6465 6620   .......    def 
+00004c80: 7061 7274 6961 6c28 7365 6c66 2c20 662c  partial(self, f,
+00004c90: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
+00004ca0: 293a 0d0a 2020 2020 2020 2020 2e2e 2e0d  ):..        ....
+00004cb0: 0a0d 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d  ...# -----------
+00004cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004cf0: 2d2d 2d2d 0d0a 0d0a 2320 544f 444f 3a20  ----....# TODO: 
+00004d00: 636f 6e74 6578 7420 6d61 6e61 6765 7220  context manager 
+00004d10: 746f 2063 6f6e 7472 6f6c 0d0a 2320 6966  to control..# if
+00004d20: 2077 6520 6164 6420 7468 6520 7479 7065   we add the type
+00004d30: 2069 6e66 6f72 6d61 7469 6f6e 2077 6865   information whe
+00004d40: 6e20 7772 6974 696e 6720 746f 206a 736f  n writing to jso
+00004d50: 6e20 6f72 206e 6f74 0d0a 0d0a 2320 544f  n or not....# TO
+00004d60: 444f 3a20 636f 6e74 6578 7420 6d61 6e61  DO: context mana
+00004d70: 6e67 6572 2074 6f20 636f 6e74 726f 6c0d  nger to control.
+00004d80: 0a23 206c 617a 7920 6465 6661 756c 7420  .# lazy default 
+00004d90: 6265 6861 7669 6f75 7220 2869 652e 2064  behaviour (ie. d
+00004da0: 6566 6175 6c74 2074 6f20 6c61 7a79 206f  efault to lazy o
+00004db0: 7220 6e6f 7429 0d0a 0d0a 2320 2d2d 2d2d  r not)....# ----
+00004dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a63  -----------....c
+00004e00: 6c61 7373 204a 534f 4e45 6e63 6f64 6572  lass JSONEncoder
+00004e10: 286a 736f 6e2e 4a53 4f4e 456e 636f 6465  (json.JSONEncode
+00004e20: 7229 3a0d 0a0d 0a20 2020 2064 6566 2069  r):....    def i
+00004e30: 7465 7265 6e63 6f64 6528 7365 6c66 2c20  terencode(self, 
+00004e40: 6f2c 202a 6172 6773 2c20 2a2a 6b77 6172  o, *args, **kwar
+00004e50: 6773 293a 0d0a 2020 2020 2020 2020 666f  gs):..        fo
+00004e60: 7220 6368 756e 6b20 696e 2073 7570 6572  r chunk in super
+00004e70: 2829 2e69 7465 7265 6e63 6f64 6528 0d0a  ().iterencode(..
+00004e80: 2020 2020 2020 2020 2020 2020 6361 7374              cast
+00004e90: 5f6a 736f 6e28 6f29 2c20 2a61 7267 732c  _json(o), *args,
+00004ea0: 202a 2a6b 7761 7267 730d 0a20 2020 2020   **kwargs..     
+00004eb0: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
+00004ec0: 2020 2079 6965 6c64 2063 6875 6e6b 0d0a     yield chunk..
+00004ed0: 0d0a 2020 2020 2320 6465 6620 6d65 7461  ..    # def meta
+00004ee0: 5f64 6566 6175 6c74 2873 656c 662c 206f  _default(self, o
+00004ef0: 626a 293a 0d0a 2020 2020 2320 2020 2020  bj):..    #     
+00004f00: 7265 7475 726e 206a 736f 6e2e 4a53 4f4e  return json.JSON
+00004f10: 456e 636f 6465 722e 6465 6661 756c 7428  Encoder.default(
+00004f20: 7365 6c66 2c20 6f62 6a29 0d0a 0d0a 2020  self, obj)....  
+00004f30: 2020 2320 6465 6620 6465 6661 756c 7428    # def default(
+00004f40: 7365 6c66 2c20 6f62 6a29 3a0d 0a20 2020  self, obj):..   
+00004f50: 2023 2020 2020 2069 6620 6973 696e 7374   #     if isinst
+00004f60: 616e 6365 286f 626a 2c20 6644 6963 7429  ance(obj, fDict)
+00004f70: 3a0d 0a20 2020 2023 2020 2020 2020 2020  :..    #        
+00004f80: 2072 6574 7572 6e20 7365 6c66 2e6d 6574   return self.met
+00004f90: 615f 6465 6661 756c 7428 6f62 6a2e 6461  a_default(obj.da
+00004fa0: 7461 290d 0a20 2020 2023 2020 2020 2072  ta)..    #     r
+00004fb0: 6574 7572 6e20 6361 7374 5f6a 736f 6e28  eturn cast_json(
+00004fc0: 6f62 6a2c 2064 6566 6175 6c74 3d73 656c  obj, default=sel
+00004fd0: 662e 6d65 7461 5f64 6566 6175 6c74 290d  f.meta_default).
+00004fe0: 0a0d 0a23 202d 2d2d 2d2d 0d0a 0d0a 636c  ...# -----....cl
+00004ff0: 6173 7320 4a53 4f4e 4465 636f 6465 7228  ass JSONDecoder(
+00005000: 6a73 6f6e 2e4a 534f 4e44 6563 6f64 6572  json.JSONDecoder
+00005010: 293a 0d0a 0d0a 2020 2020 6465 6620 5f5f  ):....    def __
+00005020: 696e 6974 5f5f 2873 656c 662c 202a 6172  init__(self, *ar
+00005030: 6773 2c20 2a2a 6b77 6172 6773 293a 0d0a  gs, **kwargs):..
+00005040: 2020 2020 2020 2020 6a73 6f6e 2e4a 534f          json.JSO
+00005050: 4e44 6563 6f64 6572 2e5f 5f69 6e69 745f  NDecoder.__init_
+00005060: 5f28 0d0a 2020 2020 2020 2020 2020 2020  _(..            
+00005070: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+00005080: 2020 206f 626a 6563 745f 686f 6f6b 3d73     object_hook=s
+00005090: 656c 662e 6f62 6a65 6374 5f68 6f6f 6b2c  elf.object_hook,
+000050a0: 0d0a 2020 2020 2020 2020 2020 2020 2a61  ..            *a
+000050b0: 7267 732c 0d0a 2020 2020 2020 2020 2020  rgs,..          
+000050c0: 2020 2a2a 6b77 6172 6773 0d0a 2020 2020    **kwargs..    
+000050d0: 2020 2020 2020 2020 230d 0a20 2020 2020          #..     
+000050e0: 2020 2029 0d0a 0d0a 2020 2020 4063 6c61     )....    @cla
+000050f0: 7373 6d65 7468 6f64 0d0a 2020 2020 6465  ssmethod..    de
+00005100: 6620 7874 7570 6c65 5f6f 626a 6563 745f  f xtuple_object_
+00005110: 686f 6f6b 2863 6c73 2c20 6429 3a0d 0a20  hook(cls, d):.. 
+00005120: 2020 2020 2020 2072 6574 7572 6e20 756e         return un
+00005130: 6361 7374 5f6a 736f 6e28 6429 0d0a 0d0a  cast_json(d)....
+00005140: 2020 2020 6465 6620 6f62 6a65 6374 5f68      def object_h
+00005150: 6f6f 6b28 7365 6c66 2c20 6429 3a0d 0a20  ook(self, d):.. 
+00005160: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00005170: 6c66 2e78 7475 706c 655f 6f62 6a65 6374  lf.xtuple_object
+00005180: 5f68 6f6f 6b28 6429 0d0a 0d0a 2320 2d2d  _hook(d)....# --
+00005190: 2d2d 2d0d 0a0d 0a64 6566 2063 6173 745f  ---....def cast_
+000051a0: 6a73 6f6e 286f 626a 2c20 6465 6661 756c  json(obj, defaul
+000051b0: 7420 3d20 6c61 6d62 6461 206f 626a 3a20  t = lambda obj: 
+000051c0: 6f62 6a29 3a0d 0a20 2020 2069 6620 6e54  obj):..    if nT
+000051d0: 7570 6c65 2e69 735f 696e 7374 616e 6365  uple.is_instance
+000051e0: 286f 626a 293a 0d0a 2020 2020 2020 2020  (obj):..        
+000051f0: 7265 7475 726e 206e 5475 706c 652e 6361  return nTuple.ca
+00005200: 7374 5f6a 736f 6e28 6f62 6a29 0d0a 2020  st_json(obj)..  
+00005210: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+00005220: 7265 7475 726e 206f 626a 2e63 6173 745f  return obj.cast_
+00005230: 6a73 6f6e 2829 0d0a 2020 2020 6578 6365  json()..    exce
+00005240: 7074 3a0d 0a20 2020 2020 2020 2072 6574  pt:..        ret
+00005250: 7572 6e20 6465 6661 756c 7428 6f62 6a29  urn default(obj)
+00005260: 0d0a 0d0a 6465 6620 756e 6361 7374 5f6a  ....def uncast_j
+00005270: 736f 6e28 6f62 6a29 3a0d 0a20 2020 2069  son(obj):..    i
+00005280: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+00005290: 286f 626a 2c20 6469 6374 293a 0d0a 2020  (obj, dict):..  
+000052a0: 2020 2020 2020 7265 7475 726e 206f 626a        return obj
+000052b0: 0d0a 2020 2020 5f5f 745f 5f20 3d20 6f62  ..    __t__ = ob
+000052c0: 6a2e 6765 7428 225f 5f74 5f5f 222c 204e  j.get("__t__", N
+000052d0: 6f6e 6529 0d0a 2020 2020 6966 205f 5f74  one)..    if __t
+000052e0: 5f5f 2069 7320 4e6f 6e65 3a0d 0a20 2020  __ is None:..   
+000052f0: 2020 2020 2072 6574 7572 6e20 6f62 6a0d       return obj.
+00005300: 0a20 2020 2063 6c73 203d 2069 5475 706c  .    cls = iTupl
+00005310: 6520 6966 205f 5f74 5f5f 203d 3d20 2269  e if __t__ == "i
+00005320: 5475 706c 6522 2065 6c73 6520 5245 4749  Tuple" else REGI
+00005330: 5354 5259 5b5f 5f74 5f5f 5d0d 0a20 2020  STRY[__t__]..   
+00005340: 2069 6620 6861 7361 7474 7228 636c 732c   if hasattr(cls,
+00005350: 2022 756e 6361 7374 5f6a 736f 6e22 293a   "uncast_json"):
+00005360: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00005370: 2063 6c73 2e75 6e63 6173 745f 6a73 6f6e   cls.uncast_json
+00005380: 286f 626a 290d 0a20 2020 2072 6574 7572  (obj)..    retur
+00005390: 6e20 636c 7328 0d0a 2020 2020 2020 2020  n cls(..        
+000053a0: 2a28 7620 666f 7220 6b2c 2076 2069 6e20  *(v for k, v in 
+000053b0: 6f62 6a2e 6974 656d 7328 2920 6966 206b  obj.items() if k
+000053c0: 2021 3d20 225f 5f74 5f5f 2229 0d0a 2020   != "__t__")..  
+000053d0: 2020 290d 0a0d 0a23 202d 2d2d 2d2d 0d0a    )....# -----..
+000053e0: 0d0a 2320 544f 444f 3a20 6653 7472 696e  ..# TODO: fStrin
+000053f0: 6720 736f 2063 616e 2064 6f20 2e70 6970  g so can do .pip
+00005400: 6520 3f0d 0a64 6566 2074 6f5f 6a73 6f6e  e ?..def to_json
+00005410: 2876 2c20 2a2a 6b77 6172 6773 293a 0d0a  (v, **kwargs):..
+00005420: 2020 2020 2222 220d 0a20 2020 203e 3e3e      """..    >>>
+00005430: 2070 7269 6e74 2869 5475 706c 6528 5b45   print(iTuple([E
+00005440: 7861 6d70 6c65 2831 2c20 2261 2229 5d29  xample(1, "a")])
+00005450: 2e70 6970 6528 746f 5f6a 736f 6e2c 2069  .pipe(to_json, i
+00005460: 6e64 656e 743d 3229 290d 0a20 2020 207b  ndent=2))..    {
+00005470: 0d0a 2020 2020 2020 225f 5f74 5f5f 223a  ..      "__t__":
+00005480: 2022 6954 7570 6c65 222c 0d0a 2020 2020   "iTuple",..    
+00005490: 2020 2264 6174 6122 3a20 5b0d 0a20 2020    "data": [..   
+000054a0: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+000054b0: 2020 2278 223a 2031 2c0d 0a20 2020 2020    "x": 1,..     
+000054c0: 2020 2020 2022 7322 3a20 2261 222c 0d0a       "s": "a",..
+000054d0: 2020 2020 2020 2020 2020 2269 7422 3a20            "it": 
+000054e0: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
+000054f0: 5f5f 745f 5f22 3a20 2269 5475 706c 6522  __t__": "iTuple"
+00005500: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00005510: 6461 7461 223a 205b 5d0d 0a20 2020 2020  data": []..     
+00005520: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
+00005530: 2020 2022 5f5f 745f 5f22 3a20 2245 7861     "__t__": "Exa
+00005540: 6d70 6c65 220d 0a20 2020 2020 2020 207d  mple"..        }
+00005550: 0d0a 2020 2020 2020 5d0d 0a20 2020 207d  ..      ]..    }
+00005560: 0d0a 2020 2020 3e3e 3e20 7072 696e 7428  ..    >>> print(
+00005570: 6954 7570 6c65 285b 0d0a 2020 2020 2e2e  iTuple([..    ..
+00005580: 2e20 2020 2020 6954 7570 6c65 285b 4578  .     iTuple([Ex
+00005590: 616d 706c 6528 312c 2022 6122 295d 290d  ample(1, "a")]).
+000055a0: 0a20 2020 202e 2e2e 205d 292e 7069 7065  .    ... ]).pipe
+000055b0: 2874 6f5f 6a73 6f6e 2c20 696e 6465 6e74  (to_json, indent
+000055c0: 3d32 2929 0d0a 2020 2020 7b0d 0a20 2020  =2))..    {..   
+000055d0: 2020 2022 5f5f 745f 5f22 3a20 2269 5475     "__t__": "iTu
+000055e0: 706c 6522 2c0d 0a20 2020 2020 2022 6461  ple",..      "da
+000055f0: 7461 223a 205b 0d0a 2020 2020 2020 2020  ta": [..        
+00005600: 7b0d 0a20 2020 2020 2020 2020 2022 5f5f  {..          "__
+00005610: 745f 5f22 3a20 2269 5475 706c 6522 2c0d  t__": "iTuple",.
+00005620: 0a20 2020 2020 2020 2020 2022 6461 7461  .          "data
+00005630: 223a 205b 0d0a 2020 2020 2020 2020 2020  ": [..          
+00005640: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
+00005650: 2020 2022 7822 3a20 312c 0d0a 2020 2020     "x": 1,..    
+00005660: 2020 2020 2020 2020 2020 2273 223a 2022            "s": "
+00005670: 6122 2c0d 0a20 2020 2020 2020 2020 2020  a",..           
+00005680: 2020 2022 6974 223a 207b 0d0a 2020 2020     "it": {..    
+00005690: 2020 2020 2020 2020 2020 2020 225f 5f74              "__t
+000056a0: 5f5f 223a 2022 6954 7570 6c65 222c 0d0a  __": "iTuple",..
+000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056c0: 2264 6174 6122 3a20 5b5d 0d0a 2020 2020  "data": []..    
+000056d0: 2020 2020 2020 2020 2020 7d2c 0d0a 2020            },..  
+000056e0: 2020 2020 2020 2020 2020 2020 225f 5f74              "__t
+000056f0: 5f5f 223a 2022 4578 616d 706c 6522 0d0a  __": "Example"..
+00005700: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
+00005710: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
+00005720: 2020 2020 7d0d 0a20 2020 2020 205d 0d0a      }..      ]..
+00005730: 2020 2020 7d0d 0a20 2020 203e 3e3e 2070      }..    >>> p
+00005740: 7269 6e74 2845 7861 6d70 6c65 2832 2c20  rint(Example(2, 
+00005750: 2262 222c 2069 5475 706c 6528 5b0d 0a20  "b", iTuple([.. 
+00005760: 2020 202e 2e2e 2020 2020 2069 5475 706c     ...     iTupl
+00005770: 6528 5b45 7861 6d70 6c65 2831 2c20 2261  e([Example(1, "a
+00005780: 2229 5d29 0d0a 2020 2020 2e2e 2e20 5d29  ")])..    ... ])
+00005790: 292e 7069 7065 2874 6f5f 6a73 6f6e 2c20  ).pipe(to_json, 
+000057a0: 696e 6465 6e74 3d32 2929 0d0a 2020 2020  indent=2))..    
+000057b0: 7b0d 0a20 2020 2020 2022 7822 3a20 322c  {..      "x": 2,
+000057c0: 0d0a 2020 2020 2020 2273 223a 2022 6222  ..      "s": "b"
+000057d0: 2c0d 0a20 2020 2020 2022 6974 223a 207b  ,..      "it": {
+000057e0: 0d0a 2020 2020 2020 2020 225f 5f74 5f5f  ..        "__t__
+000057f0: 223a 2022 6954 7570 6c65 222c 0d0a 2020  ": "iTuple",..  
+00005800: 2020 2020 2020 2264 6174 6122 3a20 5b0d        "data": [.
+00005810: 0a20 2020 2020 2020 2020 207b 0d0a 2020  .          {..  
+00005820: 2020 2020 2020 2020 2020 225f 5f74 5f5f            "__t__
+00005830: 223a 2022 6954 7570 6c65 222c 0d0a 2020  ": "iTuple",..  
+00005840: 2020 2020 2020 2020 2020 2264 6174 6122            "data"
+00005850: 3a20 5b0d 0a20 2020 2020 2020 2020 2020  : [..           
+00005860: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+00005870: 2020 2020 2020 2278 223a 2031 2c0d 0a20        "x": 1,.. 
+00005880: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00005890: 7322 3a20 2261 222c 0d0a 2020 2020 2020  s": "a",..      
+000058a0: 2020 2020 2020 2020 2020 2269 7422 3a20            "it": 
+000058b0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+000058c0: 2020 2020 2022 5f5f 745f 5f22 3a20 2269       "__t__": "i
+000058d0: 5475 706c 6522 2c0d 0a20 2020 2020 2020  Tuple",..       
+000058e0: 2020 2020 2020 2020 2020 2022 6461 7461             "data
+000058f0: 223a 205b 5d0d 0a20 2020 2020 2020 2020  ": []..         
+00005900: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
+00005910: 2020 2020 2020 2020 2020 2022 5f5f 745f             "__t_
+00005920: 5f22 3a20 2245 7861 6d70 6c65 220d 0a20  _": "Example".. 
+00005930: 2020 2020 2020 2020 2020 2020 207d 0d0a               }..
+00005940: 2020 2020 2020 2020 2020 2020 5d0d 0a20              ].. 
+00005950: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
+00005960: 2020 2020 5d0d 0a20 2020 2020 207d 2c0d      ]..      },.
+00005970: 0a20 2020 2020 2022 5f5f 745f 5f22 3a20  .      "__t__": 
+00005980: 2245 7861 6d70 6c65 220d 0a20 2020 207d  "Example"..    }
+00005990: 0d0a 2020 2020 2222 220d 0a20 2020 2072  ..    """..    r
+000059a0: 6574 7572 6e20 6a73 6f6e 2e64 756d 7073  eturn json.dumps
+000059b0: 2876 2c20 636c 733d 4a53 4f4e 456e 636f  (v, cls=JSONEnco
+000059c0: 6465 722c 202a 2a6b 7761 7267 7329 0d0a  der, **kwargs)..
+000059d0: 0d0a 6465 6620 6672 6f6d 5f6a 736f 6e28  ..def from_json(
+000059e0: 763a 2073 7472 2c20 2a2a 6b77 6172 6773  v: str, **kwargs
+000059f0: 293a 0d0a 2020 2020 2222 220d 0a20 2020  ):..    """..   
+00005a00: 203e 3e3e 2065 7820 3d20 6954 7570 6c65   >>> ex = iTuple
+00005a10: 285b 4578 616d 706c 6528 312c 2022 6122  ([Example(1, "a"
+00005a20: 295d 290d 0a20 2020 203e 3e3e 2066 726f  )])..    >>> fro
+00005a30: 6d5f 6a73 6f6e 2865 782e 7069 7065 2874  m_json(ex.pipe(t
+00005a40: 6f5f 6a73 6f6e 2929 0d0a 2020 2020 6954  o_json))..    iT
+00005a50: 7570 6c65 2845 7861 6d70 6c65 2878 3d31  uple(Example(x=1
+00005a60: 2c20 733d 2761 272c 2069 743d 6954 7570  , s='a', it=iTup
+00005a70: 6c65 2829 2929 0d0a 2020 2020 3e3e 3e20  le()))..    >>> 
+00005a80: 6672 6f6d 5f6a 736f 6e28 0d0a 2020 2020  from_json(..    
+00005a90: 2e2e 2e20 2020 2020 6954 7570 6c65 285b  ...     iTuple([
+00005aa0: 6954 7570 6c65 285b 4578 616d 706c 6528  iTuple([Example(
+00005ab0: 312c 2022 6122 295d 295d 292e 7069 7065  1, "a")])]).pipe
+00005ac0: 2874 6f5f 6a73 6f6e 290d 0a20 2020 202e  (to_json)..    .
+00005ad0: 2e2e 2029 0d0a 2020 2020 6954 7570 6c65  .. )..    iTuple
+00005ae0: 2869 5475 706c 6528 4578 616d 706c 6528  (iTuple(Example(
+00005af0: 783d 312c 2073 3d27 6127 2c20 6974 3d69  x=1, s='a', it=i
+00005b00: 5475 706c 6528 2929 2929 0d0a 2020 2020  Tuple())))..    
+00005b10: 3e3e 3e20 6672 6f6d 5f6a 736f 6e28 0d0a  >>> from_json(..
+00005b20: 2020 2020 2e2e 2e20 2020 2020 4578 616d      ...     Exam
+00005b30: 706c 6528 322c 2022 6222 2c20 6954 7570  ple(2, "b", iTup
+00005b40: 6c65 285b 0d0a 2020 2020 2e2e 2e20 2020  le([..    ...   
+00005b50: 2020 2020 2020 6954 7570 6c65 285b 4578        iTuple([Ex
+00005b60: 616d 706c 6528 312c 2022 6122 295d 290d  ample(1, "a")]).
+00005b70: 0a20 2020 202e 2e2e 2020 2020 205d 2929  .    ...     ]))
+00005b80: 2e70 6970 6528 746f 5f6a 736f 6e29 0d0a  .pipe(to_json)..
+00005b90: 2020 2020 2e2e 2e20 290d 0a20 2020 2045      ... )..    E
+00005ba0: 7861 6d70 6c65 2878 3d32 2c20 733d 2762  xample(x=2, s='b
+00005bb0: 272c 2069 743d 6954 7570 6c65 2869 5475  ', it=iTuple(iTu
+00005bc0: 706c 6528 4578 616d 706c 6528 783d 312c  ple(Example(x=1,
+00005bd0: 2073 3d27 6127 2c20 6974 3d69 5475 706c   s='a', it=iTupl
+00005be0: 6528 2929 2929 290d 0a20 2020 2022 2222  e()))))..    """
+00005bf0: 0d0a 2020 2020 7265 7475 726e 206a 736f  ..    return jso
+00005c00: 6e2e 6c6f 6164 7328 762c 2063 6c73 3d4a  n.loads(v, cls=J
+00005c10: 534f 4e44 6563 6f64 6572 2c20 2a2a 6b77  SONDecoder, **kw
+00005c20: 6172 6773 290d 0a0d 0a64 6566 206c 6f61  args)....def loa
+00005c30: 645f 6a73 6f6e 2866 293a 0d0a 2020 2020  d_json(f):..    
+00005c40: 7265 7475 726e 206a 736f 6e2e 6c6f 6164  return json.load
+00005c50: 2866 2c20 636c 733d 4a53 4f4e 4465 636f  (f, cls=JSONDeco
+00005c60: 6465 7229 0d0a 0d0a 6465 6620 6475 6d70  der)....def dump
+00005c70: 5f6a 736f 6e28 662c 2076 293a 0d0a 2020  _json(f, v):..  
+00005c80: 2020 7265 7475 726e 206a 736f 6e2e 6475    return json.du
+00005c90: 6d70 2866 2c20 762c 2063 6c73 3d4a 534f  mp(f, v, cls=JSO
+00005ca0: 4e45 6e63 6f64 6572 290d 0a0d 0a23 202d  NEncoder)....# -
 00005cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00005cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00005cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00005ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a  --------------..
-00005cf0: 0d0a 2320 696d 706f 7274 206d 6973 632e  ..# import misc.
-00005d00: 7065 7266 6d6f 6e0d 0a0d 0a23 2064 6566  perfmon....# def
-00005d10: 2069 6e74 5f6d 656d 6f72 795f 6765 6e28   int_memory_gen(
-00005d20: 6375 6d3d 4661 6c73 6529 3a0d 0a23 2020  cum=False):..#  
-00005d30: 2020 2069 203d 2030 0d0a 2320 2020 2020     i = 0..#     
-00005d40: 7768 696c 6520 5472 7565 3a0d 0a23 2020  while True:..#  
-00005d50: 2020 2020 2020 2079 6965 6c64 2069 0d0a         yield i..
-00005d60: 2320 2020 2020 7265 7475 726e 0d0a 0d0a  #     return....
-00005d70: 2320 6465 6620 6469 6374 5f6d 656d 6f72  # def dict_memor
-00005d80: 795f 6765 6e28 6375 6d3d 4661 6c73 6529  y_gen(cum=False)
-00005d90: 3a0d 0a23 2020 2020 2069 203d 2030 0d0a  :..#     i = 0..
-00005da0: 2320 2020 2020 6966 2063 756d 3a0d 0a23  #     if cum:..#
-00005db0: 2020 2020 2020 2020 2077 6869 6c65 2054           while T
-00005dc0: 7275 653a 0d0a 2320 2020 2020 2020 2020  rue:..#         
-00005dd0: 2020 2020 7969 656c 6420 7b69 693a 2069      yield {ii: i
-00005de0: 6920 666f 7220 6969 2069 6e20 7261 6e67  i for ii in rang
-00005df0: 6528 6929 7d0d 0a23 2020 2020 2020 2020  e(i)}..#        
-00005e00: 2020 2020 2069 202b 3d20 310d 0a23 2020       i += 1..#  
-00005e10: 2020 2065 6c73 653a 0d0a 2320 2020 2020     else:..#     
-00005e20: 2020 2020 7768 696c 6520 5472 7565 3a0d      while True:.
-00005e30: 0a23 2020 2020 2020 2020 2020 2020 2079  .#             y
-00005e40: 6965 6c64 207b 693a 2069 7d0d 0a23 2020  ield {i: i}..#  
-00005e50: 2020 2020 2020 2020 2020 2069 202b 3d20             i += 
-00005e60: 310d 0a23 2020 2020 2072 6574 7572 6e0d  1..#     return.
-00005e70: 0a0d 0a23 2064 6566 206c 6973 745f 6d65  ...# def list_me
-00005e80: 6d6f 7279 5f67 656e 2863 756d 3d46 616c  mory_gen(cum=Fal
-00005e90: 7365 293a 0d0a 2320 2020 2020 6920 3d20  se):..#     i = 
-00005ea0: 300d 0a23 2020 2020 2069 6620 6375 6d3a  0..#     if cum:
-00005eb0: 0d0a 2320 2020 2020 2020 2020 7768 696c  ..#         whil
-00005ec0: 6520 5472 7565 3a0d 0a23 2020 2020 2020  e True:..#      
-00005ed0: 2020 2020 2020 2079 6965 6c64 206c 6973         yield lis
-00005ee0: 7428 7261 6e67 6528 6929 290d 0a23 2020  t(range(i))..#  
-00005ef0: 2020 2020 2020 2020 2020 2069 202b 3d20             i += 
-00005f00: 310d 0a23 2020 2020 2065 6c73 653a 0d0a  1..#     else:..
-00005f10: 2320 2020 2020 2020 2020 7768 696c 6520  #         while 
-00005f20: 5472 7565 3a0d 0a23 2020 2020 2020 2020  True:..#        
-00005f30: 2020 2020 2079 6965 6c64 205b 695d 0d0a       yield [i]..
-00005f40: 2320 2020 2020 2020 2020 2020 2020 6920  #             i 
-00005f50: 2b3d 2031 0d0a 2320 2020 2020 7265 7475  += 1..#     retu
-00005f60: 726e 0d0a 0d0a 2320 6465 6620 6954 7570  rn....# def iTup
-00005f70: 6c65 5f6d 656d 6f72 795f 6765 6e28 6375  le_memory_gen(cu
-00005f80: 6d3d 4661 6c73 6529 3a0d 0a23 2020 2020  m=False):..#    
-00005f90: 2069 203d 2030 0d0a 2320 2020 2020 6966   i = 0..#     if
-00005fa0: 2063 756d 3a0d 0a23 2020 2020 2020 2020   cum:..#        
-00005fb0: 2077 6869 6c65 2054 7275 653a 0d0a 2320   while True:..# 
-00005fc0: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
-00005fd0: 6420 6954 7570 6c65 2872 616e 6765 2869  d iTuple(range(i
-00005fe0: 2929 0d0a 2320 2020 2020 2020 2020 2020  ))..#           
-00005ff0: 2020 6920 2b3d 2031 0d0a 2320 2020 2020    i += 1..#     
-00006000: 656c 7365 3a0d 0a23 2020 2020 2020 2020  else:..#        
-00006010: 2077 6869 6c65 2054 7275 653a 0d0a 2320   while True:..# 
-00006020: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
-00006030: 6420 6954 7570 6c65 285b 695d 290d 0a23  d iTuple([i])..#
-00006040: 2020 2020 2020 2020 2020 2020 2069 202b               i +
-00006050: 3d20 310d 0a23 2020 2020 2072 6574 7572  = 1..#     retur
-00006060: 6e0d 0a0d 0a23 2070 7269 6e74 2822 696e  n....# print("in
-00006070: 7422 2c20 6d69 7363 2e70 6572 666d 6f6e  t", misc.perfmon
-00006080: 2e70 726f 6669 6c65 5f6d 656d 6f72 7928  .profile_memory(
-00006090: 0d0a 2320 2020 2020 696e 745f 6d65 6d6f  ..#     int_memo
-000060a0: 7279 5f67 656e 0d0a 2320 2929 0d0a 0d0a  ry_gen..# ))....
-000060b0: 2320 7072 696e 7428 226c 6973 7422 2c20  # print("list", 
-000060c0: 6d69 7363 2e70 6572 666d 6f6e 2e70 726f  misc.perfmon.pro
-000060d0: 6669 6c65 5f6d 656d 6f72 7928 0d0a 2320  file_memory(..# 
-000060e0: 2020 2020 6c69 7374 5f6d 656d 6f72 795f      list_memory_
-000060f0: 6765 6e0d 0a23 2029 290d 0a0d 0a23 2070  gen..# ))....# p
-00006100: 7269 6e74 2822 6954 7570 6c65 222c 206d  rint("iTuple", m
-00006110: 6973 632e 7065 7266 6d6f 6e2e 7072 6f66  isc.perfmon.prof
-00006120: 696c 655f 6d65 6d6f 7279 280d 0a23 2020  ile_memory(..#  
-00006130: 2020 2069 5475 706c 655f 6d65 6d6f 7279     iTuple_memory
-00006140: 5f67 656e 0d0a 2320 2929 0d0a 0d0a 2320  _gen..# ))....# 
-00006150: 7072 696e 7428 226c 6973 7420 6375 6d22  print("list cum"
-00006160: 2c20 6d69 7363 2e70 6572 666d 6f6e 2e70  , misc.perfmon.p
-00006170: 726f 6669 6c65 5f6d 656d 6f72 7928 0d0a  rofile_memory(..
-00006180: 2320 2020 2020 6c69 7374 5f6d 656d 6f72  #     list_memor
-00006190: 795f 6765 6e2c 2063 756d 3d54 7275 652c  y_gen, cum=True,
-000061a0: 0d0a 2320 2929 0d0a 0d0a 2320 7072 696e  ..# ))....# prin
-000061b0: 7428 2269 5475 706c 6520 6375 6d22 2c20  t("iTuple cum", 
-000061c0: 6d69 7363 2e70 6572 666d 6f6e 2e70 726f  misc.perfmon.pro
-000061d0: 6669 6c65 5f6d 656d 6f72 7928 0d0a 2320  file_memory(..# 
-000061e0: 2020 2020 6954 7570 6c65 5f6d 656d 6f72      iTuple_memor
-000061f0: 795f 6765 6e2c 2063 756d 3d54 7275 652c  y_gen, cum=True,
-00006200: 0d0a 2320 2929 0d0a 0d0a 2320 2d2d 2d2d  ..# ))....# ----
-00006210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a23  -----------....#
-00006250: 2073 203d 2053 2831 290d 0a23 2073 5f70   s = S(1)..# s_p
-00006260: 6172 656e 7420 3d20 535f 5061 7265 6e74  arent = S_Parent
-00006270: 2873 290d 0a0d 0a23 2070 7269 6e74 2873  (s)....# print(s
-00006280: 2e63 6c73 2e61 6e6e 6f74 6174 696f 6e73  .cls.annotations
-00006290: 2873 2929 0d0a 0d0a 2320 7072 696e 7428  (s))....# print(
-000062a0: 732e 636c 7329 0d0a 0d0a 2320 7072 696e  s.cls)....# prin
-000062b0: 7428 735f 7061 7265 6e74 2e63 6173 745f  t(s_parent.cast_
-000062c0: 6a73 6f6e 2829 290d 0a0d 0a23 2070 7269  json())....# pri
-000062d0: 6e74 2869 5475 706c 6528 5b73 5f70 6172  nt(iTuple([s_par
-000062e0: 656e 745d 292e 6361 7374 5f6a 736f 6e28  ent]).cast_json(
-000062f0: 2929 0d0a 0d0a 2320 2320 2d2d 2d2d 2d2d  ))....# # ------
-00006300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006330: 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a23 206c  ---------....# l
-00006340: 203d 2069 5475 706c 6528 5b73 5d29 0d0a   = iTuple([s])..
-00006350: 0d0a 2320 7072 696e 7428 6c2e 6578 7465  ..# print(l.exte
-00006360: 6e64 285b 325d 2929 0d0a 0d0a 2320 7072  nd([2]))....# pr
-00006370: 696e 7428 6c2e 6170 7065 6e64 2831 2929  int(l.append(1))
-00006380: 0d0a 0d0a 2320 7072 696e 7428 6c2e 6d61  ....# print(l.ma
-00006390: 7028 7072 696e 7429 290d 0a0d 0a23 2023  p(print))....# #
-000063a0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-000063b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000063c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000063d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000063e0: 0d0a 0d0a 2320 7072 696e 7428 732e 636c  ....# print(s.cl
-000063f0: 7329 0d0a 0d0a 2320 7072 696e 7428 2253  s)....# print("S
-00006400: 686f 756c 6420 6265 2074 7275 653a 222c  hould be true:",
-00006410: 206e 5475 706c 652e 6973 5f69 6e73 7461   nTuple.is_insta
-00006420: 6e63 6528 7329 290d 0a23 2070 7269 6e74  nce(s))..# print
-00006430: 2822 5368 6f75 6c64 2062 6520 6661 6c73  ("Should be fals
-00006440: 653a 222c 206e 5475 706c 652e 6973 5f73  e:", nTuple.is_s
-00006450: 7562 636c 6173 7328 7329 290d 0a0d 0a23  ubclass(s))....#
-00006460: 2070 7269 6e74 2822 5368 6f75 6c64 2062   print("Should b
-00006470: 6520 7472 7565 3a22 2c20 6e54 7570 6c65  e true:", nTuple
-00006480: 2e69 735f 7375 6263 6c61 7373 2853 2929  .is_subclass(S))
-00006490: 0d0a 2320 7072 696e 7428 2253 686f 756c  ..# print("Shoul
-000064a0: 6420 6265 2066 616c 7365 3a22 2c20 6e54  d be false:", nT
-000064b0: 7570 6c65 2e69 735f 696e 7374 616e 6365  uple.is_instance
-000064c0: 2853 2929 0d0a 0d0a 2320 2d2d 2d2d 2d2d  (S))....# ------
-000064d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000064e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000064f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006500: 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a23 204e  ---------....# N
-00006510: 4f54 453a 2069 2063 6f75 646c 2069 6e20  OTE: i coudl in 
-00006520: 7468 656f 7279 2067 656e 6572 6174 6520  theory generate 
-00006530: 7371 6c61 6c63 6865 6d79 2074 6162 6c65  sqlalchemy table
-00006540: 730d 0a0d 0a23 2062 6173 6564 206f 6e20  s....# based on 
-00006550: 7468 6520 7374 7275 6374 2064 6566 696e  the struct defin
-00006560: 6974 696f 6e0d 0a0d 0a23 206a 6f69 6e73  ition....# joins
-00006570: 2070 7265 7375 6d61 626c 7920 6172 6520   presumably are 
-00006580: 7468 656e 206d 616e 7561 6c3f 0d0a 0d0a  then manual?....
-00006590: 2320 7769 7468 2073 7461 6e64 6172 6469  # with standardi
-000065a0: 7365 6420 6567 2e20 7065 7273 6973 7420  sed eg. persist 
-000065b0: 6d65 7468 6f64 7320 6261 7365 6420 6f6e  methods based on
-000065c0: 2075 6e69 7175 6520 6b65 7973 2c20 6574   unique keys, et
-000065d0: 632e 0d0a 0d0a 2320 6275 7420 616e 7920  c.....# but any 
-000065e0: 706f 696e 743f 0d0a 0d0a 2320 6861 6e64  point?....# hand
-000065f0: 6c65 2064 6174 6573 2061 7320 7469 6e79  le dates as tiny
-00006600: 2073 7472 7563 7473 3f0d 0a23 2073 7572   structs?..# sur
-00006610: 656c 7920 7072 6f68 6962 6974 6976 656c  ely prohibitivel
-00006620: 7920 6578 7065 6e73 6976 650d 0a0d 0a23  y expensive....#
-00006630: 2074 7570 6c65 7320 7065 7268 6170 7320   tuples perhaps 
-00006640: 6e6f 743f 2062 7574 2073 7469 6c6c 2061  not? but still a
-00006650: 2062 6974 2c20 616e 6420 616c 6c20 7468   bit, and all th
-00006660: 6520 6461 7465 7469 6d65 206d 6574 686f  e datetime metho
-00006670: 6473 2073 7564 6465 6e6c 7920 776f 756c  ds suddenly woul
-00006680: 646e 2774 2077 6f72 6b2e 0d0a 0d0a 2320  dn't work.....# 
-00006690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000066a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000066b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000066c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d  ---------------.
-000066d0: 0a                                       .
+00005cf0: 0d0a 5f5f 616c 6c5f 5f20 3d20 5b0d 0a20  ..__all__ = [.. 
+00005d00: 2020 2022 6954 7570 6c65 222c 0d0a 2020     "iTuple",..  
+00005d10: 2020 226e 5475 706c 6522 2c0d 0a20 2020    "nTuple",..   
+00005d20: 2022 6644 6963 7422 2c0d 0a20 2020 2022   "fDict",..    "
+00005d30: 4a53 4f4e 4465 636f 6465 7222 2c0d 0a20  JSONDecoder",.. 
+00005d40: 2020 2022 4a53 4f4e 456e 636f 6465 7222     "JSONEncoder"
+00005d50: 2c0d 0a5d 0d0a 0d0a 2320 2d2d 2d2d 2d2d  ,..]....# ------
+00005d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005d90: 2d2d 2d2d 2d2d 2d2d 2d0d 0a              ---------..
```

### Comparing `xtuples-0.0.3/.gitignore` & `xtuples-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.3/LICENSE.txt` & `xtuples-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.3/pyproject.toml` & `xtuples-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.3/PKG-INFO` & `xtuples-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtuples
-Version: 0.0.3
+Version: 0.0.4
 Project-URL: Documentation, https://tomjrwilliams.github.io/xtuples/
 Project-URL: Issues, https://github.com/tomjrwilliams/xtuples/issues
 Project-URL: Source, https://github.com/tomjrwilliams/xtuples
 Author-email: Tom Williams <tomjrw@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

