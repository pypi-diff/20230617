# Comparing `tmp/pocketsearch-0.7.1.tar.gz` & `tmp/pocketsearch-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketsearch-0.7.1.tar", last modified: Mon Jun 12 14:26:23 2023, max compression
+gzip compressed data, was "pocketsearch-0.8.0.tar", last modified: Sat Jun 17 10:05:35 2023, max compression
```

## Comparing `pocketsearch-0.7.1.tar` & `pocketsearch-0.8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:26:23.198541 pocketsearch-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-12 14:26:14.000000 pocketsearch-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-06-12 14:26:23.194541 pocketsearch-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-06-12 14:26:14.000000 pocketsearch-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:26:23.198541 pocketsearch-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-12 14:26:14.000000 pocketsearch-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:26:23.194541 pocketsearch-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:26:23.194541 pocketsearch-0.7.1/src/pocketsearch/
--rw-r--r--   0 runner    (1001) docker     (123)    42408 2023-06-12 14:26:14.000000 pocketsearch-0.7.1/src/pocketsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21934 2023-06-12 14:26:14.000000 pocketsearch-0.7.1/src/pocketsearch/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:26:23.194541 pocketsearch-0.7.1/src/pocketsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-06-12 14:26:23.000000 pocketsearch-0.7.1/src/pocketsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-12 14:26:23.000000 pocketsearch-0.7.1/src/pocketsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:26:23.000000 pocketsearch-0.7.1/src/pocketsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 14:26:23.000000 pocketsearch-0.7.1/src/pocketsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:05:35.526325 pocketsearch-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-17 10:05:26.000000 pocketsearch-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14923 2023-06-17 10:05:35.526325 pocketsearch-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13864 2023-06-17 10:05:26.000000 pocketsearch-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 10:05:35.526325 pocketsearch-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-17 10:05:26.000000 pocketsearch-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:05:35.522325 pocketsearch-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:05:35.522325 pocketsearch-0.8.0/src/pocketsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)    46516 2023-06-17 10:05:26.000000 pocketsearch-0.8.0/src/pocketsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24733 2023-06-17 10:05:26.000000 pocketsearch-0.8.0/src/pocketsearch/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:05:35.526325 pocketsearch-0.8.0/src/pocketsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14923 2023-06-17 10:05:35.000000 pocketsearch-0.8.0/src/pocketsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-17 10:05:35.000000 pocketsearch-0.8.0/src/pocketsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 10:05:35.000000 pocketsearch-0.8.0/src/pocketsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 10:05:35.000000 pocketsearch-0.8.0/src/pocketsearch.egg-info/top_level.txt
```

### Comparing `pocketsearch-0.7.1/LICENSE` & `pocketsearch-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.7.1/PKG-INFO` & `pocketsearch-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.7.1
+Version: 0.8.0
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Project-URL: Change log, https://github.com/kaykay-dv/pocketsearch/blob/main/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
@@ -148,14 +148,51 @@
 # Order by text in ascending order
 pocket_search.search(text__allow_boolean="hello OR world").order_by("text")
 # This is equivalent to the previous call:
 pocket_search.search(text__allow_boolean="hello OR world").order_by("+text")
 # Order by text in descending order
 pocket_search.search(text__allow_boolean="hello OR world").order_by("-text")
 ```
+
+## Highlighting and extracting snippets from results
+
+FTS5 provides 2 functions to highlight tokens found in text and extracting snippets from a text. 
+There are 2 methods to support this in pocketsearch:
+
+```Python
+pocket_search.search(text="hello").highlight("text")[0].text
+*Hello* World !
+```
+
+The keyword arguments marker_start and marker_end allow you to control how highlighting is done:
+
+```Python
+pocket_search.search(text="hello").highlight("text",marker_start="[",marker_end="]")[0].text
+[Hello] World !
+```
+
+The positional arguments of the highlight method represent the fields you want to hightlight. 
+
+If you have very long text, you might want to only show a snippet with all terms found in your +
+search results. This can be done with the snippet method. Assuming we have the article 
+on inverted indices (https://en.wikipedia.org/wiki/Inverted_index) in our database we can extract snippets like this:
+
+```Python
+pocket_search.search(text="inverted file").snippet("text",snippet_length=16)[0].text
+'In computer science, an *inverted* index (also referred to as a postings list, postings *file*, or...'
+```
+
+Similar to the highlight method, the snippet method highlights tokens found. snippet_length defines 
+the maximum number of tokens that should be contained in the snippet. It must be greater than 0 and lesser 
+than 64. You can change the markers by providing text_before and text_after arguments:
+
+```Python
+pocket_search.search(text="inverted file").snippet("text",snippet_length=16,text_before="<",text_after=">")[0].text
+```
+
 # Schemas
 
 A search index may have an arbitrary list of fields that can be searched. Schemas 
 are defined through Schema classes:
 
 ```Python
 from pocketsearch import Schema, PocketSearch
```

### Comparing `pocketsearch-0.7.1/README.md` & `pocketsearch-0.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -124,14 +124,51 @@
 # Order by text in ascending order
 pocket_search.search(text__allow_boolean="hello OR world").order_by("text")
 # This is equivalent to the previous call:
 pocket_search.search(text__allow_boolean="hello OR world").order_by("+text")
 # Order by text in descending order
 pocket_search.search(text__allow_boolean="hello OR world").order_by("-text")
 ```
+
+## Highlighting and extracting snippets from results
+
+FTS5 provides 2 functions to highlight tokens found in text and extracting snippets from a text. 
+There are 2 methods to support this in pocketsearch:
+
+```Python
+pocket_search.search(text="hello").highlight("text")[0].text
+*Hello* World !
+```
+
+The keyword arguments marker_start and marker_end allow you to control how highlighting is done:
+
+```Python
+pocket_search.search(text="hello").highlight("text",marker_start="[",marker_end="]")[0].text
+[Hello] World !
+```
+
+The positional arguments of the highlight method represent the fields you want to hightlight. 
+
+If you have very long text, you might want to only show a snippet with all terms found in your +
+search results. This can be done with the snippet method. Assuming we have the article 
+on inverted indices (https://en.wikipedia.org/wiki/Inverted_index) in our database we can extract snippets like this:
+
+```Python
+pocket_search.search(text="inverted file").snippet("text",snippet_length=16)[0].text
+'In computer science, an *inverted* index (also referred to as a postings list, postings *file*, or...'
+```
+
+Similar to the highlight method, the snippet method highlights tokens found. snippet_length defines 
+the maximum number of tokens that should be contained in the snippet. It must be greater than 0 and lesser 
+than 64. You can change the markers by providing text_before and text_after arguments:
+
+```Python
+pocket_search.search(text="inverted file").snippet("text",snippet_length=16,text_before="<",text_after=">")[0].text
+```
+
 # Schemas
 
 A search index may have an arbitrary list of fields that can be searched. Schemas 
 are defined through Schema classes:
 
 ```Python
 from pocketsearch import Schema, PocketSearch
```

### Comparing `pocketsearch-0.7.1/setup.py` & `pocketsearch-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pocketsearch",
-    version = "0.7.1",
+    version = "0.8.0",
     author = "kaykay-dv",
     author_email = "kaykay2306@gmail.com",
     description = "A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/kaykay-dv/pocketsearch/",
     project_urls = {
```

### Comparing `pocketsearch-0.7.1/src/pocketsearch/__init__.py` & `pocketsearch-0.8.0/src/pocketsearch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,17 +247,19 @@
         Thrown, if the schema cannot be generated.
         '''
 
     def __init__(self, name):
         self._meta = self.Meta()
         self.name = name
         self.fields = {}
+        self.field_index = {} # required by some SQL functions, e.g. highlight
         self.fields_with_default = {}
         self.reverse_lookup = {}
         self.id_field = None
+        field_index=0
         for elem in dir(self):
             obj = getattr(self, elem)
             if isinstance(obj, Field):
                 if elem.startswith("_") or "__" in elem:
                     raise self.SchemaError(
                         "Cannot use '%s' as field name. Field name may not start with an underscore and may not contain double underscores." %
                         elem)
@@ -267,14 +269,17 @@
                 self.fields[elem].schema = self
                 self.fields[elem].name = elem
                 self.reverse_lookup[obj] = elem
                 if obj.is_id_field:
                     if self.id_field is not None:
                         raise self.SchemaError("You can only provide one IDField per schema. The current IDField is: %s" % self.id_field)
                     self.id_field = obj.name
+                if obj.fts_enabled():
+                    self.field_index[obj.name]=field_index
+                    field_index+=1
 
         for field in self:
             if field.default is not None:
                 self.fields_with_default[field.name] = field
 
     def get_field(self, field_name, raise_exception=False):
         '''
@@ -351,33 +356,75 @@
     def to_sql(self):
         '''
         This class must be implemented by any class subclassing SQLQueryComponent.
         It should return a string containing valid SQL.
         '''
         raise NotImplementedError()
 
+class Function:
+    '''
+    SQL function applied to fields in the select part 
+    of the query
+    '''
+
+class Highlight(Function):
+    '''
+    Highlight SQL function
+    '''
+
+    def __init__(self,marker_start,marker_end):
+        self.marker_start = marker_start
+        self.marker_end = marker_end
+
+    def to_sql(self,field):
+        return "highlight({table}_fts, {index}, '{m_start}', '{m_end}') as {field}".format(field=field.name,
+                                                                                     table=field.schema.name,
+                                                                                     index=field.schema.field_index[field.name],
+                                                                                     m_start=self.marker_start,
+                                                                                     m_end=self.marker_end)
+
+class Snippet(Function):
+    '''
+    Snippet SQL function
+    '''
+
+    def __init__(self,text_before,text_after,snippet_length=16):
+        self.text_before = text_before
+        self.text_after = text_after
+        self.snippet_length=snippet_length
+
+    def to_sql(self,field):
+        return "snippet({table}_fts, {index}, '{t_before}', '{t_after}','...',{l}) as {field}".format(field=field.name,
+                                                                                     table=field.schema.name,
+                                                                                     index=field.schema.field_index[field.name],
+                                                                                     t_before=self.text_before,
+                                                                                     l=self.snippet_length,
+                                                                                     t_after=self.text_after)
 
 class Select(SQLQueryComponent):
     '''
     A single field selected in the query.
     '''
 
-    def __init__(self, field, sql_query):
+    def __init__(self, field, sql_query,function=None):
         super().__init__(sql_query)
         self.field = field
+        self.function = function
 
     def to_sql(self):
         if type(self.field) is str:
             return self.field
         else:
             if isinstance(self.field, Date):
                 return "{full_name} as \"{name} [date]\"".format(full_name=self.field.get_full_qualified_name(), name=self.field.name)
             elif isinstance(self.field, Datetime):
                 return "{full_name} as \"{name} [timestamp]\"".format(full_name=self.field.get_full_qualified_name(), name=self.field.name)
-        return self.field.get_full_qualified_name()
+        if self.function is None:
+            return self.field.get_full_qualified_name()
+        return self.function.to_sql(self.field)
 
 
 class Count(SQLQueryComponent):
     '''
     Count statement in the select part
     '''
 
@@ -630,14 +677,30 @@
         If clear is set to True, any items that have been added
         prior will be cleared.
         '''
         if clear:
             self.v_select.clear()
         self.v_select.append(Select(field=field, sql_query=self))
 
+    def highlight(self,field,marker_start,marker_end):
+        '''
+        Marks given field for highlightening results
+        '''
+        for select in self.v_select:
+            if select.field.name == field.name:
+                select.function = Highlight(marker_start=marker_start,marker_end=marker_end)
+
+    def snippet(self,field,text_before,text_after,snippet_length=16):
+        '''
+        Marks given field for extracting snippets
+        '''
+        for select in self.v_select:
+            if select.field.name == field.name:
+                select.function = Snippet(text_before=text_before,text_after=text_after,snippet_length=snippet_length)        
+
     def table(self, table_name, clear=False):
         '''
         Adds a reference to the from clause in the SQL statement.
         If clear is set to True, any items that have been added
         prior will be cleared.
         '''
         if clear:
@@ -736,15 +799,15 @@
         self.sql_query = SQLQuery(search_instance=search_instance)
         self.unions = []
         for field in self.search_instance.schema.get_fields():
             self.sql_query.select(field=field)
         for argument in arguments.values():
             for lookup in argument.lookups:
                 self.sql_query.where(field=argument.field, lookup=lookup)
-        self.sql_query.select("rank")
+        #self.sql_query.select("rank")
         self.sql_query.table(table_name=self.search_instance.schema.name)
         self.sql_query.table(table_name="%s_fts" % self.search_instance.schema.name)
         self.sql_query.join(self.sql_query.v_from_tables[0], self.sql_query.v_from_tables[1], "id", "rowid")
         self.sql_query.order_by("+rank")
         self.sql_query.limit_and_offset(limit=10, offset=0)
         #self._defaults_set = True
         self._default_order_by_set = True
@@ -820,14 +883,38 @@
         self._default_values_set = False
         for a in args:
             field = self.search_instance.schema.get_field(a, raise_exception=True)
             self.sql_query.select(field,clear=self._default_values_set)
             self._default_values_set = False
         return self
 
+    def highlight(self,*args,marker_start="*",marker_end="*"):
+        '''
+        Marks given field for highlight
+        '''
+        for a in args:
+            field_obj = self.search_instance.schema.get_field(a, raise_exception=True)
+            if not(field_obj.fts_enabled()):
+                raise self.QueryError("highlight can only be applied to Text fields with index set to True.")
+            self.sql_query.highlight(field_obj,marker_start=marker_start,marker_end=marker_end)
+        return self
+
+    def snippet(self,*args,text_before="*",text_after="*",snippet_length=16):
+        '''
+        Marks given field for snippet
+        '''
+        if snippet_length <=0 or snippet_length >=64:
+            raise self.QueryError("snippet_length must be greater than 0 and lesser than 64.")
+        for a in args:
+            field_obj = self.search_instance.schema.get_field(a, raise_exception=True)
+            if not(field_obj.fts_enabled()):
+                raise self.QueryError("snippet can only be applied to Text fields with index set to True.")
+            self.sql_query.snippet(field_obj,text_before=text_before,text_after=text_after,snippet_length=snippet_length)
+        return self
+
     def _build_results(self, results):
         documents = SearchResult()
         for result in results:
             document = Document(result.keys())
             for field in result.keys():
                 setattr(document, field, result[field])
             documents = documents + document
```

### Comparing `pocketsearch-0.7.1/src/pocketsearch/tests.py` & `pocketsearch-0.8.0/src/pocketsearch/tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,14 +98,54 @@
             "England is in Europe.",
             "Paris is the captial of france.",
         ]
         self.pocket_search = PocketSearch(index_name="text_data",writeable=True)
         for elem in self.data:
             self.pocket_search.insert(text=elem)
 
+class SQLFunctionTests(BaseTest):
+
+    def test_highlight(self):
+        self.assertEqual("*fox*" in self.pocket_search.search(text="fox").highlight("text")[0].text,True)
+
+    def test_highlight_alternative_marker(self):
+        self.assertEqual("<b>fox</b>" in self.pocket_search.search(text="fox").highlight("text",marker_start="<b>",marker_end="</b>")[0].text,True)
+
+    def test_snippet(self):
+        text = '''
+        In computer science, an inverted index (also referred to as a postings list, postings file, or inverted file) is a 
+        database index storing a mapping from content, such as words or numbers, to its locations in a table, or in a 
+        document or a set of documents (named in contrast to a forward index, which maps from documents to content).
+        The purpose of an inverted index is to allow fast full-text searches, at a cost of increased processing when a 
+        document is added to the database.[2] The inverted file may be the database file itself, rather than its index. 
+        It is the most popular data structure used in document retrieval systems,[3] used on a large scale for example in search engines.
+        '''
+        self.pocket_search.insert(text=text)
+        result = self.pocket_search.search(text="forward index").snippet("text")[0].text
+        eq = self.assertEqual
+        eq("*forward*" in result,True)
+        eq("*index*" in result,True)
+        # Test alternative before/after text
+        result = self.pocket_search.search(text="forward index").snippet("text",text_before="<b>",text_after="</b>")[0].text
+        eq("<b>forward</b>" in result , True)
+        eq("<b>index</b>" in result , True)
+
+    def test_snippet_length_too_big(self):
+        '''
+        Snippets may not exceed 64 tokens
+        '''
+        with self.assertRaises(Query.QueryError):
+            self.pocket_search.search(text="forward index").snippet("text",snippet_length=128)
+
+    def test_snippet_length_too_small(self):
+        '''
+        Snippets must have at least 1 token
+        '''        
+        with self.assertRaises(Query.QueryError):
+            self.pocket_search.search(text="forward index").snippet("text",snippet_length=0)        
 
 class OperatorSearch(BaseTest):
     '''
     Tests covering the usage of boolean operators and prefix search
     '''
 
     def test_search_len_func(self):
@@ -395,22 +435,18 @@
         self.assertEqual(self.pocket_search.search(text="A", title="A", category="A")[0].title, "A")
         # As all fields are AND'ed - this query will show no results
         self.assertEqual(self.pocket_search.search(text="C", title="C", category="C").count(), 0)
         # Now order the results by title, this should bring "A" first:
         #results = self.pocket_search.search(text="C",title="C",category="C").order_by("title")
         # self.assertEqual(results[0].title,"A")
 
-    def test_rank_multiple_field_or_query(self):
-        pass
-
 
 class StemmingTests(unittest.TestCase):
 
     def setUp(self):
-        # Data taken from Wikipedia (also using some special characters)
         self.data = [
             "Tests need to be performed on a regular basis.",
             "Die Anforderungen müssen genau definiert sein."
         ]
         self.pocket_search = PocketSearch(writeable=True)
         for content in self.data:
             self.pocket_search.insert(text=content)
@@ -471,14 +507,30 @@
         self.pocket_search.insert(f1=32,
                                   f2='text',
                                   f3='abc'.encode("utf-8"),
                                   f4=2/3,
                                   f5=datetime.datetime.now(),
                                   f6=datetime.date.today())
 
+    def test_apply_highlight_to_non_fts_field(self):
+        '''
+        When the highlight function is applied to non-FTS
+        field, a query error should be raised:
+        '''
+        with self.assertRaises(Query.QueryError):
+            self.pocket_search.search(f1=32).highlight("f1")
+        with self.assertRaises(Query.QueryError):
+            self.pocket_search.search(f1=32).highlight("f3")
+        with self.assertRaises(Query.QueryError):
+            self.pocket_search.search(f1=32).highlight("f4")
+        with self.assertRaises(Query.QueryError):
+            self.pocket_search.search(f1=32).highlight("f5")
+        with self.assertRaises(Query.QueryError):
+            self.pocket_search.search(f1=32).highlight("f6")
+
     def test_create(self):
         result = self.pocket_search.search(id=1)
         self.assertEqual(type(result[0].f6), datetime.date)
         # search for dates
 
     def test_search_dates_equals(self):
         year = datetime.date.today().year
@@ -510,14 +562,15 @@
             ("Apple", 3, "Fruit"),
             ("Orange", 4, "Fruit"),
             ("Peach", 5, "Fruit"),
             ("Banana", 6, "Fruit"),
         ]:
             self.pocket_search.insert(description=product, price=price, category=category)
 
+
     def test_filter_numeric_values_equal(self):
         self.assertEqual(self.pocket_search.search(price=3).count(), 1)
 
     def test_filter_numeric_values_greater_than(self):
         self.assertEqual(self.pocket_search.search(price__gt=3).count(), 3)
 
     def test_filter_numeric_values_greater_than_equal(self):
```

### Comparing `pocketsearch-0.7.1/src/pocketsearch.egg-info/PKG-INFO` & `pocketsearch-0.8.0/src/pocketsearch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.7.1
+Version: 0.8.0
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Project-URL: Change log, https://github.com/kaykay-dv/pocketsearch/blob/main/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
@@ -148,14 +148,51 @@
 # Order by text in ascending order
 pocket_search.search(text__allow_boolean="hello OR world").order_by("text")
 # This is equivalent to the previous call:
 pocket_search.search(text__allow_boolean="hello OR world").order_by("+text")
 # Order by text in descending order
 pocket_search.search(text__allow_boolean="hello OR world").order_by("-text")
 ```
+
+## Highlighting and extracting snippets from results
+
+FTS5 provides 2 functions to highlight tokens found in text and extracting snippets from a text. 
+There are 2 methods to support this in pocketsearch:
+
+```Python
+pocket_search.search(text="hello").highlight("text")[0].text
+*Hello* World !
+```
+
+The keyword arguments marker_start and marker_end allow you to control how highlighting is done:
+
+```Python
+pocket_search.search(text="hello").highlight("text",marker_start="[",marker_end="]")[0].text
+[Hello] World !
+```
+
+The positional arguments of the highlight method represent the fields you want to hightlight. 
+
+If you have very long text, you might want to only show a snippet with all terms found in your +
+search results. This can be done with the snippet method. Assuming we have the article 
+on inverted indices (https://en.wikipedia.org/wiki/Inverted_index) in our database we can extract snippets like this:
+
+```Python
+pocket_search.search(text="inverted file").snippet("text",snippet_length=16)[0].text
+'In computer science, an *inverted* index (also referred to as a postings list, postings *file*, or...'
+```
+
+Similar to the highlight method, the snippet method highlights tokens found. snippet_length defines 
+the maximum number of tokens that should be contained in the snippet. It must be greater than 0 and lesser 
+than 64. You can change the markers by providing text_before and text_after arguments:
+
+```Python
+pocket_search.search(text="inverted file").snippet("text",snippet_length=16,text_before="<",text_after=">")[0].text
+```
+
 # Schemas
 
 A search index may have an arbitrary list of fields that can be searched. Schemas 
 are defined through Schema classes:
 
 ```Python
 from pocketsearch import Schema, PocketSearch
```

