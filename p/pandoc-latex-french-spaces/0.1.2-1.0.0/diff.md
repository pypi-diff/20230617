# Comparing `tmp/pandoc-latex-french-spaces-0.1.2.tar.gz` & `tmp/pandoc_latex_french_spaces-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc-latex-french-spaces-0.1.2.tar", last modified: Tue Feb 23 16:30:19 2021, max compression
+gzip compressed data, was "pandoc_latex_french_spaces-1.0.0.tar", max compression
```

## Comparing `pandoc-latex-french-spaces-0.1.2.tar` & `pandoc_latex_french_spaces-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,5 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 16:30:19.477855 pandoc-latex-french-spaces-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2021-02-23 16:30:11.000000 pandoc-latex-french-spaces-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-02-23 16:30:11.000000 pandoc-latex-french-spaces-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4521 2021-02-23 16:30:19.477855 pandoc-latex-french-spaces-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2836 2021-02-23 16:30:11.000000 pandoc-latex-french-spaces-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 16:30:19.477855 pandoc-latex-french-spaces-0.1.2/pandoc_latex_french_spaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4521 2021-02-23 16:30:19.000000 pandoc-latex-french-spaces-0.1.2/pandoc_latex_french_spaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      380 2021-02-23 16:30:19.000000 pandoc-latex-french-spaces-0.1.2/pandoc_latex_french_spaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-23 16:30:19.000000 pandoc-latex-french-spaces-0.1.2/pandoc_latex_french_spaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-02-23 16:30:19.000000 pandoc-latex-french-spaces-0.1.2/pandoc_latex_french_spaces.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-02-23 16:30:19.000000 pandoc-latex-french-spaces-0.1.2/pandoc_latex_french_spaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-02-23 16:30:19.000000 pandoc-latex-french-spaces-0.1.2/pandoc_latex_french_spaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      929 2021-02-23 16:30:11.000000 pandoc-latex-french-spaces-0.1.2/pandoc_latex_french_spaces.py
--rw-r--r--   0 runner    (1001) docker     (121)      151 2021-02-23 16:30:19.477855 pandoc-latex-french-spaces-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3845 2021-02-23 16:30:11.000000 pandoc-latex-french-spaces-0.1.2/setup.py
+-rw-r--r--   0        0        0     1521 2023-06-17 15:21:00.730985 pandoc_latex_french_spaces-1.0.0/LICENSE
+-rw-r--r--   0        0        0     9097 2023-06-17 15:21:00.730985 pandoc_latex_french_spaces-1.0.0/README.md
+-rw-r--r--   0        0        0     1168 2023-06-17 15:21:00.730985 pandoc_latex_french_spaces-1.0.0/pandoc_latex_french_spaces.py
+-rw-r--r--   0        0        0     2954 2023-06-17 15:21:00.730985 pandoc_latex_french_spaces-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10218 1970-01-01 00:00:00.000000 pandoc_latex_french_spaces-1.0.0/PKG-INFO
```

### Comparing `pandoc-latex-french-spaces-0.1.2/LICENSE` & `pandoc_latex_french_spaces-1.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2018-2021, Christophe Demko
+Copyright (c) 2018-2023, Christophe Demko
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `pandoc-latex-french-spaces-0.1.2/pandoc_latex_french_spaces.py` & `pandoc_latex_french_spaces-1.0.0/pandoc_latex_french_spaces.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,52 @@
 #!/usr/bin/env python3
 
-
 """
-Pandoc filter for converting spaces to non-breakable spaces in LaTeX
-for french ponctuation
+Pandoc filter for converting spaces to non-breakable spaces.
+
+This filter is for use in LaTeX for french ponctuation.
 """
 
-from panflute import Space, Str, RawInline, run_filter  # type: ignore
+from panflute import RawInline, Space, Str, run_filter  # type: ignore
 
 
 def spaces(elem, doc):
     """
     Add LaTeX spaces when needed.
+
+    Arguments
+    ---------
+    elem
+        A tree element
+    doc
+        The pandoc document
+
+    Returns
+    -------
+        A RawInLine or None.
     """
     # Is it in the right format and is it a Space?
-    if doc.format in ["latex", "beamer"] and isinstance(elem, Space):
-        if isinstance(elem.prev, Str) and elem.prev.text in ["«", "“", "‹"]:
+    if doc.format in ("latex", "beamer") and isinstance(elem, Space):
+        if isinstance(elem.prev, Str) and elem.prev.text in ("«", "“", "‹"):
             return RawInline("\\thinspace{}", "tex")
         if isinstance(elem.next, Str):
             if elem.next.text == ":":
                 return RawInline("~", "tex")
-            if elem.next.text in [";", "?", "!", "»", "”", "›"]:
+            if elem.next.text in (";", "?", "!", "»", "”", "›"):
                 return RawInline("\\thinspace{}", "tex")
     return None
 
 
 def main(doc=None):
     """
-    main function.
+    Process conversion.
+
+    Arguments
+    ---------
+    doc
+        The pandoc document
     """
-    return run_filter(spaces, doc=doc)
+    run_filter(spaces, doc=doc)
 
 
 if __name__ == "__main__":
     main()
```

