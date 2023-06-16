# Comparing `tmp/parsetypes-0.3.tar.gz` & `tmp/parsetypes-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsetypes-0.3.tar", last modified: Tue May 30 01:28:56 2023, max compression
+gzip compressed data, was "parsetypes-0.3.1.tar", last modified: Fri Jun 16 23:41:07 2023, max compression
```

## Comparing `parsetypes-0.3.tar` & `parsetypes-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 01:28:56.021063 parsetypes-0.3/
--rw-rw-rw-   0        0        0     1314 2023-05-30 01:28:26.000000 parsetypes-0.3/CHANGELOG.md
--rw-rw-rw-   0        0        0       22 2023-05-28 02:54:36.000000 parsetypes-0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     7200 2023-05-30 01:28:56.021063 parsetypes-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4183 2023-05-28 23:00:42.000000 parsetypes-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 01:28:56.006545 parsetypes-0.3/docs/
-drwxrwxrwx   0        0        0        0 2023-05-30 01:28:56.012545 parsetypes-0.3/docs/html/
--rw-rw-rw-   0        0        0     1729 2023-05-30 01:28:47.000000 parsetypes-0.3/docs/html/favicon.png
--rw-rw-rw-   0        0        0      141 2023-05-30 01:28:46.000000 parsetypes-0.3/docs/html/index.html
--rw-rw-rw-   0        0        0   597050 2023-05-30 01:28:46.000000 parsetypes-0.3/docs/html/parsetypes.html
--rw-rw-rw-   0        0        0   226407 2023-05-30 01:28:47.000000 parsetypes-0.3/docs/html/search.js
--rw-rw-rw-   0        0        0     2297 2023-05-28 04:48:55.000000 parsetypes-0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 01:28:56.021063 parsetypes-0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-30 01:28:56.006545 parsetypes-0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 01:28:56.016062 parsetypes-0.3/src/parsetypes/
--rw-rw-rw-   0        0        0      631 2023-05-30 01:28:26.000000 parsetypes-0.3/src/parsetypes/__init__.py
--rw-rw-rw-   0        0        0     1299 2023-05-30 01:28:26.000000 parsetypes-0.3/src/parsetypes/_common.py
--rw-rw-rw-   0        0        0      348 2023-05-28 04:48:55.000000 parsetypes-0.3/src/parsetypes/_compat.py
--rw-rw-rw-   0        0        0    44045 2023-05-30 01:28:26.000000 parsetypes-0.3/src/parsetypes/_parser.py
--rw-rw-rw-   0        0        0     5201 2023-05-30 01:28:26.000000 parsetypes-0.3/src/parsetypes/_reduce_types.py
-drwxrwxrwx   0        0        0        0 2023-05-30 01:28:56.019063 parsetypes-0.3/src/parsetypes.egg-info/
--rw-rw-rw-   0        0        0     7200 2023-05-30 01:28:55.000000 parsetypes-0.3/src/parsetypes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-05-30 01:28:56.000000 parsetypes-0.3/src/parsetypes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 01:28:55.000000 parsetypes-0.3/src/parsetypes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      296 2023-05-30 01:28:55.000000 parsetypes-0.3/src/parsetypes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-30 01:28:55.000000 parsetypes-0.3/src/parsetypes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-30 01:28:56.020063 parsetypes-0.3/tests/
--rw-rw-rw-   0        0        0    70189 2023-05-30 01:28:26.000000 parsetypes-0.3/tests/test_parser.py
--rw-rw-rw-   0        0        0     8837 2023-05-28 04:48:55.000000 parsetypes-0.3/tests/test_reduce_types.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:41:07.264475 parsetypes-0.3.1/
+-rw-rw-rw-   0        0        0     1548 2023-06-16 23:39:36.000000 parsetypes-0.3.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0       22 2023-05-28 02:54:36.000000 parsetypes-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7436 2023-06-16 23:41:07.264475 parsetypes-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4183 2023-05-28 23:00:42.000000 parsetypes-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 23:41:07.249449 parsetypes-0.3.1/docs/
+drwxrwxrwx   0        0        0        0 2023-06-16 23:41:07.257476 parsetypes-0.3.1/docs/html/
+-rw-rw-rw-   0        0        0     1729 2023-06-16 23:40:58.000000 parsetypes-0.3.1/docs/html/favicon.png
+-rw-rw-rw-   0        0        0      141 2023-06-16 23:40:57.000000 parsetypes-0.3.1/docs/html/index.html
+-rw-rw-rw-   0        0        0   593363 2023-06-16 23:40:57.000000 parsetypes-0.3.1/docs/html/parsetypes.html
+-rw-rw-rw-   0        0        0   228557 2023-06-16 23:40:58.000000 parsetypes-0.3.1/docs/html/search.js
+-rw-rw-rw-   0        0        0     2297 2023-05-28 04:48:55.000000 parsetypes-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 23:41:07.264475 parsetypes-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 23:41:07.250452 parsetypes-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 23:41:07.260476 parsetypes-0.3.1/src/parsetypes/
+-rw-rw-rw-   0        0        0      633 2023-06-16 23:40:42.000000 parsetypes-0.3.1/src/parsetypes/__init__.py
+-rw-rw-rw-   0        0        0     1299 2023-05-30 01:37:10.000000 parsetypes-0.3.1/src/parsetypes/_common.py
+-rw-rw-rw-   0        0        0      348 2023-05-28 04:48:55.000000 parsetypes-0.3.1/src/parsetypes/_compat.py
+-rw-rw-rw-   0        0        0    44629 2023-06-16 23:29:21.000000 parsetypes-0.3.1/src/parsetypes/_parser.py
+-rw-rw-rw-   0        0        0     5201 2023-05-30 01:28:26.000000 parsetypes-0.3.1/src/parsetypes/_reduce_types.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:41:07.262476 parsetypes-0.3.1/src/parsetypes.egg-info/
+-rw-rw-rw-   0        0        0     7436 2023-06-16 23:41:07.000000 parsetypes-0.3.1/src/parsetypes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-06-16 23:41:07.000000 parsetypes-0.3.1/src/parsetypes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 23:41:07.000000 parsetypes-0.3.1/src/parsetypes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      296 2023-06-16 23:41:07.000000 parsetypes-0.3.1/src/parsetypes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-16 23:41:07.000000 parsetypes-0.3.1/src/parsetypes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 23:41:07.263476 parsetypes-0.3.1/tests/
+-rw-rw-rw-   0        0        0    71380 2023-06-16 23:35:10.000000 parsetypes-0.3.1/tests/test_parser.py
+-rw-rw-rw-   0        0        0     8837 2023-05-28 04:48:55.000000 parsetypes-0.3.1/tests/test_reduce_types.py
```

### Comparing `parsetypes-0.3/CHANGELOG.md` & `parsetypes-0.3.1/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>parsetypes ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>parsetypes ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
+### 0.3.1
+
+- Added the arguments `allow_negative` and `allow_sign` (both `True` by default) to <code><var>parser</var>.parse_int()</code>, for parity with <code><var>parser</var>.is_int()</code> which already had these arguments
+
 ### 0.3
 
 - Made the previously public but undocumented instance variables of TypeParser that corresponded to the constructor arguments private instead
 - Added public properties to TypeParser for accessing or modifying the same settings in a controlled manner
 
 ### 0.2.6
```

### Comparing `parsetypes-0.3/PKG-INFO` & `parsetypes-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsetypes
-Version: 0.3
+Version: 0.3.1
 Summary: Parse serialised data to recover their original underlying types
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/parsetypes
 Project-URL: Documentation, https://parsetypes.gnayihs.uy/
 Project-URL: Issues, https://github.com/yushiyangk/parsetypes/issues
 Keywords: python,str,string,types,conversion
@@ -158,14 +158,18 @@
 
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>parsetypes ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>parsetypes ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
+### 0.3.1
+
+- Added the arguments `allow_negative` and `allow_sign` (both `True` by default) to <code><var>parser</var>.parse_int()</code>, for parity with <code><var>parser</var>.is_int()</code> which already had these arguments
+
 ### 0.3
 
 - Made the previously public but undocumented instance variables of TypeParser that corresponded to the constructor arguments private instead
 - Added public properties to TypeParser for accessing or modifying the same settings in a controlled manner
 
 ### 0.2.6
```

### Comparing `parsetypes-0.3/README.md` & `parsetypes-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `parsetypes-0.3/docs/html/favicon.png` & `parsetypes-0.3.1/docs/html/favicon.png`

 * *Files identical despite different names*

### Comparing `parsetypes-0.3/docs/html/parsetypes.html` & `parsetypes-0.3.1/docs/html/parsetypes.html`

 * *Files 0% similar despite different names*

```diff
@@ -20,78 +20,23 @@
 
 				const id = hrefParts[1];
 				const target = document.getElementById(id);
 				if (target?.contains(a)) {
 					a.removeAttribute('href');
 				}
 			});
-
-			// Rearrange function signatures in summary to prepare for elision
-			document.querySelectorAll('.pdoc .summary dt').forEach((heading) => {
-				const returnType = heading.querySelector('.return-annotation');
-				const signature = heading.querySelector('.signature');
-				if (returnType !== null) {
-					heading.appendChild(returnType);
-				} else {
-					// ( <- workaround for bad parenthesis matching in text editor
-					if (signature !== null && signature.childNodes !== null && signature.lastChild?.nodeType === Node.TEXT_NODE && signature.lastChild?.textContent === ")") {
-						heading.appendChild(signature.lastChild);
-					}
-				}
-				if (signature !== null && signature.childNodes !== null && signature.firstChild?.textContent === '(') {
-					const name = heading.querySelector('.name');
-					heading.insertBefore(signature.firstChild, signature);
-				}
-				// ) <- workaround for bad parenthesis matching in text editor
-			});
-			// Elision of function signatures except return type
-			document.querySelectorAll('.pdoc .summary').forEach((summary) => {
-				// Instead of observing resize of every single dt, just observe the parent .summary instead since they have the same width
-				const summaryMarginLeft = parseInt(window.getComputedStyle(summary).marginLeft);
-				console.log(summaryMarginLeft);
-				const headings = summary.querySelectorAll('dt');
-				const headingsArray = [...headings];
-      			const names = headingsArray.map((h) => h.querySelector('.name'));
-      			const signatures = headingsArray.map((h) => h.querySelector('.signature'));
-				const returnTypes = headingsArray.map((h) => h.querySelector('.return-annotation'));
-				const summaryResizeObserver = new ResizeObserver((entries) => {
-					for (const entry of entries) {
-						if (entry.contentBoxSize !== null && entry.contentBoxSize[0] !== null) {
-							const containerWidth = entry.contentBoxSize[0].inlineSize;
-							headings.forEach((heading, i) => {
-								if (names[i] !== null && signatures[i] !== null) {
-									const nameWidth = names[i].scrollWidth;
-									const signatureWidth = signatures[i].scrollWidth;
-									let returnTypeWidth = 0;
-									if (returnTypes[i] !== null) {
-										returnTypeWidth = returnTypes[i].scrollWidth;
-									}
-									// Need to add padding, border, margin widths too in principle, but they are 0
-									if (nameWidth + signatureWidth + returnTypeWidth + summaryMarginLeft > containerWidth) {
-										signatures[i].style.width = (containerWidth - nameWidth - returnTypeWidth - summaryMarginLeft) + 'px';
-									} else if (signatures[i].style.width !== '') {
-										signatures[i].style.removeProperty('width');
-									}
-								}
-							});
-						}
-					}
-				});
-				summaryResizeObserver.observe(summary);
-			});
-
 		});
 	</script>
 
     <style>/*! * Bootstrap Reboot v5.0.0 (https://getbootstrap.com/) * Copyright 2011-2021 The Bootstrap Authors * Copyright 2011-2021 Twitter, Inc. * Licensed under MIT (https://github.com/twbs/bootstrap/blob/main/LICENSE) * Forked from Normalize.css, licensed MIT (https://github.com/necolas/normalize.css/blob/master/LICENSE.md) */*,::after,::before{box-sizing:border-box}@media (prefers-reduced-motion:no-preference){:root{scroll-behavior:smooth}}body{margin:0;font-family:system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial,"Noto Sans","Liberation Sans",sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";font-size:1rem;font-weight:400;line-height:1.5;color:#212529;background-color:#fff;-webkit-text-size-adjust:100%;-webkit-tap-highlight-color:transparent}hr{margin:1rem 0;color:inherit;background-color:currentColor;border:0;opacity:.25}hr:not([size]){height:1px}h1,h2,h3,h4,h5,h6{margin-top:0;margin-bottom:.5rem;font-weight:500;line-height:1.2}h1{font-size:calc(1.375rem + 1.5vw)}@media (min-width:1200px){h1{font-size:2.5rem}}h2{font-size:calc(1.325rem + .9vw)}@media (min-width:1200px){h2{font-size:2rem}}h3{font-size:calc(1.3rem + .6vw)}@media (min-width:1200px){h3{font-size:1.75rem}}h4{font-size:calc(1.275rem + .3vw)}@media (min-width:1200px){h4{font-size:1.5rem}}h5{font-size:1.25rem}h6{font-size:1rem}p{margin-top:0;margin-bottom:1rem}abbr[data-bs-original-title],abbr[title]{-webkit-text-decoration:underline dotted;text-decoration:underline dotted;cursor:help;-webkit-text-decoration-skip-ink:none;text-decoration-skip-ink:none}address{margin-bottom:1rem;font-style:normal;line-height:inherit}ol,ul{padding-left:2rem}dl,ol,ul{margin-top:0;margin-bottom:1rem}ol ol,ol ul,ul ol,ul ul{margin-bottom:0}dt{font-weight:700}dd{margin-bottom:.5rem;margin-left:0}blockquote{margin:0 0 1rem}b,strong{font-weight:bolder}small{font-size:.875em}mark{padding:.2em;background-color:#fcf8e3}sub,sup{position:relative;font-size:.75em;line-height:0;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}a{color:#0d6efd;text-decoration:underline}a:hover{color:#0a58ca}a:not([href]):not([class]),a:not([href]):not([class]):hover{color:inherit;text-decoration:none}code,kbd,pre,samp{font-family:SFMono-Regular,Menlo,Monaco,Consolas,"Liberation Mono","Courier New",monospace;font-size:1em;direction:ltr;unicode-bidi:bidi-override}pre{display:block;margin-top:0;margin-bottom:1rem;overflow:auto;font-size:.875em}pre code{font-size:inherit;color:inherit;word-break:normal}code{font-size:.875em;color:#d63384;word-wrap:break-word}a>code{color:inherit}kbd{padding:.2rem .4rem;font-size:.875em;color:#fff;background-color:#212529;border-radius:.2rem}kbd kbd{padding:0;font-size:1em;font-weight:700}figure{margin:0 0 1rem}img,svg{vertical-align:middle}table{caption-side:bottom;border-collapse:collapse}caption{padding-top:.5rem;padding-bottom:.5rem;color:#6c757d;text-align:left}th{text-align:inherit;text-align:-webkit-match-parent}tbody,td,tfoot,th,thead,tr{border-color:inherit;border-style:solid;border-width:0}label{display:inline-block}button{border-radius:0}button:focus:not(:focus-visible){outline:0}button,input,optgroup,select,textarea{margin:0;font-family:inherit;font-size:inherit;line-height:inherit}button,select{text-transform:none}[role=button]{cursor:pointer}select{word-wrap:normal}select:disabled{opacity:1}[list]::-webkit-calendar-picker-indicator{display:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button}[type=button]:not(:disabled),[type=reset]:not(:disabled),[type=submit]:not(:disabled),button:not(:disabled){cursor:pointer}::-moz-focus-inner{padding:0;border-style:none}textarea{resize:vertical}fieldset{min-width:0;padding:0;margin:0;border:0}legend{float:left;width:100%;padding:0;margin-bottom:.5rem;font-size:calc(1.275rem + .3vw);line-height:inherit}@media (min-width:1200px){legend{font-size:1.5rem}}legend+*{clear:left}::-webkit-datetime-edit-day-field,::-webkit-datetime-edit-fields-wrapper,::-webkit-datetime-edit-hour-field,::-webkit-datetime-edit-minute,::-webkit-datetime-edit-month-field,::-webkit-datetime-edit-text,::-webkit-datetime-edit-year-field{padding:0}::-webkit-inner-spin-button{height:auto}[type=search]{outline-offset:-2px;-webkit-appearance:textfield}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-color-swatch-wrapper{padding:0}::file-selector-button{font:inherit}::-webkit-file-upload-button{font:inherit;-webkit-appearance:button}output{display:inline-block}iframe{border:0}summary{display:list-item;cursor:pointer}progress{vertical-align:baseline}[hidden]{display:none!important}</style>
     <style>/*! syntax-highlighting.css */pre{line-height:125%;}span.linenos{color:inherit; background-color:transparent; padding-left:5px; padding-right:20px;}.pdoc-code .hll{background-color:#ffffcc}.pdoc-code{background:#f8f8f8;}.pdoc-code .c{color:#3D7B7B; font-style:italic}.pdoc-code .err{border:1px solid #FF0000}.pdoc-code .k{color:#008000; font-weight:bold}.pdoc-code .o{color:#666666}.pdoc-code .ch{color:#3D7B7B; font-style:italic}.pdoc-code .cm{color:#3D7B7B; font-style:italic}.pdoc-code .cp{color:#9C6500}.pdoc-code .cpf{color:#3D7B7B; font-style:italic}.pdoc-code .c1{color:#3D7B7B; font-style:italic}.pdoc-code .cs{color:#3D7B7B; font-style:italic}.pdoc-code .gd{color:#A00000}.pdoc-code .ge{font-style:italic}.pdoc-code .gr{color:#E40000}.pdoc-code .gh{color:#000080; font-weight:bold}.pdoc-code .gi{color:#008400}.pdoc-code .go{color:#717171}.pdoc-code .gp{color:#000080; font-weight:bold}.pdoc-code .gs{font-weight:bold}.pdoc-code .gu{color:#800080; font-weight:bold}.pdoc-code .gt{color:#0044DD}.pdoc-code .kc{color:#008000; font-weight:bold}.pdoc-code .kd{color:#008000; font-weight:bold}.pdoc-code .kn{color:#008000; font-weight:bold}.pdoc-code .kp{color:#008000}.pdoc-code .kr{color:#008000; font-weight:bold}.pdoc-code .kt{color:#B00040}.pdoc-code .m{color:#666666}.pdoc-code .s{color:#BA2121}.pdoc-code .na{color:#687822}.pdoc-code .nb{color:#008000}.pdoc-code .nc{color:#0000FF; font-weight:bold}.pdoc-code .no{color:#880000}.pdoc-code .nd{color:#AA22FF}.pdoc-code .ni{color:#717171; font-weight:bold}.pdoc-code .ne{color:#CB3F38; font-weight:bold}.pdoc-code .nf{color:#0000FF}.pdoc-code .nl{color:#767600}.pdoc-code .nn{color:#0000FF; font-weight:bold}.pdoc-code .nt{color:#008000; font-weight:bold}.pdoc-code .nv{color:#19177C}.pdoc-code .ow{color:#AA22FF; font-weight:bold}.pdoc-code .w{color:#bbbbbb}.pdoc-code .mb{color:#666666}.pdoc-code .mf{color:#666666}.pdoc-code .mh{color:#666666}.pdoc-code .mi{color:#666666}.pdoc-code .mo{color:#666666}.pdoc-code .sa{color:#BA2121}.pdoc-code .sb{color:#BA2121}.pdoc-code .sc{color:#BA2121}.pdoc-code .dl{color:#BA2121}.pdoc-code .sd{color:#BA2121; font-style:italic}.pdoc-code .s2{color:#BA2121}.pdoc-code .se{color:#AA5D1F; font-weight:bold}.pdoc-code .sh{color:#BA2121}.pdoc-code .si{color:#A45A77; font-weight:bold}.pdoc-code .sx{color:#008000}.pdoc-code .sr{color:#A45A77}.pdoc-code .s1{color:#BA2121}.pdoc-code .ss{color:#19177C}.pdoc-code .bp{color:#008000}.pdoc-code .fm{color:#0000FF}.pdoc-code .vc{color:#19177C}.pdoc-code .vg{color:#19177C}.pdoc-code .vi{color:#19177C}.pdoc-code .vm{color:#19177C}.pdoc-code .il{color:#666666}</style>
     <style>/*! theme.css */:root{--pdoc-background:#fff;}.pdoc{--text:#212529;--muted:#6c757d;--link:#3660a5;--link-hover:#1659c5;--code:#f8f8f8;--active:#fff598;--accent:#eee;--accent2:#c1c1c1;--nav-hover:rgba(255, 255, 255, 0.5);--name:#0066BB;--def:#008800;--annotation:#007020;}</style>
     <style>/*! layout.css */html, body{width:100%;height:100%;}html, main{scroll-behavior:smooth;}body{background-color:var(--pdoc-background);}@media (max-width:769px){#navtoggle{cursor:pointer;position:absolute;width:50px;height:40px;top:1rem;right:1rem;border-color:var(--text);color:var(--text);display:flex;opacity:0.8;z-index:999;}#navtoggle:hover{opacity:1;}#togglestate + div{display:none;}#togglestate:checked + div{display:inherit;}main, header{padding:2rem 3vw;}header + main{margin-top:-3rem;}.git-button{display:none !important;}nav input[type="search"]{max-width:77%;}nav input[type="search"]:first-child{margin-top:-6px;}nav input[type="search"]:valid ~ *{display:none !important;}}@media (min-width:770px){:root{--sidebar-width:clamp(12.5rem, 28vw, 22rem);}nav{position:fixed;overflow:auto;height:100vh;width:var(--sidebar-width);}main, header{padding:3rem 2rem 3rem calc(var(--sidebar-width) + 3rem);width:calc(54rem + var(--sidebar-width));max-width:100%;}header + main{margin-top:-4rem;}#navtoggle{display:none;}}#togglestate{position:absolute;height:0;opacity:0;}nav.pdoc{--pad:clamp(0.5rem, 2vw, 1.75rem);--indent:1.5rem;background-color:var(--accent);border-right:1px solid var(--accent2);box-shadow:0 0 20px rgba(50, 50, 50, .2) inset;padding:0 0 0 var(--pad);overflow-wrap:anywhere;scrollbar-width:thin; scrollbar-color:var(--accent2) transparent }nav.pdoc::-webkit-scrollbar{width:.4rem; }nav.pdoc::-webkit-scrollbar-thumb{background-color:var(--accent2); }nav.pdoc > div{padding:var(--pad) 0;}nav.pdoc .module-list-button{display:inline-flex;align-items:center;color:var(--text);border-color:var(--muted);margin-bottom:1rem;}nav.pdoc .module-list-button:hover{border-color:var(--text);}nav.pdoc input[type=search]{display:block;outline-offset:0;width:calc(100% - var(--pad));}nav.pdoc .logo{max-width:calc(100% - var(--pad));max-height:35vh;display:block;margin:0 auto 1rem;transform:translate(calc(-.5 * var(--pad)), 0);}nav.pdoc ul{list-style:none;padding-left:0;}nav.pdoc > div > ul{margin-left:calc(0px - var(--pad));}nav.pdoc li a{padding:.2rem 0 .2rem calc(var(--pad) + var(--indent));}nav.pdoc > div > ul > li > a{padding-left:var(--pad);}nav.pdoc li{transition:all 100ms;}nav.pdoc li:hover{background-color:var(--nav-hover);}nav.pdoc a, nav.pdoc a:hover{color:var(--text);}nav.pdoc a{display:block;}nav.pdoc > h2:first-of-type{margin-top:1.5rem;}nav.pdoc .class:before{content:"class ";color:var(--muted);}nav.pdoc .function:after{content:"()";color:var(--muted);}nav.pdoc footer:before{content:"";display:block;width:calc(100% - var(--pad));border-top:solid var(--accent2) 1px;margin-top:1.5rem;padding-top:.5rem;}nav.pdoc footer{font-size:small;}</style>
     <style>/*! content.css */.pdoc{color:var(--text);box-sizing:border-box;line-height:1.5;background:none;}.pdoc .pdoc-button{cursor:pointer;display:inline-block;border:solid black 1px;border-radius:2px;font-size:.75rem;padding:calc(0.5em - 1px) 1em;transition:100ms all;}.pdoc .pdoc-alert{padding:1rem 1rem 1rem calc(1.5rem + 24px);border:1px solid transparent;border-radius:.25rem;background-repeat:no-repeat;background-position:1rem center;margin-bottom:1rem;}.pdoc .pdoc-alert > *:last-child{margin-bottom:0;}.pdoc .pdoc-alert-note {color:#084298;background-color:#cfe2ff;border-color:#b6d4fe;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23084298%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M8%2016A8%208%200%201%200%208%200a8%208%200%200%200%200%2016zm.93-9.412-1%204.705c-.07.34.029.533.304.533.194%200%20.487-.07.686-.246l-.088.416c-.287.346-.92.598-1.465.598-.703%200-1.002-.422-.808-1.319l.738-3.468c.064-.293.006-.399-.287-.47l-.451-.081.082-.381%202.29-.287zM8%205.5a1%201%200%201%201%200-2%201%201%200%200%201%200%202z%22/%3E%3C/svg%3E");}.pdoc .pdoc-alert-warning{color:#664d03;background-color:#fff3cd;border-color:#ffecb5;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23664d03%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M8.982%201.566a1.13%201.13%200%200%200-1.96%200L.165%2013.233c-.457.778.091%201.767.98%201.767h13.713c.889%200%201.438-.99.98-1.767L8.982%201.566zM8%205c.535%200%20.954.462.9.995l-.35%203.507a.552.552%200%200%201-1.1%200L7.1%205.995A.905.905%200%200%201%208%205zm.002%206a1%201%200%201%201%200%202%201%201%200%200%201%200-2z%22/%3E%3C/svg%3E");}.pdoc .pdoc-alert-danger{color:#842029;background-color:#f8d7da;border-color:#f5c2c7;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23842029%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M5.52.359A.5.5%200%200%201%206%200h4a.5.5%200%200%201%20.474.658L8.694%206H12.5a.5.5%200%200%201%20.395.807l-7%209a.5.5%200%200%201-.873-.454L6.823%209.5H3.5a.5.5%200%200%201-.48-.641l2.5-8.5z%22/%3E%3C/svg%3E");}.pdoc .visually-hidden{position:absolute !important;width:1px !important;height:1px !important;padding:0 !important;margin:-1px !important;overflow:hidden !important;clip:rect(0, 0, 0, 0) !important;white-space:nowrap !important;border:0 !important;}.pdoc h1, .pdoc h2, .pdoc h3{font-weight:300;margin:.3em 0;padding:.2em 0;}.pdoc > section:not(.module-info) h1{font-size:1.5rem;font-weight:500;}.pdoc > section:not(.module-info) h2{font-size:1.4rem;font-weight:500;}.pdoc > section:not(.module-info) h3{font-size:1.3rem;font-weight:500;}.pdoc > section:not(.module-info) h4{font-size:1.2rem;}.pdoc > section:not(.module-info) h5{font-size:1.1rem;}.pdoc a{text-decoration:none;color:var(--link);}.pdoc a:hover{color:var(--link-hover);}.pdoc blockquote{margin-left:2rem;}.pdoc pre{border-top:1px solid var(--accent2);border-bottom:1px solid var(--accent2);margin-top:0;margin-bottom:1em;padding:.5rem 0 .5rem .5rem;overflow-x:auto;background-color:var(--code);}.pdoc code{color:var(--text);padding:.2em .4em;margin:0;font-size:85%;background-color:var(--code);border-radius:6px;}.pdoc a > code{color:inherit;}.pdoc pre > code{display:inline-block;font-size:inherit;background:none;border:none;padding:0;}.pdoc > section:not(.module-info){margin-bottom:1.5rem;}.pdoc .modulename{margin-top:0;font-weight:bold;}.pdoc .modulename a{color:var(--link);transition:100ms all;}.pdoc .git-button{float:right;border:solid var(--link) 1px;}.pdoc .git-button:hover{background-color:var(--link);color:var(--pdoc-background);}.view-source-toggle-state,.view-source-toggle-state ~ .pdoc-code{display:none;}.view-source-toggle-state:checked ~ .pdoc-code{display:block;}.view-source-button{display:inline-block;float:right;font-size:.75rem;line-height:1.5rem;color:var(--muted);padding:0 .4rem 0 1.3rem;cursor:pointer;text-indent:-2px;}.view-source-button > span{visibility:hidden;}.module-info .view-source-button{float:none;display:flex;justify-content:flex-end;margin:-1.2rem .4rem -.2rem 0;}.view-source-button::before{position:absolute;content:"View Source";display:list-item;list-style-type:disclosure-closed;}.view-source-toggle-state:checked ~ .attr .view-source-button::before,.view-source-toggle-state:checked ~ .view-source-button::before{list-style-type:disclosure-open;}.pdoc .docstring{margin-bottom:1.5rem;}.pdoc section:not(.module-info) .docstring{margin-left:clamp(0rem, 5vw - 2rem, 1rem);}.pdoc .docstring .pdoc-code{margin-left:1em;margin-right:1em;}.pdoc h1:target,.pdoc h2:target,.pdoc h3:target,.pdoc h4:target,.pdoc h5:target,.pdoc h6:target,.pdoc .pdoc-code > pre > span:target{background-color:var(--active);box-shadow:-1rem 0 0 0 var(--active);}.pdoc .pdoc-code > pre > span:target{display:block;}.pdoc div:target > .attr,.pdoc section:target > .attr,.pdoc dd:target > a{background-color:var(--active);}.pdoc *{scroll-margin:2rem;}.pdoc .pdoc-code .linenos{user-select:none;}.pdoc .attr:hover{filter:contrast(0.95);}.pdoc section, .pdoc .classattr{position:relative;}.pdoc .headerlink{--width:clamp(1rem, 3vw, 2rem);position:absolute;top:0;left:calc(0rem - var(--width));transition:all 100ms ease-in-out;opacity:0;}.pdoc .headerlink::before{content:"#";display:block;text-align:center;width:var(--width);height:2.3rem;line-height:2.3rem;font-size:1.5rem;}.pdoc .attr:hover ~ .headerlink,.pdoc *:target > .headerlink,.pdoc .headerlink:hover{opacity:1;}.pdoc .attr{display:block;margin:.5rem 0 .5rem;padding:.4rem .4rem .4rem 1rem;background-color:var(--accent);overflow-x:auto;}.pdoc .classattr{margin-left:2rem;}.pdoc .name{color:var(--name);font-weight:bold;}.pdoc .def{color:var(--def);font-weight:bold;}.pdoc .signature{background-color:transparent;}.pdoc .param, .pdoc .return-annotation{white-space:pre;}.pdoc .signature.multiline .param{display:block;}.pdoc .signature.condensed .param{display:inline-block;}.pdoc .annotation{color:var(--annotation);}.pdoc .view-value-toggle-state,.pdoc .view-value-toggle-state ~ .default_value{display:none;}.pdoc .view-value-toggle-state:checked ~ .default_value{display:inherit;}.pdoc .view-value-button{font-size:.5rem;vertical-align:middle;border-style:dashed;margin-top:-0.1rem;}.pdoc .view-value-button:hover{background:white;}.pdoc .view-value-button::before{content:"show";text-align:center;width:2.2em;display:inline-block;}.pdoc .view-value-toggle-state:checked ~ .view-value-button::before{content:"hide";}.pdoc .inherited{margin-left:2rem;}.pdoc .inherited dt{font-weight:700;}.pdoc .inherited dt, .pdoc .inherited dd{display:inline;margin-left:0;margin-bottom:.5rem;}.pdoc .inherited dd:not(:last-child):after{content:", ";}.pdoc .inherited .class:before{content:"class ";}.pdoc .inherited .function a:after{content:"()";}.pdoc .search-result .docstring{overflow:auto;max-height:25vh;}.pdoc .search-result.focused > .attr{background-color:var(--active);}.pdoc .attribution{margin-top:2rem;display:block;opacity:0.5;transition:all 200ms;filter:grayscale(100%);}.pdoc .attribution:hover{opacity:1;filter:grayscale(0%);}.pdoc .attribution img{margin-left:5px;height:35px;vertical-align:middle;width:70px;transition:all 200ms;}.pdoc table{display:block;width:max-content;max-width:100%;overflow:auto;margin-bottom:1rem;}.pdoc table th{font-weight:600;}.pdoc table th, .pdoc table td{padding:6px 13px;border:1px solid var(--accent2);}</style>
-    <style>/*! custom.css */nav.pdoc .attribution{	font-size:small;	display:none;}nav.pdoc .attribution img{	height:2em;	width:unset;	margin-left:0.1em;}nav.pdoc .function::after{	content:none;}.pdoc > section:not(.module-info) h2{	font-size:1.3rem;}.pdoc code{	padding:0.2em 0.2em;}.pdoc pre{	tab-size:4;}.pdoc section{	margin-bottom:2.25rem;}.pdoc .classattr, .pdoc .inherited{	margin-top:2.25rem;	margin-bottom:2.25rem;}.pdoc .docstring{	margin-bottom:1rem;}.pdoc .docstring .pdoc-code{	margin-left:unset;	margin-right:unset;}.pdoc .attr{	font-family:SFMono-Regular,Menlo,Monaco,Consolas,"Liberation Mono","Courier New",monospace;	tab-size:4;}.pdoc .decorator{	color:var(--muted);}.pdoc .summary{	margin-bottom:1rem;margin-left:clamp(0rem, 5vw - 2rem, 1rem);}.pdoc .summary dt{	font-family:SFMono-Regular,Menlo,Monaco,Consolas,"Liberation Mono","Courier New",monospace;	white-space:nowrap;}.pdoc .summary dt .signature{	display:inline-block;	box-sizing:border-box;	vertical-align:bottom;	overflow-x:hidden;	text-overflow:ellipsis;}.pdoc .summary dt .signature .param{	display:inline;	white-space:nowrap;}</style></head>
+    <style>/*! custom.css */nav.pdoc .attribution{	font-size:small;	display:none;}nav.pdoc .attribution img{	height:2em;	width:unset;	margin-left:0.1em;}nav.pdoc .function::after{	content:none;}.pdoc > section:not(.module-info) h2{	font-size:1.3rem;}.pdoc code{	padding:0.2em 0.2em;}.pdoc pre{	tab-size:4;}.pdoc section{	margin-bottom:2.25rem;}.pdoc .classattr, .pdoc .inherited{	margin-top:2.25rem;	margin-bottom:2.25rem;}.pdoc .docstring{	margin-bottom:1rem;}.pdoc .docstring .pdoc-code{	margin-left:unset;	margin-right:unset;}.pdoc .attr{	font-family:SFMono-Regular,Menlo,Monaco,Consolas,"Liberation Mono","Courier New",monospace;	tab-size:4;}.pdoc .decorator{	color:var(--muted);}</style></head>
 <body>
     <nav class="pdoc">
         <label id="navtoggle" for="togglestate" class="pdoc-button"><svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'><path stroke-linecap='round' stroke="currentColor" stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/></svg></label>
         <input id="togglestate" type="checkbox" aria-hidden="true" tabindex="-1">
         <div>
 
 
@@ -164,17 +109,14 @@
 			</li>
 			<li>
 						<a class="function" href="#reduce_types">reduce_types<span class="decorator">()</span></a>
 			</li>
 			<li>
 					<a class="class" href="#Nullable">Nullable</a>
 							<ul class="memberlist">
-            			<li>
-            						<a class="function" href="#Nullable.__init__">Nullable</a>
-            			</li>
             	</ul>
 
 			</li>
 	</ul>
 
 
 
@@ -198,30 +140,29 @@
 
 <ul>
 <li>treat <code>inf</code> as either a float or a normal string</li>
 <li>give exact Decimal values instead of floats</li>
 <li>detect inline lists</li>
 </ul></div>
 
-
                         <input id="mod-parsetypes-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-parsetypes-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos"> 1</span></a><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a><span class="sd">	This package provides tools for parsing serialised data to recover their original underlying types.</span>
 </span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a>
 </span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="sd">	The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="sd">	- treat `inf` as either a float or a normal string</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a><span class="sd">	- give exact Decimal values instead of floats</span>
 </span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="sd">	- detect inline lists</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>
 </span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;0.3&quot;</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;0.3.1&quot;</span>
 </span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>
 </span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a><span class="kn">from</span> <span class="nn">._common</span> <span class="kn">import</span> <span class="n">AnyScalar</span><span class="p">,</span> <span class="n">AnyScalarType</span><span class="p">,</span> <span class="n">AnyValue</span><span class="p">,</span> <span class="n">AnyValueType</span><span class="p">,</span> <span class="n">GenericValue</span><span class="p">,</span> <span class="n">Nullable</span>
 </span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a><span class="kn">from</span> <span class="nn">._parser</span> <span class="kn">import</span> <span class="n">TypeParser</span>
 </span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a><span class="kn">from</span> <span class="nn">._reduce_types</span> <span class="kn">import</span> <span class="n">reduce_types</span>
 </span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a>
 </span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a><span class="n">__all__</span> <span class="o">=</span> <span class="p">(</span><span class="s1">&#39;TypeParser&#39;</span><span class="p">,</span> <span class="s1">&#39;reduce_types&#39;</span><span class="p">,</span> <span class="s1">&#39;Nullable&#39;</span><span class="p">)</span>
 </span></pre></div>
@@ -722,15 +663,15 @@
 </span><span id="TypeParser-539"><a href="#TypeParser-539"><span class="linenos"> 539</span></a><span class="sd">			`value`</span>
 </span><span id="TypeParser-540"><a href="#TypeParser-540"><span class="linenos"> 540</span></a><span class="sd">			: string to be checked</span>
 </span><span id="TypeParser-541"><a href="#TypeParser-541"><span class="linenos"> 541</span></a>
 </span><span id="TypeParser-542"><a href="#TypeParser-542"><span class="linenos"> 542</span></a><span class="sd">			Keyword arguments</span>
 </span><span id="TypeParser-543"><a href="#TypeParser-543"><span class="linenos"> 543</span></a><span class="sd">			-----------------</span>
 </span><span id="TypeParser-544"><a href="#TypeParser-544"><span class="linenos"> 544</span></a>
 </span><span id="TypeParser-545"><a href="#TypeParser-545"><span class="linenos"> 545</span></a><span class="sd">			`allow_negative`</span>
-</span><span id="TypeParser-546"><a href="#TypeParser-546"><span class="linenos"> 546</span></a><span class="sd">			: whether to accept negative values</span>
+</span><span id="TypeParser-546"><a href="#TypeParser-546"><span class="linenos"> 546</span></a><span class="sd">			: whether to accept negative values. Since negative values are always indicated with a negative sign, `allow_sign` must also be True (which is the default setting) for this to have any effect.</span>
 </span><span id="TypeParser-547"><a href="#TypeParser-547"><span class="linenos"> 547</span></a>
 </span><span id="TypeParser-548"><a href="#TypeParser-548"><span class="linenos"> 548</span></a><span class="sd">			`allow_sign`</span>
 </span><span id="TypeParser-549"><a href="#TypeParser-549"><span class="linenos"> 549</span></a><span class="sd">			: whether to accept values prepended with a sign character. If False, it implies that `allow_negative` is False also.</span>
 </span><span id="TypeParser-550"><a href="#TypeParser-550"><span class="linenos"> 550</span></a>
 </span><span id="TypeParser-551"><a href="#TypeParser-551"><span class="linenos"> 551</span></a><span class="sd">			`allow_scientific`</span>
 </span><span id="TypeParser-552"><a href="#TypeParser-552"><span class="linenos"> 552</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;M&lt;/var&gt; must be an integer and &lt;var&gt;X&lt;/var&gt; must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</span>
 </span><span id="TypeParser-553"><a href="#TypeParser-553"><span class="linenos"> 553</span></a>
@@ -941,548 +882,553 @@
 </span><span id="TypeParser-758"><a href="#TypeParser-758"><span class="linenos"> 758</span></a>			<span class="k">return</span> <span class="kc">True</span>
 </span><span id="TypeParser-759"><a href="#TypeParser-759"><span class="linenos"> 759</span></a>		<span class="k">if</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_match_false_values</span><span class="p">:</span>
 </span><span id="TypeParser-760"><a href="#TypeParser-760"><span class="linenos"> 760</span></a>			<span class="k">return</span> <span class="kc">False</span>
 </span><span id="TypeParser-761"><a href="#TypeParser-761"><span class="linenos"> 761</span></a>
 </span><span id="TypeParser-762"><a href="#TypeParser-762"><span class="linenos"> 762</span></a>		<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;not a boolean: </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="TypeParser-763"><a href="#TypeParser-763"><span class="linenos"> 763</span></a>
 </span><span id="TypeParser-764"><a href="#TypeParser-764"><span class="linenos"> 764</span></a>
-</span><span id="TypeParser-765"><a href="#TypeParser-765"><span class="linenos"> 765</span></a>	<span class="k">def</span> <span class="nf">parse_int</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="TypeParser-765"><a href="#TypeParser-765"><span class="linenos"> 765</span></a>	<span class="k">def</span> <span class="nf">parse_int</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_negative</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_sign</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
 </span><span id="TypeParser-766"><a href="#TypeParser-766"><span class="linenos"> 766</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="TypeParser-767"><a href="#TypeParser-767"><span class="linenos"> 767</span></a><span class="sd">			Parse a string and return it as an int if possible</span>
 </span><span id="TypeParser-768"><a href="#TypeParser-768"><span class="linenos"> 768</span></a>
 </span><span id="TypeParser-769"><a href="#TypeParser-769"><span class="linenos"> 769</span></a><span class="sd">			If the string represents a bool, it will be converted to `1` for True and `0` for False.</span>
 </span><span id="TypeParser-770"><a href="#TypeParser-770"><span class="linenos"> 770</span></a>
 </span><span id="TypeParser-771"><a href="#TypeParser-771"><span class="linenos"> 771</span></a><span class="sd">			Arguments</span>
 </span><span id="TypeParser-772"><a href="#TypeParser-772"><span class="linenos"> 772</span></a><span class="sd">			---------</span>
 </span><span id="TypeParser-773"><a href="#TypeParser-773"><span class="linenos"> 773</span></a><span class="sd">			`value`</span>
 </span><span id="TypeParser-774"><a href="#TypeParser-774"><span class="linenos"> 774</span></a><span class="sd">			: string to be parsed</span>
 </span><span id="TypeParser-775"><a href="#TypeParser-775"><span class="linenos"> 775</span></a>
 </span><span id="TypeParser-776"><a href="#TypeParser-776"><span class="linenos"> 776</span></a><span class="sd">			Keyword arguments</span>
 </span><span id="TypeParser-777"><a href="#TypeParser-777"><span class="linenos"> 777</span></a><span class="sd">			-----------------</span>
 </span><span id="TypeParser-778"><a href="#TypeParser-778"><span class="linenos"> 778</span></a>
-</span><span id="TypeParser-779"><a href="#TypeParser-779"><span class="linenos"> 779</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser-780"><a href="#TypeParser-780"><span class="linenos"> 780</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;M&lt;/var&gt; must be an integer and &lt;var&gt;X&lt;/var&gt; must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</span>
+</span><span id="TypeParser-779"><a href="#TypeParser-779"><span class="linenos"> 779</span></a><span class="sd">			`allow_negative`</span>
+</span><span id="TypeParser-780"><a href="#TypeParser-780"><span class="linenos"> 780</span></a><span class="sd">			: whether to accept negative values. Since negative values are always indicated with a negative sign, `allow_sign` must also be True (which is the default setting) for this to have any effect.</span>
 </span><span id="TypeParser-781"><a href="#TypeParser-781"><span class="linenos"> 781</span></a>
-</span><span id="TypeParser-782"><a href="#TypeParser-782"><span class="linenos"> 782</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-783"><a href="#TypeParser-783"><span class="linenos"> 783</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-784"><a href="#TypeParser-784"><span class="linenos"> 784</span></a><span class="sd">			parsed int value</span>
-</span><span id="TypeParser-785"><a href="#TypeParser-785"><span class="linenos"> 785</span></a>
-</span><span id="TypeParser-786"><a href="#TypeParser-786"><span class="linenos"> 786</span></a><span class="sd">			Raises</span>
-</span><span id="TypeParser-787"><a href="#TypeParser-787"><span class="linenos"> 787</span></a><span class="sd">			------</span>
-</span><span id="TypeParser-788"><a href="#TypeParser-788"><span class="linenos"> 788</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
-</span><span id="TypeParser-789"><a href="#TypeParser-789"><span class="linenos"> 789</span></a>
-</span><span id="TypeParser-790"><a href="#TypeParser-790"><span class="linenos"> 790</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-791"><a href="#TypeParser-791"><span class="linenos"> 791</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-792"><a href="#TypeParser-792"><span class="linenos"> 792</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-793"><a href="#TypeParser-793"><span class="linenos"> 793</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-794"><a href="#TypeParser-794"><span class="linenos"> 794</span></a><span class="sd">			parser.parse_int(&quot;0&quot;)    # 0</span>
-</span><span id="TypeParser-795"><a href="#TypeParser-795"><span class="linenos"> 795</span></a><span class="sd">			parser.parse_int(&quot;-1&quot;)   # -1</span>
-</span><span id="TypeParser-796"><a href="#TypeParser-796"><span class="linenos"> 796</span></a><span class="sd">			parser.parse_int(&quot;2e3&quot;)  # 2000</span>
-</span><span id="TypeParser-797"><a href="#TypeParser-797"><span class="linenos"> 797</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-798"><a href="#TypeParser-798"><span class="linenos"> 798</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-799"><a href="#TypeParser-799"><span class="linenos"> 799</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
-</span><span id="TypeParser-800"><a href="#TypeParser-800"><span class="linenos"> 800</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="TypeParser-801"><a href="#TypeParser-801"><span class="linenos"> 801</span></a>
-</span><span id="TypeParser-802"><a href="#TypeParser-802"><span class="linenos"> 802</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">):</span>
-</span><span id="TypeParser-803"><a href="#TypeParser-803"><span class="linenos"> 803</span></a>			<span class="k">if</span> <span class="n">allow_scientific</span><span class="p">:</span>
-</span><span id="TypeParser-804"><a href="#TypeParser-804"><span class="linenos"> 804</span></a>				<span class="n">value</span><span class="p">,</span> <span class="n">exp</span> <span class="o">=</span> <span class="n">_decompose_string_pair</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_scientific_char</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_int_case_sensitive</span><span class="p">)</span>
-</span><span id="TypeParser-805"><a href="#TypeParser-805"><span class="linenos"> 805</span></a>				<span class="k">if</span> <span class="n">exp</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="TypeParser-806"><a href="#TypeParser-806"><span class="linenos"> 806</span></a>					<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span> <span class="o">-</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span><span class="p">}):</span>
-</span><span id="TypeParser-807"><a href="#TypeParser-807"><span class="linenos"> 807</span></a>						<span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">+</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
-</span><span id="TypeParser-808"><a href="#TypeParser-808"><span class="linenos"> 808</span></a>					<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">*</span> <span class="p">(</span><span class="mi">10</span> <span class="o">**</span> <span class="nb">int</span><span class="p">(</span><span class="n">exp</span><span class="p">))</span>
-</span><span id="TypeParser-809"><a href="#TypeParser-809"><span class="linenos"> 809</span></a>
-</span><span id="TypeParser-810"><a href="#TypeParser-810"><span class="linenos"> 810</span></a>			<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span> <span class="o">-</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span><span class="p">}):</span>
-</span><span id="TypeParser-811"><a href="#TypeParser-811"><span class="linenos"> 811</span></a>				<span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">+</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
-</span><span id="TypeParser-812"><a href="#TypeParser-812"><span class="linenos"> 812</span></a>			<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-813"><a href="#TypeParser-813"><span class="linenos"> 813</span></a>
-</span><span id="TypeParser-814"><a href="#TypeParser-814"><span class="linenos"> 814</span></a>		<span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser-815"><a href="#TypeParser-815"><span class="linenos"> 815</span></a>			<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
-</span><span id="TypeParser-816"><a href="#TypeParser-816"><span class="linenos"> 816</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-817"><a href="#TypeParser-817"><span class="linenos"> 817</span></a>			<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;not an integer: </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="TypeParser-818"><a href="#TypeParser-818"><span class="linenos"> 818</span></a>
+</span><span id="TypeParser-782"><a href="#TypeParser-782"><span class="linenos"> 782</span></a><span class="sd">			`allow_sign`</span>
+</span><span id="TypeParser-783"><a href="#TypeParser-783"><span class="linenos"> 783</span></a><span class="sd">			: whether to accept values prepended with a sign character. If False, it implies that `allow_negative` is False also.</span>
+</span><span id="TypeParser-784"><a href="#TypeParser-784"><span class="linenos"> 784</span></a>
+</span><span id="TypeParser-785"><a href="#TypeParser-785"><span class="linenos"> 785</span></a><span class="sd">			`allow_scientific`</span>
+</span><span id="TypeParser-786"><a href="#TypeParser-786"><span class="linenos"> 786</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;M&lt;/var&gt; must be an integer and &lt;var&gt;X&lt;/var&gt; must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</span>
+</span><span id="TypeParser-787"><a href="#TypeParser-787"><span class="linenos"> 787</span></a>
+</span><span id="TypeParser-788"><a href="#TypeParser-788"><span class="linenos"> 788</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-789"><a href="#TypeParser-789"><span class="linenos"> 789</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-790"><a href="#TypeParser-790"><span class="linenos"> 790</span></a><span class="sd">			parsed int value</span>
+</span><span id="TypeParser-791"><a href="#TypeParser-791"><span class="linenos"> 791</span></a>
+</span><span id="TypeParser-792"><a href="#TypeParser-792"><span class="linenos"> 792</span></a><span class="sd">			Raises</span>
+</span><span id="TypeParser-793"><a href="#TypeParser-793"><span class="linenos"> 793</span></a><span class="sd">			------</span>
+</span><span id="TypeParser-794"><a href="#TypeParser-794"><span class="linenos"> 794</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
+</span><span id="TypeParser-795"><a href="#TypeParser-795"><span class="linenos"> 795</span></a>
+</span><span id="TypeParser-796"><a href="#TypeParser-796"><span class="linenos"> 796</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-797"><a href="#TypeParser-797"><span class="linenos"> 797</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-798"><a href="#TypeParser-798"><span class="linenos"> 798</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-799"><a href="#TypeParser-799"><span class="linenos"> 799</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-800"><a href="#TypeParser-800"><span class="linenos"> 800</span></a><span class="sd">			parser.parse_int(&quot;0&quot;)    # 0</span>
+</span><span id="TypeParser-801"><a href="#TypeParser-801"><span class="linenos"> 801</span></a><span class="sd">			parser.parse_int(&quot;-1&quot;)   # -1</span>
+</span><span id="TypeParser-802"><a href="#TypeParser-802"><span class="linenos"> 802</span></a><span class="sd">			parser.parse_int(&quot;2e3&quot;)  # 2000</span>
+</span><span id="TypeParser-803"><a href="#TypeParser-803"><span class="linenos"> 803</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-804"><a href="#TypeParser-804"><span class="linenos"> 804</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-805"><a href="#TypeParser-805"><span class="linenos"> 805</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
+</span><span id="TypeParser-806"><a href="#TypeParser-806"><span class="linenos"> 806</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="TypeParser-807"><a href="#TypeParser-807"><span class="linenos"> 807</span></a>
+</span><span id="TypeParser-808"><a href="#TypeParser-808"><span class="linenos"> 808</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="n">allow_negative</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="n">allow_sign</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">):</span>
+</span><span id="TypeParser-809"><a href="#TypeParser-809"><span class="linenos"> 809</span></a>			<span class="k">if</span> <span class="n">allow_scientific</span><span class="p">:</span>
+</span><span id="TypeParser-810"><a href="#TypeParser-810"><span class="linenos"> 810</span></a>				<span class="n">value</span><span class="p">,</span> <span class="n">exp</span> <span class="o">=</span> <span class="n">_decompose_string_pair</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_scientific_char</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_int_case_sensitive</span><span class="p">)</span>
+</span><span id="TypeParser-811"><a href="#TypeParser-811"><span class="linenos"> 811</span></a>				<span class="k">if</span> <span class="n">exp</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="TypeParser-812"><a href="#TypeParser-812"><span class="linenos"> 812</span></a>					<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span> <span class="o">-</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span><span class="p">}):</span>
+</span><span id="TypeParser-813"><a href="#TypeParser-813"><span class="linenos"> 813</span></a>						<span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">+</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
+</span><span id="TypeParser-814"><a href="#TypeParser-814"><span class="linenos"> 814</span></a>					<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">*</span> <span class="p">(</span><span class="mi">10</span> <span class="o">**</span> <span class="nb">int</span><span class="p">(</span><span class="n">exp</span><span class="p">))</span>
+</span><span id="TypeParser-815"><a href="#TypeParser-815"><span class="linenos"> 815</span></a>
+</span><span id="TypeParser-816"><a href="#TypeParser-816"><span class="linenos"> 816</span></a>			<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span> <span class="o">-</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span><span class="p">}):</span>
+</span><span id="TypeParser-817"><a href="#TypeParser-817"><span class="linenos"> 817</span></a>				<span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">+</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
+</span><span id="TypeParser-818"><a href="#TypeParser-818"><span class="linenos"> 818</span></a>			<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
 </span><span id="TypeParser-819"><a href="#TypeParser-819"><span class="linenos"> 819</span></a>
-</span><span id="TypeParser-820"><a href="#TypeParser-820"><span class="linenos"> 820</span></a>	<span class="k">def</span> <span class="nf">_parse_floatlike</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span>
-</span><span id="TypeParser-821"><a href="#TypeParser-821"><span class="linenos"> 821</span></a>		<span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="TypeParser-822"><a href="#TypeParser-822"><span class="linenos"> 822</span></a>		<span class="n">converter</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">bool</span><span class="p">]],</span> <span class="n">_FloatLike</span><span class="p">],</span>
-</span><span id="TypeParser-823"><a href="#TypeParser-823"><span class="linenos"> 823</span></a>		<span class="n">inf_value</span><span class="p">:</span> <span class="n">_FloatLike</span><span class="p">,</span>
-</span><span id="TypeParser-824"><a href="#TypeParser-824"><span class="linenos"> 824</span></a>		<span class="n">nan_value</span><span class="p">:</span> <span class="n">_FloatLike</span><span class="p">,</span>
-</span><span id="TypeParser-825"><a href="#TypeParser-825"><span class="linenos"> 825</span></a>		<span class="o">*</span><span class="p">,</span>
-</span><span id="TypeParser-826"><a href="#TypeParser-826"><span class="linenos"> 826</span></a>		<span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="TypeParser-827"><a href="#TypeParser-827"><span class="linenos"> 827</span></a>		<span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="TypeParser-828"><a href="#TypeParser-828"><span class="linenos"> 828</span></a>		<span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span>
-</span><span id="TypeParser-829"><a href="#TypeParser-829"><span class="linenos"> 829</span></a>	<span class="p">)</span> <span class="o">-&gt;</span> <span class="n">_FloatLike</span><span class="p">:</span>
-</span><span id="TypeParser-830"><a href="#TypeParser-830"><span class="linenos"> 830</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
-</span><span id="TypeParser-831"><a href="#TypeParser-831"><span class="linenos"> 831</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="TypeParser-832"><a href="#TypeParser-832"><span class="linenos"> 832</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span> <span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span> <span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">):</span>
-</span><span id="TypeParser-833"><a href="#TypeParser-833"><span class="linenos"> 833</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_float_case_sensitive</span><span class="p">:</span>
-</span><span id="TypeParser-834"><a href="#TypeParser-834"><span class="linenos"> 834</span></a>				<span class="n">special_value</span> <span class="o">=</span> <span class="n">value</span>
-</span><span id="TypeParser-835"><a href="#TypeParser-835"><span class="linenos"> 835</span></a>			<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-836"><a href="#TypeParser-836"><span class="linenos"> 836</span></a>				<span class="n">special_value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="TypeParser-837"><a href="#TypeParser-837"><span class="linenos"> 837</span></a>			<span class="k">if</span> <span class="n">allow_inf</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_match_inf_values</span><span class="p">:</span>
-</span><span id="TypeParser-838"><a href="#TypeParser-838"><span class="linenos"> 838</span></a>				<span class="k">return</span> <span class="n">inf_value</span>
-</span><span id="TypeParser-839"><a href="#TypeParser-839"><span class="linenos"> 839</span></a>			<span class="k">if</span> <span class="n">allow_nan</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_match_nan_values</span><span class="p">:</span>
-</span><span id="TypeParser-840"><a href="#TypeParser-840"><span class="linenos"> 840</span></a>				<span class="k">return</span> <span class="n">nan_value</span>
-</span><span id="TypeParser-841"><a href="#TypeParser-841"><span class="linenos"> 841</span></a>
-</span><span id="TypeParser-842"><a href="#TypeParser-842"><span class="linenos"> 842</span></a>			<span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sign_chars</span><span class="p">:</span>
-</span><span id="TypeParser-843"><a href="#TypeParser-843"><span class="linenos"> 843</span></a>				<span class="n">positive_part</span> <span class="o">=</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
-</span><span id="TypeParser-844"><a href="#TypeParser-844"><span class="linenos"> 844</span></a>				<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_float_case_sensitive</span><span class="p">:</span>
-</span><span id="TypeParser-845"><a href="#TypeParser-845"><span class="linenos"> 845</span></a>					<span class="n">special_value</span> <span class="o">=</span> <span class="n">positive_part</span>
-</span><span id="TypeParser-846"><a href="#TypeParser-846"><span class="linenos"> 846</span></a>				<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-847"><a href="#TypeParser-847"><span class="linenos"> 847</span></a>					<span class="n">special_value</span> <span class="o">=</span> <span class="n">positive_part</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="TypeParser-848"><a href="#TypeParser-848"><span class="linenos"> 848</span></a>				<span class="k">if</span> <span class="n">allow_inf</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_match_inf_values</span><span class="p">:</span>
-</span><span id="TypeParser-849"><a href="#TypeParser-849"><span class="linenos"> 849</span></a>					<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span><span class="p">:</span>
-</span><span id="TypeParser-850"><a href="#TypeParser-850"><span class="linenos"> 850</span></a>						<span class="k">return</span> <span class="o">-</span><span class="mi">1</span> <span class="o">*</span> <span class="n">inf_value</span>
-</span><span id="TypeParser-851"><a href="#TypeParser-851"><span class="linenos"> 851</span></a>					<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-852"><a href="#TypeParser-852"><span class="linenos"> 852</span></a>						<span class="k">return</span> <span class="n">inf_value</span>
-</span><span id="TypeParser-853"><a href="#TypeParser-853"><span class="linenos"> 853</span></a>				<span class="k">if</span> <span class="n">allow_nan</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_match_nan_values</span><span class="p">:</span>
-</span><span id="TypeParser-854"><a href="#TypeParser-854"><span class="linenos"> 854</span></a>					<span class="k">return</span> <span class="n">nan_value</span>
-</span><span id="TypeParser-855"><a href="#TypeParser-855"><span class="linenos"> 855</span></a>
-</span><span id="TypeParser-856"><a href="#TypeParser-856"><span class="linenos"> 856</span></a>				<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span><span class="p">:</span>
-</span><span id="TypeParser-857"><a href="#TypeParser-857"><span class="linenos"> 857</span></a>					<span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">+</span> <span class="n">positive_part</span>
-</span><span id="TypeParser-858"><a href="#TypeParser-858"><span class="linenos"> 858</span></a>			<span class="k">return</span> <span class="n">converter</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-859"><a href="#TypeParser-859"><span class="linenos"> 859</span></a>		<span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser-860"><a href="#TypeParser-860"><span class="linenos"> 860</span></a>			<span class="k">return</span> <span class="n">converter</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
-</span><span id="TypeParser-861"><a href="#TypeParser-861"><span class="linenos"> 861</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-862"><a href="#TypeParser-862"><span class="linenos"> 862</span></a>			<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;not a </span><span class="si">{</span><span class="n">_FloatLike</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="TypeParser-863"><a href="#TypeParser-863"><span class="linenos"> 863</span></a>
-</span><span id="TypeParser-864"><a href="#TypeParser-864"><span class="linenos"> 864</span></a>
-</span><span id="TypeParser-865"><a href="#TypeParser-865"><span class="linenos"> 865</span></a>	<span class="k">def</span> <span class="nf">parse_float</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="TypeParser-866"><a href="#TypeParser-866"><span class="linenos"> 866</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-867"><a href="#TypeParser-867"><span class="linenos"> 867</span></a><span class="sd">			Parse a string and return it as a (non-exact) float if possible</span>
-</span><span id="TypeParser-868"><a href="#TypeParser-868"><span class="linenos"> 868</span></a>
-</span><span id="TypeParser-869"><a href="#TypeParser-869"><span class="linenos"> 869</span></a><span class="sd">			If the string represents a bool, it will be converted to `1.` for True and `0.` for False. If the string represents an int, it will be converted to a float also.</span>
+</span><span id="TypeParser-820"><a href="#TypeParser-820"><span class="linenos"> 820</span></a>		<span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser-821"><a href="#TypeParser-821"><span class="linenos"> 821</span></a>			<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
+</span><span id="TypeParser-822"><a href="#TypeParser-822"><span class="linenos"> 822</span></a>		<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-823"><a href="#TypeParser-823"><span class="linenos"> 823</span></a>			<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;not an integer: </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="TypeParser-824"><a href="#TypeParser-824"><span class="linenos"> 824</span></a>
+</span><span id="TypeParser-825"><a href="#TypeParser-825"><span class="linenos"> 825</span></a>
+</span><span id="TypeParser-826"><a href="#TypeParser-826"><span class="linenos"> 826</span></a>	<span class="k">def</span> <span class="nf">_parse_floatlike</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span>
+</span><span id="TypeParser-827"><a href="#TypeParser-827"><span class="linenos"> 827</span></a>		<span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="TypeParser-828"><a href="#TypeParser-828"><span class="linenos"> 828</span></a>		<span class="n">converter</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">bool</span><span class="p">]],</span> <span class="n">_FloatLike</span><span class="p">],</span>
+</span><span id="TypeParser-829"><a href="#TypeParser-829"><span class="linenos"> 829</span></a>		<span class="n">inf_value</span><span class="p">:</span> <span class="n">_FloatLike</span><span class="p">,</span>
+</span><span id="TypeParser-830"><a href="#TypeParser-830"><span class="linenos"> 830</span></a>		<span class="n">nan_value</span><span class="p">:</span> <span class="n">_FloatLike</span><span class="p">,</span>
+</span><span id="TypeParser-831"><a href="#TypeParser-831"><span class="linenos"> 831</span></a>		<span class="o">*</span><span class="p">,</span>
+</span><span id="TypeParser-832"><a href="#TypeParser-832"><span class="linenos"> 832</span></a>		<span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="TypeParser-833"><a href="#TypeParser-833"><span class="linenos"> 833</span></a>		<span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="TypeParser-834"><a href="#TypeParser-834"><span class="linenos"> 834</span></a>		<span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span>
+</span><span id="TypeParser-835"><a href="#TypeParser-835"><span class="linenos"> 835</span></a>	<span class="p">)</span> <span class="o">-&gt;</span> <span class="n">_FloatLike</span><span class="p">:</span>
+</span><span id="TypeParser-836"><a href="#TypeParser-836"><span class="linenos"> 836</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
+</span><span id="TypeParser-837"><a href="#TypeParser-837"><span class="linenos"> 837</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="TypeParser-838"><a href="#TypeParser-838"><span class="linenos"> 838</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span> <span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span> <span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">):</span>
+</span><span id="TypeParser-839"><a href="#TypeParser-839"><span class="linenos"> 839</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_float_case_sensitive</span><span class="p">:</span>
+</span><span id="TypeParser-840"><a href="#TypeParser-840"><span class="linenos"> 840</span></a>				<span class="n">special_value</span> <span class="o">=</span> <span class="n">value</span>
+</span><span id="TypeParser-841"><a href="#TypeParser-841"><span class="linenos"> 841</span></a>			<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-842"><a href="#TypeParser-842"><span class="linenos"> 842</span></a>				<span class="n">special_value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="TypeParser-843"><a href="#TypeParser-843"><span class="linenos"> 843</span></a>			<span class="k">if</span> <span class="n">allow_inf</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_match_inf_values</span><span class="p">:</span>
+</span><span id="TypeParser-844"><a href="#TypeParser-844"><span class="linenos"> 844</span></a>				<span class="k">return</span> <span class="n">inf_value</span>
+</span><span id="TypeParser-845"><a href="#TypeParser-845"><span class="linenos"> 845</span></a>			<span class="k">if</span> <span class="n">allow_nan</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_match_nan_values</span><span class="p">:</span>
+</span><span id="TypeParser-846"><a href="#TypeParser-846"><span class="linenos"> 846</span></a>				<span class="k">return</span> <span class="n">nan_value</span>
+</span><span id="TypeParser-847"><a href="#TypeParser-847"><span class="linenos"> 847</span></a>
+</span><span id="TypeParser-848"><a href="#TypeParser-848"><span class="linenos"> 848</span></a>			<span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sign_chars</span><span class="p">:</span>
+</span><span id="TypeParser-849"><a href="#TypeParser-849"><span class="linenos"> 849</span></a>				<span class="n">positive_part</span> <span class="o">=</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
+</span><span id="TypeParser-850"><a href="#TypeParser-850"><span class="linenos"> 850</span></a>				<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_float_case_sensitive</span><span class="p">:</span>
+</span><span id="TypeParser-851"><a href="#TypeParser-851"><span class="linenos"> 851</span></a>					<span class="n">special_value</span> <span class="o">=</span> <span class="n">positive_part</span>
+</span><span id="TypeParser-852"><a href="#TypeParser-852"><span class="linenos"> 852</span></a>				<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-853"><a href="#TypeParser-853"><span class="linenos"> 853</span></a>					<span class="n">special_value</span> <span class="o">=</span> <span class="n">positive_part</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="TypeParser-854"><a href="#TypeParser-854"><span class="linenos"> 854</span></a>				<span class="k">if</span> <span class="n">allow_inf</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_match_inf_values</span><span class="p">:</span>
+</span><span id="TypeParser-855"><a href="#TypeParser-855"><span class="linenos"> 855</span></a>					<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span><span class="p">:</span>
+</span><span id="TypeParser-856"><a href="#TypeParser-856"><span class="linenos"> 856</span></a>						<span class="k">return</span> <span class="o">-</span><span class="mi">1</span> <span class="o">*</span> <span class="n">inf_value</span>
+</span><span id="TypeParser-857"><a href="#TypeParser-857"><span class="linenos"> 857</span></a>					<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-858"><a href="#TypeParser-858"><span class="linenos"> 858</span></a>						<span class="k">return</span> <span class="n">inf_value</span>
+</span><span id="TypeParser-859"><a href="#TypeParser-859"><span class="linenos"> 859</span></a>				<span class="k">if</span> <span class="n">allow_nan</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_match_nan_values</span><span class="p">:</span>
+</span><span id="TypeParser-860"><a href="#TypeParser-860"><span class="linenos"> 860</span></a>					<span class="k">return</span> <span class="n">nan_value</span>
+</span><span id="TypeParser-861"><a href="#TypeParser-861"><span class="linenos"> 861</span></a>
+</span><span id="TypeParser-862"><a href="#TypeParser-862"><span class="linenos"> 862</span></a>				<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span><span class="p">:</span>
+</span><span id="TypeParser-863"><a href="#TypeParser-863"><span class="linenos"> 863</span></a>					<span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">+</span> <span class="n">positive_part</span>
+</span><span id="TypeParser-864"><a href="#TypeParser-864"><span class="linenos"> 864</span></a>			<span class="k">return</span> <span class="n">converter</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-865"><a href="#TypeParser-865"><span class="linenos"> 865</span></a>		<span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser-866"><a href="#TypeParser-866"><span class="linenos"> 866</span></a>			<span class="k">return</span> <span class="n">converter</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
+</span><span id="TypeParser-867"><a href="#TypeParser-867"><span class="linenos"> 867</span></a>		<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-868"><a href="#TypeParser-868"><span class="linenos"> 868</span></a>			<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;not a </span><span class="si">{</span><span class="n">_FloatLike</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="TypeParser-869"><a href="#TypeParser-869"><span class="linenos"> 869</span></a>
 </span><span id="TypeParser-870"><a href="#TypeParser-870"><span class="linenos"> 870</span></a>
-</span><span id="TypeParser-871"><a href="#TypeParser-871"><span class="linenos"> 871</span></a><span class="sd">			Behaves analogously to `parse_decimal()`, except that that returns an exact Decimal instead.</span>
-</span><span id="TypeParser-872"><a href="#TypeParser-872"><span class="linenos"> 872</span></a>
-</span><span id="TypeParser-873"><a href="#TypeParser-873"><span class="linenos"> 873</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser-874"><a href="#TypeParser-874"><span class="linenos"> 874</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser-875"><a href="#TypeParser-875"><span class="linenos"> 875</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-876"><a href="#TypeParser-876"><span class="linenos"> 876</span></a><span class="sd">			: string to be parsed</span>
-</span><span id="TypeParser-877"><a href="#TypeParser-877"><span class="linenos"> 877</span></a>
-</span><span id="TypeParser-878"><a href="#TypeParser-878"><span class="linenos"> 878</span></a><span class="sd">			Keyword arguments</span>
-</span><span id="TypeParser-879"><a href="#TypeParser-879"><span class="linenos"> 879</span></a><span class="sd">			-----------------</span>
-</span><span id="TypeParser-880"><a href="#TypeParser-880"><span class="linenos"> 880</span></a>
-</span><span id="TypeParser-881"><a href="#TypeParser-881"><span class="linenos"> 881</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser-882"><a href="#TypeParser-882"><span class="linenos"> 882</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
+</span><span id="TypeParser-871"><a href="#TypeParser-871"><span class="linenos"> 871</span></a>	<span class="k">def</span> <span class="nf">parse_float</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="TypeParser-872"><a href="#TypeParser-872"><span class="linenos"> 872</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-873"><a href="#TypeParser-873"><span class="linenos"> 873</span></a><span class="sd">			Parse a string and return it as a (non-exact) float if possible</span>
+</span><span id="TypeParser-874"><a href="#TypeParser-874"><span class="linenos"> 874</span></a>
+</span><span id="TypeParser-875"><a href="#TypeParser-875"><span class="linenos"> 875</span></a><span class="sd">			If the string represents a bool, it will be converted to `1.` for True and `0.` for False. If the string represents an int, it will be converted to a float also.</span>
+</span><span id="TypeParser-876"><a href="#TypeParser-876"><span class="linenos"> 876</span></a>
+</span><span id="TypeParser-877"><a href="#TypeParser-877"><span class="linenos"> 877</span></a><span class="sd">			Behaves analogously to `parse_decimal()`, except that that returns an exact Decimal instead.</span>
+</span><span id="TypeParser-878"><a href="#TypeParser-878"><span class="linenos"> 878</span></a>
+</span><span id="TypeParser-879"><a href="#TypeParser-879"><span class="linenos"> 879</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser-880"><a href="#TypeParser-880"><span class="linenos"> 880</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser-881"><a href="#TypeParser-881"><span class="linenos"> 881</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-882"><a href="#TypeParser-882"><span class="linenos"> 882</span></a><span class="sd">			: string to be parsed</span>
 </span><span id="TypeParser-883"><a href="#TypeParser-883"><span class="linenos"> 883</span></a>
-</span><span id="TypeParser-884"><a href="#TypeParser-884"><span class="linenos"> 884</span></a><span class="sd">			`allow_inf`</span>
-</span><span id="TypeParser-885"><a href="#TypeParser-885"><span class="linenos"> 885</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.inf_values&lt;/code&gt; (empty set by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.float_case_sensitive&lt;/code&gt;, which is False by default.</span>
+</span><span id="TypeParser-884"><a href="#TypeParser-884"><span class="linenos"> 884</span></a><span class="sd">			Keyword arguments</span>
+</span><span id="TypeParser-885"><a href="#TypeParser-885"><span class="linenos"> 885</span></a><span class="sd">			-----------------</span>
 </span><span id="TypeParser-886"><a href="#TypeParser-886"><span class="linenos"> 886</span></a>
-</span><span id="TypeParser-887"><a href="#TypeParser-887"><span class="linenos"> 887</span></a><span class="sd">			`allow_nan`</span>
-</span><span id="TypeParser-888"><a href="#TypeParser-888"><span class="linenos"> 888</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.nan_values&lt;/code&gt; (empty set by default) are interpeted as NaN. The case sensitivity of this matching also depends on &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.float_case_sensitive&lt;/code&gt;, which is False by default.</span>
+</span><span id="TypeParser-887"><a href="#TypeParser-887"><span class="linenos"> 887</span></a><span class="sd">			`allow_scientific`</span>
+</span><span id="TypeParser-888"><a href="#TypeParser-888"><span class="linenos"> 888</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
 </span><span id="TypeParser-889"><a href="#TypeParser-889"><span class="linenos"> 889</span></a>
-</span><span id="TypeParser-890"><a href="#TypeParser-890"><span class="linenos"> 890</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-891"><a href="#TypeParser-891"><span class="linenos"> 891</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-892"><a href="#TypeParser-892"><span class="linenos"> 892</span></a><span class="sd">			parsed float value</span>
-</span><span id="TypeParser-893"><a href="#TypeParser-893"><span class="linenos"> 893</span></a>
-</span><span id="TypeParser-894"><a href="#TypeParser-894"><span class="linenos"> 894</span></a><span class="sd">			Raises</span>
-</span><span id="TypeParser-895"><a href="#TypeParser-895"><span class="linenos"> 895</span></a><span class="sd">			------</span>
-</span><span id="TypeParser-896"><a href="#TypeParser-896"><span class="linenos"> 896</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
-</span><span id="TypeParser-897"><a href="#TypeParser-897"><span class="linenos"> 897</span></a>
-</span><span id="TypeParser-898"><a href="#TypeParser-898"><span class="linenos"> 898</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-899"><a href="#TypeParser-899"><span class="linenos"> 899</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-900"><a href="#TypeParser-900"><span class="linenos"> 900</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-901"><a href="#TypeParser-901"><span class="linenos"> 901</span></a><span class="sd">			parser = TypeParser(inf_values=[&quot;inf&quot;], nan_values=[&quot;nan&quot;])</span>
-</span><span id="TypeParser-902"><a href="#TypeParser-902"><span class="linenos"> 902</span></a><span class="sd">			parser.parse_float(&quot;1.&quot;)       # 1.</span>
-</span><span id="TypeParser-903"><a href="#TypeParser-903"><span class="linenos"> 903</span></a><span class="sd">			parser.parse_float(&quot;1.23e2&quot;)   # 123.</span>
-</span><span id="TypeParser-904"><a href="#TypeParser-904"><span class="linenos"> 904</span></a><span class="sd">			parser.parse_float(&quot;1.23e-2&quot;)  # 0.0123</span>
-</span><span id="TypeParser-905"><a href="#TypeParser-905"><span class="linenos"> 905</span></a><span class="sd">			parser.parse_float(&quot;inf&quot;)      # math.inf</span>
-</span><span id="TypeParser-906"><a href="#TypeParser-906"><span class="linenos"> 906</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-907"><a href="#TypeParser-907"><span class="linenos"> 907</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-908"><a href="#TypeParser-908"><span class="linenos"> 908</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_parse_floatlike</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">math</span><span class="o">.</span><span class="n">inf</span><span class="p">,</span> <span class="n">math</span><span class="o">.</span><span class="n">nan</span><span class="p">,</span>
-</span><span id="TypeParser-909"><a href="#TypeParser-909"><span class="linenos"> 909</span></a>			<span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span>
-</span><span id="TypeParser-910"><a href="#TypeParser-910"><span class="linenos"> 910</span></a>			<span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span>
-</span><span id="TypeParser-911"><a href="#TypeParser-911"><span class="linenos"> 911</span></a>			<span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">,</span>
-</span><span id="TypeParser-912"><a href="#TypeParser-912"><span class="linenos"> 912</span></a>		<span class="p">)</span>
-</span><span id="TypeParser-913"><a href="#TypeParser-913"><span class="linenos"> 913</span></a>
-</span><span id="TypeParser-914"><a href="#TypeParser-914"><span class="linenos"> 914</span></a>
-</span><span id="TypeParser-915"><a href="#TypeParser-915"><span class="linenos"> 915</span></a>	<span class="k">def</span> <span class="nf">parse_decimal</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Decimal</span><span class="p">:</span>
-</span><span id="TypeParser-916"><a href="#TypeParser-916"><span class="linenos"> 916</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-917"><a href="#TypeParser-917"><span class="linenos"> 917</span></a><span class="sd">			Parse a string and return it as an exact Decimal if possible</span>
-</span><span id="TypeParser-918"><a href="#TypeParser-918"><span class="linenos"> 918</span></a>
-</span><span id="TypeParser-919"><a href="#TypeParser-919"><span class="linenos"> 919</span></a><span class="sd">			If the string represents a bool, it will be converted to `Decimal(1)` for True and `Decimal(0)` for False. If the string represents an int, it will be converted to a Decimal also.</span>
+</span><span id="TypeParser-890"><a href="#TypeParser-890"><span class="linenos"> 890</span></a><span class="sd">			`allow_inf`</span>
+</span><span id="TypeParser-891"><a href="#TypeParser-891"><span class="linenos"> 891</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.inf_values&lt;/code&gt; (empty set by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.float_case_sensitive&lt;/code&gt;, which is False by default.</span>
+</span><span id="TypeParser-892"><a href="#TypeParser-892"><span class="linenos"> 892</span></a>
+</span><span id="TypeParser-893"><a href="#TypeParser-893"><span class="linenos"> 893</span></a><span class="sd">			`allow_nan`</span>
+</span><span id="TypeParser-894"><a href="#TypeParser-894"><span class="linenos"> 894</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.nan_values&lt;/code&gt; (empty set by default) are interpeted as NaN. The case sensitivity of this matching also depends on &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.float_case_sensitive&lt;/code&gt;, which is False by default.</span>
+</span><span id="TypeParser-895"><a href="#TypeParser-895"><span class="linenos"> 895</span></a>
+</span><span id="TypeParser-896"><a href="#TypeParser-896"><span class="linenos"> 896</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-897"><a href="#TypeParser-897"><span class="linenos"> 897</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-898"><a href="#TypeParser-898"><span class="linenos"> 898</span></a><span class="sd">			parsed float value</span>
+</span><span id="TypeParser-899"><a href="#TypeParser-899"><span class="linenos"> 899</span></a>
+</span><span id="TypeParser-900"><a href="#TypeParser-900"><span class="linenos"> 900</span></a><span class="sd">			Raises</span>
+</span><span id="TypeParser-901"><a href="#TypeParser-901"><span class="linenos"> 901</span></a><span class="sd">			------</span>
+</span><span id="TypeParser-902"><a href="#TypeParser-902"><span class="linenos"> 902</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
+</span><span id="TypeParser-903"><a href="#TypeParser-903"><span class="linenos"> 903</span></a>
+</span><span id="TypeParser-904"><a href="#TypeParser-904"><span class="linenos"> 904</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-905"><a href="#TypeParser-905"><span class="linenos"> 905</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-906"><a href="#TypeParser-906"><span class="linenos"> 906</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-907"><a href="#TypeParser-907"><span class="linenos"> 907</span></a><span class="sd">			parser = TypeParser(inf_values=[&quot;inf&quot;], nan_values=[&quot;nan&quot;])</span>
+</span><span id="TypeParser-908"><a href="#TypeParser-908"><span class="linenos"> 908</span></a><span class="sd">			parser.parse_float(&quot;1.&quot;)       # 1.</span>
+</span><span id="TypeParser-909"><a href="#TypeParser-909"><span class="linenos"> 909</span></a><span class="sd">			parser.parse_float(&quot;1.23e2&quot;)   # 123.</span>
+</span><span id="TypeParser-910"><a href="#TypeParser-910"><span class="linenos"> 910</span></a><span class="sd">			parser.parse_float(&quot;1.23e-2&quot;)  # 0.0123</span>
+</span><span id="TypeParser-911"><a href="#TypeParser-911"><span class="linenos"> 911</span></a><span class="sd">			parser.parse_float(&quot;inf&quot;)      # math.inf</span>
+</span><span id="TypeParser-912"><a href="#TypeParser-912"><span class="linenos"> 912</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-913"><a href="#TypeParser-913"><span class="linenos"> 913</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-914"><a href="#TypeParser-914"><span class="linenos"> 914</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_parse_floatlike</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">math</span><span class="o">.</span><span class="n">inf</span><span class="p">,</span> <span class="n">math</span><span class="o">.</span><span class="n">nan</span><span class="p">,</span>
+</span><span id="TypeParser-915"><a href="#TypeParser-915"><span class="linenos"> 915</span></a>			<span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span>
+</span><span id="TypeParser-916"><a href="#TypeParser-916"><span class="linenos"> 916</span></a>			<span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span>
+</span><span id="TypeParser-917"><a href="#TypeParser-917"><span class="linenos"> 917</span></a>			<span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">,</span>
+</span><span id="TypeParser-918"><a href="#TypeParser-918"><span class="linenos"> 918</span></a>		<span class="p">)</span>
+</span><span id="TypeParser-919"><a href="#TypeParser-919"><span class="linenos"> 919</span></a>
 </span><span id="TypeParser-920"><a href="#TypeParser-920"><span class="linenos"> 920</span></a>
-</span><span id="TypeParser-921"><a href="#TypeParser-921"><span class="linenos"> 921</span></a><span class="sd">			Behaves analogously to `parse_float()`, except that that returns a non-exact float instead.</span>
-</span><span id="TypeParser-922"><a href="#TypeParser-922"><span class="linenos"> 922</span></a>
-</span><span id="TypeParser-923"><a href="#TypeParser-923"><span class="linenos"> 923</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser-924"><a href="#TypeParser-924"><span class="linenos"> 924</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser-925"><a href="#TypeParser-925"><span class="linenos"> 925</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-926"><a href="#TypeParser-926"><span class="linenos"> 926</span></a><span class="sd">			: string to be parsed</span>
-</span><span id="TypeParser-927"><a href="#TypeParser-927"><span class="linenos"> 927</span></a>
-</span><span id="TypeParser-928"><a href="#TypeParser-928"><span class="linenos"> 928</span></a><span class="sd">			Keyword arguments</span>
-</span><span id="TypeParser-929"><a href="#TypeParser-929"><span class="linenos"> 929</span></a><span class="sd">			-----------------</span>
-</span><span id="TypeParser-930"><a href="#TypeParser-930"><span class="linenos"> 930</span></a>
-</span><span id="TypeParser-931"><a href="#TypeParser-931"><span class="linenos"> 931</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser-932"><a href="#TypeParser-932"><span class="linenos"> 932</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
+</span><span id="TypeParser-921"><a href="#TypeParser-921"><span class="linenos"> 921</span></a>	<span class="k">def</span> <span class="nf">parse_decimal</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Decimal</span><span class="p">:</span>
+</span><span id="TypeParser-922"><a href="#TypeParser-922"><span class="linenos"> 922</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-923"><a href="#TypeParser-923"><span class="linenos"> 923</span></a><span class="sd">			Parse a string and return it as an exact Decimal if possible</span>
+</span><span id="TypeParser-924"><a href="#TypeParser-924"><span class="linenos"> 924</span></a>
+</span><span id="TypeParser-925"><a href="#TypeParser-925"><span class="linenos"> 925</span></a><span class="sd">			If the string represents a bool, it will be converted to `Decimal(1)` for True and `Decimal(0)` for False. If the string represents an int, it will be converted to a Decimal also.</span>
+</span><span id="TypeParser-926"><a href="#TypeParser-926"><span class="linenos"> 926</span></a>
+</span><span id="TypeParser-927"><a href="#TypeParser-927"><span class="linenos"> 927</span></a><span class="sd">			Behaves analogously to `parse_float()`, except that that returns a non-exact float instead.</span>
+</span><span id="TypeParser-928"><a href="#TypeParser-928"><span class="linenos"> 928</span></a>
+</span><span id="TypeParser-929"><a href="#TypeParser-929"><span class="linenos"> 929</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser-930"><a href="#TypeParser-930"><span class="linenos"> 930</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser-931"><a href="#TypeParser-931"><span class="linenos"> 931</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-932"><a href="#TypeParser-932"><span class="linenos"> 932</span></a><span class="sd">			: string to be parsed</span>
 </span><span id="TypeParser-933"><a href="#TypeParser-933"><span class="linenos"> 933</span></a>
-</span><span id="TypeParser-934"><a href="#TypeParser-934"><span class="linenos"> 934</span></a><span class="sd">			`allow_inf`</span>
-</span><span id="TypeParser-935"><a href="#TypeParser-935"><span class="linenos"> 935</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.inf_values&lt;/code&gt; (empty set by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.float_case_sensitive&lt;/code&gt;, which is False by default.</span>
+</span><span id="TypeParser-934"><a href="#TypeParser-934"><span class="linenos"> 934</span></a><span class="sd">			Keyword arguments</span>
+</span><span id="TypeParser-935"><a href="#TypeParser-935"><span class="linenos"> 935</span></a><span class="sd">			-----------------</span>
 </span><span id="TypeParser-936"><a href="#TypeParser-936"><span class="linenos"> 936</span></a>
-</span><span id="TypeParser-937"><a href="#TypeParser-937"><span class="linenos"> 937</span></a><span class="sd">			`allow_nan`</span>
-</span><span id="TypeParser-938"><a href="#TypeParser-938"><span class="linenos"> 938</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.nan_values&lt;/code&gt; (empty set by default) are interpeted as NaN. The case sensitivity of this matching also depends on &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.float_case_sensitive&lt;/code&gt;, which is False by default.</span>
+</span><span id="TypeParser-937"><a href="#TypeParser-937"><span class="linenos"> 937</span></a><span class="sd">			`allow_scientific`</span>
+</span><span id="TypeParser-938"><a href="#TypeParser-938"><span class="linenos"> 938</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
 </span><span id="TypeParser-939"><a href="#TypeParser-939"><span class="linenos"> 939</span></a>
-</span><span id="TypeParser-940"><a href="#TypeParser-940"><span class="linenos"> 940</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-941"><a href="#TypeParser-941"><span class="linenos"> 941</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-942"><a href="#TypeParser-942"><span class="linenos"> 942</span></a><span class="sd">			parsed Decimal value</span>
-</span><span id="TypeParser-943"><a href="#TypeParser-943"><span class="linenos"> 943</span></a>
-</span><span id="TypeParser-944"><a href="#TypeParser-944"><span class="linenos"> 944</span></a><span class="sd">			Raises</span>
-</span><span id="TypeParser-945"><a href="#TypeParser-945"><span class="linenos"> 945</span></a><span class="sd">			------</span>
-</span><span id="TypeParser-946"><a href="#TypeParser-946"><span class="linenos"> 946</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
-</span><span id="TypeParser-947"><a href="#TypeParser-947"><span class="linenos"> 947</span></a>
-</span><span id="TypeParser-948"><a href="#TypeParser-948"><span class="linenos"> 948</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-949"><a href="#TypeParser-949"><span class="linenos"> 949</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-950"><a href="#TypeParser-950"><span class="linenos"> 950</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-951"><a href="#TypeParser-951"><span class="linenos"> 951</span></a><span class="sd">			parser = TypeParser(inf_values=[&quot;inf&quot;], nan_values=[&quot;nan&quot;])</span>
-</span><span id="TypeParser-952"><a href="#TypeParser-952"><span class="linenos"> 952</span></a><span class="sd">			parser.parse_decimal(&quot;1.&quot;)       # Decimal(1)</span>
-</span><span id="TypeParser-953"><a href="#TypeParser-953"><span class="linenos"> 953</span></a><span class="sd">			parser.parse_decimal(&quot;1.23e2&quot;)   # Decimal(123)</span>
-</span><span id="TypeParser-954"><a href="#TypeParser-954"><span class="linenos"> 954</span></a><span class="sd">			parser.parse_decimal(&quot;1.23e-2&quot;)  # Decimal(123) / Decimal(10000)</span>
-</span><span id="TypeParser-955"><a href="#TypeParser-955"><span class="linenos"> 955</span></a><span class="sd">			parser.parse_decimal(&quot;inf&quot;)      # Decimal(math.inf)</span>
-</span><span id="TypeParser-956"><a href="#TypeParser-956"><span class="linenos"> 956</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-957"><a href="#TypeParser-957"><span class="linenos"> 957</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-958"><a href="#TypeParser-958"><span class="linenos"> 958</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_parse_floatlike</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">Decimal</span><span class="p">,</span> <span class="n">Decimal</span><span class="p">(</span><span class="n">math</span><span class="o">.</span><span class="n">inf</span><span class="p">),</span> <span class="n">Decimal</span><span class="p">(</span><span class="n">math</span><span class="o">.</span><span class="n">nan</span><span class="p">),</span>
-</span><span id="TypeParser-959"><a href="#TypeParser-959"><span class="linenos"> 959</span></a>			<span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span>
-</span><span id="TypeParser-960"><a href="#TypeParser-960"><span class="linenos"> 960</span></a>			<span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span>
-</span><span id="TypeParser-961"><a href="#TypeParser-961"><span class="linenos"> 961</span></a>			<span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">,</span>
-</span><span id="TypeParser-962"><a href="#TypeParser-962"><span class="linenos"> 962</span></a>		<span class="p">)</span>
-</span><span id="TypeParser-963"><a href="#TypeParser-963"><span class="linenos"> 963</span></a>
-</span><span id="TypeParser-964"><a href="#TypeParser-964"><span class="linenos"> 964</span></a>
-</span><span id="TypeParser-965"><a href="#TypeParser-965"><span class="linenos"> 965</span></a>	<span class="k">def</span> <span class="nf">infer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
-</span><span id="TypeParser-966"><a href="#TypeParser-966"><span class="linenos"> 966</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-967"><a href="#TypeParser-967"><span class="linenos"> 967</span></a><span class="sd">			Infer the underlying type of a string</span>
-</span><span id="TypeParser-968"><a href="#TypeParser-968"><span class="linenos"> 968</span></a>
-</span><span id="TypeParser-969"><a href="#TypeParser-969"><span class="linenos"> 969</span></a><span class="sd">			Also check for inline lists if &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.list_delimiter&lt;/code&gt; is not None.</span>
+</span><span id="TypeParser-940"><a href="#TypeParser-940"><span class="linenos"> 940</span></a><span class="sd">			`allow_inf`</span>
+</span><span id="TypeParser-941"><a href="#TypeParser-941"><span class="linenos"> 941</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.inf_values&lt;/code&gt; (empty set by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.float_case_sensitive&lt;/code&gt;, which is False by default.</span>
+</span><span id="TypeParser-942"><a href="#TypeParser-942"><span class="linenos"> 942</span></a>
+</span><span id="TypeParser-943"><a href="#TypeParser-943"><span class="linenos"> 943</span></a><span class="sd">			`allow_nan`</span>
+</span><span id="TypeParser-944"><a href="#TypeParser-944"><span class="linenos"> 944</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.nan_values&lt;/code&gt; (empty set by default) are interpeted as NaN. The case sensitivity of this matching also depends on &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.float_case_sensitive&lt;/code&gt;, which is False by default.</span>
+</span><span id="TypeParser-945"><a href="#TypeParser-945"><span class="linenos"> 945</span></a>
+</span><span id="TypeParser-946"><a href="#TypeParser-946"><span class="linenos"> 946</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-947"><a href="#TypeParser-947"><span class="linenos"> 947</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-948"><a href="#TypeParser-948"><span class="linenos"> 948</span></a><span class="sd">			parsed Decimal value</span>
+</span><span id="TypeParser-949"><a href="#TypeParser-949"><span class="linenos"> 949</span></a>
+</span><span id="TypeParser-950"><a href="#TypeParser-950"><span class="linenos"> 950</span></a><span class="sd">			Raises</span>
+</span><span id="TypeParser-951"><a href="#TypeParser-951"><span class="linenos"> 951</span></a><span class="sd">			------</span>
+</span><span id="TypeParser-952"><a href="#TypeParser-952"><span class="linenos"> 952</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
+</span><span id="TypeParser-953"><a href="#TypeParser-953"><span class="linenos"> 953</span></a>
+</span><span id="TypeParser-954"><a href="#TypeParser-954"><span class="linenos"> 954</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-955"><a href="#TypeParser-955"><span class="linenos"> 955</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-956"><a href="#TypeParser-956"><span class="linenos"> 956</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-957"><a href="#TypeParser-957"><span class="linenos"> 957</span></a><span class="sd">			parser = TypeParser(inf_values=[&quot;inf&quot;], nan_values=[&quot;nan&quot;])</span>
+</span><span id="TypeParser-958"><a href="#TypeParser-958"><span class="linenos"> 958</span></a><span class="sd">			parser.parse_decimal(&quot;1.&quot;)       # Decimal(1)</span>
+</span><span id="TypeParser-959"><a href="#TypeParser-959"><span class="linenos"> 959</span></a><span class="sd">			parser.parse_decimal(&quot;1.23e2&quot;)   # Decimal(123)</span>
+</span><span id="TypeParser-960"><a href="#TypeParser-960"><span class="linenos"> 960</span></a><span class="sd">			parser.parse_decimal(&quot;1.23e-2&quot;)  # Decimal(123) / Decimal(10000)</span>
+</span><span id="TypeParser-961"><a href="#TypeParser-961"><span class="linenos"> 961</span></a><span class="sd">			parser.parse_decimal(&quot;inf&quot;)      # Decimal(math.inf)</span>
+</span><span id="TypeParser-962"><a href="#TypeParser-962"><span class="linenos"> 962</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-963"><a href="#TypeParser-963"><span class="linenos"> 963</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-964"><a href="#TypeParser-964"><span class="linenos"> 964</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_parse_floatlike</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">Decimal</span><span class="p">,</span> <span class="n">Decimal</span><span class="p">(</span><span class="n">math</span><span class="o">.</span><span class="n">inf</span><span class="p">),</span> <span class="n">Decimal</span><span class="p">(</span><span class="n">math</span><span class="o">.</span><span class="n">nan</span><span class="p">),</span>
+</span><span id="TypeParser-965"><a href="#TypeParser-965"><span class="linenos"> 965</span></a>			<span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span>
+</span><span id="TypeParser-966"><a href="#TypeParser-966"><span class="linenos"> 966</span></a>			<span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span>
+</span><span id="TypeParser-967"><a href="#TypeParser-967"><span class="linenos"> 967</span></a>			<span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">,</span>
+</span><span id="TypeParser-968"><a href="#TypeParser-968"><span class="linenos"> 968</span></a>		<span class="p">)</span>
+</span><span id="TypeParser-969"><a href="#TypeParser-969"><span class="linenos"> 969</span></a>
 </span><span id="TypeParser-970"><a href="#TypeParser-970"><span class="linenos"> 970</span></a>
-</span><span id="TypeParser-971"><a href="#TypeParser-971"><span class="linenos"> 971</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser-972"><a href="#TypeParser-972"><span class="linenos"> 972</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser-973"><a href="#TypeParser-973"><span class="linenos"> 973</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-974"><a href="#TypeParser-974"><span class="linenos"> 974</span></a><span class="sd">			: the string for which the type should be inferred</span>
-</span><span id="TypeParser-975"><a href="#TypeParser-975"><span class="linenos"> 975</span></a>
-</span><span id="TypeParser-976"><a href="#TypeParser-976"><span class="linenos"> 976</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-977"><a href="#TypeParser-977"><span class="linenos"> 977</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-978"><a href="#TypeParser-978"><span class="linenos"> 978</span></a><span class="sd">			inferred type</span>
-</span><span id="TypeParser-979"><a href="#TypeParser-979"><span class="linenos"> 979</span></a>
-</span><span id="TypeParser-980"><a href="#TypeParser-980"><span class="linenos"> 980</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-981"><a href="#TypeParser-981"><span class="linenos"> 981</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-982"><a href="#TypeParser-982"><span class="linenos"> 982</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-983"><a href="#TypeParser-983"><span class="linenos"> 983</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-984"><a href="#TypeParser-984"><span class="linenos"> 984</span></a><span class="sd">			parser.infer(&quot;true&quot;)  # bool</span>
-</span><span id="TypeParser-985"><a href="#TypeParser-985"><span class="linenos"> 985</span></a><span class="sd">			parser.infer(&quot;2.0&quot;)   # float</span>
-</span><span id="TypeParser-986"><a href="#TypeParser-986"><span class="linenos"> 986</span></a><span class="sd">			parser.infer(&quot;abc&quot;)   # str</span>
-</span><span id="TypeParser-987"><a href="#TypeParser-987"><span class="linenos"> 987</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-988"><a href="#TypeParser-988"><span class="linenos"> 988</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-989"><a href="#TypeParser-989"><span class="linenos"> 989</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser-990"><a href="#TypeParser-990"><span class="linenos"> 990</span></a>			<span class="k">return</span> <span class="n">NoneType</span>
-</span><span id="TypeParser-991"><a href="#TypeParser-991"><span class="linenos"> 991</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser-992"><a href="#TypeParser-992"><span class="linenos"> 992</span></a>			<span class="k">return</span> <span class="nb">bool</span>
-</span><span id="TypeParser-993"><a href="#TypeParser-993"><span class="linenos"> 993</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser-994"><a href="#TypeParser-994"><span class="linenos"> 994</span></a>			<span class="k">return</span> <span class="nb">int</span>
-</span><span id="TypeParser-995"><a href="#TypeParser-995"><span class="linenos"> 995</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser-996"><a href="#TypeParser-996"><span class="linenos"> 996</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_use_decimal</span><span class="p">:</span>
-</span><span id="TypeParser-997"><a href="#TypeParser-997"><span class="linenos"> 997</span></a>				<span class="k">return</span> <span class="n">Decimal</span>
-</span><span id="TypeParser-998"><a href="#TypeParser-998"><span class="linenos"> 998</span></a>			<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-999"><a href="#TypeParser-999"><span class="linenos"> 999</span></a>				<span class="k">return</span> <span class="nb">float</span>
-</span><span id="TypeParser-1000"><a href="#TypeParser-1000"><span class="linenos">1000</span></a>
-</span><span id="TypeParser-1001"><a href="#TypeParser-1001"><span class="linenos">1001</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
-</span><span id="TypeParser-1002"><a href="#TypeParser-1002"><span class="linenos">1002</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="TypeParser-1003"><a href="#TypeParser-1003"><span class="linenos">1003</span></a>
-</span><span id="TypeParser-1004"><a href="#TypeParser-1004"><span class="linenos">1004</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_list_delimiter</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">_list_delimiter</span> <span class="ow">in</span> <span class="n">value</span><span class="p">:</span>
-</span><span id="TypeParser-1005"><a href="#TypeParser-1005"><span class="linenos">1005</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_list_delimiter</span><span class="p">)</span>
-</span><span id="TypeParser-1006"><a href="#TypeParser-1006"><span class="linenos">1006</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
-</span><span id="TypeParser-1007"><a href="#TypeParser-1007"><span class="linenos">1007</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
-</span><span id="TypeParser-1008"><a href="#TypeParser-1008"><span class="linenos">1008</span></a>			<span class="n">reduced_type</span> <span class="o">=</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">subvalue</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">)</span>
-</span><span id="TypeParser-1009"><a href="#TypeParser-1009"><span class="linenos">1009</span></a>			<span class="n">r</span> <span class="o">=</span> <span class="nb">list</span><span class="p">[</span><span class="n">reduced_type</span><span class="p">]</span>
-</span><span id="TypeParser-1010"><a href="#TypeParser-1010"><span class="linenos">1010</span></a>			<span class="k">return</span> <span class="n">r</span>
-</span><span id="TypeParser-1011"><a href="#TypeParser-1011"><span class="linenos">1011</span></a>
-</span><span id="TypeParser-1012"><a href="#TypeParser-1012"><span class="linenos">1012</span></a>		<span class="k">return</span> <span class="n">GenericValue</span>
-</span><span id="TypeParser-1013"><a href="#TypeParser-1013"><span class="linenos">1013</span></a>
-</span><span id="TypeParser-1014"><a href="#TypeParser-1014"><span class="linenos">1014</span></a>
-</span><span id="TypeParser-1015"><a href="#TypeParser-1015"><span class="linenos">1015</span></a>	<span class="k">def</span> <span class="nf">infer_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
-</span><span id="TypeParser-1016"><a href="#TypeParser-1016"><span class="linenos">1016</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-1017"><a href="#TypeParser-1017"><span class="linenos">1017</span></a><span class="sd">			Infer the underlying common type of a series of strings</span>
-</span><span id="TypeParser-1018"><a href="#TypeParser-1018"><span class="linenos">1018</span></a>
-</span><span id="TypeParser-1019"><a href="#TypeParser-1019"><span class="linenos">1019</span></a><span class="sd">			If the values in the series do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-971"><a href="#TypeParser-971"><span class="linenos"> 971</span></a>	<span class="k">def</span> <span class="nf">infer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
+</span><span id="TypeParser-972"><a href="#TypeParser-972"><span class="linenos"> 972</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-973"><a href="#TypeParser-973"><span class="linenos"> 973</span></a><span class="sd">			Infer the underlying type of a string</span>
+</span><span id="TypeParser-974"><a href="#TypeParser-974"><span class="linenos"> 974</span></a>
+</span><span id="TypeParser-975"><a href="#TypeParser-975"><span class="linenos"> 975</span></a><span class="sd">			Also check for inline lists if &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.list_delimiter&lt;/code&gt; is not None.</span>
+</span><span id="TypeParser-976"><a href="#TypeParser-976"><span class="linenos"> 976</span></a>
+</span><span id="TypeParser-977"><a href="#TypeParser-977"><span class="linenos"> 977</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser-978"><a href="#TypeParser-978"><span class="linenos"> 978</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser-979"><a href="#TypeParser-979"><span class="linenos"> 979</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-980"><a href="#TypeParser-980"><span class="linenos"> 980</span></a><span class="sd">			: the string for which the type should be inferred</span>
+</span><span id="TypeParser-981"><a href="#TypeParser-981"><span class="linenos"> 981</span></a>
+</span><span id="TypeParser-982"><a href="#TypeParser-982"><span class="linenos"> 982</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-983"><a href="#TypeParser-983"><span class="linenos"> 983</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-984"><a href="#TypeParser-984"><span class="linenos"> 984</span></a><span class="sd">			inferred type</span>
+</span><span id="TypeParser-985"><a href="#TypeParser-985"><span class="linenos"> 985</span></a>
+</span><span id="TypeParser-986"><a href="#TypeParser-986"><span class="linenos"> 986</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-987"><a href="#TypeParser-987"><span class="linenos"> 987</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-988"><a href="#TypeParser-988"><span class="linenos"> 988</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-989"><a href="#TypeParser-989"><span class="linenos"> 989</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-990"><a href="#TypeParser-990"><span class="linenos"> 990</span></a><span class="sd">			parser.infer(&quot;true&quot;)  # bool</span>
+</span><span id="TypeParser-991"><a href="#TypeParser-991"><span class="linenos"> 991</span></a><span class="sd">			parser.infer(&quot;2.0&quot;)   # float</span>
+</span><span id="TypeParser-992"><a href="#TypeParser-992"><span class="linenos"> 992</span></a><span class="sd">			parser.infer(&quot;abc&quot;)   # str</span>
+</span><span id="TypeParser-993"><a href="#TypeParser-993"><span class="linenos"> 993</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-994"><a href="#TypeParser-994"><span class="linenos"> 994</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-995"><a href="#TypeParser-995"><span class="linenos"> 995</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser-996"><a href="#TypeParser-996"><span class="linenos"> 996</span></a>			<span class="k">return</span> <span class="n">NoneType</span>
+</span><span id="TypeParser-997"><a href="#TypeParser-997"><span class="linenos"> 997</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser-998"><a href="#TypeParser-998"><span class="linenos"> 998</span></a>			<span class="k">return</span> <span class="nb">bool</span>
+</span><span id="TypeParser-999"><a href="#TypeParser-999"><span class="linenos"> 999</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser-1000"><a href="#TypeParser-1000"><span class="linenos">1000</span></a>			<span class="k">return</span> <span class="nb">int</span>
+</span><span id="TypeParser-1001"><a href="#TypeParser-1001"><span class="linenos">1001</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser-1002"><a href="#TypeParser-1002"><span class="linenos">1002</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_use_decimal</span><span class="p">:</span>
+</span><span id="TypeParser-1003"><a href="#TypeParser-1003"><span class="linenos">1003</span></a>				<span class="k">return</span> <span class="n">Decimal</span>
+</span><span id="TypeParser-1004"><a href="#TypeParser-1004"><span class="linenos">1004</span></a>			<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-1005"><a href="#TypeParser-1005"><span class="linenos">1005</span></a>				<span class="k">return</span> <span class="nb">float</span>
+</span><span id="TypeParser-1006"><a href="#TypeParser-1006"><span class="linenos">1006</span></a>
+</span><span id="TypeParser-1007"><a href="#TypeParser-1007"><span class="linenos">1007</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
+</span><span id="TypeParser-1008"><a href="#TypeParser-1008"><span class="linenos">1008</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="TypeParser-1009"><a href="#TypeParser-1009"><span class="linenos">1009</span></a>
+</span><span id="TypeParser-1010"><a href="#TypeParser-1010"><span class="linenos">1010</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_list_delimiter</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">_list_delimiter</span> <span class="ow">in</span> <span class="n">value</span><span class="p">:</span>
+</span><span id="TypeParser-1011"><a href="#TypeParser-1011"><span class="linenos">1011</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_list_delimiter</span><span class="p">)</span>
+</span><span id="TypeParser-1012"><a href="#TypeParser-1012"><span class="linenos">1012</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
+</span><span id="TypeParser-1013"><a href="#TypeParser-1013"><span class="linenos">1013</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
+</span><span id="TypeParser-1014"><a href="#TypeParser-1014"><span class="linenos">1014</span></a>			<span class="n">reduced_type</span> <span class="o">=</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">subvalue</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">)</span>
+</span><span id="TypeParser-1015"><a href="#TypeParser-1015"><span class="linenos">1015</span></a>			<span class="n">r</span> <span class="o">=</span> <span class="nb">list</span><span class="p">[</span><span class="n">reduced_type</span><span class="p">]</span>
+</span><span id="TypeParser-1016"><a href="#TypeParser-1016"><span class="linenos">1016</span></a>			<span class="k">return</span> <span class="n">r</span>
+</span><span id="TypeParser-1017"><a href="#TypeParser-1017"><span class="linenos">1017</span></a>
+</span><span id="TypeParser-1018"><a href="#TypeParser-1018"><span class="linenos">1018</span></a>		<span class="k">return</span> <span class="n">GenericValue</span>
+</span><span id="TypeParser-1019"><a href="#TypeParser-1019"><span class="linenos">1019</span></a>
 </span><span id="TypeParser-1020"><a href="#TypeParser-1020"><span class="linenos">1020</span></a>
-</span><span id="TypeParser-1021"><a href="#TypeParser-1021"><span class="linenos">1021</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser-1022"><a href="#TypeParser-1022"><span class="linenos">1022</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser-1023"><a href="#TypeParser-1023"><span class="linenos">1023</span></a><span class="sd">			`values`</span>
-</span><span id="TypeParser-1024"><a href="#TypeParser-1024"><span class="linenos">1024</span></a><span class="sd">			: series of strings for which the type should be inferred</span>
-</span><span id="TypeParser-1025"><a href="#TypeParser-1025"><span class="linenos">1025</span></a>
-</span><span id="TypeParser-1026"><a href="#TypeParser-1026"><span class="linenos">1026</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-1027"><a href="#TypeParser-1027"><span class="linenos">1027</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-1028"><a href="#TypeParser-1028"><span class="linenos">1028</span></a><span class="sd">			inferred type</span>
-</span><span id="TypeParser-1029"><a href="#TypeParser-1029"><span class="linenos">1029</span></a>
-</span><span id="TypeParser-1030"><a href="#TypeParser-1030"><span class="linenos">1030</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-1031"><a href="#TypeParser-1031"><span class="linenos">1031</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-1032"><a href="#TypeParser-1032"><span class="linenos">1032</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-1033"><a href="#TypeParser-1033"><span class="linenos">1033</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-1034"><a href="#TypeParser-1034"><span class="linenos">1034</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2&quot;, &quot;3.4&quot;])       # float</span>
-</span><span id="TypeParser-1035"><a href="#TypeParser-1035"><span class="linenos">1035</span></a><span class="sd">			parser.infer_series([&quot;true&quot;, &quot;false&quot;, &quot;2&quot;])  # int</span>
-</span><span id="TypeParser-1036"><a href="#TypeParser-1036"><span class="linenos">1036</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])     # str</span>
-</span><span id="TypeParser-1037"><a href="#TypeParser-1037"><span class="linenos">1037</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-1038"><a href="#TypeParser-1038"><span class="linenos">1038</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-1039"><a href="#TypeParser-1039"><span class="linenos">1039</span></a>		<span class="k">return</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="TypeParser-1040"><a href="#TypeParser-1040"><span class="linenos">1040</span></a>
-</span><span id="TypeParser-1041"><a href="#TypeParser-1041"><span class="linenos">1041</span></a>
-</span><span id="TypeParser-1042"><a href="#TypeParser-1042"><span class="linenos">1042</span></a>	<span class="k">def</span> <span class="nf">infer_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValueType</span><span class="p">]:</span>
-</span><span id="TypeParser-1043"><a href="#TypeParser-1043"><span class="linenos">1043</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-1044"><a href="#TypeParser-1044"><span class="linenos">1044</span></a><span class="sd">			Infer the underlying common type for each column of a table of strings</span>
-</span><span id="TypeParser-1045"><a href="#TypeParser-1045"><span class="linenos">1045</span></a>
-</span><span id="TypeParser-1046"><a href="#TypeParser-1046"><span class="linenos">1046</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-1021"><a href="#TypeParser-1021"><span class="linenos">1021</span></a>	<span class="k">def</span> <span class="nf">infer_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
+</span><span id="TypeParser-1022"><a href="#TypeParser-1022"><span class="linenos">1022</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-1023"><a href="#TypeParser-1023"><span class="linenos">1023</span></a><span class="sd">			Infer the underlying common type of a series of strings</span>
+</span><span id="TypeParser-1024"><a href="#TypeParser-1024"><span class="linenos">1024</span></a>
+</span><span id="TypeParser-1025"><a href="#TypeParser-1025"><span class="linenos">1025</span></a><span class="sd">			If the values in the series do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-1026"><a href="#TypeParser-1026"><span class="linenos">1026</span></a>
+</span><span id="TypeParser-1027"><a href="#TypeParser-1027"><span class="linenos">1027</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser-1028"><a href="#TypeParser-1028"><span class="linenos">1028</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser-1029"><a href="#TypeParser-1029"><span class="linenos">1029</span></a><span class="sd">			`values`</span>
+</span><span id="TypeParser-1030"><a href="#TypeParser-1030"><span class="linenos">1030</span></a><span class="sd">			: series of strings for which the type should be inferred</span>
+</span><span id="TypeParser-1031"><a href="#TypeParser-1031"><span class="linenos">1031</span></a>
+</span><span id="TypeParser-1032"><a href="#TypeParser-1032"><span class="linenos">1032</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-1033"><a href="#TypeParser-1033"><span class="linenos">1033</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-1034"><a href="#TypeParser-1034"><span class="linenos">1034</span></a><span class="sd">			inferred type</span>
+</span><span id="TypeParser-1035"><a href="#TypeParser-1035"><span class="linenos">1035</span></a>
+</span><span id="TypeParser-1036"><a href="#TypeParser-1036"><span class="linenos">1036</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-1037"><a href="#TypeParser-1037"><span class="linenos">1037</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-1038"><a href="#TypeParser-1038"><span class="linenos">1038</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-1039"><a href="#TypeParser-1039"><span class="linenos">1039</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-1040"><a href="#TypeParser-1040"><span class="linenos">1040</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2&quot;, &quot;3.4&quot;])       # float</span>
+</span><span id="TypeParser-1041"><a href="#TypeParser-1041"><span class="linenos">1041</span></a><span class="sd">			parser.infer_series([&quot;true&quot;, &quot;false&quot;, &quot;2&quot;])  # int</span>
+</span><span id="TypeParser-1042"><a href="#TypeParser-1042"><span class="linenos">1042</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])     # str</span>
+</span><span id="TypeParser-1043"><a href="#TypeParser-1043"><span class="linenos">1043</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-1044"><a href="#TypeParser-1044"><span class="linenos">1044</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-1045"><a href="#TypeParser-1045"><span class="linenos">1045</span></a>		<span class="k">return</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="TypeParser-1046"><a href="#TypeParser-1046"><span class="linenos">1046</span></a>
 </span><span id="TypeParser-1047"><a href="#TypeParser-1047"><span class="linenos">1047</span></a>
-</span><span id="TypeParser-1048"><a href="#TypeParser-1048"><span class="linenos">1048</span></a><span class="sd">			Note that the individual inferred types of every value in the table must be able to fit into memory.</span>
-</span><span id="TypeParser-1049"><a href="#TypeParser-1049"><span class="linenos">1049</span></a>
-</span><span id="TypeParser-1050"><a href="#TypeParser-1050"><span class="linenos">1050</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser-1051"><a href="#TypeParser-1051"><span class="linenos">1051</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser-1052"><a href="#TypeParser-1052"><span class="linenos">1052</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser-1053"><a href="#TypeParser-1053"><span class="linenos">1053</span></a><span class="sd">			: table of strings for which the types should be inferred, in row-major order</span>
-</span><span id="TypeParser-1054"><a href="#TypeParser-1054"><span class="linenos">1054</span></a>
-</span><span id="TypeParser-1055"><a href="#TypeParser-1055"><span class="linenos">1055</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-1056"><a href="#TypeParser-1056"><span class="linenos">1056</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-1057"><a href="#TypeParser-1057"><span class="linenos">1057</span></a><span class="sd">			inferred types</span>
-</span><span id="TypeParser-1058"><a href="#TypeParser-1058"><span class="linenos">1058</span></a>
-</span><span id="TypeParser-1059"><a href="#TypeParser-1059"><span class="linenos">1059</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-1060"><a href="#TypeParser-1060"><span class="linenos">1060</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-1061"><a href="#TypeParser-1061"><span class="linenos">1061</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-1062"><a href="#TypeParser-1062"><span class="linenos">1062</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-1063"><a href="#TypeParser-1063"><span class="linenos">1063</span></a><span class="sd">			parser.infer_table([</span>
-</span><span id="TypeParser-1064"><a href="#TypeParser-1064"><span class="linenos">1064</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser-1065"><a href="#TypeParser-1065"><span class="linenos">1065</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser-1066"><a href="#TypeParser-1066"><span class="linenos">1066</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
-</span><span id="TypeParser-1067"><a href="#TypeParser-1067"><span class="linenos">1067</span></a><span class="sd">			])</span>
-</span><span id="TypeParser-1068"><a href="#TypeParser-1068"><span class="linenos">1068</span></a><span class="sd">			# [float, int, str]</span>
-</span><span id="TypeParser-1069"><a href="#TypeParser-1069"><span class="linenos">1069</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-1070"><a href="#TypeParser-1070"><span class="linenos">1070</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-1071"><a href="#TypeParser-1071"><span class="linenos">1071</span></a>		<span class="n">rows_iter</span> <span class="o">=</span> <span class="nb">iter</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
-</span><span id="TypeParser-1072"><a href="#TypeParser-1072"><span class="linenos">1072</span></a>		<span class="n">first_row</span> <span class="o">=</span> <span class="nb">next</span><span class="p">(</span><span class="n">rows_iter</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
-</span><span id="TypeParser-1073"><a href="#TypeParser-1073"><span class="linenos">1073</span></a>		<span class="k">if</span> <span class="n">first_row</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="TypeParser-1074"><a href="#TypeParser-1074"><span class="linenos">1074</span></a>			<span class="k">return</span> <span class="p">[]</span>
-</span><span id="TypeParser-1075"><a href="#TypeParser-1075"><span class="linenos">1075</span></a>
-</span><span id="TypeParser-1076"><a href="#TypeParser-1076"><span class="linenos">1076</span></a>		<span class="n">num_cols</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">first_row</span><span class="p">)</span>
-</span><span id="TypeParser-1077"><a href="#TypeParser-1077"><span class="linenos">1077</span></a>		<span class="k">if</span> <span class="n">num_cols</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="TypeParser-1078"><a href="#TypeParser-1078"><span class="linenos">1078</span></a>			<span class="k">return</span> <span class="p">[]</span>
-</span><span id="TypeParser-1079"><a href="#TypeParser-1079"><span class="linenos">1079</span></a>
-</span><span id="TypeParser-1080"><a href="#TypeParser-1080"><span class="linenos">1080</span></a>		<span class="n">table</span> <span class="o">=</span> <span class="n">_TypeTable</span><span class="p">([[</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)]</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">first_row</span><span class="p">])</span>
-</span><span id="TypeParser-1081"><a href="#TypeParser-1081"><span class="linenos">1081</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows_iter</span><span class="p">:</span>
-</span><span id="TypeParser-1082"><a href="#TypeParser-1082"><span class="linenos">1082</span></a>			<span class="n">table</span><span class="o">.</span><span class="n">add_row</span><span class="p">([</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">row</span><span class="p">])</span>
-</span><span id="TypeParser-1083"><a href="#TypeParser-1083"><span class="linenos">1083</span></a>
-</span><span id="TypeParser-1084"><a href="#TypeParser-1084"><span class="linenos">1084</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">reduce_types</span><span class="p">(</span><span class="n">col</span><span class="p">)</span> <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="n">table</span><span class="o">.</span><span class="n">cols</span><span class="p">]</span>
+</span><span id="TypeParser-1048"><a href="#TypeParser-1048"><span class="linenos">1048</span></a>	<span class="k">def</span> <span class="nf">infer_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValueType</span><span class="p">]:</span>
+</span><span id="TypeParser-1049"><a href="#TypeParser-1049"><span class="linenos">1049</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-1050"><a href="#TypeParser-1050"><span class="linenos">1050</span></a><span class="sd">			Infer the underlying common type for each column of a table of strings</span>
+</span><span id="TypeParser-1051"><a href="#TypeParser-1051"><span class="linenos">1051</span></a>
+</span><span id="TypeParser-1052"><a href="#TypeParser-1052"><span class="linenos">1052</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-1053"><a href="#TypeParser-1053"><span class="linenos">1053</span></a>
+</span><span id="TypeParser-1054"><a href="#TypeParser-1054"><span class="linenos">1054</span></a><span class="sd">			Note that the individual inferred types of every value in the table must be able to fit into memory.</span>
+</span><span id="TypeParser-1055"><a href="#TypeParser-1055"><span class="linenos">1055</span></a>
+</span><span id="TypeParser-1056"><a href="#TypeParser-1056"><span class="linenos">1056</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser-1057"><a href="#TypeParser-1057"><span class="linenos">1057</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser-1058"><a href="#TypeParser-1058"><span class="linenos">1058</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser-1059"><a href="#TypeParser-1059"><span class="linenos">1059</span></a><span class="sd">			: table of strings for which the types should be inferred, in row-major order</span>
+</span><span id="TypeParser-1060"><a href="#TypeParser-1060"><span class="linenos">1060</span></a>
+</span><span id="TypeParser-1061"><a href="#TypeParser-1061"><span class="linenos">1061</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-1062"><a href="#TypeParser-1062"><span class="linenos">1062</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-1063"><a href="#TypeParser-1063"><span class="linenos">1063</span></a><span class="sd">			inferred types</span>
+</span><span id="TypeParser-1064"><a href="#TypeParser-1064"><span class="linenos">1064</span></a>
+</span><span id="TypeParser-1065"><a href="#TypeParser-1065"><span class="linenos">1065</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-1066"><a href="#TypeParser-1066"><span class="linenos">1066</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-1067"><a href="#TypeParser-1067"><span class="linenos">1067</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-1068"><a href="#TypeParser-1068"><span class="linenos">1068</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-1069"><a href="#TypeParser-1069"><span class="linenos">1069</span></a><span class="sd">			parser.infer_table([</span>
+</span><span id="TypeParser-1070"><a href="#TypeParser-1070"><span class="linenos">1070</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser-1071"><a href="#TypeParser-1071"><span class="linenos">1071</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser-1072"><a href="#TypeParser-1072"><span class="linenos">1072</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
+</span><span id="TypeParser-1073"><a href="#TypeParser-1073"><span class="linenos">1073</span></a><span class="sd">			])</span>
+</span><span id="TypeParser-1074"><a href="#TypeParser-1074"><span class="linenos">1074</span></a><span class="sd">			# [float, int, str]</span>
+</span><span id="TypeParser-1075"><a href="#TypeParser-1075"><span class="linenos">1075</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-1076"><a href="#TypeParser-1076"><span class="linenos">1076</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-1077"><a href="#TypeParser-1077"><span class="linenos">1077</span></a>		<span class="n">rows_iter</span> <span class="o">=</span> <span class="nb">iter</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
+</span><span id="TypeParser-1078"><a href="#TypeParser-1078"><span class="linenos">1078</span></a>		<span class="n">first_row</span> <span class="o">=</span> <span class="nb">next</span><span class="p">(</span><span class="n">rows_iter</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
+</span><span id="TypeParser-1079"><a href="#TypeParser-1079"><span class="linenos">1079</span></a>		<span class="k">if</span> <span class="n">first_row</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="TypeParser-1080"><a href="#TypeParser-1080"><span class="linenos">1080</span></a>			<span class="k">return</span> <span class="p">[]</span>
+</span><span id="TypeParser-1081"><a href="#TypeParser-1081"><span class="linenos">1081</span></a>
+</span><span id="TypeParser-1082"><a href="#TypeParser-1082"><span class="linenos">1082</span></a>		<span class="n">num_cols</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">first_row</span><span class="p">)</span>
+</span><span id="TypeParser-1083"><a href="#TypeParser-1083"><span class="linenos">1083</span></a>		<span class="k">if</span> <span class="n">num_cols</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="TypeParser-1084"><a href="#TypeParser-1084"><span class="linenos">1084</span></a>			<span class="k">return</span> <span class="p">[]</span>
 </span><span id="TypeParser-1085"><a href="#TypeParser-1085"><span class="linenos">1085</span></a>
-</span><span id="TypeParser-1086"><a href="#TypeParser-1086"><span class="linenos">1086</span></a>
-</span><span id="TypeParser-1087"><a href="#TypeParser-1087"><span class="linenos">1087</span></a>	<span class="k">def</span> <span class="nf">convert</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_type</span><span class="p">:</span> <span class="n">AnyValueType</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
-</span><span id="TypeParser-1088"><a href="#TypeParser-1088"><span class="linenos">1088</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-1089"><a href="#TypeParser-1089"><span class="linenos">1089</span></a><span class="sd">			Convert a string to the specified target type if possible</span>
-</span><span id="TypeParser-1090"><a href="#TypeParser-1090"><span class="linenos">1090</span></a>
-</span><span id="TypeParser-1091"><a href="#TypeParser-1091"><span class="linenos">1091</span></a><span class="sd">			Valid values for `target_type` include any return value from `infer()`, `infer_series()` and `infer_table()`. To infer and convert the string automatically, use `parse()`, `parse_series()` or `parse_table()` instead.</span>
+</span><span id="TypeParser-1086"><a href="#TypeParser-1086"><span class="linenos">1086</span></a>		<span class="n">table</span> <span class="o">=</span> <span class="n">_TypeTable</span><span class="p">([[</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)]</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">first_row</span><span class="p">])</span>
+</span><span id="TypeParser-1087"><a href="#TypeParser-1087"><span class="linenos">1087</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows_iter</span><span class="p">:</span>
+</span><span id="TypeParser-1088"><a href="#TypeParser-1088"><span class="linenos">1088</span></a>			<span class="n">table</span><span class="o">.</span><span class="n">add_row</span><span class="p">([</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">row</span><span class="p">])</span>
+</span><span id="TypeParser-1089"><a href="#TypeParser-1089"><span class="linenos">1089</span></a>
+</span><span id="TypeParser-1090"><a href="#TypeParser-1090"><span class="linenos">1090</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">reduce_types</span><span class="p">(</span><span class="n">col</span><span class="p">)</span> <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="n">table</span><span class="o">.</span><span class="n">cols</span><span class="p">]</span>
+</span><span id="TypeParser-1091"><a href="#TypeParser-1091"><span class="linenos">1091</span></a>
 </span><span id="TypeParser-1092"><a href="#TypeParser-1092"><span class="linenos">1092</span></a>
-</span><span id="TypeParser-1093"><a href="#TypeParser-1093"><span class="linenos">1093</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser-1094"><a href="#TypeParser-1094"><span class="linenos">1094</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser-1095"><a href="#TypeParser-1095"><span class="linenos">1095</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-1096"><a href="#TypeParser-1096"><span class="linenos">1096</span></a><span class="sd">			: the string to be converted</span>
-</span><span id="TypeParser-1097"><a href="#TypeParser-1097"><span class="linenos">1097</span></a>
-</span><span id="TypeParser-1098"><a href="#TypeParser-1098"><span class="linenos">1098</span></a><span class="sd">			`target_type`</span>
-</span><span id="TypeParser-1099"><a href="#TypeParser-1099"><span class="linenos">1099</span></a><span class="sd">			: type to which the value should be converted</span>
-</span><span id="TypeParser-1100"><a href="#TypeParser-1100"><span class="linenos">1100</span></a>
-</span><span id="TypeParser-1101"><a href="#TypeParser-1101"><span class="linenos">1101</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-1102"><a href="#TypeParser-1102"><span class="linenos">1102</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-1103"><a href="#TypeParser-1103"><span class="linenos">1103</span></a><span class="sd">			converted value</span>
-</span><span id="TypeParser-1104"><a href="#TypeParser-1104"><span class="linenos">1104</span></a>
-</span><span id="TypeParser-1105"><a href="#TypeParser-1105"><span class="linenos">1105</span></a><span class="sd">			Raises</span>
-</span><span id="TypeParser-1106"><a href="#TypeParser-1106"><span class="linenos">1106</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-1107"><a href="#TypeParser-1107"><span class="linenos">1107</span></a><span class="sd">			`ValueError`</span>
-</span><span id="TypeParser-1108"><a href="#TypeParser-1108"><span class="linenos">1108</span></a><span class="sd">			: if `value` cannot be converted to `target_type`</span>
-</span><span id="TypeParser-1109"><a href="#TypeParser-1109"><span class="linenos">1109</span></a>
-</span><span id="TypeParser-1110"><a href="#TypeParser-1110"><span class="linenos">1110</span></a><span class="sd">			`TypeError`</span>
-</span><span id="TypeParser-1111"><a href="#TypeParser-1111"><span class="linenos">1111</span></a><span class="sd">			: if `target_type` is not a valid type</span>
-</span><span id="TypeParser-1112"><a href="#TypeParser-1112"><span class="linenos">1112</span></a>
-</span><span id="TypeParser-1113"><a href="#TypeParser-1113"><span class="linenos">1113</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-1114"><a href="#TypeParser-1114"><span class="linenos">1114</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-1115"><a href="#TypeParser-1115"><span class="linenos">1115</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-1116"><a href="#TypeParser-1116"><span class="linenos">1116</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-1117"><a href="#TypeParser-1117"><span class="linenos">1117</span></a><span class="sd">			parser.convert(&quot;true&quot;, bool)  # True</span>
-</span><span id="TypeParser-1118"><a href="#TypeParser-1118"><span class="linenos">1118</span></a><span class="sd">			parser.convert(&quot;2&quot;, int)      # 2</span>
-</span><span id="TypeParser-1119"><a href="#TypeParser-1119"><span class="linenos">1119</span></a><span class="sd">			parser.convert(&quot;2&quot;, float)    # 2.</span>
-</span><span id="TypeParser-1120"><a href="#TypeParser-1120"><span class="linenos">1120</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-1121"><a href="#TypeParser-1121"><span class="linenos">1121</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-1122"><a href="#TypeParser-1122"><span class="linenos">1122</span></a>		<span class="n">base</span><span class="p">,</span> <span class="n">type_args</span> <span class="o">=</span> <span class="n">_decompose_type</span><span class="p">(</span><span class="n">target_type</span><span class="p">)</span>
-</span><span id="TypeParser-1123"><a href="#TypeParser-1123"><span class="linenos">1123</span></a>		<span class="k">if</span> <span class="n">base</span> <span class="o">==</span> <span class="n">NoneType</span><span class="p">:</span>
-</span><span id="TypeParser-1124"><a href="#TypeParser-1124"><span class="linenos">1124</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_none</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-1125"><a href="#TypeParser-1125"><span class="linenos">1125</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="TypeParser-1126"><a href="#TypeParser-1126"><span class="linenos">1126</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-1127"><a href="#TypeParser-1127"><span class="linenos">1127</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="TypeParser-1128"><a href="#TypeParser-1128"><span class="linenos">1128</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-1129"><a href="#TypeParser-1129"><span class="linenos">1129</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Decimal</span><span class="p">:</span>
-</span><span id="TypeParser-1130"><a href="#TypeParser-1130"><span class="linenos">1130</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_decimal</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-1131"><a href="#TypeParser-1131"><span class="linenos">1131</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="TypeParser-1132"><a href="#TypeParser-1132"><span class="linenos">1132</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-1133"><a href="#TypeParser-1133"><span class="linenos">1133</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="TypeParser-1134"><a href="#TypeParser-1134"><span class="linenos">1134</span></a>			<span class="k">return</span> <span class="n">value</span>
-</span><span id="TypeParser-1135"><a href="#TypeParser-1135"><span class="linenos">1135</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Nullable</span><span class="p">:</span>
-</span><span id="TypeParser-1136"><a href="#TypeParser-1136"><span class="linenos">1136</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser-1137"><a href="#TypeParser-1137"><span class="linenos">1137</span></a>				<span class="k">return</span> <span class="kc">None</span>
-</span><span id="TypeParser-1138"><a href="#TypeParser-1138"><span class="linenos">1138</span></a>			<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-1139"><a href="#TypeParser-1139"><span class="linenos">1139</span></a>				<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="TypeParser-1140"><a href="#TypeParser-1140"><span class="linenos">1140</span></a>					<span class="n">inner_type</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="TypeParser-1141"><a href="#TypeParser-1141"><span class="linenos">1141</span></a>					<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inner_type</span><span class="p">)</span>
-</span><span id="TypeParser-1142"><a href="#TypeParser-1142"><span class="linenos">1142</span></a>				<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-1143"><a href="#TypeParser-1143"><span class="linenos">1143</span></a>					<span class="k">return</span> <span class="n">value</span>
-</span><span id="TypeParser-1144"><a href="#TypeParser-1144"><span class="linenos">1144</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">list</span><span class="p">:</span>
-</span><span id="TypeParser-1145"><a href="#TypeParser-1145"><span class="linenos">1145</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_list_delimiter</span><span class="p">)</span>
-</span><span id="TypeParser-1146"><a href="#TypeParser-1146"><span class="linenos">1146</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
-</span><span id="TypeParser-1147"><a href="#TypeParser-1147"><span class="linenos">1147</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
-</span><span id="TypeParser-1148"><a href="#TypeParser-1148"><span class="linenos">1148</span></a>			<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="TypeParser-1149"><a href="#TypeParser-1149"><span class="linenos">1149</span></a>				<span class="n">subtype</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="TypeParser-1150"><a href="#TypeParser-1150"><span class="linenos">1150</span></a>				<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">subvalue</span><span class="p">,</span> <span class="n">subtype</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
-</span><span id="TypeParser-1151"><a href="#TypeParser-1151"><span class="linenos">1151</span></a>			<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-1152"><a href="#TypeParser-1152"><span class="linenos">1152</span></a>				<span class="k">return</span> <span class="n">subvalues</span>
-</span><span id="TypeParser-1153"><a href="#TypeParser-1153"><span class="linenos">1153</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-1154"><a href="#TypeParser-1154"><span class="linenos">1154</span></a>			<span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot convert to type: </span><span class="si">{</span><span class="n">target_type</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="TypeParser-1155"><a href="#TypeParser-1155"><span class="linenos">1155</span></a>
-</span><span id="TypeParser-1156"><a href="#TypeParser-1156"><span class="linenos">1156</span></a>
-</span><span id="TypeParser-1157"><a href="#TypeParser-1157"><span class="linenos">1157</span></a>	<span class="k">def</span> <span class="nf">parse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
-</span><span id="TypeParser-1158"><a href="#TypeParser-1158"><span class="linenos">1158</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-1159"><a href="#TypeParser-1159"><span class="linenos">1159</span></a><span class="sd">			Parse a string and convert it to its underlying type</span>
-</span><span id="TypeParser-1160"><a href="#TypeParser-1160"><span class="linenos">1160</span></a>
-</span><span id="TypeParser-1161"><a href="#TypeParser-1161"><span class="linenos">1161</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser-1162"><a href="#TypeParser-1162"><span class="linenos">1162</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser-1163"><a href="#TypeParser-1163"><span class="linenos">1163</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-1164"><a href="#TypeParser-1164"><span class="linenos">1164</span></a><span class="sd">			: the string to be parsed</span>
-</span><span id="TypeParser-1165"><a href="#TypeParser-1165"><span class="linenos">1165</span></a>
-</span><span id="TypeParser-1166"><a href="#TypeParser-1166"><span class="linenos">1166</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-1167"><a href="#TypeParser-1167"><span class="linenos">1167</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-1168"><a href="#TypeParser-1168"><span class="linenos">1168</span></a><span class="sd">			converted value</span>
-</span><span id="TypeParser-1169"><a href="#TypeParser-1169"><span class="linenos">1169</span></a>
-</span><span id="TypeParser-1170"><a href="#TypeParser-1170"><span class="linenos">1170</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-1171"><a href="#TypeParser-1171"><span class="linenos">1171</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-1172"><a href="#TypeParser-1172"><span class="linenos">1172</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-1173"><a href="#TypeParser-1173"><span class="linenos">1173</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-1174"><a href="#TypeParser-1174"><span class="linenos">1174</span></a><span class="sd">			parser.parse(&quot;true&quot;)  # True</span>
-</span><span id="TypeParser-1175"><a href="#TypeParser-1175"><span class="linenos">1175</span></a><span class="sd">			parser.parse(&quot;2.0&quot;)   # 2.</span>
-</span><span id="TypeParser-1176"><a href="#TypeParser-1176"><span class="linenos">1176</span></a><span class="sd">			parser.parse(&quot;abc&quot;)   # &quot;abc&quot;</span>
-</span><span id="TypeParser-1177"><a href="#TypeParser-1177"><span class="linenos">1177</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-1178"><a href="#TypeParser-1178"><span class="linenos">1178</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-1179"><a href="#TypeParser-1179"><span class="linenos">1179</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
-</span><span id="TypeParser-1180"><a href="#TypeParser-1180"><span class="linenos">1180</span></a>
-</span><span id="TypeParser-1181"><a href="#TypeParser-1181"><span class="linenos">1181</span></a>
-</span><span id="TypeParser-1182"><a href="#TypeParser-1182"><span class="linenos">1182</span></a>	<span class="k">def</span> <span class="nf">parse_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]:</span>
-</span><span id="TypeParser-1183"><a href="#TypeParser-1183"><span class="linenos">1183</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-1184"><a href="#TypeParser-1184"><span class="linenos">1184</span></a><span class="sd">			Parse a series of strings and convert them to their underlying common type</span>
-</span><span id="TypeParser-1185"><a href="#TypeParser-1185"><span class="linenos">1185</span></a>
-</span><span id="TypeParser-1186"><a href="#TypeParser-1186"><span class="linenos">1186</span></a><span class="sd">			If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-1093"><a href="#TypeParser-1093"><span class="linenos">1093</span></a>	<span class="k">def</span> <span class="nf">convert</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_type</span><span class="p">:</span> <span class="n">AnyValueType</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
+</span><span id="TypeParser-1094"><a href="#TypeParser-1094"><span class="linenos">1094</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-1095"><a href="#TypeParser-1095"><span class="linenos">1095</span></a><span class="sd">			Convert a string to the specified target type if possible</span>
+</span><span id="TypeParser-1096"><a href="#TypeParser-1096"><span class="linenos">1096</span></a>
+</span><span id="TypeParser-1097"><a href="#TypeParser-1097"><span class="linenos">1097</span></a><span class="sd">			Valid values for `target_type` include any return value from `infer()`, `infer_series()` and `infer_table()`. To infer and convert the string automatically, use `parse()`, `parse_series()` or `parse_table()` instead.</span>
+</span><span id="TypeParser-1098"><a href="#TypeParser-1098"><span class="linenos">1098</span></a>
+</span><span id="TypeParser-1099"><a href="#TypeParser-1099"><span class="linenos">1099</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser-1100"><a href="#TypeParser-1100"><span class="linenos">1100</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser-1101"><a href="#TypeParser-1101"><span class="linenos">1101</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-1102"><a href="#TypeParser-1102"><span class="linenos">1102</span></a><span class="sd">			: the string to be converted</span>
+</span><span id="TypeParser-1103"><a href="#TypeParser-1103"><span class="linenos">1103</span></a>
+</span><span id="TypeParser-1104"><a href="#TypeParser-1104"><span class="linenos">1104</span></a><span class="sd">			`target_type`</span>
+</span><span id="TypeParser-1105"><a href="#TypeParser-1105"><span class="linenos">1105</span></a><span class="sd">			: type to which the value should be converted</span>
+</span><span id="TypeParser-1106"><a href="#TypeParser-1106"><span class="linenos">1106</span></a>
+</span><span id="TypeParser-1107"><a href="#TypeParser-1107"><span class="linenos">1107</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-1108"><a href="#TypeParser-1108"><span class="linenos">1108</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-1109"><a href="#TypeParser-1109"><span class="linenos">1109</span></a><span class="sd">			converted value</span>
+</span><span id="TypeParser-1110"><a href="#TypeParser-1110"><span class="linenos">1110</span></a>
+</span><span id="TypeParser-1111"><a href="#TypeParser-1111"><span class="linenos">1111</span></a><span class="sd">			Raises</span>
+</span><span id="TypeParser-1112"><a href="#TypeParser-1112"><span class="linenos">1112</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-1113"><a href="#TypeParser-1113"><span class="linenos">1113</span></a><span class="sd">			`ValueError`</span>
+</span><span id="TypeParser-1114"><a href="#TypeParser-1114"><span class="linenos">1114</span></a><span class="sd">			: if `value` cannot be converted to `target_type`</span>
+</span><span id="TypeParser-1115"><a href="#TypeParser-1115"><span class="linenos">1115</span></a>
+</span><span id="TypeParser-1116"><a href="#TypeParser-1116"><span class="linenos">1116</span></a><span class="sd">			`TypeError`</span>
+</span><span id="TypeParser-1117"><a href="#TypeParser-1117"><span class="linenos">1117</span></a><span class="sd">			: if `target_type` is not a valid type</span>
+</span><span id="TypeParser-1118"><a href="#TypeParser-1118"><span class="linenos">1118</span></a>
+</span><span id="TypeParser-1119"><a href="#TypeParser-1119"><span class="linenos">1119</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-1120"><a href="#TypeParser-1120"><span class="linenos">1120</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-1121"><a href="#TypeParser-1121"><span class="linenos">1121</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-1122"><a href="#TypeParser-1122"><span class="linenos">1122</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-1123"><a href="#TypeParser-1123"><span class="linenos">1123</span></a><span class="sd">			parser.convert(&quot;true&quot;, bool)  # True</span>
+</span><span id="TypeParser-1124"><a href="#TypeParser-1124"><span class="linenos">1124</span></a><span class="sd">			parser.convert(&quot;2&quot;, int)      # 2</span>
+</span><span id="TypeParser-1125"><a href="#TypeParser-1125"><span class="linenos">1125</span></a><span class="sd">			parser.convert(&quot;2&quot;, float)    # 2.</span>
+</span><span id="TypeParser-1126"><a href="#TypeParser-1126"><span class="linenos">1126</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-1127"><a href="#TypeParser-1127"><span class="linenos">1127</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-1128"><a href="#TypeParser-1128"><span class="linenos">1128</span></a>		<span class="n">base</span><span class="p">,</span> <span class="n">type_args</span> <span class="o">=</span> <span class="n">_decompose_type</span><span class="p">(</span><span class="n">target_type</span><span class="p">)</span>
+</span><span id="TypeParser-1129"><a href="#TypeParser-1129"><span class="linenos">1129</span></a>		<span class="k">if</span> <span class="n">base</span> <span class="o">==</span> <span class="n">NoneType</span><span class="p">:</span>
+</span><span id="TypeParser-1130"><a href="#TypeParser-1130"><span class="linenos">1130</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_none</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-1131"><a href="#TypeParser-1131"><span class="linenos">1131</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="TypeParser-1132"><a href="#TypeParser-1132"><span class="linenos">1132</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-1133"><a href="#TypeParser-1133"><span class="linenos">1133</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="TypeParser-1134"><a href="#TypeParser-1134"><span class="linenos">1134</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-1135"><a href="#TypeParser-1135"><span class="linenos">1135</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Decimal</span><span class="p">:</span>
+</span><span id="TypeParser-1136"><a href="#TypeParser-1136"><span class="linenos">1136</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_decimal</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-1137"><a href="#TypeParser-1137"><span class="linenos">1137</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="TypeParser-1138"><a href="#TypeParser-1138"><span class="linenos">1138</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-1139"><a href="#TypeParser-1139"><span class="linenos">1139</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser-1140"><a href="#TypeParser-1140"><span class="linenos">1140</span></a>			<span class="k">return</span> <span class="n">value</span>
+</span><span id="TypeParser-1141"><a href="#TypeParser-1141"><span class="linenos">1141</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Nullable</span><span class="p">:</span>
+</span><span id="TypeParser-1142"><a href="#TypeParser-1142"><span class="linenos">1142</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser-1143"><a href="#TypeParser-1143"><span class="linenos">1143</span></a>				<span class="k">return</span> <span class="kc">None</span>
+</span><span id="TypeParser-1144"><a href="#TypeParser-1144"><span class="linenos">1144</span></a>			<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-1145"><a href="#TypeParser-1145"><span class="linenos">1145</span></a>				<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser-1146"><a href="#TypeParser-1146"><span class="linenos">1146</span></a>					<span class="n">inner_type</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="TypeParser-1147"><a href="#TypeParser-1147"><span class="linenos">1147</span></a>					<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inner_type</span><span class="p">)</span>
+</span><span id="TypeParser-1148"><a href="#TypeParser-1148"><span class="linenos">1148</span></a>				<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-1149"><a href="#TypeParser-1149"><span class="linenos">1149</span></a>					<span class="k">return</span> <span class="n">value</span>
+</span><span id="TypeParser-1150"><a href="#TypeParser-1150"><span class="linenos">1150</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">list</span><span class="p">:</span>
+</span><span id="TypeParser-1151"><a href="#TypeParser-1151"><span class="linenos">1151</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_list_delimiter</span><span class="p">)</span>
+</span><span id="TypeParser-1152"><a href="#TypeParser-1152"><span class="linenos">1152</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
+</span><span id="TypeParser-1153"><a href="#TypeParser-1153"><span class="linenos">1153</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
+</span><span id="TypeParser-1154"><a href="#TypeParser-1154"><span class="linenos">1154</span></a>			<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser-1155"><a href="#TypeParser-1155"><span class="linenos">1155</span></a>				<span class="n">subtype</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="TypeParser-1156"><a href="#TypeParser-1156"><span class="linenos">1156</span></a>				<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">subvalue</span><span class="p">,</span> <span class="n">subtype</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
+</span><span id="TypeParser-1157"><a href="#TypeParser-1157"><span class="linenos">1157</span></a>			<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-1158"><a href="#TypeParser-1158"><span class="linenos">1158</span></a>				<span class="k">return</span> <span class="n">subvalues</span>
+</span><span id="TypeParser-1159"><a href="#TypeParser-1159"><span class="linenos">1159</span></a>		<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-1160"><a href="#TypeParser-1160"><span class="linenos">1160</span></a>			<span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot convert to type: </span><span class="si">{</span><span class="n">target_type</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="TypeParser-1161"><a href="#TypeParser-1161"><span class="linenos">1161</span></a>
+</span><span id="TypeParser-1162"><a href="#TypeParser-1162"><span class="linenos">1162</span></a>
+</span><span id="TypeParser-1163"><a href="#TypeParser-1163"><span class="linenos">1163</span></a>	<span class="k">def</span> <span class="nf">parse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
+</span><span id="TypeParser-1164"><a href="#TypeParser-1164"><span class="linenos">1164</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-1165"><a href="#TypeParser-1165"><span class="linenos">1165</span></a><span class="sd">			Parse a string and convert it to its underlying type</span>
+</span><span id="TypeParser-1166"><a href="#TypeParser-1166"><span class="linenos">1166</span></a>
+</span><span id="TypeParser-1167"><a href="#TypeParser-1167"><span class="linenos">1167</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser-1168"><a href="#TypeParser-1168"><span class="linenos">1168</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser-1169"><a href="#TypeParser-1169"><span class="linenos">1169</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-1170"><a href="#TypeParser-1170"><span class="linenos">1170</span></a><span class="sd">			: the string to be parsed</span>
+</span><span id="TypeParser-1171"><a href="#TypeParser-1171"><span class="linenos">1171</span></a>
+</span><span id="TypeParser-1172"><a href="#TypeParser-1172"><span class="linenos">1172</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-1173"><a href="#TypeParser-1173"><span class="linenos">1173</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-1174"><a href="#TypeParser-1174"><span class="linenos">1174</span></a><span class="sd">			converted value</span>
+</span><span id="TypeParser-1175"><a href="#TypeParser-1175"><span class="linenos">1175</span></a>
+</span><span id="TypeParser-1176"><a href="#TypeParser-1176"><span class="linenos">1176</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-1177"><a href="#TypeParser-1177"><span class="linenos">1177</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-1178"><a href="#TypeParser-1178"><span class="linenos">1178</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-1179"><a href="#TypeParser-1179"><span class="linenos">1179</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-1180"><a href="#TypeParser-1180"><span class="linenos">1180</span></a><span class="sd">			parser.parse(&quot;true&quot;)  # True</span>
+</span><span id="TypeParser-1181"><a href="#TypeParser-1181"><span class="linenos">1181</span></a><span class="sd">			parser.parse(&quot;2.0&quot;)   # 2.</span>
+</span><span id="TypeParser-1182"><a href="#TypeParser-1182"><span class="linenos">1182</span></a><span class="sd">			parser.parse(&quot;abc&quot;)   # &quot;abc&quot;</span>
+</span><span id="TypeParser-1183"><a href="#TypeParser-1183"><span class="linenos">1183</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-1184"><a href="#TypeParser-1184"><span class="linenos">1184</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-1185"><a href="#TypeParser-1185"><span class="linenos">1185</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
+</span><span id="TypeParser-1186"><a href="#TypeParser-1186"><span class="linenos">1186</span></a>
 </span><span id="TypeParser-1187"><a href="#TypeParser-1187"><span class="linenos">1187</span></a>
-</span><span id="TypeParser-1188"><a href="#TypeParser-1188"><span class="linenos">1188</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser-1189"><a href="#TypeParser-1189"><span class="linenos">1189</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser-1190"><a href="#TypeParser-1190"><span class="linenos">1190</span></a><span class="sd">			`values`</span>
-</span><span id="TypeParser-1191"><a href="#TypeParser-1191"><span class="linenos">1191</span></a><span class="sd">			: series of strings to be parsed</span>
-</span><span id="TypeParser-1192"><a href="#TypeParser-1192"><span class="linenos">1192</span></a>
-</span><span id="TypeParser-1193"><a href="#TypeParser-1193"><span class="linenos">1193</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-1194"><a href="#TypeParser-1194"><span class="linenos">1194</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-1195"><a href="#TypeParser-1195"><span class="linenos">1195</span></a><span class="sd">			converted values</span>
-</span><span id="TypeParser-1196"><a href="#TypeParser-1196"><span class="linenos">1196</span></a>
-</span><span id="TypeParser-1197"><a href="#TypeParser-1197"><span class="linenos">1197</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-1198"><a href="#TypeParser-1198"><span class="linenos">1198</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-1199"><a href="#TypeParser-1199"><span class="linenos">1199</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-1200"><a href="#TypeParser-1200"><span class="linenos">1200</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-1201"><a href="#TypeParser-1201"><span class="linenos">1201</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2&quot;, &quot;3&quot;])        # [1, 2, 3]</span>
-</span><span id="TypeParser-1202"><a href="#TypeParser-1202"><span class="linenos">1202</span></a><span class="sd">			parser.parse_series([&quot;5&quot;, &quot;6.7&quot;, &quot;8.&quot;])     # [5., 6.7, 8.]</span>
-</span><span id="TypeParser-1203"><a href="#TypeParser-1203"><span class="linenos">1203</span></a><span class="sd">			parser.parse_series([&quot;true&quot;, &quot;false&quot;, &quot;&quot;])  # [True, False, None]</span>
-</span><span id="TypeParser-1204"><a href="#TypeParser-1204"><span class="linenos">1204</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])    # [&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;]</span>
-</span><span id="TypeParser-1205"><a href="#TypeParser-1205"><span class="linenos">1205</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-1206"><a href="#TypeParser-1206"><span class="linenos">1206</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-1207"><a href="#TypeParser-1207"><span class="linenos">1207</span></a>		<span class="n">inferred</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_series</span><span class="p">(</span><span class="n">values</span><span class="p">)</span>
-</span><span id="TypeParser-1208"><a href="#TypeParser-1208"><span class="linenos">1208</span></a>		<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">]</span>
-</span><span id="TypeParser-1209"><a href="#TypeParser-1209"><span class="linenos">1209</span></a>
-</span><span id="TypeParser-1210"><a href="#TypeParser-1210"><span class="linenos">1210</span></a>
-</span><span id="TypeParser-1211"><a href="#TypeParser-1211"><span class="linenos">1211</span></a>	<span class="k">def</span> <span class="nf">parse_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
-</span><span id="TypeParser-1212"><a href="#TypeParser-1212"><span class="linenos">1212</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-1213"><a href="#TypeParser-1213"><span class="linenos">1213</span></a><span class="sd">			Parse a table of strings and convert them to the underlying common type of each column</span>
-</span><span id="TypeParser-1214"><a href="#TypeParser-1214"><span class="linenos">1214</span></a>
-</span><span id="TypeParser-1215"><a href="#TypeParser-1215"><span class="linenos">1215</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-1188"><a href="#TypeParser-1188"><span class="linenos">1188</span></a>	<span class="k">def</span> <span class="nf">parse_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]:</span>
+</span><span id="TypeParser-1189"><a href="#TypeParser-1189"><span class="linenos">1189</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-1190"><a href="#TypeParser-1190"><span class="linenos">1190</span></a><span class="sd">			Parse a series of strings and convert them to their underlying common type</span>
+</span><span id="TypeParser-1191"><a href="#TypeParser-1191"><span class="linenos">1191</span></a>
+</span><span id="TypeParser-1192"><a href="#TypeParser-1192"><span class="linenos">1192</span></a><span class="sd">			If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-1193"><a href="#TypeParser-1193"><span class="linenos">1193</span></a>
+</span><span id="TypeParser-1194"><a href="#TypeParser-1194"><span class="linenos">1194</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser-1195"><a href="#TypeParser-1195"><span class="linenos">1195</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser-1196"><a href="#TypeParser-1196"><span class="linenos">1196</span></a><span class="sd">			`values`</span>
+</span><span id="TypeParser-1197"><a href="#TypeParser-1197"><span class="linenos">1197</span></a><span class="sd">			: series of strings to be parsed</span>
+</span><span id="TypeParser-1198"><a href="#TypeParser-1198"><span class="linenos">1198</span></a>
+</span><span id="TypeParser-1199"><a href="#TypeParser-1199"><span class="linenos">1199</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-1200"><a href="#TypeParser-1200"><span class="linenos">1200</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-1201"><a href="#TypeParser-1201"><span class="linenos">1201</span></a><span class="sd">			converted values</span>
+</span><span id="TypeParser-1202"><a href="#TypeParser-1202"><span class="linenos">1202</span></a>
+</span><span id="TypeParser-1203"><a href="#TypeParser-1203"><span class="linenos">1203</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-1204"><a href="#TypeParser-1204"><span class="linenos">1204</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-1205"><a href="#TypeParser-1205"><span class="linenos">1205</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-1206"><a href="#TypeParser-1206"><span class="linenos">1206</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-1207"><a href="#TypeParser-1207"><span class="linenos">1207</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2&quot;, &quot;3&quot;])        # [1, 2, 3]</span>
+</span><span id="TypeParser-1208"><a href="#TypeParser-1208"><span class="linenos">1208</span></a><span class="sd">			parser.parse_series([&quot;5&quot;, &quot;6.7&quot;, &quot;8.&quot;])     # [5., 6.7, 8.]</span>
+</span><span id="TypeParser-1209"><a href="#TypeParser-1209"><span class="linenos">1209</span></a><span class="sd">			parser.parse_series([&quot;true&quot;, &quot;false&quot;, &quot;&quot;])  # [True, False, None]</span>
+</span><span id="TypeParser-1210"><a href="#TypeParser-1210"><span class="linenos">1210</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])    # [&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;]</span>
+</span><span id="TypeParser-1211"><a href="#TypeParser-1211"><span class="linenos">1211</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-1212"><a href="#TypeParser-1212"><span class="linenos">1212</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-1213"><a href="#TypeParser-1213"><span class="linenos">1213</span></a>		<span class="n">inferred</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_series</span><span class="p">(</span><span class="n">values</span><span class="p">)</span>
+</span><span id="TypeParser-1214"><a href="#TypeParser-1214"><span class="linenos">1214</span></a>		<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">]</span>
+</span><span id="TypeParser-1215"><a href="#TypeParser-1215"><span class="linenos">1215</span></a>
 </span><span id="TypeParser-1216"><a href="#TypeParser-1216"><span class="linenos">1216</span></a>
-</span><span id="TypeParser-1217"><a href="#TypeParser-1217"><span class="linenos">1217</span></a><span class="sd">			Note that the type to which the values should be converted is determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.</span>
-</span><span id="TypeParser-1218"><a href="#TypeParser-1218"><span class="linenos">1218</span></a>
-</span><span id="TypeParser-1219"><a href="#TypeParser-1219"><span class="linenos">1219</span></a><span class="sd">			This is a function that computes the entire table and returns it all at once. The generator function `iterate_table()` behaves analogously, except that it computes and yields each row one at a time instead.</span>
+</span><span id="TypeParser-1217"><a href="#TypeParser-1217"><span class="linenos">1217</span></a>	<span class="k">def</span> <span class="nf">parse_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
+</span><span id="TypeParser-1218"><a href="#TypeParser-1218"><span class="linenos">1218</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-1219"><a href="#TypeParser-1219"><span class="linenos">1219</span></a><span class="sd">			Parse a table of strings and convert them to the underlying common type of each column</span>
 </span><span id="TypeParser-1220"><a href="#TypeParser-1220"><span class="linenos">1220</span></a>
-</span><span id="TypeParser-1221"><a href="#TypeParser-1221"><span class="linenos">1221</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser-1222"><a href="#TypeParser-1222"><span class="linenos">1222</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser-1223"><a href="#TypeParser-1223"><span class="linenos">1223</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser-1224"><a href="#TypeParser-1224"><span class="linenos">1224</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
-</span><span id="TypeParser-1225"><a href="#TypeParser-1225"><span class="linenos">1225</span></a>
-</span><span id="TypeParser-1226"><a href="#TypeParser-1226"><span class="linenos">1226</span></a><span class="sd">			`iterator`</span>
-</span><span id="TypeParser-1227"><a href="#TypeParser-1227"><span class="linenos">1227</span></a><span class="sd">			: whether the parsed values should be yielded as an iterator. If False, which is the default, the entire table is computed and returned as a list of lists. If True, this function behaves as a generator, and the rows of the table are computed and yielded one at a time. However, note that even when set to True, the type inference requires that inferred type of each individual value must all be able to fit into memory at once.</span>
-</span><span id="TypeParser-1228"><a href="#TypeParser-1228"><span class="linenos">1228</span></a>
-</span><span id="TypeParser-1229"><a href="#TypeParser-1229"><span class="linenos">1229</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-1230"><a href="#TypeParser-1230"><span class="linenos">1230</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-1231"><a href="#TypeParser-1231"><span class="linenos">1231</span></a><span class="sd">			converted table of values, in row-major order</span>
-</span><span id="TypeParser-1232"><a href="#TypeParser-1232"><span class="linenos">1232</span></a>
-</span><span id="TypeParser-1233"><a href="#TypeParser-1233"><span class="linenos">1233</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-1234"><a href="#TypeParser-1234"><span class="linenos">1234</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-1235"><a href="#TypeParser-1235"><span class="linenos">1235</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-1236"><a href="#TypeParser-1236"><span class="linenos">1236</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-1237"><a href="#TypeParser-1237"><span class="linenos">1237</span></a><span class="sd">			table = parser.parse_table([</span>
-</span><span id="TypeParser-1238"><a href="#TypeParser-1238"><span class="linenos">1238</span></a><span class="sd">				[&quot;1&quot;, &quot;5&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser-1239"><a href="#TypeParser-1239"><span class="linenos">1239</span></a><span class="sd">				[&quot;2&quot;, &quot;6.7&quot;, &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser-1240"><a href="#TypeParser-1240"><span class="linenos">1240</span></a><span class="sd">				[&quot;3&quot;, &quot;8.0&quot;, &quot;&quot;,      &quot;abc&quot;],</span>
-</span><span id="TypeParser-1241"><a href="#TypeParser-1241"><span class="linenos">1241</span></a><span class="sd">			]):</span>
-</span><span id="TypeParser-1242"><a href="#TypeParser-1242"><span class="linenos">1242</span></a><span class="sd">			assert table == [</span>
-</span><span id="TypeParser-1243"><a href="#TypeParser-1243"><span class="linenos">1243</span></a><span class="sd">				[1, 5.,  True,  &quot;1&quot;],</span>
-</span><span id="TypeParser-1244"><a href="#TypeParser-1244"><span class="linenos">1244</span></a><span class="sd">				[2, 6.7, False, &quot;2.3&quot;],</span>
-</span><span id="TypeParser-1245"><a href="#TypeParser-1245"><span class="linenos">1245</span></a><span class="sd">				[3, 8.,  None,  &quot;abc&quot;],</span>
-</span><span id="TypeParser-1246"><a href="#TypeParser-1246"><span class="linenos">1246</span></a><span class="sd">			]</span>
-</span><span id="TypeParser-1247"><a href="#TypeParser-1247"><span class="linenos">1247</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-1248"><a href="#TypeParser-1248"><span class="linenos">1248</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-1249"><a href="#TypeParser-1249"><span class="linenos">1249</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">converted_row</span> <span class="k">for</span> <span class="n">converted_row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">iterate_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)]</span>
-</span><span id="TypeParser-1250"><a href="#TypeParser-1250"><span class="linenos">1250</span></a>
-</span><span id="TypeParser-1251"><a href="#TypeParser-1251"><span class="linenos">1251</span></a>
-</span><span id="TypeParser-1252"><a href="#TypeParser-1252"><span class="linenos">1252</span></a>	<span class="k">def</span> <span class="nf">iterate_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="n">Iterator</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
-</span><span id="TypeParser-1253"><a href="#TypeParser-1253"><span class="linenos">1253</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-1254"><a href="#TypeParser-1254"><span class="linenos">1254</span></a><span class="sd">			Parse a table of strings for the underlying common type of each column, then convert and yield each row</span>
-</span><span id="TypeParser-1255"><a href="#TypeParser-1255"><span class="linenos">1255</span></a>
-</span><span id="TypeParser-1256"><a href="#TypeParser-1256"><span class="linenos">1256</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-1221"><a href="#TypeParser-1221"><span class="linenos">1221</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-1222"><a href="#TypeParser-1222"><span class="linenos">1222</span></a>
+</span><span id="TypeParser-1223"><a href="#TypeParser-1223"><span class="linenos">1223</span></a><span class="sd">			Note that the type to which the values should be converted is determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.</span>
+</span><span id="TypeParser-1224"><a href="#TypeParser-1224"><span class="linenos">1224</span></a>
+</span><span id="TypeParser-1225"><a href="#TypeParser-1225"><span class="linenos">1225</span></a><span class="sd">			This is a function that computes the entire table and returns it all at once. The generator function `iterate_table()` behaves analogously, except that it computes and yields each row one at a time instead.</span>
+</span><span id="TypeParser-1226"><a href="#TypeParser-1226"><span class="linenos">1226</span></a>
+</span><span id="TypeParser-1227"><a href="#TypeParser-1227"><span class="linenos">1227</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser-1228"><a href="#TypeParser-1228"><span class="linenos">1228</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser-1229"><a href="#TypeParser-1229"><span class="linenos">1229</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser-1230"><a href="#TypeParser-1230"><span class="linenos">1230</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
+</span><span id="TypeParser-1231"><a href="#TypeParser-1231"><span class="linenos">1231</span></a>
+</span><span id="TypeParser-1232"><a href="#TypeParser-1232"><span class="linenos">1232</span></a><span class="sd">			`iterator`</span>
+</span><span id="TypeParser-1233"><a href="#TypeParser-1233"><span class="linenos">1233</span></a><span class="sd">			: whether the parsed values should be yielded as an iterator. If False, which is the default, the entire table is computed and returned as a list of lists. If True, this function behaves as a generator, and the rows of the table are computed and yielded one at a time. However, note that even when set to True, the type inference requires that inferred type of each individual value must all be able to fit into memory at once.</span>
+</span><span id="TypeParser-1234"><a href="#TypeParser-1234"><span class="linenos">1234</span></a>
+</span><span id="TypeParser-1235"><a href="#TypeParser-1235"><span class="linenos">1235</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-1236"><a href="#TypeParser-1236"><span class="linenos">1236</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-1237"><a href="#TypeParser-1237"><span class="linenos">1237</span></a><span class="sd">			converted table of values, in row-major order</span>
+</span><span id="TypeParser-1238"><a href="#TypeParser-1238"><span class="linenos">1238</span></a>
+</span><span id="TypeParser-1239"><a href="#TypeParser-1239"><span class="linenos">1239</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-1240"><a href="#TypeParser-1240"><span class="linenos">1240</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-1241"><a href="#TypeParser-1241"><span class="linenos">1241</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-1242"><a href="#TypeParser-1242"><span class="linenos">1242</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-1243"><a href="#TypeParser-1243"><span class="linenos">1243</span></a><span class="sd">			table = parser.parse_table([</span>
+</span><span id="TypeParser-1244"><a href="#TypeParser-1244"><span class="linenos">1244</span></a><span class="sd">				[&quot;1&quot;, &quot;5&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser-1245"><a href="#TypeParser-1245"><span class="linenos">1245</span></a><span class="sd">				[&quot;2&quot;, &quot;6.7&quot;, &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser-1246"><a href="#TypeParser-1246"><span class="linenos">1246</span></a><span class="sd">				[&quot;3&quot;, &quot;8.0&quot;, &quot;&quot;,      &quot;abc&quot;],</span>
+</span><span id="TypeParser-1247"><a href="#TypeParser-1247"><span class="linenos">1247</span></a><span class="sd">			]):</span>
+</span><span id="TypeParser-1248"><a href="#TypeParser-1248"><span class="linenos">1248</span></a><span class="sd">			assert table == [</span>
+</span><span id="TypeParser-1249"><a href="#TypeParser-1249"><span class="linenos">1249</span></a><span class="sd">				[1, 5.,  True,  &quot;1&quot;],</span>
+</span><span id="TypeParser-1250"><a href="#TypeParser-1250"><span class="linenos">1250</span></a><span class="sd">				[2, 6.7, False, &quot;2.3&quot;],</span>
+</span><span id="TypeParser-1251"><a href="#TypeParser-1251"><span class="linenos">1251</span></a><span class="sd">				[3, 8.,  None,  &quot;abc&quot;],</span>
+</span><span id="TypeParser-1252"><a href="#TypeParser-1252"><span class="linenos">1252</span></a><span class="sd">			]</span>
+</span><span id="TypeParser-1253"><a href="#TypeParser-1253"><span class="linenos">1253</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-1254"><a href="#TypeParser-1254"><span class="linenos">1254</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-1255"><a href="#TypeParser-1255"><span class="linenos">1255</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">converted_row</span> <span class="k">for</span> <span class="n">converted_row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">iterate_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)]</span>
+</span><span id="TypeParser-1256"><a href="#TypeParser-1256"><span class="linenos">1256</span></a>
 </span><span id="TypeParser-1257"><a href="#TypeParser-1257"><span class="linenos">1257</span></a>
-</span><span id="TypeParser-1258"><a href="#TypeParser-1258"><span class="linenos">1258</span></a><span class="sd">			This is a generator function that computes and yields each row one at a time. However, note that in order to determine the types to which each column should be converted, the individual inferred types of every value in the table must still be able to fit into memory.</span>
-</span><span id="TypeParser-1259"><a href="#TypeParser-1259"><span class="linenos">1259</span></a>
-</span><span id="TypeParser-1260"><a href="#TypeParser-1260"><span class="linenos">1260</span></a><span class="sd">			The function `parse_table()` behaves analogously, except that it computes the entire table and returns it as a list of lists instead.</span>
+</span><span id="TypeParser-1258"><a href="#TypeParser-1258"><span class="linenos">1258</span></a>	<span class="k">def</span> <span class="nf">iterate_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="n">Iterator</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
+</span><span id="TypeParser-1259"><a href="#TypeParser-1259"><span class="linenos">1259</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-1260"><a href="#TypeParser-1260"><span class="linenos">1260</span></a><span class="sd">			Parse a table of strings for the underlying common type of each column, then convert and yield each row</span>
 </span><span id="TypeParser-1261"><a href="#TypeParser-1261"><span class="linenos">1261</span></a>
-</span><span id="TypeParser-1262"><a href="#TypeParser-1262"><span class="linenos">1262</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser-1263"><a href="#TypeParser-1263"><span class="linenos">1263</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser-1264"><a href="#TypeParser-1264"><span class="linenos">1264</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser-1265"><a href="#TypeParser-1265"><span class="linenos">1265</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
-</span><span id="TypeParser-1266"><a href="#TypeParser-1266"><span class="linenos">1266</span></a>
-</span><span id="TypeParser-1267"><a href="#TypeParser-1267"><span class="linenos">1267</span></a><span class="sd">			Yields</span>
-</span><span id="TypeParser-1268"><a href="#TypeParser-1268"><span class="linenos">1268</span></a><span class="sd">			------</span>
-</span><span id="TypeParser-1269"><a href="#TypeParser-1269"><span class="linenos">1269</span></a><span class="sd">			each row of converted table values</span>
-</span><span id="TypeParser-1270"><a href="#TypeParser-1270"><span class="linenos">1270</span></a>
-</span><span id="TypeParser-1271"><a href="#TypeParser-1271"><span class="linenos">1271</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-1272"><a href="#TypeParser-1272"><span class="linenos">1272</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-1273"><a href="#TypeParser-1273"><span class="linenos">1273</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-1274"><a href="#TypeParser-1274"><span class="linenos">1274</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-1275"><a href="#TypeParser-1275"><span class="linenos">1275</span></a><span class="sd">			table = parser.iterate_table([</span>
-</span><span id="TypeParser-1276"><a href="#TypeParser-1276"><span class="linenos">1276</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser-1277"><a href="#TypeParser-1277"><span class="linenos">1277</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser-1278"><a href="#TypeParser-1278"><span class="linenos">1278</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
-</span><span id="TypeParser-1279"><a href="#TypeParser-1279"><span class="linenos">1279</span></a><span class="sd">			]):</span>
-</span><span id="TypeParser-1280"><a href="#TypeParser-1280"><span class="linenos">1280</span></a><span class="sd">			assert next(table) == [1.,  1, &quot;1&quot;]</span>
-</span><span id="TypeParser-1281"><a href="#TypeParser-1281"><span class="linenos">1281</span></a><span class="sd">			assert next(table) == [2.,  0, &quot;2.3&quot;]</span>
-</span><span id="TypeParser-1282"><a href="#TypeParser-1282"><span class="linenos">1282</span></a><span class="sd">			assert next(table) == [3.4, 2, &quot;abc&quot;]</span>
-</span><span id="TypeParser-1283"><a href="#TypeParser-1283"><span class="linenos">1283</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-1284"><a href="#TypeParser-1284"><span class="linenos">1284</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-1285"><a href="#TypeParser-1285"><span class="linenos">1285</span></a>		<span class="n">inferred_types</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
-</span><span id="TypeParser-1286"><a href="#TypeParser-1286"><span class="linenos">1286</span></a>
-</span><span id="TypeParser-1287"><a href="#TypeParser-1287"><span class="linenos">1287</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows</span><span class="p">:</span>
-</span><span id="TypeParser-1288"><a href="#TypeParser-1288"><span class="linenos">1288</span></a>			<span class="k">yield</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span><span class="p">,</span> <span class="n">inferred</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">row</span><span class="p">,</span> <span class="n">inferred_types</span><span class="p">)]</span>
+</span><span id="TypeParser-1262"><a href="#TypeParser-1262"><span class="linenos">1262</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-1263"><a href="#TypeParser-1263"><span class="linenos">1263</span></a>
+</span><span id="TypeParser-1264"><a href="#TypeParser-1264"><span class="linenos">1264</span></a><span class="sd">			This is a generator function that computes and yields each row one at a time. However, note that in order to determine the types to which each column should be converted, the individual inferred types of every value in the table must still be able to fit into memory.</span>
+</span><span id="TypeParser-1265"><a href="#TypeParser-1265"><span class="linenos">1265</span></a>
+</span><span id="TypeParser-1266"><a href="#TypeParser-1266"><span class="linenos">1266</span></a><span class="sd">			The function `parse_table()` behaves analogously, except that it computes the entire table and returns it as a list of lists instead.</span>
+</span><span id="TypeParser-1267"><a href="#TypeParser-1267"><span class="linenos">1267</span></a>
+</span><span id="TypeParser-1268"><a href="#TypeParser-1268"><span class="linenos">1268</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser-1269"><a href="#TypeParser-1269"><span class="linenos">1269</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser-1270"><a href="#TypeParser-1270"><span class="linenos">1270</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser-1271"><a href="#TypeParser-1271"><span class="linenos">1271</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
+</span><span id="TypeParser-1272"><a href="#TypeParser-1272"><span class="linenos">1272</span></a>
+</span><span id="TypeParser-1273"><a href="#TypeParser-1273"><span class="linenos">1273</span></a><span class="sd">			Yields</span>
+</span><span id="TypeParser-1274"><a href="#TypeParser-1274"><span class="linenos">1274</span></a><span class="sd">			------</span>
+</span><span id="TypeParser-1275"><a href="#TypeParser-1275"><span class="linenos">1275</span></a><span class="sd">			each row of converted table values</span>
+</span><span id="TypeParser-1276"><a href="#TypeParser-1276"><span class="linenos">1276</span></a>
+</span><span id="TypeParser-1277"><a href="#TypeParser-1277"><span class="linenos">1277</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-1278"><a href="#TypeParser-1278"><span class="linenos">1278</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-1279"><a href="#TypeParser-1279"><span class="linenos">1279</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-1280"><a href="#TypeParser-1280"><span class="linenos">1280</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-1281"><a href="#TypeParser-1281"><span class="linenos">1281</span></a><span class="sd">			table = parser.iterate_table([</span>
+</span><span id="TypeParser-1282"><a href="#TypeParser-1282"><span class="linenos">1282</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser-1283"><a href="#TypeParser-1283"><span class="linenos">1283</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser-1284"><a href="#TypeParser-1284"><span class="linenos">1284</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
+</span><span id="TypeParser-1285"><a href="#TypeParser-1285"><span class="linenos">1285</span></a><span class="sd">			]):</span>
+</span><span id="TypeParser-1286"><a href="#TypeParser-1286"><span class="linenos">1286</span></a><span class="sd">			assert next(table) == [1.,  1, &quot;1&quot;]</span>
+</span><span id="TypeParser-1287"><a href="#TypeParser-1287"><span class="linenos">1287</span></a><span class="sd">			assert next(table) == [2.,  0, &quot;2.3&quot;]</span>
+</span><span id="TypeParser-1288"><a href="#TypeParser-1288"><span class="linenos">1288</span></a><span class="sd">			assert next(table) == [3.4, 2, &quot;abc&quot;]</span>
+</span><span id="TypeParser-1289"><a href="#TypeParser-1289"><span class="linenos">1289</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-1290"><a href="#TypeParser-1290"><span class="linenos">1290</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-1291"><a href="#TypeParser-1291"><span class="linenos">1291</span></a>		<span class="n">inferred_types</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
+</span><span id="TypeParser-1292"><a href="#TypeParser-1292"><span class="linenos">1292</span></a>
+</span><span id="TypeParser-1293"><a href="#TypeParser-1293"><span class="linenos">1293</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows</span><span class="p">:</span>
+</span><span id="TypeParser-1294"><a href="#TypeParser-1294"><span class="linenos">1294</span></a>			<span class="k">yield</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span><span class="p">,</span> <span class="n">inferred</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">row</span><span class="p">,</span> <span class="n">inferred_types</span><span class="p">)]</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>A parser that can be used to infer the underlying types of data serialised as strings, and to convert them into their original underlying types.</p>
 
 <p>The behaviour of the parser and the type inference can be configured either in the constructor or using mutable properties of a parser instance. See the constructor documentation for the list of available options.</p></div>
 
 
-
                             <div id="TypeParser.__init__" class="classattr">
                                         <input id="TypeParser.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="name">TypeParser</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="o">*</span>,</span><span class="param">	<span class="n">trim</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">use_decimal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">list_delimiter</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">none_values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s1">&#39;&#39;</span><span class="p">]</span>,</span><span class="param">	<span class="n">none_case_sensitive</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">true_values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s1">&#39;true&#39;</span><span class="p">]</span>,</span><span class="param">	<span class="n">false_values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s1">&#39;false&#39;</span><span class="p">]</span>,</span><span class="param">	<span class="n">bool_case_sensitive</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">int_case_sensitive</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">inf_values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>,</span><span class="param">	<span class="n">nan_values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>,</span><span class="param">	<span class="n">float_case_sensitive</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">case_sensitive</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">bool</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span></span>)</span>
 
 
@@ -1682,15 +1628,14 @@
 : whether all matches should be made in a case-sensitive manner. Sets all of <code>none_case_sensitive</code>, <code>bool_case_sensitive</code>, <code>int_case_sensitive</code>, <code>float_case_sensitive</code> to the same value, discarding any individual settings.</p>
 
 <h2 id="raises">Raises</h2>
 
 <p><code>ValueError</code> if any of the options would lead to ambiguities during parsing</p></div>
 
 
-
                             </div>
                             <div id="TypeParser.is_none" class="classattr">
                                         <input id="TypeParser.is_none-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">is_none</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">value</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
@@ -1755,15 +1700,14 @@
 <pre><span></span><code><span class="n">parser</span> <span class="o">=</span> <span class="n">TypeParser</span><span class="p">()</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>     <span class="c1"># True</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="s2">&quot;abc&quot;</span><span class="p">)</span>  <span class="c1"># False</span>
 </code></pre>
 </div></div>
 
 
-
                             </div>
                             <div id="TypeParser.is_bool" class="classattr">
                                         <input id="TypeParser.is_bool-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">is_bool</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">value</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
@@ -1832,15 +1776,14 @@
 <span class="n">parser</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="s2">&quot;true&quot;</span><span class="p">)</span>  <span class="c1"># True</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>      <span class="c1"># True</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="s2">&quot;abc&quot;</span><span class="p">)</span>   <span class="c1"># False</span>
 </code></pre>
 </div></div>
 
 
-
                             </div>
                             <div id="TypeParser.is_int" class="classattr">
                                         <input id="TypeParser.is_int-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">is_int</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="o">*</span>,</span><span class="param">	<span class="n">allow_negative</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">allow_sign</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
@@ -1859,15 +1802,15 @@
 </span><span id="TypeParser.is_int-539"><a href="#TypeParser.is_int-539"><span class="linenos">539</span></a><span class="sd">			`value`</span>
 </span><span id="TypeParser.is_int-540"><a href="#TypeParser.is_int-540"><span class="linenos">540</span></a><span class="sd">			: string to be checked</span>
 </span><span id="TypeParser.is_int-541"><a href="#TypeParser.is_int-541"><span class="linenos">541</span></a>
 </span><span id="TypeParser.is_int-542"><a href="#TypeParser.is_int-542"><span class="linenos">542</span></a><span class="sd">			Keyword arguments</span>
 </span><span id="TypeParser.is_int-543"><a href="#TypeParser.is_int-543"><span class="linenos">543</span></a><span class="sd">			-----------------</span>
 </span><span id="TypeParser.is_int-544"><a href="#TypeParser.is_int-544"><span class="linenos">544</span></a>
 </span><span id="TypeParser.is_int-545"><a href="#TypeParser.is_int-545"><span class="linenos">545</span></a><span class="sd">			`allow_negative`</span>
-</span><span id="TypeParser.is_int-546"><a href="#TypeParser.is_int-546"><span class="linenos">546</span></a><span class="sd">			: whether to accept negative values</span>
+</span><span id="TypeParser.is_int-546"><a href="#TypeParser.is_int-546"><span class="linenos">546</span></a><span class="sd">			: whether to accept negative values. Since negative values are always indicated with a negative sign, `allow_sign` must also be True (which is the default setting) for this to have any effect.</span>
 </span><span id="TypeParser.is_int-547"><a href="#TypeParser.is_int-547"><span class="linenos">547</span></a>
 </span><span id="TypeParser.is_int-548"><a href="#TypeParser.is_int-548"><span class="linenos">548</span></a><span class="sd">			`allow_sign`</span>
 </span><span id="TypeParser.is_int-549"><a href="#TypeParser.is_int-549"><span class="linenos">549</span></a><span class="sd">			: whether to accept values prepended with a sign character. If False, it implies that `allow_negative` is False also.</span>
 </span><span id="TypeParser.is_int-550"><a href="#TypeParser.is_int-550"><span class="linenos">550</span></a>
 </span><span id="TypeParser.is_int-551"><a href="#TypeParser.is_int-551"><span class="linenos">551</span></a><span class="sd">			`allow_scientific`</span>
 </span><span id="TypeParser.is_int-552"><a href="#TypeParser.is_int-552"><span class="linenos">552</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;M&lt;/var&gt; must be an integer and &lt;var&gt;X&lt;/var&gt; must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</span>
 </span><span id="TypeParser.is_int-553"><a href="#TypeParser.is_int-553"><span class="linenos">553</span></a>
@@ -1932,15 +1875,15 @@
 
 <p><code>value</code>
 : string to be checked</p>
 
 <h2 id="keyword-arguments">Keyword arguments</h2>
 
 <p><code>allow_negative</code>
-: whether to accept negative values</p>
+: whether to accept negative values. Since negative values are always indicated with a negative sign, <code>allow_sign</code> must also be True (which is the default setting) for this to have any effect.</p>
 
 <p><code>allow_sign</code>
 : whether to accept values prepended with a sign character. If False, it implies that <code>allow_negative</code> is False also.</p>
 
 <p><code>allow_scientific</code>
 : whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var> must be an integer and <var>X</var> must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</p>
 
@@ -1956,15 +1899,14 @@
 <span class="n">parser</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="s2">&quot;-1&quot;</span><span class="p">)</span>   <span class="c1"># True</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="s2">&quot;abc&quot;</span><span class="p">)</span>  <span class="c1"># False</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>     <span class="c1"># False</span>
 </code></pre>
 </div></div>
 
 
-
                             </div>
                             <div id="TypeParser.is_float" class="classattr">
                                         <input id="TypeParser.is_float-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">is_float</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="o">*</span>,</span><span class="param">	<span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
@@ -2085,15 +2027,14 @@
 <span class="n">parser</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="s2">&quot;12.3e-2&quot;</span><span class="p">)</span>  <span class="c1"># True</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="s2">&quot;abc&quot;</span><span class="p">)</span>      <span class="c1"># False</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>         <span class="c1"># False</span>
 </code></pre>
 </div></div>
 
 
-
                             </div>
                             <div id="TypeParser.is_decimal" class="classattr">
                                         <input id="TypeParser.is_decimal-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">is_decimal</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="o">*</span>,</span><span class="param">	<span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
@@ -2111,15 +2052,14 @@
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Alias of <code><a href="#TypeParser.is_float">is_float()</a></code></p></div>
 
 
-
                             </div>
                             <div id="TypeParser.parse_none" class="classattr">
                                         <input id="TypeParser.parse_none-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">parse_none</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">value</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="kc">None</span>:</span></span>
@@ -2187,15 +2127,14 @@
 <pre><span></span><code><span class="n">parser</span> <span class="o">=</span> <span class="n">TypeParser</span><span class="p">()</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">parse_none</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>     <span class="c1"># None</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">parse_none</span><span class="p">(</span><span class="s2">&quot;abc&quot;</span><span class="p">)</span>  <span class="c1"># raises ValueError</span>
 </code></pre>
 </div></div>
 
 
-
                             </div>
                             <div id="TypeParser.parse_bool" class="classattr">
                                         <input id="TypeParser.parse_bool-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">parse_bool</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">value</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
@@ -2273,81 +2212,86 @@
 <pre><span></span><code><span class="n">parser</span> <span class="o">=</span> <span class="n">TypeParser</span><span class="p">()</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="s2">&quot;true&quot;</span><span class="p">)</span>   <span class="c1"># True</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="s2">&quot;FALSE&quot;</span><span class="p">)</span>  <span class="c1"># False</span>
 </code></pre>
 </div></div>
 
 
-
                             </div>
                             <div id="TypeParser.parse_int" class="classattr">
                                         <input id="TypeParser.parse_int-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">parse_int</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">value</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="o">*</span>, </span><span class="param"><span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">int</span>:</span></span>
+        <span class="name">parse_int</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="o">*</span>,</span><span class="param">	<span class="n">allow_negative</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">allow_sign</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">int</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.parse_int-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.parse_int"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_int-765"><a href="#TypeParser.parse_int-765"><span class="linenos">765</span></a>	<span class="k">def</span> <span class="nf">parse_int</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_int-765"><a href="#TypeParser.parse_int-765"><span class="linenos">765</span></a>	<span class="k">def</span> <span class="nf">parse_int</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_negative</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_sign</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
 </span><span id="TypeParser.parse_int-766"><a href="#TypeParser.parse_int-766"><span class="linenos">766</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="TypeParser.parse_int-767"><a href="#TypeParser.parse_int-767"><span class="linenos">767</span></a><span class="sd">			Parse a string and return it as an int if possible</span>
 </span><span id="TypeParser.parse_int-768"><a href="#TypeParser.parse_int-768"><span class="linenos">768</span></a>
 </span><span id="TypeParser.parse_int-769"><a href="#TypeParser.parse_int-769"><span class="linenos">769</span></a><span class="sd">			If the string represents a bool, it will be converted to `1` for True and `0` for False.</span>
 </span><span id="TypeParser.parse_int-770"><a href="#TypeParser.parse_int-770"><span class="linenos">770</span></a>
 </span><span id="TypeParser.parse_int-771"><a href="#TypeParser.parse_int-771"><span class="linenos">771</span></a><span class="sd">			Arguments</span>
 </span><span id="TypeParser.parse_int-772"><a href="#TypeParser.parse_int-772"><span class="linenos">772</span></a><span class="sd">			---------</span>
 </span><span id="TypeParser.parse_int-773"><a href="#TypeParser.parse_int-773"><span class="linenos">773</span></a><span class="sd">			`value`</span>
 </span><span id="TypeParser.parse_int-774"><a href="#TypeParser.parse_int-774"><span class="linenos">774</span></a><span class="sd">			: string to be parsed</span>
 </span><span id="TypeParser.parse_int-775"><a href="#TypeParser.parse_int-775"><span class="linenos">775</span></a>
 </span><span id="TypeParser.parse_int-776"><a href="#TypeParser.parse_int-776"><span class="linenos">776</span></a><span class="sd">			Keyword arguments</span>
 </span><span id="TypeParser.parse_int-777"><a href="#TypeParser.parse_int-777"><span class="linenos">777</span></a><span class="sd">			-----------------</span>
 </span><span id="TypeParser.parse_int-778"><a href="#TypeParser.parse_int-778"><span class="linenos">778</span></a>
-</span><span id="TypeParser.parse_int-779"><a href="#TypeParser.parse_int-779"><span class="linenos">779</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser.parse_int-780"><a href="#TypeParser.parse_int-780"><span class="linenos">780</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;M&lt;/var&gt; must be an integer and &lt;var&gt;X&lt;/var&gt; must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</span>
+</span><span id="TypeParser.parse_int-779"><a href="#TypeParser.parse_int-779"><span class="linenos">779</span></a><span class="sd">			`allow_negative`</span>
+</span><span id="TypeParser.parse_int-780"><a href="#TypeParser.parse_int-780"><span class="linenos">780</span></a><span class="sd">			: whether to accept negative values. Since negative values are always indicated with a negative sign, `allow_sign` must also be True (which is the default setting) for this to have any effect.</span>
 </span><span id="TypeParser.parse_int-781"><a href="#TypeParser.parse_int-781"><span class="linenos">781</span></a>
-</span><span id="TypeParser.parse_int-782"><a href="#TypeParser.parse_int-782"><span class="linenos">782</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.parse_int-783"><a href="#TypeParser.parse_int-783"><span class="linenos">783</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.parse_int-784"><a href="#TypeParser.parse_int-784"><span class="linenos">784</span></a><span class="sd">			parsed int value</span>
-</span><span id="TypeParser.parse_int-785"><a href="#TypeParser.parse_int-785"><span class="linenos">785</span></a>
-</span><span id="TypeParser.parse_int-786"><a href="#TypeParser.parse_int-786"><span class="linenos">786</span></a><span class="sd">			Raises</span>
-</span><span id="TypeParser.parse_int-787"><a href="#TypeParser.parse_int-787"><span class="linenos">787</span></a><span class="sd">			------</span>
-</span><span id="TypeParser.parse_int-788"><a href="#TypeParser.parse_int-788"><span class="linenos">788</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
-</span><span id="TypeParser.parse_int-789"><a href="#TypeParser.parse_int-789"><span class="linenos">789</span></a>
-</span><span id="TypeParser.parse_int-790"><a href="#TypeParser.parse_int-790"><span class="linenos">790</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.parse_int-791"><a href="#TypeParser.parse_int-791"><span class="linenos">791</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.parse_int-792"><a href="#TypeParser.parse_int-792"><span class="linenos">792</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.parse_int-793"><a href="#TypeParser.parse_int-793"><span class="linenos">793</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.parse_int-794"><a href="#TypeParser.parse_int-794"><span class="linenos">794</span></a><span class="sd">			parser.parse_int(&quot;0&quot;)    # 0</span>
-</span><span id="TypeParser.parse_int-795"><a href="#TypeParser.parse_int-795"><span class="linenos">795</span></a><span class="sd">			parser.parse_int(&quot;-1&quot;)   # -1</span>
-</span><span id="TypeParser.parse_int-796"><a href="#TypeParser.parse_int-796"><span class="linenos">796</span></a><span class="sd">			parser.parse_int(&quot;2e3&quot;)  # 2000</span>
-</span><span id="TypeParser.parse_int-797"><a href="#TypeParser.parse_int-797"><span class="linenos">797</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.parse_int-798"><a href="#TypeParser.parse_int-798"><span class="linenos">798</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_int-799"><a href="#TypeParser.parse_int-799"><span class="linenos">799</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
-</span><span id="TypeParser.parse_int-800"><a href="#TypeParser.parse_int-800"><span class="linenos">800</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="TypeParser.parse_int-801"><a href="#TypeParser.parse_int-801"><span class="linenos">801</span></a>
-</span><span id="TypeParser.parse_int-802"><a href="#TypeParser.parse_int-802"><span class="linenos">802</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">):</span>
-</span><span id="TypeParser.parse_int-803"><a href="#TypeParser.parse_int-803"><span class="linenos">803</span></a>			<span class="k">if</span> <span class="n">allow_scientific</span><span class="p">:</span>
-</span><span id="TypeParser.parse_int-804"><a href="#TypeParser.parse_int-804"><span class="linenos">804</span></a>				<span class="n">value</span><span class="p">,</span> <span class="n">exp</span> <span class="o">=</span> <span class="n">_decompose_string_pair</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_scientific_char</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_int_case_sensitive</span><span class="p">)</span>
-</span><span id="TypeParser.parse_int-805"><a href="#TypeParser.parse_int-805"><span class="linenos">805</span></a>				<span class="k">if</span> <span class="n">exp</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="TypeParser.parse_int-806"><a href="#TypeParser.parse_int-806"><span class="linenos">806</span></a>					<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span> <span class="o">-</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span><span class="p">}):</span>
-</span><span id="TypeParser.parse_int-807"><a href="#TypeParser.parse_int-807"><span class="linenos">807</span></a>						<span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">+</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
-</span><span id="TypeParser.parse_int-808"><a href="#TypeParser.parse_int-808"><span class="linenos">808</span></a>					<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">*</span> <span class="p">(</span><span class="mi">10</span> <span class="o">**</span> <span class="nb">int</span><span class="p">(</span><span class="n">exp</span><span class="p">))</span>
-</span><span id="TypeParser.parse_int-809"><a href="#TypeParser.parse_int-809"><span class="linenos">809</span></a>
-</span><span id="TypeParser.parse_int-810"><a href="#TypeParser.parse_int-810"><span class="linenos">810</span></a>			<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span> <span class="o">-</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span><span class="p">}):</span>
-</span><span id="TypeParser.parse_int-811"><a href="#TypeParser.parse_int-811"><span class="linenos">811</span></a>				<span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">+</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
-</span><span id="TypeParser.parse_int-812"><a href="#TypeParser.parse_int-812"><span class="linenos">812</span></a>			<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser.parse_int-813"><a href="#TypeParser.parse_int-813"><span class="linenos">813</span></a>
-</span><span id="TypeParser.parse_int-814"><a href="#TypeParser.parse_int-814"><span class="linenos">814</span></a>		<span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser.parse_int-815"><a href="#TypeParser.parse_int-815"><span class="linenos">815</span></a>			<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
-</span><span id="TypeParser.parse_int-816"><a href="#TypeParser.parse_int-816"><span class="linenos">816</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser.parse_int-817"><a href="#TypeParser.parse_int-817"><span class="linenos">817</span></a>			<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;not an integer: </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="TypeParser.parse_int-782"><a href="#TypeParser.parse_int-782"><span class="linenos">782</span></a><span class="sd">			`allow_sign`</span>
+</span><span id="TypeParser.parse_int-783"><a href="#TypeParser.parse_int-783"><span class="linenos">783</span></a><span class="sd">			: whether to accept values prepended with a sign character. If False, it implies that `allow_negative` is False also.</span>
+</span><span id="TypeParser.parse_int-784"><a href="#TypeParser.parse_int-784"><span class="linenos">784</span></a>
+</span><span id="TypeParser.parse_int-785"><a href="#TypeParser.parse_int-785"><span class="linenos">785</span></a><span class="sd">			`allow_scientific`</span>
+</span><span id="TypeParser.parse_int-786"><a href="#TypeParser.parse_int-786"><span class="linenos">786</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;M&lt;/var&gt; must be an integer and &lt;var&gt;X&lt;/var&gt; must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</span>
+</span><span id="TypeParser.parse_int-787"><a href="#TypeParser.parse_int-787"><span class="linenos">787</span></a>
+</span><span id="TypeParser.parse_int-788"><a href="#TypeParser.parse_int-788"><span class="linenos">788</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.parse_int-789"><a href="#TypeParser.parse_int-789"><span class="linenos">789</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.parse_int-790"><a href="#TypeParser.parse_int-790"><span class="linenos">790</span></a><span class="sd">			parsed int value</span>
+</span><span id="TypeParser.parse_int-791"><a href="#TypeParser.parse_int-791"><span class="linenos">791</span></a>
+</span><span id="TypeParser.parse_int-792"><a href="#TypeParser.parse_int-792"><span class="linenos">792</span></a><span class="sd">			Raises</span>
+</span><span id="TypeParser.parse_int-793"><a href="#TypeParser.parse_int-793"><span class="linenos">793</span></a><span class="sd">			------</span>
+</span><span id="TypeParser.parse_int-794"><a href="#TypeParser.parse_int-794"><span class="linenos">794</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
+</span><span id="TypeParser.parse_int-795"><a href="#TypeParser.parse_int-795"><span class="linenos">795</span></a>
+</span><span id="TypeParser.parse_int-796"><a href="#TypeParser.parse_int-796"><span class="linenos">796</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.parse_int-797"><a href="#TypeParser.parse_int-797"><span class="linenos">797</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.parse_int-798"><a href="#TypeParser.parse_int-798"><span class="linenos">798</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.parse_int-799"><a href="#TypeParser.parse_int-799"><span class="linenos">799</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.parse_int-800"><a href="#TypeParser.parse_int-800"><span class="linenos">800</span></a><span class="sd">			parser.parse_int(&quot;0&quot;)    # 0</span>
+</span><span id="TypeParser.parse_int-801"><a href="#TypeParser.parse_int-801"><span class="linenos">801</span></a><span class="sd">			parser.parse_int(&quot;-1&quot;)   # -1</span>
+</span><span id="TypeParser.parse_int-802"><a href="#TypeParser.parse_int-802"><span class="linenos">802</span></a><span class="sd">			parser.parse_int(&quot;2e3&quot;)  # 2000</span>
+</span><span id="TypeParser.parse_int-803"><a href="#TypeParser.parse_int-803"><span class="linenos">803</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.parse_int-804"><a href="#TypeParser.parse_int-804"><span class="linenos">804</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_int-805"><a href="#TypeParser.parse_int-805"><span class="linenos">805</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
+</span><span id="TypeParser.parse_int-806"><a href="#TypeParser.parse_int-806"><span class="linenos">806</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="TypeParser.parse_int-807"><a href="#TypeParser.parse_int-807"><span class="linenos">807</span></a>
+</span><span id="TypeParser.parse_int-808"><a href="#TypeParser.parse_int-808"><span class="linenos">808</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="n">allow_negative</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="n">allow_sign</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">):</span>
+</span><span id="TypeParser.parse_int-809"><a href="#TypeParser.parse_int-809"><span class="linenos">809</span></a>			<span class="k">if</span> <span class="n">allow_scientific</span><span class="p">:</span>
+</span><span id="TypeParser.parse_int-810"><a href="#TypeParser.parse_int-810"><span class="linenos">810</span></a>				<span class="n">value</span><span class="p">,</span> <span class="n">exp</span> <span class="o">=</span> <span class="n">_decompose_string_pair</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_scientific_char</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_int_case_sensitive</span><span class="p">)</span>
+</span><span id="TypeParser.parse_int-811"><a href="#TypeParser.parse_int-811"><span class="linenos">811</span></a>				<span class="k">if</span> <span class="n">exp</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="TypeParser.parse_int-812"><a href="#TypeParser.parse_int-812"><span class="linenos">812</span></a>					<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span> <span class="o">-</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span><span class="p">}):</span>
+</span><span id="TypeParser.parse_int-813"><a href="#TypeParser.parse_int-813"><span class="linenos">813</span></a>						<span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">+</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
+</span><span id="TypeParser.parse_int-814"><a href="#TypeParser.parse_int-814"><span class="linenos">814</span></a>					<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">*</span> <span class="p">(</span><span class="mi">10</span> <span class="o">**</span> <span class="nb">int</span><span class="p">(</span><span class="n">exp</span><span class="p">))</span>
+</span><span id="TypeParser.parse_int-815"><a href="#TypeParser.parse_int-815"><span class="linenos">815</span></a>
+</span><span id="TypeParser.parse_int-816"><a href="#TypeParser.parse_int-816"><span class="linenos">816</span></a>			<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span> <span class="o">-</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span><span class="p">}):</span>
+</span><span id="TypeParser.parse_int-817"><a href="#TypeParser.parse_int-817"><span class="linenos">817</span></a>				<span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">+</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
+</span><span id="TypeParser.parse_int-818"><a href="#TypeParser.parse_int-818"><span class="linenos">818</span></a>			<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser.parse_int-819"><a href="#TypeParser.parse_int-819"><span class="linenos">819</span></a>
+</span><span id="TypeParser.parse_int-820"><a href="#TypeParser.parse_int-820"><span class="linenos">820</span></a>		<span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser.parse_int-821"><a href="#TypeParser.parse_int-821"><span class="linenos">821</span></a>			<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
+</span><span id="TypeParser.parse_int-822"><a href="#TypeParser.parse_int-822"><span class="linenos">822</span></a>		<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser.parse_int-823"><a href="#TypeParser.parse_int-823"><span class="linenos">823</span></a>			<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;not an integer: </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Parse a string and return it as an int if possible</p>
 
 <p>If the string represents a bool, it will be converted to <code>1</code> for True and <code>0</code> for False.</p>
@@ -2355,14 +2299,20 @@
 <h2 id="arguments">Arguments</h2>
 
 <p><code>value</code>
 : string to be parsed</p>
 
 <h2 id="keyword-arguments">Keyword arguments</h2>
 
+<p><code>allow_negative</code>
+: whether to accept negative values. Since negative values are always indicated with a negative sign, <code>allow_sign</code> must also be True (which is the default setting) for this to have any effect.</p>
+
+<p><code>allow_sign</code>
+: whether to accept values prepended with a sign character. If False, it implies that <code>allow_negative</code> is False also.</p>
+
 <p><code>allow_scientific</code>
 : whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var> must be an integer and <var>X</var> must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</p>
 
 <h2 id="returns">Returns</h2>
 
 <p>parsed int value</p>
 
@@ -2377,76 +2327,75 @@
 <span class="n">parser</span><span class="o">.</span><span class="n">parse_int</span><span class="p">(</span><span class="s2">&quot;0&quot;</span><span class="p">)</span>    <span class="c1"># 0</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">parse_int</span><span class="p">(</span><span class="s2">&quot;-1&quot;</span><span class="p">)</span>   <span class="c1"># -1</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">parse_int</span><span class="p">(</span><span class="s2">&quot;2e3&quot;</span><span class="p">)</span>  <span class="c1"># 2000</span>
 </code></pre>
 </div></div>
 
 
-
                             </div>
                             <div id="TypeParser.parse_float" class="classattr">
                                         <input id="TypeParser.parse_float-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">parse_float</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="o">*</span>,</span><span class="param">	<span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">float</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.parse_float-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.parse_float"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_float-865"><a href="#TypeParser.parse_float-865"><span class="linenos">865</span></a>	<span class="k">def</span> <span class="nf">parse_float</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="TypeParser.parse_float-866"><a href="#TypeParser.parse_float-866"><span class="linenos">866</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_float-867"><a href="#TypeParser.parse_float-867"><span class="linenos">867</span></a><span class="sd">			Parse a string and return it as a (non-exact) float if possible</span>
-</span><span id="TypeParser.parse_float-868"><a href="#TypeParser.parse_float-868"><span class="linenos">868</span></a>
-</span><span id="TypeParser.parse_float-869"><a href="#TypeParser.parse_float-869"><span class="linenos">869</span></a><span class="sd">			If the string represents a bool, it will be converted to `1.` for True and `0.` for False. If the string represents an int, it will be converted to a float also.</span>
-</span><span id="TypeParser.parse_float-870"><a href="#TypeParser.parse_float-870"><span class="linenos">870</span></a>
-</span><span id="TypeParser.parse_float-871"><a href="#TypeParser.parse_float-871"><span class="linenos">871</span></a><span class="sd">			Behaves analogously to `parse_decimal()`, except that that returns an exact Decimal instead.</span>
-</span><span id="TypeParser.parse_float-872"><a href="#TypeParser.parse_float-872"><span class="linenos">872</span></a>
-</span><span id="TypeParser.parse_float-873"><a href="#TypeParser.parse_float-873"><span class="linenos">873</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser.parse_float-874"><a href="#TypeParser.parse_float-874"><span class="linenos">874</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser.parse_float-875"><a href="#TypeParser.parse_float-875"><span class="linenos">875</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser.parse_float-876"><a href="#TypeParser.parse_float-876"><span class="linenos">876</span></a><span class="sd">			: string to be parsed</span>
-</span><span id="TypeParser.parse_float-877"><a href="#TypeParser.parse_float-877"><span class="linenos">877</span></a>
-</span><span id="TypeParser.parse_float-878"><a href="#TypeParser.parse_float-878"><span class="linenos">878</span></a><span class="sd">			Keyword arguments</span>
-</span><span id="TypeParser.parse_float-879"><a href="#TypeParser.parse_float-879"><span class="linenos">879</span></a><span class="sd">			-----------------</span>
-</span><span id="TypeParser.parse_float-880"><a href="#TypeParser.parse_float-880"><span class="linenos">880</span></a>
-</span><span id="TypeParser.parse_float-881"><a href="#TypeParser.parse_float-881"><span class="linenos">881</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser.parse_float-882"><a href="#TypeParser.parse_float-882"><span class="linenos">882</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_float-871"><a href="#TypeParser.parse_float-871"><span class="linenos">871</span></a>	<span class="k">def</span> <span class="nf">parse_float</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="TypeParser.parse_float-872"><a href="#TypeParser.parse_float-872"><span class="linenos">872</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_float-873"><a href="#TypeParser.parse_float-873"><span class="linenos">873</span></a><span class="sd">			Parse a string and return it as a (non-exact) float if possible</span>
+</span><span id="TypeParser.parse_float-874"><a href="#TypeParser.parse_float-874"><span class="linenos">874</span></a>
+</span><span id="TypeParser.parse_float-875"><a href="#TypeParser.parse_float-875"><span class="linenos">875</span></a><span class="sd">			If the string represents a bool, it will be converted to `1.` for True and `0.` for False. If the string represents an int, it will be converted to a float also.</span>
+</span><span id="TypeParser.parse_float-876"><a href="#TypeParser.parse_float-876"><span class="linenos">876</span></a>
+</span><span id="TypeParser.parse_float-877"><a href="#TypeParser.parse_float-877"><span class="linenos">877</span></a><span class="sd">			Behaves analogously to `parse_decimal()`, except that that returns an exact Decimal instead.</span>
+</span><span id="TypeParser.parse_float-878"><a href="#TypeParser.parse_float-878"><span class="linenos">878</span></a>
+</span><span id="TypeParser.parse_float-879"><a href="#TypeParser.parse_float-879"><span class="linenos">879</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser.parse_float-880"><a href="#TypeParser.parse_float-880"><span class="linenos">880</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser.parse_float-881"><a href="#TypeParser.parse_float-881"><span class="linenos">881</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser.parse_float-882"><a href="#TypeParser.parse_float-882"><span class="linenos">882</span></a><span class="sd">			: string to be parsed</span>
 </span><span id="TypeParser.parse_float-883"><a href="#TypeParser.parse_float-883"><span class="linenos">883</span></a>
-</span><span id="TypeParser.parse_float-884"><a href="#TypeParser.parse_float-884"><span class="linenos">884</span></a><span class="sd">			`allow_inf`</span>
-</span><span id="TypeParser.parse_float-885"><a href="#TypeParser.parse_float-885"><span class="linenos">885</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.inf_values&lt;/code&gt; (empty set by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.float_case_sensitive&lt;/code&gt;, which is False by default.</span>
+</span><span id="TypeParser.parse_float-884"><a href="#TypeParser.parse_float-884"><span class="linenos">884</span></a><span class="sd">			Keyword arguments</span>
+</span><span id="TypeParser.parse_float-885"><a href="#TypeParser.parse_float-885"><span class="linenos">885</span></a><span class="sd">			-----------------</span>
 </span><span id="TypeParser.parse_float-886"><a href="#TypeParser.parse_float-886"><span class="linenos">886</span></a>
-</span><span id="TypeParser.parse_float-887"><a href="#TypeParser.parse_float-887"><span class="linenos">887</span></a><span class="sd">			`allow_nan`</span>
-</span><span id="TypeParser.parse_float-888"><a href="#TypeParser.parse_float-888"><span class="linenos">888</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.nan_values&lt;/code&gt; (empty set by default) are interpeted as NaN. The case sensitivity of this matching also depends on &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.float_case_sensitive&lt;/code&gt;, which is False by default.</span>
+</span><span id="TypeParser.parse_float-887"><a href="#TypeParser.parse_float-887"><span class="linenos">887</span></a><span class="sd">			`allow_scientific`</span>
+</span><span id="TypeParser.parse_float-888"><a href="#TypeParser.parse_float-888"><span class="linenos">888</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
 </span><span id="TypeParser.parse_float-889"><a href="#TypeParser.parse_float-889"><span class="linenos">889</span></a>
-</span><span id="TypeParser.parse_float-890"><a href="#TypeParser.parse_float-890"><span class="linenos">890</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.parse_float-891"><a href="#TypeParser.parse_float-891"><span class="linenos">891</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.parse_float-892"><a href="#TypeParser.parse_float-892"><span class="linenos">892</span></a><span class="sd">			parsed float value</span>
-</span><span id="TypeParser.parse_float-893"><a href="#TypeParser.parse_float-893"><span class="linenos">893</span></a>
-</span><span id="TypeParser.parse_float-894"><a href="#TypeParser.parse_float-894"><span class="linenos">894</span></a><span class="sd">			Raises</span>
-</span><span id="TypeParser.parse_float-895"><a href="#TypeParser.parse_float-895"><span class="linenos">895</span></a><span class="sd">			------</span>
-</span><span id="TypeParser.parse_float-896"><a href="#TypeParser.parse_float-896"><span class="linenos">896</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
-</span><span id="TypeParser.parse_float-897"><a href="#TypeParser.parse_float-897"><span class="linenos">897</span></a>
-</span><span id="TypeParser.parse_float-898"><a href="#TypeParser.parse_float-898"><span class="linenos">898</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.parse_float-899"><a href="#TypeParser.parse_float-899"><span class="linenos">899</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.parse_float-900"><a href="#TypeParser.parse_float-900"><span class="linenos">900</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.parse_float-901"><a href="#TypeParser.parse_float-901"><span class="linenos">901</span></a><span class="sd">			parser = TypeParser(inf_values=[&quot;inf&quot;], nan_values=[&quot;nan&quot;])</span>
-</span><span id="TypeParser.parse_float-902"><a href="#TypeParser.parse_float-902"><span class="linenos">902</span></a><span class="sd">			parser.parse_float(&quot;1.&quot;)       # 1.</span>
-</span><span id="TypeParser.parse_float-903"><a href="#TypeParser.parse_float-903"><span class="linenos">903</span></a><span class="sd">			parser.parse_float(&quot;1.23e2&quot;)   # 123.</span>
-</span><span id="TypeParser.parse_float-904"><a href="#TypeParser.parse_float-904"><span class="linenos">904</span></a><span class="sd">			parser.parse_float(&quot;1.23e-2&quot;)  # 0.0123</span>
-</span><span id="TypeParser.parse_float-905"><a href="#TypeParser.parse_float-905"><span class="linenos">905</span></a><span class="sd">			parser.parse_float(&quot;inf&quot;)      # math.inf</span>
-</span><span id="TypeParser.parse_float-906"><a href="#TypeParser.parse_float-906"><span class="linenos">906</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.parse_float-907"><a href="#TypeParser.parse_float-907"><span class="linenos">907</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_float-908"><a href="#TypeParser.parse_float-908"><span class="linenos">908</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_parse_floatlike</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">math</span><span class="o">.</span><span class="n">inf</span><span class="p">,</span> <span class="n">math</span><span class="o">.</span><span class="n">nan</span><span class="p">,</span>
-</span><span id="TypeParser.parse_float-909"><a href="#TypeParser.parse_float-909"><span class="linenos">909</span></a>			<span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span>
-</span><span id="TypeParser.parse_float-910"><a href="#TypeParser.parse_float-910"><span class="linenos">910</span></a>			<span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span>
-</span><span id="TypeParser.parse_float-911"><a href="#TypeParser.parse_float-911"><span class="linenos">911</span></a>			<span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">,</span>
-</span><span id="TypeParser.parse_float-912"><a href="#TypeParser.parse_float-912"><span class="linenos">912</span></a>		<span class="p">)</span>
+</span><span id="TypeParser.parse_float-890"><a href="#TypeParser.parse_float-890"><span class="linenos">890</span></a><span class="sd">			`allow_inf`</span>
+</span><span id="TypeParser.parse_float-891"><a href="#TypeParser.parse_float-891"><span class="linenos">891</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.inf_values&lt;/code&gt; (empty set by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.float_case_sensitive&lt;/code&gt;, which is False by default.</span>
+</span><span id="TypeParser.parse_float-892"><a href="#TypeParser.parse_float-892"><span class="linenos">892</span></a>
+</span><span id="TypeParser.parse_float-893"><a href="#TypeParser.parse_float-893"><span class="linenos">893</span></a><span class="sd">			`allow_nan`</span>
+</span><span id="TypeParser.parse_float-894"><a href="#TypeParser.parse_float-894"><span class="linenos">894</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.nan_values&lt;/code&gt; (empty set by default) are interpeted as NaN. The case sensitivity of this matching also depends on &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.float_case_sensitive&lt;/code&gt;, which is False by default.</span>
+</span><span id="TypeParser.parse_float-895"><a href="#TypeParser.parse_float-895"><span class="linenos">895</span></a>
+</span><span id="TypeParser.parse_float-896"><a href="#TypeParser.parse_float-896"><span class="linenos">896</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.parse_float-897"><a href="#TypeParser.parse_float-897"><span class="linenos">897</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.parse_float-898"><a href="#TypeParser.parse_float-898"><span class="linenos">898</span></a><span class="sd">			parsed float value</span>
+</span><span id="TypeParser.parse_float-899"><a href="#TypeParser.parse_float-899"><span class="linenos">899</span></a>
+</span><span id="TypeParser.parse_float-900"><a href="#TypeParser.parse_float-900"><span class="linenos">900</span></a><span class="sd">			Raises</span>
+</span><span id="TypeParser.parse_float-901"><a href="#TypeParser.parse_float-901"><span class="linenos">901</span></a><span class="sd">			------</span>
+</span><span id="TypeParser.parse_float-902"><a href="#TypeParser.parse_float-902"><span class="linenos">902</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
+</span><span id="TypeParser.parse_float-903"><a href="#TypeParser.parse_float-903"><span class="linenos">903</span></a>
+</span><span id="TypeParser.parse_float-904"><a href="#TypeParser.parse_float-904"><span class="linenos">904</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.parse_float-905"><a href="#TypeParser.parse_float-905"><span class="linenos">905</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.parse_float-906"><a href="#TypeParser.parse_float-906"><span class="linenos">906</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.parse_float-907"><a href="#TypeParser.parse_float-907"><span class="linenos">907</span></a><span class="sd">			parser = TypeParser(inf_values=[&quot;inf&quot;], nan_values=[&quot;nan&quot;])</span>
+</span><span id="TypeParser.parse_float-908"><a href="#TypeParser.parse_float-908"><span class="linenos">908</span></a><span class="sd">			parser.parse_float(&quot;1.&quot;)       # 1.</span>
+</span><span id="TypeParser.parse_float-909"><a href="#TypeParser.parse_float-909"><span class="linenos">909</span></a><span class="sd">			parser.parse_float(&quot;1.23e2&quot;)   # 123.</span>
+</span><span id="TypeParser.parse_float-910"><a href="#TypeParser.parse_float-910"><span class="linenos">910</span></a><span class="sd">			parser.parse_float(&quot;1.23e-2&quot;)  # 0.0123</span>
+</span><span id="TypeParser.parse_float-911"><a href="#TypeParser.parse_float-911"><span class="linenos">911</span></a><span class="sd">			parser.parse_float(&quot;inf&quot;)      # math.inf</span>
+</span><span id="TypeParser.parse_float-912"><a href="#TypeParser.parse_float-912"><span class="linenos">912</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.parse_float-913"><a href="#TypeParser.parse_float-913"><span class="linenos">913</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_float-914"><a href="#TypeParser.parse_float-914"><span class="linenos">914</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_parse_floatlike</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">math</span><span class="o">.</span><span class="n">inf</span><span class="p">,</span> <span class="n">math</span><span class="o">.</span><span class="n">nan</span><span class="p">,</span>
+</span><span id="TypeParser.parse_float-915"><a href="#TypeParser.parse_float-915"><span class="linenos">915</span></a>			<span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span>
+</span><span id="TypeParser.parse_float-916"><a href="#TypeParser.parse_float-916"><span class="linenos">916</span></a>			<span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span>
+</span><span id="TypeParser.parse_float-917"><a href="#TypeParser.parse_float-917"><span class="linenos">917</span></a>			<span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">,</span>
+</span><span id="TypeParser.parse_float-918"><a href="#TypeParser.parse_float-918"><span class="linenos">918</span></a>		<span class="p">)</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Parse a string and return it as a (non-exact) float if possible</p>
 
 <p>If the string represents a bool, it will be converted to <code>1.</code> for True and <code>0.</code> for False. If the string represents an int, it will be converted to a float also.</p>
@@ -2485,76 +2434,75 @@
 <span class="n">parser</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="s2">&quot;1.23e2&quot;</span><span class="p">)</span>   <span class="c1"># 123.</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="s2">&quot;1.23e-2&quot;</span><span class="p">)</span>  <span class="c1"># 0.0123</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="s2">&quot;inf&quot;</span><span class="p">)</span>      <span class="c1"># math.inf</span>
 </code></pre>
 </div></div>
 
 
-
                             </div>
                             <div id="TypeParser.parse_decimal" class="classattr">
                                         <input id="TypeParser.parse_decimal-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">parse_decimal</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="o">*</span>,</span><span class="param">	<span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.parse_decimal-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.parse_decimal"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_decimal-915"><a href="#TypeParser.parse_decimal-915"><span class="linenos">915</span></a>	<span class="k">def</span> <span class="nf">parse_decimal</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Decimal</span><span class="p">:</span>
-</span><span id="TypeParser.parse_decimal-916"><a href="#TypeParser.parse_decimal-916"><span class="linenos">916</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_decimal-917"><a href="#TypeParser.parse_decimal-917"><span class="linenos">917</span></a><span class="sd">			Parse a string and return it as an exact Decimal if possible</span>
-</span><span id="TypeParser.parse_decimal-918"><a href="#TypeParser.parse_decimal-918"><span class="linenos">918</span></a>
-</span><span id="TypeParser.parse_decimal-919"><a href="#TypeParser.parse_decimal-919"><span class="linenos">919</span></a><span class="sd">			If the string represents a bool, it will be converted to `Decimal(1)` for True and `Decimal(0)` for False. If the string represents an int, it will be converted to a Decimal also.</span>
-</span><span id="TypeParser.parse_decimal-920"><a href="#TypeParser.parse_decimal-920"><span class="linenos">920</span></a>
-</span><span id="TypeParser.parse_decimal-921"><a href="#TypeParser.parse_decimal-921"><span class="linenos">921</span></a><span class="sd">			Behaves analogously to `parse_float()`, except that that returns a non-exact float instead.</span>
-</span><span id="TypeParser.parse_decimal-922"><a href="#TypeParser.parse_decimal-922"><span class="linenos">922</span></a>
-</span><span id="TypeParser.parse_decimal-923"><a href="#TypeParser.parse_decimal-923"><span class="linenos">923</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser.parse_decimal-924"><a href="#TypeParser.parse_decimal-924"><span class="linenos">924</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser.parse_decimal-925"><a href="#TypeParser.parse_decimal-925"><span class="linenos">925</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser.parse_decimal-926"><a href="#TypeParser.parse_decimal-926"><span class="linenos">926</span></a><span class="sd">			: string to be parsed</span>
-</span><span id="TypeParser.parse_decimal-927"><a href="#TypeParser.parse_decimal-927"><span class="linenos">927</span></a>
-</span><span id="TypeParser.parse_decimal-928"><a href="#TypeParser.parse_decimal-928"><span class="linenos">928</span></a><span class="sd">			Keyword arguments</span>
-</span><span id="TypeParser.parse_decimal-929"><a href="#TypeParser.parse_decimal-929"><span class="linenos">929</span></a><span class="sd">			-----------------</span>
-</span><span id="TypeParser.parse_decimal-930"><a href="#TypeParser.parse_decimal-930"><span class="linenos">930</span></a>
-</span><span id="TypeParser.parse_decimal-931"><a href="#TypeParser.parse_decimal-931"><span class="linenos">931</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser.parse_decimal-932"><a href="#TypeParser.parse_decimal-932"><span class="linenos">932</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_decimal-921"><a href="#TypeParser.parse_decimal-921"><span class="linenos">921</span></a>	<span class="k">def</span> <span class="nf">parse_decimal</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Decimal</span><span class="p">:</span>
+</span><span id="TypeParser.parse_decimal-922"><a href="#TypeParser.parse_decimal-922"><span class="linenos">922</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_decimal-923"><a href="#TypeParser.parse_decimal-923"><span class="linenos">923</span></a><span class="sd">			Parse a string and return it as an exact Decimal if possible</span>
+</span><span id="TypeParser.parse_decimal-924"><a href="#TypeParser.parse_decimal-924"><span class="linenos">924</span></a>
+</span><span id="TypeParser.parse_decimal-925"><a href="#TypeParser.parse_decimal-925"><span class="linenos">925</span></a><span class="sd">			If the string represents a bool, it will be converted to `Decimal(1)` for True and `Decimal(0)` for False. If the string represents an int, it will be converted to a Decimal also.</span>
+</span><span id="TypeParser.parse_decimal-926"><a href="#TypeParser.parse_decimal-926"><span class="linenos">926</span></a>
+</span><span id="TypeParser.parse_decimal-927"><a href="#TypeParser.parse_decimal-927"><span class="linenos">927</span></a><span class="sd">			Behaves analogously to `parse_float()`, except that that returns a non-exact float instead.</span>
+</span><span id="TypeParser.parse_decimal-928"><a href="#TypeParser.parse_decimal-928"><span class="linenos">928</span></a>
+</span><span id="TypeParser.parse_decimal-929"><a href="#TypeParser.parse_decimal-929"><span class="linenos">929</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser.parse_decimal-930"><a href="#TypeParser.parse_decimal-930"><span class="linenos">930</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser.parse_decimal-931"><a href="#TypeParser.parse_decimal-931"><span class="linenos">931</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser.parse_decimal-932"><a href="#TypeParser.parse_decimal-932"><span class="linenos">932</span></a><span class="sd">			: string to be parsed</span>
 </span><span id="TypeParser.parse_decimal-933"><a href="#TypeParser.parse_decimal-933"><span class="linenos">933</span></a>
-</span><span id="TypeParser.parse_decimal-934"><a href="#TypeParser.parse_decimal-934"><span class="linenos">934</span></a><span class="sd">			`allow_inf`</span>
-</span><span id="TypeParser.parse_decimal-935"><a href="#TypeParser.parse_decimal-935"><span class="linenos">935</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.inf_values&lt;/code&gt; (empty set by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.float_case_sensitive&lt;/code&gt;, which is False by default.</span>
+</span><span id="TypeParser.parse_decimal-934"><a href="#TypeParser.parse_decimal-934"><span class="linenos">934</span></a><span class="sd">			Keyword arguments</span>
+</span><span id="TypeParser.parse_decimal-935"><a href="#TypeParser.parse_decimal-935"><span class="linenos">935</span></a><span class="sd">			-----------------</span>
 </span><span id="TypeParser.parse_decimal-936"><a href="#TypeParser.parse_decimal-936"><span class="linenos">936</span></a>
-</span><span id="TypeParser.parse_decimal-937"><a href="#TypeParser.parse_decimal-937"><span class="linenos">937</span></a><span class="sd">			`allow_nan`</span>
-</span><span id="TypeParser.parse_decimal-938"><a href="#TypeParser.parse_decimal-938"><span class="linenos">938</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.nan_values&lt;/code&gt; (empty set by default) are interpeted as NaN. The case sensitivity of this matching also depends on &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.float_case_sensitive&lt;/code&gt;, which is False by default.</span>
+</span><span id="TypeParser.parse_decimal-937"><a href="#TypeParser.parse_decimal-937"><span class="linenos">937</span></a><span class="sd">			`allow_scientific`</span>
+</span><span id="TypeParser.parse_decimal-938"><a href="#TypeParser.parse_decimal-938"><span class="linenos">938</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
 </span><span id="TypeParser.parse_decimal-939"><a href="#TypeParser.parse_decimal-939"><span class="linenos">939</span></a>
-</span><span id="TypeParser.parse_decimal-940"><a href="#TypeParser.parse_decimal-940"><span class="linenos">940</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.parse_decimal-941"><a href="#TypeParser.parse_decimal-941"><span class="linenos">941</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.parse_decimal-942"><a href="#TypeParser.parse_decimal-942"><span class="linenos">942</span></a><span class="sd">			parsed Decimal value</span>
-</span><span id="TypeParser.parse_decimal-943"><a href="#TypeParser.parse_decimal-943"><span class="linenos">943</span></a>
-</span><span id="TypeParser.parse_decimal-944"><a href="#TypeParser.parse_decimal-944"><span class="linenos">944</span></a><span class="sd">			Raises</span>
-</span><span id="TypeParser.parse_decimal-945"><a href="#TypeParser.parse_decimal-945"><span class="linenos">945</span></a><span class="sd">			------</span>
-</span><span id="TypeParser.parse_decimal-946"><a href="#TypeParser.parse_decimal-946"><span class="linenos">946</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
-</span><span id="TypeParser.parse_decimal-947"><a href="#TypeParser.parse_decimal-947"><span class="linenos">947</span></a>
-</span><span id="TypeParser.parse_decimal-948"><a href="#TypeParser.parse_decimal-948"><span class="linenos">948</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.parse_decimal-949"><a href="#TypeParser.parse_decimal-949"><span class="linenos">949</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.parse_decimal-950"><a href="#TypeParser.parse_decimal-950"><span class="linenos">950</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.parse_decimal-951"><a href="#TypeParser.parse_decimal-951"><span class="linenos">951</span></a><span class="sd">			parser = TypeParser(inf_values=[&quot;inf&quot;], nan_values=[&quot;nan&quot;])</span>
-</span><span id="TypeParser.parse_decimal-952"><a href="#TypeParser.parse_decimal-952"><span class="linenos">952</span></a><span class="sd">			parser.parse_decimal(&quot;1.&quot;)       # Decimal(1)</span>
-</span><span id="TypeParser.parse_decimal-953"><a href="#TypeParser.parse_decimal-953"><span class="linenos">953</span></a><span class="sd">			parser.parse_decimal(&quot;1.23e2&quot;)   # Decimal(123)</span>
-</span><span id="TypeParser.parse_decimal-954"><a href="#TypeParser.parse_decimal-954"><span class="linenos">954</span></a><span class="sd">			parser.parse_decimal(&quot;1.23e-2&quot;)  # Decimal(123) / Decimal(10000)</span>
-</span><span id="TypeParser.parse_decimal-955"><a href="#TypeParser.parse_decimal-955"><span class="linenos">955</span></a><span class="sd">			parser.parse_decimal(&quot;inf&quot;)      # Decimal(math.inf)</span>
-</span><span id="TypeParser.parse_decimal-956"><a href="#TypeParser.parse_decimal-956"><span class="linenos">956</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.parse_decimal-957"><a href="#TypeParser.parse_decimal-957"><span class="linenos">957</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_decimal-958"><a href="#TypeParser.parse_decimal-958"><span class="linenos">958</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_parse_floatlike</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">Decimal</span><span class="p">,</span> <span class="n">Decimal</span><span class="p">(</span><span class="n">math</span><span class="o">.</span><span class="n">inf</span><span class="p">),</span> <span class="n">Decimal</span><span class="p">(</span><span class="n">math</span><span class="o">.</span><span class="n">nan</span><span class="p">),</span>
-</span><span id="TypeParser.parse_decimal-959"><a href="#TypeParser.parse_decimal-959"><span class="linenos">959</span></a>			<span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span>
-</span><span id="TypeParser.parse_decimal-960"><a href="#TypeParser.parse_decimal-960"><span class="linenos">960</span></a>			<span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span>
-</span><span id="TypeParser.parse_decimal-961"><a href="#TypeParser.parse_decimal-961"><span class="linenos">961</span></a>			<span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">,</span>
-</span><span id="TypeParser.parse_decimal-962"><a href="#TypeParser.parse_decimal-962"><span class="linenos">962</span></a>		<span class="p">)</span>
+</span><span id="TypeParser.parse_decimal-940"><a href="#TypeParser.parse_decimal-940"><span class="linenos">940</span></a><span class="sd">			`allow_inf`</span>
+</span><span id="TypeParser.parse_decimal-941"><a href="#TypeParser.parse_decimal-941"><span class="linenos">941</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.inf_values&lt;/code&gt; (empty set by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.float_case_sensitive&lt;/code&gt;, which is False by default.</span>
+</span><span id="TypeParser.parse_decimal-942"><a href="#TypeParser.parse_decimal-942"><span class="linenos">942</span></a>
+</span><span id="TypeParser.parse_decimal-943"><a href="#TypeParser.parse_decimal-943"><span class="linenos">943</span></a><span class="sd">			`allow_nan`</span>
+</span><span id="TypeParser.parse_decimal-944"><a href="#TypeParser.parse_decimal-944"><span class="linenos">944</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.nan_values&lt;/code&gt; (empty set by default) are interpeted as NaN. The case sensitivity of this matching also depends on &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.float_case_sensitive&lt;/code&gt;, which is False by default.</span>
+</span><span id="TypeParser.parse_decimal-945"><a href="#TypeParser.parse_decimal-945"><span class="linenos">945</span></a>
+</span><span id="TypeParser.parse_decimal-946"><a href="#TypeParser.parse_decimal-946"><span class="linenos">946</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.parse_decimal-947"><a href="#TypeParser.parse_decimal-947"><span class="linenos">947</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.parse_decimal-948"><a href="#TypeParser.parse_decimal-948"><span class="linenos">948</span></a><span class="sd">			parsed Decimal value</span>
+</span><span id="TypeParser.parse_decimal-949"><a href="#TypeParser.parse_decimal-949"><span class="linenos">949</span></a>
+</span><span id="TypeParser.parse_decimal-950"><a href="#TypeParser.parse_decimal-950"><span class="linenos">950</span></a><span class="sd">			Raises</span>
+</span><span id="TypeParser.parse_decimal-951"><a href="#TypeParser.parse_decimal-951"><span class="linenos">951</span></a><span class="sd">			------</span>
+</span><span id="TypeParser.parse_decimal-952"><a href="#TypeParser.parse_decimal-952"><span class="linenos">952</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
+</span><span id="TypeParser.parse_decimal-953"><a href="#TypeParser.parse_decimal-953"><span class="linenos">953</span></a>
+</span><span id="TypeParser.parse_decimal-954"><a href="#TypeParser.parse_decimal-954"><span class="linenos">954</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.parse_decimal-955"><a href="#TypeParser.parse_decimal-955"><span class="linenos">955</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.parse_decimal-956"><a href="#TypeParser.parse_decimal-956"><span class="linenos">956</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.parse_decimal-957"><a href="#TypeParser.parse_decimal-957"><span class="linenos">957</span></a><span class="sd">			parser = TypeParser(inf_values=[&quot;inf&quot;], nan_values=[&quot;nan&quot;])</span>
+</span><span id="TypeParser.parse_decimal-958"><a href="#TypeParser.parse_decimal-958"><span class="linenos">958</span></a><span class="sd">			parser.parse_decimal(&quot;1.&quot;)       # Decimal(1)</span>
+</span><span id="TypeParser.parse_decimal-959"><a href="#TypeParser.parse_decimal-959"><span class="linenos">959</span></a><span class="sd">			parser.parse_decimal(&quot;1.23e2&quot;)   # Decimal(123)</span>
+</span><span id="TypeParser.parse_decimal-960"><a href="#TypeParser.parse_decimal-960"><span class="linenos">960</span></a><span class="sd">			parser.parse_decimal(&quot;1.23e-2&quot;)  # Decimal(123) / Decimal(10000)</span>
+</span><span id="TypeParser.parse_decimal-961"><a href="#TypeParser.parse_decimal-961"><span class="linenos">961</span></a><span class="sd">			parser.parse_decimal(&quot;inf&quot;)      # Decimal(math.inf)</span>
+</span><span id="TypeParser.parse_decimal-962"><a href="#TypeParser.parse_decimal-962"><span class="linenos">962</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.parse_decimal-963"><a href="#TypeParser.parse_decimal-963"><span class="linenos">963</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_decimal-964"><a href="#TypeParser.parse_decimal-964"><span class="linenos">964</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_parse_floatlike</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">Decimal</span><span class="p">,</span> <span class="n">Decimal</span><span class="p">(</span><span class="n">math</span><span class="o">.</span><span class="n">inf</span><span class="p">),</span> <span class="n">Decimal</span><span class="p">(</span><span class="n">math</span><span class="o">.</span><span class="n">nan</span><span class="p">),</span>
+</span><span id="TypeParser.parse_decimal-965"><a href="#TypeParser.parse_decimal-965"><span class="linenos">965</span></a>			<span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span>
+</span><span id="TypeParser.parse_decimal-966"><a href="#TypeParser.parse_decimal-966"><span class="linenos">966</span></a>			<span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span>
+</span><span id="TypeParser.parse_decimal-967"><a href="#TypeParser.parse_decimal-967"><span class="linenos">967</span></a>			<span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">,</span>
+</span><span id="TypeParser.parse_decimal-968"><a href="#TypeParser.parse_decimal-968"><span class="linenos">968</span></a>		<span class="p">)</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Parse a string and return it as an exact Decimal if possible</p>
 
 <p>If the string represents a bool, it will be converted to <code>Decimal(1)</code> for True and <code>Decimal(0)</code> for False. If the string represents an int, it will be converted to a Decimal also.</p>
@@ -2593,76 +2541,75 @@
 <span class="n">parser</span><span class="o">.</span><span class="n">parse_decimal</span><span class="p">(</span><span class="s2">&quot;1.23e2&quot;</span><span class="p">)</span>   <span class="c1"># Decimal(123)</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">parse_decimal</span><span class="p">(</span><span class="s2">&quot;1.23e-2&quot;</span><span class="p">)</span>  <span class="c1"># Decimal(123) / Decimal(10000)</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">parse_decimal</span><span class="p">(</span><span class="s2">&quot;inf&quot;</span><span class="p">)</span>      <span class="c1"># Decimal(math.inf)</span>
 </code></pre>
 </div></div>
 
 
-
                             </div>
                             <div id="TypeParser.infer" class="classattr">
                                         <input id="TypeParser.infer-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">infer</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n"><a href="#Nullable">Nullable</a></span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.infer-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.infer"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.infer-965"><a href="#TypeParser.infer-965"><span class="linenos"> 965</span></a>	<span class="k">def</span> <span class="nf">infer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
-</span><span id="TypeParser.infer-966"><a href="#TypeParser.infer-966"><span class="linenos"> 966</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.infer-967"><a href="#TypeParser.infer-967"><span class="linenos"> 967</span></a><span class="sd">			Infer the underlying type of a string</span>
-</span><span id="TypeParser.infer-968"><a href="#TypeParser.infer-968"><span class="linenos"> 968</span></a>
-</span><span id="TypeParser.infer-969"><a href="#TypeParser.infer-969"><span class="linenos"> 969</span></a><span class="sd">			Also check for inline lists if &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.list_delimiter&lt;/code&gt; is not None.</span>
-</span><span id="TypeParser.infer-970"><a href="#TypeParser.infer-970"><span class="linenos"> 970</span></a>
-</span><span id="TypeParser.infer-971"><a href="#TypeParser.infer-971"><span class="linenos"> 971</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser.infer-972"><a href="#TypeParser.infer-972"><span class="linenos"> 972</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser.infer-973"><a href="#TypeParser.infer-973"><span class="linenos"> 973</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser.infer-974"><a href="#TypeParser.infer-974"><span class="linenos"> 974</span></a><span class="sd">			: the string for which the type should be inferred</span>
-</span><span id="TypeParser.infer-975"><a href="#TypeParser.infer-975"><span class="linenos"> 975</span></a>
-</span><span id="TypeParser.infer-976"><a href="#TypeParser.infer-976"><span class="linenos"> 976</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.infer-977"><a href="#TypeParser.infer-977"><span class="linenos"> 977</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.infer-978"><a href="#TypeParser.infer-978"><span class="linenos"> 978</span></a><span class="sd">			inferred type</span>
-</span><span id="TypeParser.infer-979"><a href="#TypeParser.infer-979"><span class="linenos"> 979</span></a>
-</span><span id="TypeParser.infer-980"><a href="#TypeParser.infer-980"><span class="linenos"> 980</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.infer-981"><a href="#TypeParser.infer-981"><span class="linenos"> 981</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.infer-982"><a href="#TypeParser.infer-982"><span class="linenos"> 982</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.infer-983"><a href="#TypeParser.infer-983"><span class="linenos"> 983</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.infer-984"><a href="#TypeParser.infer-984"><span class="linenos"> 984</span></a><span class="sd">			parser.infer(&quot;true&quot;)  # bool</span>
-</span><span id="TypeParser.infer-985"><a href="#TypeParser.infer-985"><span class="linenos"> 985</span></a><span class="sd">			parser.infer(&quot;2.0&quot;)   # float</span>
-</span><span id="TypeParser.infer-986"><a href="#TypeParser.infer-986"><span class="linenos"> 986</span></a><span class="sd">			parser.infer(&quot;abc&quot;)   # str</span>
-</span><span id="TypeParser.infer-987"><a href="#TypeParser.infer-987"><span class="linenos"> 987</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.infer-988"><a href="#TypeParser.infer-988"><span class="linenos"> 988</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.infer-989"><a href="#TypeParser.infer-989"><span class="linenos"> 989</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser.infer-990"><a href="#TypeParser.infer-990"><span class="linenos"> 990</span></a>			<span class="k">return</span> <span class="n">NoneType</span>
-</span><span id="TypeParser.infer-991"><a href="#TypeParser.infer-991"><span class="linenos"> 991</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser.infer-992"><a href="#TypeParser.infer-992"><span class="linenos"> 992</span></a>			<span class="k">return</span> <span class="nb">bool</span>
-</span><span id="TypeParser.infer-993"><a href="#TypeParser.infer-993"><span class="linenos"> 993</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser.infer-994"><a href="#TypeParser.infer-994"><span class="linenos"> 994</span></a>			<span class="k">return</span> <span class="nb">int</span>
-</span><span id="TypeParser.infer-995"><a href="#TypeParser.infer-995"><span class="linenos"> 995</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser.infer-996"><a href="#TypeParser.infer-996"><span class="linenos"> 996</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_use_decimal</span><span class="p">:</span>
-</span><span id="TypeParser.infer-997"><a href="#TypeParser.infer-997"><span class="linenos"> 997</span></a>				<span class="k">return</span> <span class="n">Decimal</span>
-</span><span id="TypeParser.infer-998"><a href="#TypeParser.infer-998"><span class="linenos"> 998</span></a>			<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser.infer-999"><a href="#TypeParser.infer-999"><span class="linenos"> 999</span></a>				<span class="k">return</span> <span class="nb">float</span>
-</span><span id="TypeParser.infer-1000"><a href="#TypeParser.infer-1000"><span class="linenos">1000</span></a>
-</span><span id="TypeParser.infer-1001"><a href="#TypeParser.infer-1001"><span class="linenos">1001</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
-</span><span id="TypeParser.infer-1002"><a href="#TypeParser.infer-1002"><span class="linenos">1002</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="TypeParser.infer-1003"><a href="#TypeParser.infer-1003"><span class="linenos">1003</span></a>
-</span><span id="TypeParser.infer-1004"><a href="#TypeParser.infer-1004"><span class="linenos">1004</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_list_delimiter</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">_list_delimiter</span> <span class="ow">in</span> <span class="n">value</span><span class="p">:</span>
-</span><span id="TypeParser.infer-1005"><a href="#TypeParser.infer-1005"><span class="linenos">1005</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_list_delimiter</span><span class="p">)</span>
-</span><span id="TypeParser.infer-1006"><a href="#TypeParser.infer-1006"><span class="linenos">1006</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
-</span><span id="TypeParser.infer-1007"><a href="#TypeParser.infer-1007"><span class="linenos">1007</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
-</span><span id="TypeParser.infer-1008"><a href="#TypeParser.infer-1008"><span class="linenos">1008</span></a>			<span class="n">reduced_type</span> <span class="o">=</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">subvalue</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">)</span>
-</span><span id="TypeParser.infer-1009"><a href="#TypeParser.infer-1009"><span class="linenos">1009</span></a>			<span class="n">r</span> <span class="o">=</span> <span class="nb">list</span><span class="p">[</span><span class="n">reduced_type</span><span class="p">]</span>
-</span><span id="TypeParser.infer-1010"><a href="#TypeParser.infer-1010"><span class="linenos">1010</span></a>			<span class="k">return</span> <span class="n">r</span>
-</span><span id="TypeParser.infer-1011"><a href="#TypeParser.infer-1011"><span class="linenos">1011</span></a>
-</span><span id="TypeParser.infer-1012"><a href="#TypeParser.infer-1012"><span class="linenos">1012</span></a>		<span class="k">return</span> <span class="n">GenericValue</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.infer-971"><a href="#TypeParser.infer-971"><span class="linenos"> 971</span></a>	<span class="k">def</span> <span class="nf">infer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
+</span><span id="TypeParser.infer-972"><a href="#TypeParser.infer-972"><span class="linenos"> 972</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.infer-973"><a href="#TypeParser.infer-973"><span class="linenos"> 973</span></a><span class="sd">			Infer the underlying type of a string</span>
+</span><span id="TypeParser.infer-974"><a href="#TypeParser.infer-974"><span class="linenos"> 974</span></a>
+</span><span id="TypeParser.infer-975"><a href="#TypeParser.infer-975"><span class="linenos"> 975</span></a><span class="sd">			Also check for inline lists if &lt;code&gt;&lt;var&gt;parser&lt;/var&gt;.list_delimiter&lt;/code&gt; is not None.</span>
+</span><span id="TypeParser.infer-976"><a href="#TypeParser.infer-976"><span class="linenos"> 976</span></a>
+</span><span id="TypeParser.infer-977"><a href="#TypeParser.infer-977"><span class="linenos"> 977</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser.infer-978"><a href="#TypeParser.infer-978"><span class="linenos"> 978</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser.infer-979"><a href="#TypeParser.infer-979"><span class="linenos"> 979</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser.infer-980"><a href="#TypeParser.infer-980"><span class="linenos"> 980</span></a><span class="sd">			: the string for which the type should be inferred</span>
+</span><span id="TypeParser.infer-981"><a href="#TypeParser.infer-981"><span class="linenos"> 981</span></a>
+</span><span id="TypeParser.infer-982"><a href="#TypeParser.infer-982"><span class="linenos"> 982</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.infer-983"><a href="#TypeParser.infer-983"><span class="linenos"> 983</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.infer-984"><a href="#TypeParser.infer-984"><span class="linenos"> 984</span></a><span class="sd">			inferred type</span>
+</span><span id="TypeParser.infer-985"><a href="#TypeParser.infer-985"><span class="linenos"> 985</span></a>
+</span><span id="TypeParser.infer-986"><a href="#TypeParser.infer-986"><span class="linenos"> 986</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.infer-987"><a href="#TypeParser.infer-987"><span class="linenos"> 987</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.infer-988"><a href="#TypeParser.infer-988"><span class="linenos"> 988</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.infer-989"><a href="#TypeParser.infer-989"><span class="linenos"> 989</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.infer-990"><a href="#TypeParser.infer-990"><span class="linenos"> 990</span></a><span class="sd">			parser.infer(&quot;true&quot;)  # bool</span>
+</span><span id="TypeParser.infer-991"><a href="#TypeParser.infer-991"><span class="linenos"> 991</span></a><span class="sd">			parser.infer(&quot;2.0&quot;)   # float</span>
+</span><span id="TypeParser.infer-992"><a href="#TypeParser.infer-992"><span class="linenos"> 992</span></a><span class="sd">			parser.infer(&quot;abc&quot;)   # str</span>
+</span><span id="TypeParser.infer-993"><a href="#TypeParser.infer-993"><span class="linenos"> 993</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.infer-994"><a href="#TypeParser.infer-994"><span class="linenos"> 994</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.infer-995"><a href="#TypeParser.infer-995"><span class="linenos"> 995</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser.infer-996"><a href="#TypeParser.infer-996"><span class="linenos"> 996</span></a>			<span class="k">return</span> <span class="n">NoneType</span>
+</span><span id="TypeParser.infer-997"><a href="#TypeParser.infer-997"><span class="linenos"> 997</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser.infer-998"><a href="#TypeParser.infer-998"><span class="linenos"> 998</span></a>			<span class="k">return</span> <span class="nb">bool</span>
+</span><span id="TypeParser.infer-999"><a href="#TypeParser.infer-999"><span class="linenos"> 999</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser.infer-1000"><a href="#TypeParser.infer-1000"><span class="linenos">1000</span></a>			<span class="k">return</span> <span class="nb">int</span>
+</span><span id="TypeParser.infer-1001"><a href="#TypeParser.infer-1001"><span class="linenos">1001</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser.infer-1002"><a href="#TypeParser.infer-1002"><span class="linenos">1002</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_use_decimal</span><span class="p">:</span>
+</span><span id="TypeParser.infer-1003"><a href="#TypeParser.infer-1003"><span class="linenos">1003</span></a>				<span class="k">return</span> <span class="n">Decimal</span>
+</span><span id="TypeParser.infer-1004"><a href="#TypeParser.infer-1004"><span class="linenos">1004</span></a>			<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser.infer-1005"><a href="#TypeParser.infer-1005"><span class="linenos">1005</span></a>				<span class="k">return</span> <span class="nb">float</span>
+</span><span id="TypeParser.infer-1006"><a href="#TypeParser.infer-1006"><span class="linenos">1006</span></a>
+</span><span id="TypeParser.infer-1007"><a href="#TypeParser.infer-1007"><span class="linenos">1007</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
+</span><span id="TypeParser.infer-1008"><a href="#TypeParser.infer-1008"><span class="linenos">1008</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="TypeParser.infer-1009"><a href="#TypeParser.infer-1009"><span class="linenos">1009</span></a>
+</span><span id="TypeParser.infer-1010"><a href="#TypeParser.infer-1010"><span class="linenos">1010</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_list_delimiter</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">_list_delimiter</span> <span class="ow">in</span> <span class="n">value</span><span class="p">:</span>
+</span><span id="TypeParser.infer-1011"><a href="#TypeParser.infer-1011"><span class="linenos">1011</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_list_delimiter</span><span class="p">)</span>
+</span><span id="TypeParser.infer-1012"><a href="#TypeParser.infer-1012"><span class="linenos">1012</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
+</span><span id="TypeParser.infer-1013"><a href="#TypeParser.infer-1013"><span class="linenos">1013</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
+</span><span id="TypeParser.infer-1014"><a href="#TypeParser.infer-1014"><span class="linenos">1014</span></a>			<span class="n">reduced_type</span> <span class="o">=</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">subvalue</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">)</span>
+</span><span id="TypeParser.infer-1015"><a href="#TypeParser.infer-1015"><span class="linenos">1015</span></a>			<span class="n">r</span> <span class="o">=</span> <span class="nb">list</span><span class="p">[</span><span class="n">reduced_type</span><span class="p">]</span>
+</span><span id="TypeParser.infer-1016"><a href="#TypeParser.infer-1016"><span class="linenos">1016</span></a>			<span class="k">return</span> <span class="n">r</span>
+</span><span id="TypeParser.infer-1017"><a href="#TypeParser.infer-1017"><span class="linenos">1017</span></a>
+</span><span id="TypeParser.infer-1018"><a href="#TypeParser.infer-1018"><span class="linenos">1018</span></a>		<span class="k">return</span> <span class="n">GenericValue</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Infer the underlying type of a string</p>
 
 <p>Also check for inline lists if <code><var>parser</var>.list_delimiter</code> is not None.</p>
@@ -2683,53 +2630,52 @@
 <span class="n">parser</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="s2">&quot;true&quot;</span><span class="p">)</span>  <span class="c1"># bool</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="s2">&quot;2.0&quot;</span><span class="p">)</span>   <span class="c1"># float</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="s2">&quot;abc&quot;</span><span class="p">)</span>   <span class="c1"># str</span>
 </code></pre>
 </div></div>
 
 
-
                             </div>
                             <div id="TypeParser.infer_series" class="classattr">
                                         <input id="TypeParser.infer_series-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">infer_series</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n"><a href="#Nullable">Nullable</a></span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.infer_series-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.infer_series"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.infer_series-1015"><a href="#TypeParser.infer_series-1015"><span class="linenos">1015</span></a>	<span class="k">def</span> <span class="nf">infer_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
-</span><span id="TypeParser.infer_series-1016"><a href="#TypeParser.infer_series-1016"><span class="linenos">1016</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.infer_series-1017"><a href="#TypeParser.infer_series-1017"><span class="linenos">1017</span></a><span class="sd">			Infer the underlying common type of a series of strings</span>
-</span><span id="TypeParser.infer_series-1018"><a href="#TypeParser.infer_series-1018"><span class="linenos">1018</span></a>
-</span><span id="TypeParser.infer_series-1019"><a href="#TypeParser.infer_series-1019"><span class="linenos">1019</span></a><span class="sd">			If the values in the series do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser.infer_series-1020"><a href="#TypeParser.infer_series-1020"><span class="linenos">1020</span></a>
-</span><span id="TypeParser.infer_series-1021"><a href="#TypeParser.infer_series-1021"><span class="linenos">1021</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser.infer_series-1022"><a href="#TypeParser.infer_series-1022"><span class="linenos">1022</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser.infer_series-1023"><a href="#TypeParser.infer_series-1023"><span class="linenos">1023</span></a><span class="sd">			`values`</span>
-</span><span id="TypeParser.infer_series-1024"><a href="#TypeParser.infer_series-1024"><span class="linenos">1024</span></a><span class="sd">			: series of strings for which the type should be inferred</span>
-</span><span id="TypeParser.infer_series-1025"><a href="#TypeParser.infer_series-1025"><span class="linenos">1025</span></a>
-</span><span id="TypeParser.infer_series-1026"><a href="#TypeParser.infer_series-1026"><span class="linenos">1026</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.infer_series-1027"><a href="#TypeParser.infer_series-1027"><span class="linenos">1027</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.infer_series-1028"><a href="#TypeParser.infer_series-1028"><span class="linenos">1028</span></a><span class="sd">			inferred type</span>
-</span><span id="TypeParser.infer_series-1029"><a href="#TypeParser.infer_series-1029"><span class="linenos">1029</span></a>
-</span><span id="TypeParser.infer_series-1030"><a href="#TypeParser.infer_series-1030"><span class="linenos">1030</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.infer_series-1031"><a href="#TypeParser.infer_series-1031"><span class="linenos">1031</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.infer_series-1032"><a href="#TypeParser.infer_series-1032"><span class="linenos">1032</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.infer_series-1033"><a href="#TypeParser.infer_series-1033"><span class="linenos">1033</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.infer_series-1034"><a href="#TypeParser.infer_series-1034"><span class="linenos">1034</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2&quot;, &quot;3.4&quot;])       # float</span>
-</span><span id="TypeParser.infer_series-1035"><a href="#TypeParser.infer_series-1035"><span class="linenos">1035</span></a><span class="sd">			parser.infer_series([&quot;true&quot;, &quot;false&quot;, &quot;2&quot;])  # int</span>
-</span><span id="TypeParser.infer_series-1036"><a href="#TypeParser.infer_series-1036"><span class="linenos">1036</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])     # str</span>
-</span><span id="TypeParser.infer_series-1037"><a href="#TypeParser.infer_series-1037"><span class="linenos">1037</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.infer_series-1038"><a href="#TypeParser.infer_series-1038"><span class="linenos">1038</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.infer_series-1039"><a href="#TypeParser.infer_series-1039"><span class="linenos">1039</span></a>		<span class="k">return</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.infer_series-1021"><a href="#TypeParser.infer_series-1021"><span class="linenos">1021</span></a>	<span class="k">def</span> <span class="nf">infer_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
+</span><span id="TypeParser.infer_series-1022"><a href="#TypeParser.infer_series-1022"><span class="linenos">1022</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.infer_series-1023"><a href="#TypeParser.infer_series-1023"><span class="linenos">1023</span></a><span class="sd">			Infer the underlying common type of a series of strings</span>
+</span><span id="TypeParser.infer_series-1024"><a href="#TypeParser.infer_series-1024"><span class="linenos">1024</span></a>
+</span><span id="TypeParser.infer_series-1025"><a href="#TypeParser.infer_series-1025"><span class="linenos">1025</span></a><span class="sd">			If the values in the series do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser.infer_series-1026"><a href="#TypeParser.infer_series-1026"><span class="linenos">1026</span></a>
+</span><span id="TypeParser.infer_series-1027"><a href="#TypeParser.infer_series-1027"><span class="linenos">1027</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser.infer_series-1028"><a href="#TypeParser.infer_series-1028"><span class="linenos">1028</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser.infer_series-1029"><a href="#TypeParser.infer_series-1029"><span class="linenos">1029</span></a><span class="sd">			`values`</span>
+</span><span id="TypeParser.infer_series-1030"><a href="#TypeParser.infer_series-1030"><span class="linenos">1030</span></a><span class="sd">			: series of strings for which the type should be inferred</span>
+</span><span id="TypeParser.infer_series-1031"><a href="#TypeParser.infer_series-1031"><span class="linenos">1031</span></a>
+</span><span id="TypeParser.infer_series-1032"><a href="#TypeParser.infer_series-1032"><span class="linenos">1032</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.infer_series-1033"><a href="#TypeParser.infer_series-1033"><span class="linenos">1033</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.infer_series-1034"><a href="#TypeParser.infer_series-1034"><span class="linenos">1034</span></a><span class="sd">			inferred type</span>
+</span><span id="TypeParser.infer_series-1035"><a href="#TypeParser.infer_series-1035"><span class="linenos">1035</span></a>
+</span><span id="TypeParser.infer_series-1036"><a href="#TypeParser.infer_series-1036"><span class="linenos">1036</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.infer_series-1037"><a href="#TypeParser.infer_series-1037"><span class="linenos">1037</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.infer_series-1038"><a href="#TypeParser.infer_series-1038"><span class="linenos">1038</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.infer_series-1039"><a href="#TypeParser.infer_series-1039"><span class="linenos">1039</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.infer_series-1040"><a href="#TypeParser.infer_series-1040"><span class="linenos">1040</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2&quot;, &quot;3.4&quot;])       # float</span>
+</span><span id="TypeParser.infer_series-1041"><a href="#TypeParser.infer_series-1041"><span class="linenos">1041</span></a><span class="sd">			parser.infer_series([&quot;true&quot;, &quot;false&quot;, &quot;2&quot;])  # int</span>
+</span><span id="TypeParser.infer_series-1042"><a href="#TypeParser.infer_series-1042"><span class="linenos">1042</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])     # str</span>
+</span><span id="TypeParser.infer_series-1043"><a href="#TypeParser.infer_series-1043"><span class="linenos">1043</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.infer_series-1044"><a href="#TypeParser.infer_series-1044"><span class="linenos">1044</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.infer_series-1045"><a href="#TypeParser.infer_series-1045"><span class="linenos">1045</span></a>		<span class="k">return</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Infer the underlying common type of a series of strings</p>
 
 <p>If the values in the series do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the series. See <code><a href="#reduce_types">parsetypes.reduce_types()</a></code> for more information.</p>
@@ -2750,71 +2696,70 @@
 <span class="n">parser</span><span class="o">.</span><span class="n">infer_series</span><span class="p">([</span><span class="s2">&quot;1&quot;</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">,</span> <span class="s2">&quot;3.4&quot;</span><span class="p">])</span>       <span class="c1"># float</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">infer_series</span><span class="p">([</span><span class="s2">&quot;true&quot;</span><span class="p">,</span> <span class="s2">&quot;false&quot;</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">])</span>  <span class="c1"># int</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">infer_series</span><span class="p">([</span><span class="s2">&quot;1&quot;</span><span class="p">,</span> <span class="s2">&quot;2.3&quot;</span><span class="p">,</span> <span class="s2">&quot;abc&quot;</span><span class="p">])</span>     <span class="c1"># str</span>
 </code></pre>
 </div></div>
 
 
-
                             </div>
                             <div id="TypeParser.infer_table" class="classattr">
                                         <input id="TypeParser.infer_table-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">infer_table</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Type</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n"><a href="#Nullable">Nullable</a></span><span class="p">,</span> <span class="nb">list</span><span class="p">]]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.infer_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.infer_table"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.infer_table-1042"><a href="#TypeParser.infer_table-1042"><span class="linenos">1042</span></a>	<span class="k">def</span> <span class="nf">infer_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValueType</span><span class="p">]:</span>
-</span><span id="TypeParser.infer_table-1043"><a href="#TypeParser.infer_table-1043"><span class="linenos">1043</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.infer_table-1044"><a href="#TypeParser.infer_table-1044"><span class="linenos">1044</span></a><span class="sd">			Infer the underlying common type for each column of a table of strings</span>
-</span><span id="TypeParser.infer_table-1045"><a href="#TypeParser.infer_table-1045"><span class="linenos">1045</span></a>
-</span><span id="TypeParser.infer_table-1046"><a href="#TypeParser.infer_table-1046"><span class="linenos">1046</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser.infer_table-1047"><a href="#TypeParser.infer_table-1047"><span class="linenos">1047</span></a>
-</span><span id="TypeParser.infer_table-1048"><a href="#TypeParser.infer_table-1048"><span class="linenos">1048</span></a><span class="sd">			Note that the individual inferred types of every value in the table must be able to fit into memory.</span>
-</span><span id="TypeParser.infer_table-1049"><a href="#TypeParser.infer_table-1049"><span class="linenos">1049</span></a>
-</span><span id="TypeParser.infer_table-1050"><a href="#TypeParser.infer_table-1050"><span class="linenos">1050</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser.infer_table-1051"><a href="#TypeParser.infer_table-1051"><span class="linenos">1051</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser.infer_table-1052"><a href="#TypeParser.infer_table-1052"><span class="linenos">1052</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser.infer_table-1053"><a href="#TypeParser.infer_table-1053"><span class="linenos">1053</span></a><span class="sd">			: table of strings for which the types should be inferred, in row-major order</span>
-</span><span id="TypeParser.infer_table-1054"><a href="#TypeParser.infer_table-1054"><span class="linenos">1054</span></a>
-</span><span id="TypeParser.infer_table-1055"><a href="#TypeParser.infer_table-1055"><span class="linenos">1055</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.infer_table-1056"><a href="#TypeParser.infer_table-1056"><span class="linenos">1056</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.infer_table-1057"><a href="#TypeParser.infer_table-1057"><span class="linenos">1057</span></a><span class="sd">			inferred types</span>
-</span><span id="TypeParser.infer_table-1058"><a href="#TypeParser.infer_table-1058"><span class="linenos">1058</span></a>
-</span><span id="TypeParser.infer_table-1059"><a href="#TypeParser.infer_table-1059"><span class="linenos">1059</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.infer_table-1060"><a href="#TypeParser.infer_table-1060"><span class="linenos">1060</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.infer_table-1061"><a href="#TypeParser.infer_table-1061"><span class="linenos">1061</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.infer_table-1062"><a href="#TypeParser.infer_table-1062"><span class="linenos">1062</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.infer_table-1063"><a href="#TypeParser.infer_table-1063"><span class="linenos">1063</span></a><span class="sd">			parser.infer_table([</span>
-</span><span id="TypeParser.infer_table-1064"><a href="#TypeParser.infer_table-1064"><span class="linenos">1064</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser.infer_table-1065"><a href="#TypeParser.infer_table-1065"><span class="linenos">1065</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser.infer_table-1066"><a href="#TypeParser.infer_table-1066"><span class="linenos">1066</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
-</span><span id="TypeParser.infer_table-1067"><a href="#TypeParser.infer_table-1067"><span class="linenos">1067</span></a><span class="sd">			])</span>
-</span><span id="TypeParser.infer_table-1068"><a href="#TypeParser.infer_table-1068"><span class="linenos">1068</span></a><span class="sd">			# [float, int, str]</span>
-</span><span id="TypeParser.infer_table-1069"><a href="#TypeParser.infer_table-1069"><span class="linenos">1069</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.infer_table-1070"><a href="#TypeParser.infer_table-1070"><span class="linenos">1070</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.infer_table-1071"><a href="#TypeParser.infer_table-1071"><span class="linenos">1071</span></a>		<span class="n">rows_iter</span> <span class="o">=</span> <span class="nb">iter</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
-</span><span id="TypeParser.infer_table-1072"><a href="#TypeParser.infer_table-1072"><span class="linenos">1072</span></a>		<span class="n">first_row</span> <span class="o">=</span> <span class="nb">next</span><span class="p">(</span><span class="n">rows_iter</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
-</span><span id="TypeParser.infer_table-1073"><a href="#TypeParser.infer_table-1073"><span class="linenos">1073</span></a>		<span class="k">if</span> <span class="n">first_row</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="TypeParser.infer_table-1074"><a href="#TypeParser.infer_table-1074"><span class="linenos">1074</span></a>			<span class="k">return</span> <span class="p">[]</span>
-</span><span id="TypeParser.infer_table-1075"><a href="#TypeParser.infer_table-1075"><span class="linenos">1075</span></a>
-</span><span id="TypeParser.infer_table-1076"><a href="#TypeParser.infer_table-1076"><span class="linenos">1076</span></a>		<span class="n">num_cols</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">first_row</span><span class="p">)</span>
-</span><span id="TypeParser.infer_table-1077"><a href="#TypeParser.infer_table-1077"><span class="linenos">1077</span></a>		<span class="k">if</span> <span class="n">num_cols</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="TypeParser.infer_table-1078"><a href="#TypeParser.infer_table-1078"><span class="linenos">1078</span></a>			<span class="k">return</span> <span class="p">[]</span>
-</span><span id="TypeParser.infer_table-1079"><a href="#TypeParser.infer_table-1079"><span class="linenos">1079</span></a>
-</span><span id="TypeParser.infer_table-1080"><a href="#TypeParser.infer_table-1080"><span class="linenos">1080</span></a>		<span class="n">table</span> <span class="o">=</span> <span class="n">_TypeTable</span><span class="p">([[</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)]</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">first_row</span><span class="p">])</span>
-</span><span id="TypeParser.infer_table-1081"><a href="#TypeParser.infer_table-1081"><span class="linenos">1081</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows_iter</span><span class="p">:</span>
-</span><span id="TypeParser.infer_table-1082"><a href="#TypeParser.infer_table-1082"><span class="linenos">1082</span></a>			<span class="n">table</span><span class="o">.</span><span class="n">add_row</span><span class="p">([</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">row</span><span class="p">])</span>
-</span><span id="TypeParser.infer_table-1083"><a href="#TypeParser.infer_table-1083"><span class="linenos">1083</span></a>
-</span><span id="TypeParser.infer_table-1084"><a href="#TypeParser.infer_table-1084"><span class="linenos">1084</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">reduce_types</span><span class="p">(</span><span class="n">col</span><span class="p">)</span> <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="n">table</span><span class="o">.</span><span class="n">cols</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.infer_table-1048"><a href="#TypeParser.infer_table-1048"><span class="linenos">1048</span></a>	<span class="k">def</span> <span class="nf">infer_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValueType</span><span class="p">]:</span>
+</span><span id="TypeParser.infer_table-1049"><a href="#TypeParser.infer_table-1049"><span class="linenos">1049</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.infer_table-1050"><a href="#TypeParser.infer_table-1050"><span class="linenos">1050</span></a><span class="sd">			Infer the underlying common type for each column of a table of strings</span>
+</span><span id="TypeParser.infer_table-1051"><a href="#TypeParser.infer_table-1051"><span class="linenos">1051</span></a>
+</span><span id="TypeParser.infer_table-1052"><a href="#TypeParser.infer_table-1052"><span class="linenos">1052</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser.infer_table-1053"><a href="#TypeParser.infer_table-1053"><span class="linenos">1053</span></a>
+</span><span id="TypeParser.infer_table-1054"><a href="#TypeParser.infer_table-1054"><span class="linenos">1054</span></a><span class="sd">			Note that the individual inferred types of every value in the table must be able to fit into memory.</span>
+</span><span id="TypeParser.infer_table-1055"><a href="#TypeParser.infer_table-1055"><span class="linenos">1055</span></a>
+</span><span id="TypeParser.infer_table-1056"><a href="#TypeParser.infer_table-1056"><span class="linenos">1056</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser.infer_table-1057"><a href="#TypeParser.infer_table-1057"><span class="linenos">1057</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser.infer_table-1058"><a href="#TypeParser.infer_table-1058"><span class="linenos">1058</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser.infer_table-1059"><a href="#TypeParser.infer_table-1059"><span class="linenos">1059</span></a><span class="sd">			: table of strings for which the types should be inferred, in row-major order</span>
+</span><span id="TypeParser.infer_table-1060"><a href="#TypeParser.infer_table-1060"><span class="linenos">1060</span></a>
+</span><span id="TypeParser.infer_table-1061"><a href="#TypeParser.infer_table-1061"><span class="linenos">1061</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.infer_table-1062"><a href="#TypeParser.infer_table-1062"><span class="linenos">1062</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.infer_table-1063"><a href="#TypeParser.infer_table-1063"><span class="linenos">1063</span></a><span class="sd">			inferred types</span>
+</span><span id="TypeParser.infer_table-1064"><a href="#TypeParser.infer_table-1064"><span class="linenos">1064</span></a>
+</span><span id="TypeParser.infer_table-1065"><a href="#TypeParser.infer_table-1065"><span class="linenos">1065</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.infer_table-1066"><a href="#TypeParser.infer_table-1066"><span class="linenos">1066</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.infer_table-1067"><a href="#TypeParser.infer_table-1067"><span class="linenos">1067</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.infer_table-1068"><a href="#TypeParser.infer_table-1068"><span class="linenos">1068</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.infer_table-1069"><a href="#TypeParser.infer_table-1069"><span class="linenos">1069</span></a><span class="sd">			parser.infer_table([</span>
+</span><span id="TypeParser.infer_table-1070"><a href="#TypeParser.infer_table-1070"><span class="linenos">1070</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser.infer_table-1071"><a href="#TypeParser.infer_table-1071"><span class="linenos">1071</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser.infer_table-1072"><a href="#TypeParser.infer_table-1072"><span class="linenos">1072</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
+</span><span id="TypeParser.infer_table-1073"><a href="#TypeParser.infer_table-1073"><span class="linenos">1073</span></a><span class="sd">			])</span>
+</span><span id="TypeParser.infer_table-1074"><a href="#TypeParser.infer_table-1074"><span class="linenos">1074</span></a><span class="sd">			# [float, int, str]</span>
+</span><span id="TypeParser.infer_table-1075"><a href="#TypeParser.infer_table-1075"><span class="linenos">1075</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.infer_table-1076"><a href="#TypeParser.infer_table-1076"><span class="linenos">1076</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.infer_table-1077"><a href="#TypeParser.infer_table-1077"><span class="linenos">1077</span></a>		<span class="n">rows_iter</span> <span class="o">=</span> <span class="nb">iter</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
+</span><span id="TypeParser.infer_table-1078"><a href="#TypeParser.infer_table-1078"><span class="linenos">1078</span></a>		<span class="n">first_row</span> <span class="o">=</span> <span class="nb">next</span><span class="p">(</span><span class="n">rows_iter</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
+</span><span id="TypeParser.infer_table-1079"><a href="#TypeParser.infer_table-1079"><span class="linenos">1079</span></a>		<span class="k">if</span> <span class="n">first_row</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="TypeParser.infer_table-1080"><a href="#TypeParser.infer_table-1080"><span class="linenos">1080</span></a>			<span class="k">return</span> <span class="p">[]</span>
+</span><span id="TypeParser.infer_table-1081"><a href="#TypeParser.infer_table-1081"><span class="linenos">1081</span></a>
+</span><span id="TypeParser.infer_table-1082"><a href="#TypeParser.infer_table-1082"><span class="linenos">1082</span></a>		<span class="n">num_cols</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">first_row</span><span class="p">)</span>
+</span><span id="TypeParser.infer_table-1083"><a href="#TypeParser.infer_table-1083"><span class="linenos">1083</span></a>		<span class="k">if</span> <span class="n">num_cols</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="TypeParser.infer_table-1084"><a href="#TypeParser.infer_table-1084"><span class="linenos">1084</span></a>			<span class="k">return</span> <span class="p">[]</span>
+</span><span id="TypeParser.infer_table-1085"><a href="#TypeParser.infer_table-1085"><span class="linenos">1085</span></a>
+</span><span id="TypeParser.infer_table-1086"><a href="#TypeParser.infer_table-1086"><span class="linenos">1086</span></a>		<span class="n">table</span> <span class="o">=</span> <span class="n">_TypeTable</span><span class="p">([[</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)]</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">first_row</span><span class="p">])</span>
+</span><span id="TypeParser.infer_table-1087"><a href="#TypeParser.infer_table-1087"><span class="linenos">1087</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows_iter</span><span class="p">:</span>
+</span><span id="TypeParser.infer_table-1088"><a href="#TypeParser.infer_table-1088"><span class="linenos">1088</span></a>			<span class="n">table</span><span class="o">.</span><span class="n">add_row</span><span class="p">([</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">row</span><span class="p">])</span>
+</span><span id="TypeParser.infer_table-1089"><a href="#TypeParser.infer_table-1089"><span class="linenos">1089</span></a>
+</span><span id="TypeParser.infer_table-1090"><a href="#TypeParser.infer_table-1090"><span class="linenos">1090</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">reduce_types</span><span class="p">(</span><span class="n">col</span><span class="p">)</span> <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="n">table</span><span class="o">.</span><span class="n">cols</span><span class="p">]</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Infer the underlying common type for each column of a table of strings</p>
 
 <p>For each column, if the values do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the column. See <code><a href="#reduce_types">parsetypes.reduce_types()</a></code> for more information.</p>
@@ -2840,96 +2785,95 @@
 	<span class="p">[</span><span class="s2">&quot;3.4&quot;</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">,</span>     <span class="s2">&quot;abc&quot;</span><span class="p">],</span>
 <span class="p">])</span>
 <span class="c1"># [float, int, str]</span>
 </code></pre>
 </div></div>
 
 
-
                             </div>
                             <div id="TypeParser.convert" class="classattr">
                                         <input id="TypeParser.convert-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">convert</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">target_type</span><span class="p">:</span> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n"><a href="#Nullable">Nullable</a></span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="nb">list</span><span class="p">]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.convert-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.convert"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.convert-1087"><a href="#TypeParser.convert-1087"><span class="linenos">1087</span></a>	<span class="k">def</span> <span class="nf">convert</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_type</span><span class="p">:</span> <span class="n">AnyValueType</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
-</span><span id="TypeParser.convert-1088"><a href="#TypeParser.convert-1088"><span class="linenos">1088</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.convert-1089"><a href="#TypeParser.convert-1089"><span class="linenos">1089</span></a><span class="sd">			Convert a string to the specified target type if possible</span>
-</span><span id="TypeParser.convert-1090"><a href="#TypeParser.convert-1090"><span class="linenos">1090</span></a>
-</span><span id="TypeParser.convert-1091"><a href="#TypeParser.convert-1091"><span class="linenos">1091</span></a><span class="sd">			Valid values for `target_type` include any return value from `infer()`, `infer_series()` and `infer_table()`. To infer and convert the string automatically, use `parse()`, `parse_series()` or `parse_table()` instead.</span>
-</span><span id="TypeParser.convert-1092"><a href="#TypeParser.convert-1092"><span class="linenos">1092</span></a>
-</span><span id="TypeParser.convert-1093"><a href="#TypeParser.convert-1093"><span class="linenos">1093</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser.convert-1094"><a href="#TypeParser.convert-1094"><span class="linenos">1094</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser.convert-1095"><a href="#TypeParser.convert-1095"><span class="linenos">1095</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser.convert-1096"><a href="#TypeParser.convert-1096"><span class="linenos">1096</span></a><span class="sd">			: the string to be converted</span>
-</span><span id="TypeParser.convert-1097"><a href="#TypeParser.convert-1097"><span class="linenos">1097</span></a>
-</span><span id="TypeParser.convert-1098"><a href="#TypeParser.convert-1098"><span class="linenos">1098</span></a><span class="sd">			`target_type`</span>
-</span><span id="TypeParser.convert-1099"><a href="#TypeParser.convert-1099"><span class="linenos">1099</span></a><span class="sd">			: type to which the value should be converted</span>
-</span><span id="TypeParser.convert-1100"><a href="#TypeParser.convert-1100"><span class="linenos">1100</span></a>
-</span><span id="TypeParser.convert-1101"><a href="#TypeParser.convert-1101"><span class="linenos">1101</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.convert-1102"><a href="#TypeParser.convert-1102"><span class="linenos">1102</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.convert-1103"><a href="#TypeParser.convert-1103"><span class="linenos">1103</span></a><span class="sd">			converted value</span>
-</span><span id="TypeParser.convert-1104"><a href="#TypeParser.convert-1104"><span class="linenos">1104</span></a>
-</span><span id="TypeParser.convert-1105"><a href="#TypeParser.convert-1105"><span class="linenos">1105</span></a><span class="sd">			Raises</span>
-</span><span id="TypeParser.convert-1106"><a href="#TypeParser.convert-1106"><span class="linenos">1106</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.convert-1107"><a href="#TypeParser.convert-1107"><span class="linenos">1107</span></a><span class="sd">			`ValueError`</span>
-</span><span id="TypeParser.convert-1108"><a href="#TypeParser.convert-1108"><span class="linenos">1108</span></a><span class="sd">			: if `value` cannot be converted to `target_type`</span>
-</span><span id="TypeParser.convert-1109"><a href="#TypeParser.convert-1109"><span class="linenos">1109</span></a>
-</span><span id="TypeParser.convert-1110"><a href="#TypeParser.convert-1110"><span class="linenos">1110</span></a><span class="sd">			`TypeError`</span>
-</span><span id="TypeParser.convert-1111"><a href="#TypeParser.convert-1111"><span class="linenos">1111</span></a><span class="sd">			: if `target_type` is not a valid type</span>
-</span><span id="TypeParser.convert-1112"><a href="#TypeParser.convert-1112"><span class="linenos">1112</span></a>
-</span><span id="TypeParser.convert-1113"><a href="#TypeParser.convert-1113"><span class="linenos">1113</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.convert-1114"><a href="#TypeParser.convert-1114"><span class="linenos">1114</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.convert-1115"><a href="#TypeParser.convert-1115"><span class="linenos">1115</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.convert-1116"><a href="#TypeParser.convert-1116"><span class="linenos">1116</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.convert-1117"><a href="#TypeParser.convert-1117"><span class="linenos">1117</span></a><span class="sd">			parser.convert(&quot;true&quot;, bool)  # True</span>
-</span><span id="TypeParser.convert-1118"><a href="#TypeParser.convert-1118"><span class="linenos">1118</span></a><span class="sd">			parser.convert(&quot;2&quot;, int)      # 2</span>
-</span><span id="TypeParser.convert-1119"><a href="#TypeParser.convert-1119"><span class="linenos">1119</span></a><span class="sd">			parser.convert(&quot;2&quot;, float)    # 2.</span>
-</span><span id="TypeParser.convert-1120"><a href="#TypeParser.convert-1120"><span class="linenos">1120</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.convert-1121"><a href="#TypeParser.convert-1121"><span class="linenos">1121</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.convert-1122"><a href="#TypeParser.convert-1122"><span class="linenos">1122</span></a>		<span class="n">base</span><span class="p">,</span> <span class="n">type_args</span> <span class="o">=</span> <span class="n">_decompose_type</span><span class="p">(</span><span class="n">target_type</span><span class="p">)</span>
-</span><span id="TypeParser.convert-1123"><a href="#TypeParser.convert-1123"><span class="linenos">1123</span></a>		<span class="k">if</span> <span class="n">base</span> <span class="o">==</span> <span class="n">NoneType</span><span class="p">:</span>
-</span><span id="TypeParser.convert-1124"><a href="#TypeParser.convert-1124"><span class="linenos">1124</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_none</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser.convert-1125"><a href="#TypeParser.convert-1125"><span class="linenos">1125</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="TypeParser.convert-1126"><a href="#TypeParser.convert-1126"><span class="linenos">1126</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser.convert-1127"><a href="#TypeParser.convert-1127"><span class="linenos">1127</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="TypeParser.convert-1128"><a href="#TypeParser.convert-1128"><span class="linenos">1128</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser.convert-1129"><a href="#TypeParser.convert-1129"><span class="linenos">1129</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Decimal</span><span class="p">:</span>
-</span><span id="TypeParser.convert-1130"><a href="#TypeParser.convert-1130"><span class="linenos">1130</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_decimal</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser.convert-1131"><a href="#TypeParser.convert-1131"><span class="linenos">1131</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="TypeParser.convert-1132"><a href="#TypeParser.convert-1132"><span class="linenos">1132</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser.convert-1133"><a href="#TypeParser.convert-1133"><span class="linenos">1133</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="TypeParser.convert-1134"><a href="#TypeParser.convert-1134"><span class="linenos">1134</span></a>			<span class="k">return</span> <span class="n">value</span>
-</span><span id="TypeParser.convert-1135"><a href="#TypeParser.convert-1135"><span class="linenos">1135</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Nullable</span><span class="p">:</span>
-</span><span id="TypeParser.convert-1136"><a href="#TypeParser.convert-1136"><span class="linenos">1136</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser.convert-1137"><a href="#TypeParser.convert-1137"><span class="linenos">1137</span></a>				<span class="k">return</span> <span class="kc">None</span>
-</span><span id="TypeParser.convert-1138"><a href="#TypeParser.convert-1138"><span class="linenos">1138</span></a>			<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser.convert-1139"><a href="#TypeParser.convert-1139"><span class="linenos">1139</span></a>				<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="TypeParser.convert-1140"><a href="#TypeParser.convert-1140"><span class="linenos">1140</span></a>					<span class="n">inner_type</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="TypeParser.convert-1141"><a href="#TypeParser.convert-1141"><span class="linenos">1141</span></a>					<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inner_type</span><span class="p">)</span>
-</span><span id="TypeParser.convert-1142"><a href="#TypeParser.convert-1142"><span class="linenos">1142</span></a>				<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser.convert-1143"><a href="#TypeParser.convert-1143"><span class="linenos">1143</span></a>					<span class="k">return</span> <span class="n">value</span>
-</span><span id="TypeParser.convert-1144"><a href="#TypeParser.convert-1144"><span class="linenos">1144</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">list</span><span class="p">:</span>
-</span><span id="TypeParser.convert-1145"><a href="#TypeParser.convert-1145"><span class="linenos">1145</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_list_delimiter</span><span class="p">)</span>
-</span><span id="TypeParser.convert-1146"><a href="#TypeParser.convert-1146"><span class="linenos">1146</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
-</span><span id="TypeParser.convert-1147"><a href="#TypeParser.convert-1147"><span class="linenos">1147</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
-</span><span id="TypeParser.convert-1148"><a href="#TypeParser.convert-1148"><span class="linenos">1148</span></a>			<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="TypeParser.convert-1149"><a href="#TypeParser.convert-1149"><span class="linenos">1149</span></a>				<span class="n">subtype</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="TypeParser.convert-1150"><a href="#TypeParser.convert-1150"><span class="linenos">1150</span></a>				<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">subvalue</span><span class="p">,</span> <span class="n">subtype</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
-</span><span id="TypeParser.convert-1151"><a href="#TypeParser.convert-1151"><span class="linenos">1151</span></a>			<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser.convert-1152"><a href="#TypeParser.convert-1152"><span class="linenos">1152</span></a>				<span class="k">return</span> <span class="n">subvalues</span>
-</span><span id="TypeParser.convert-1153"><a href="#TypeParser.convert-1153"><span class="linenos">1153</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser.convert-1154"><a href="#TypeParser.convert-1154"><span class="linenos">1154</span></a>			<span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot convert to type: </span><span class="si">{</span><span class="n">target_type</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.convert-1093"><a href="#TypeParser.convert-1093"><span class="linenos">1093</span></a>	<span class="k">def</span> <span class="nf">convert</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_type</span><span class="p">:</span> <span class="n">AnyValueType</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
+</span><span id="TypeParser.convert-1094"><a href="#TypeParser.convert-1094"><span class="linenos">1094</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.convert-1095"><a href="#TypeParser.convert-1095"><span class="linenos">1095</span></a><span class="sd">			Convert a string to the specified target type if possible</span>
+</span><span id="TypeParser.convert-1096"><a href="#TypeParser.convert-1096"><span class="linenos">1096</span></a>
+</span><span id="TypeParser.convert-1097"><a href="#TypeParser.convert-1097"><span class="linenos">1097</span></a><span class="sd">			Valid values for `target_type` include any return value from `infer()`, `infer_series()` and `infer_table()`. To infer and convert the string automatically, use `parse()`, `parse_series()` or `parse_table()` instead.</span>
+</span><span id="TypeParser.convert-1098"><a href="#TypeParser.convert-1098"><span class="linenos">1098</span></a>
+</span><span id="TypeParser.convert-1099"><a href="#TypeParser.convert-1099"><span class="linenos">1099</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser.convert-1100"><a href="#TypeParser.convert-1100"><span class="linenos">1100</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser.convert-1101"><a href="#TypeParser.convert-1101"><span class="linenos">1101</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser.convert-1102"><a href="#TypeParser.convert-1102"><span class="linenos">1102</span></a><span class="sd">			: the string to be converted</span>
+</span><span id="TypeParser.convert-1103"><a href="#TypeParser.convert-1103"><span class="linenos">1103</span></a>
+</span><span id="TypeParser.convert-1104"><a href="#TypeParser.convert-1104"><span class="linenos">1104</span></a><span class="sd">			`target_type`</span>
+</span><span id="TypeParser.convert-1105"><a href="#TypeParser.convert-1105"><span class="linenos">1105</span></a><span class="sd">			: type to which the value should be converted</span>
+</span><span id="TypeParser.convert-1106"><a href="#TypeParser.convert-1106"><span class="linenos">1106</span></a>
+</span><span id="TypeParser.convert-1107"><a href="#TypeParser.convert-1107"><span class="linenos">1107</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.convert-1108"><a href="#TypeParser.convert-1108"><span class="linenos">1108</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.convert-1109"><a href="#TypeParser.convert-1109"><span class="linenos">1109</span></a><span class="sd">			converted value</span>
+</span><span id="TypeParser.convert-1110"><a href="#TypeParser.convert-1110"><span class="linenos">1110</span></a>
+</span><span id="TypeParser.convert-1111"><a href="#TypeParser.convert-1111"><span class="linenos">1111</span></a><span class="sd">			Raises</span>
+</span><span id="TypeParser.convert-1112"><a href="#TypeParser.convert-1112"><span class="linenos">1112</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.convert-1113"><a href="#TypeParser.convert-1113"><span class="linenos">1113</span></a><span class="sd">			`ValueError`</span>
+</span><span id="TypeParser.convert-1114"><a href="#TypeParser.convert-1114"><span class="linenos">1114</span></a><span class="sd">			: if `value` cannot be converted to `target_type`</span>
+</span><span id="TypeParser.convert-1115"><a href="#TypeParser.convert-1115"><span class="linenos">1115</span></a>
+</span><span id="TypeParser.convert-1116"><a href="#TypeParser.convert-1116"><span class="linenos">1116</span></a><span class="sd">			`TypeError`</span>
+</span><span id="TypeParser.convert-1117"><a href="#TypeParser.convert-1117"><span class="linenos">1117</span></a><span class="sd">			: if `target_type` is not a valid type</span>
+</span><span id="TypeParser.convert-1118"><a href="#TypeParser.convert-1118"><span class="linenos">1118</span></a>
+</span><span id="TypeParser.convert-1119"><a href="#TypeParser.convert-1119"><span class="linenos">1119</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.convert-1120"><a href="#TypeParser.convert-1120"><span class="linenos">1120</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.convert-1121"><a href="#TypeParser.convert-1121"><span class="linenos">1121</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.convert-1122"><a href="#TypeParser.convert-1122"><span class="linenos">1122</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.convert-1123"><a href="#TypeParser.convert-1123"><span class="linenos">1123</span></a><span class="sd">			parser.convert(&quot;true&quot;, bool)  # True</span>
+</span><span id="TypeParser.convert-1124"><a href="#TypeParser.convert-1124"><span class="linenos">1124</span></a><span class="sd">			parser.convert(&quot;2&quot;, int)      # 2</span>
+</span><span id="TypeParser.convert-1125"><a href="#TypeParser.convert-1125"><span class="linenos">1125</span></a><span class="sd">			parser.convert(&quot;2&quot;, float)    # 2.</span>
+</span><span id="TypeParser.convert-1126"><a href="#TypeParser.convert-1126"><span class="linenos">1126</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.convert-1127"><a href="#TypeParser.convert-1127"><span class="linenos">1127</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.convert-1128"><a href="#TypeParser.convert-1128"><span class="linenos">1128</span></a>		<span class="n">base</span><span class="p">,</span> <span class="n">type_args</span> <span class="o">=</span> <span class="n">_decompose_type</span><span class="p">(</span><span class="n">target_type</span><span class="p">)</span>
+</span><span id="TypeParser.convert-1129"><a href="#TypeParser.convert-1129"><span class="linenos">1129</span></a>		<span class="k">if</span> <span class="n">base</span> <span class="o">==</span> <span class="n">NoneType</span><span class="p">:</span>
+</span><span id="TypeParser.convert-1130"><a href="#TypeParser.convert-1130"><span class="linenos">1130</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_none</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser.convert-1131"><a href="#TypeParser.convert-1131"><span class="linenos">1131</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="TypeParser.convert-1132"><a href="#TypeParser.convert-1132"><span class="linenos">1132</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser.convert-1133"><a href="#TypeParser.convert-1133"><span class="linenos">1133</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="TypeParser.convert-1134"><a href="#TypeParser.convert-1134"><span class="linenos">1134</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser.convert-1135"><a href="#TypeParser.convert-1135"><span class="linenos">1135</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Decimal</span><span class="p">:</span>
+</span><span id="TypeParser.convert-1136"><a href="#TypeParser.convert-1136"><span class="linenos">1136</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_decimal</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser.convert-1137"><a href="#TypeParser.convert-1137"><span class="linenos">1137</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="TypeParser.convert-1138"><a href="#TypeParser.convert-1138"><span class="linenos">1138</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser.convert-1139"><a href="#TypeParser.convert-1139"><span class="linenos">1139</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser.convert-1140"><a href="#TypeParser.convert-1140"><span class="linenos">1140</span></a>			<span class="k">return</span> <span class="n">value</span>
+</span><span id="TypeParser.convert-1141"><a href="#TypeParser.convert-1141"><span class="linenos">1141</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Nullable</span><span class="p">:</span>
+</span><span id="TypeParser.convert-1142"><a href="#TypeParser.convert-1142"><span class="linenos">1142</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser.convert-1143"><a href="#TypeParser.convert-1143"><span class="linenos">1143</span></a>				<span class="k">return</span> <span class="kc">None</span>
+</span><span id="TypeParser.convert-1144"><a href="#TypeParser.convert-1144"><span class="linenos">1144</span></a>			<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser.convert-1145"><a href="#TypeParser.convert-1145"><span class="linenos">1145</span></a>				<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser.convert-1146"><a href="#TypeParser.convert-1146"><span class="linenos">1146</span></a>					<span class="n">inner_type</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="TypeParser.convert-1147"><a href="#TypeParser.convert-1147"><span class="linenos">1147</span></a>					<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inner_type</span><span class="p">)</span>
+</span><span id="TypeParser.convert-1148"><a href="#TypeParser.convert-1148"><span class="linenos">1148</span></a>				<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser.convert-1149"><a href="#TypeParser.convert-1149"><span class="linenos">1149</span></a>					<span class="k">return</span> <span class="n">value</span>
+</span><span id="TypeParser.convert-1150"><a href="#TypeParser.convert-1150"><span class="linenos">1150</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">list</span><span class="p">:</span>
+</span><span id="TypeParser.convert-1151"><a href="#TypeParser.convert-1151"><span class="linenos">1151</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_list_delimiter</span><span class="p">)</span>
+</span><span id="TypeParser.convert-1152"><a href="#TypeParser.convert-1152"><span class="linenos">1152</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_trim</span><span class="p">:</span>
+</span><span id="TypeParser.convert-1153"><a href="#TypeParser.convert-1153"><span class="linenos">1153</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
+</span><span id="TypeParser.convert-1154"><a href="#TypeParser.convert-1154"><span class="linenos">1154</span></a>			<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser.convert-1155"><a href="#TypeParser.convert-1155"><span class="linenos">1155</span></a>				<span class="n">subtype</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="TypeParser.convert-1156"><a href="#TypeParser.convert-1156"><span class="linenos">1156</span></a>				<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">subvalue</span><span class="p">,</span> <span class="n">subtype</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
+</span><span id="TypeParser.convert-1157"><a href="#TypeParser.convert-1157"><span class="linenos">1157</span></a>			<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser.convert-1158"><a href="#TypeParser.convert-1158"><span class="linenos">1158</span></a>				<span class="k">return</span> <span class="n">subvalues</span>
+</span><span id="TypeParser.convert-1159"><a href="#TypeParser.convert-1159"><span class="linenos">1159</span></a>		<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser.convert-1160"><a href="#TypeParser.convert-1160"><span class="linenos">1160</span></a>			<span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot convert to type: </span><span class="si">{</span><span class="n">target_type</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Convert a string to the specified target type if possible</p>
 
 <p>Valid values for <code>target_type</code> include any return value from <code><a href="#TypeParser.infer">infer()</a></code>, <code><a href="#TypeParser.infer_series">infer_series()</a></code> and <code><a href="#TypeParser.infer_table">infer_table()</a></code>. To infer and convert the string automatically, use <code><a href="#TypeParser.parse">parse()</a></code>, <code><a href="#TypeParser.parse_series">parse_series()</a></code> or <code><a href="#TypeParser.parse_table">parse_table()</a></code> instead.</p>
@@ -2961,51 +2905,50 @@
 <span class="n">parser</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="s2">&quot;true&quot;</span><span class="p">,</span> <span class="nb">bool</span><span class="p">)</span>  <span class="c1"># True</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="s2">&quot;2&quot;</span><span class="p">,</span> <span class="nb">int</span><span class="p">)</span>      <span class="c1"># 2</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="s2">&quot;2&quot;</span><span class="p">,</span> <span class="nb">float</span><span class="p">)</span>    <span class="c1"># 2.</span>
 </code></pre>
 </div></div>
 
 
-
                             </div>
                             <div id="TypeParser.parse" class="classattr">
                                         <input id="TypeParser.parse-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">parse</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="nb">list</span><span class="p">]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.parse-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.parse"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse-1157"><a href="#TypeParser.parse-1157"><span class="linenos">1157</span></a>	<span class="k">def</span> <span class="nf">parse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
-</span><span id="TypeParser.parse-1158"><a href="#TypeParser.parse-1158"><span class="linenos">1158</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse-1159"><a href="#TypeParser.parse-1159"><span class="linenos">1159</span></a><span class="sd">			Parse a string and convert it to its underlying type</span>
-</span><span id="TypeParser.parse-1160"><a href="#TypeParser.parse-1160"><span class="linenos">1160</span></a>
-</span><span id="TypeParser.parse-1161"><a href="#TypeParser.parse-1161"><span class="linenos">1161</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser.parse-1162"><a href="#TypeParser.parse-1162"><span class="linenos">1162</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser.parse-1163"><a href="#TypeParser.parse-1163"><span class="linenos">1163</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser.parse-1164"><a href="#TypeParser.parse-1164"><span class="linenos">1164</span></a><span class="sd">			: the string to be parsed</span>
-</span><span id="TypeParser.parse-1165"><a href="#TypeParser.parse-1165"><span class="linenos">1165</span></a>
-</span><span id="TypeParser.parse-1166"><a href="#TypeParser.parse-1166"><span class="linenos">1166</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.parse-1167"><a href="#TypeParser.parse-1167"><span class="linenos">1167</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.parse-1168"><a href="#TypeParser.parse-1168"><span class="linenos">1168</span></a><span class="sd">			converted value</span>
-</span><span id="TypeParser.parse-1169"><a href="#TypeParser.parse-1169"><span class="linenos">1169</span></a>
-</span><span id="TypeParser.parse-1170"><a href="#TypeParser.parse-1170"><span class="linenos">1170</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.parse-1171"><a href="#TypeParser.parse-1171"><span class="linenos">1171</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.parse-1172"><a href="#TypeParser.parse-1172"><span class="linenos">1172</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.parse-1173"><a href="#TypeParser.parse-1173"><span class="linenos">1173</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.parse-1174"><a href="#TypeParser.parse-1174"><span class="linenos">1174</span></a><span class="sd">			parser.parse(&quot;true&quot;)  # True</span>
-</span><span id="TypeParser.parse-1175"><a href="#TypeParser.parse-1175"><span class="linenos">1175</span></a><span class="sd">			parser.parse(&quot;2.0&quot;)   # 2.</span>
-</span><span id="TypeParser.parse-1176"><a href="#TypeParser.parse-1176"><span class="linenos">1176</span></a><span class="sd">			parser.parse(&quot;abc&quot;)   # &quot;abc&quot;</span>
-</span><span id="TypeParser.parse-1177"><a href="#TypeParser.parse-1177"><span class="linenos">1177</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.parse-1178"><a href="#TypeParser.parse-1178"><span class="linenos">1178</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse-1179"><a href="#TypeParser.parse-1179"><span class="linenos">1179</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse-1163"><a href="#TypeParser.parse-1163"><span class="linenos">1163</span></a>	<span class="k">def</span> <span class="nf">parse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
+</span><span id="TypeParser.parse-1164"><a href="#TypeParser.parse-1164"><span class="linenos">1164</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse-1165"><a href="#TypeParser.parse-1165"><span class="linenos">1165</span></a><span class="sd">			Parse a string and convert it to its underlying type</span>
+</span><span id="TypeParser.parse-1166"><a href="#TypeParser.parse-1166"><span class="linenos">1166</span></a>
+</span><span id="TypeParser.parse-1167"><a href="#TypeParser.parse-1167"><span class="linenos">1167</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser.parse-1168"><a href="#TypeParser.parse-1168"><span class="linenos">1168</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser.parse-1169"><a href="#TypeParser.parse-1169"><span class="linenos">1169</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser.parse-1170"><a href="#TypeParser.parse-1170"><span class="linenos">1170</span></a><span class="sd">			: the string to be parsed</span>
+</span><span id="TypeParser.parse-1171"><a href="#TypeParser.parse-1171"><span class="linenos">1171</span></a>
+</span><span id="TypeParser.parse-1172"><a href="#TypeParser.parse-1172"><span class="linenos">1172</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.parse-1173"><a href="#TypeParser.parse-1173"><span class="linenos">1173</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.parse-1174"><a href="#TypeParser.parse-1174"><span class="linenos">1174</span></a><span class="sd">			converted value</span>
+</span><span id="TypeParser.parse-1175"><a href="#TypeParser.parse-1175"><span class="linenos">1175</span></a>
+</span><span id="TypeParser.parse-1176"><a href="#TypeParser.parse-1176"><span class="linenos">1176</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.parse-1177"><a href="#TypeParser.parse-1177"><span class="linenos">1177</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.parse-1178"><a href="#TypeParser.parse-1178"><span class="linenos">1178</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.parse-1179"><a href="#TypeParser.parse-1179"><span class="linenos">1179</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.parse-1180"><a href="#TypeParser.parse-1180"><span class="linenos">1180</span></a><span class="sd">			parser.parse(&quot;true&quot;)  # True</span>
+</span><span id="TypeParser.parse-1181"><a href="#TypeParser.parse-1181"><span class="linenos">1181</span></a><span class="sd">			parser.parse(&quot;2.0&quot;)   # 2.</span>
+</span><span id="TypeParser.parse-1182"><a href="#TypeParser.parse-1182"><span class="linenos">1182</span></a><span class="sd">			parser.parse(&quot;abc&quot;)   # &quot;abc&quot;</span>
+</span><span id="TypeParser.parse-1183"><a href="#TypeParser.parse-1183"><span class="linenos">1183</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.parse-1184"><a href="#TypeParser.parse-1184"><span class="linenos">1184</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse-1185"><a href="#TypeParser.parse-1185"><span class="linenos">1185</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Parse a string and convert it to its underlying type</p>
 
 <h2 id="arguments">Arguments</h2>
@@ -3024,55 +2967,54 @@
 <span class="n">parser</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="s2">&quot;true&quot;</span><span class="p">)</span>  <span class="c1"># True</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="s2">&quot;2.0&quot;</span><span class="p">)</span>   <span class="c1"># 2.</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="s2">&quot;abc&quot;</span><span class="p">)</span>   <span class="c1"># &quot;abc&quot;</span>
 </code></pre>
 </div></div>
 
 
-
                             </div>
                             <div id="TypeParser.parse_series" class="classattr">
                                         <input id="TypeParser.parse_series-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">parse_series</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.parse_series-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.parse_series"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_series-1182"><a href="#TypeParser.parse_series-1182"><span class="linenos">1182</span></a>	<span class="k">def</span> <span class="nf">parse_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]:</span>
-</span><span id="TypeParser.parse_series-1183"><a href="#TypeParser.parse_series-1183"><span class="linenos">1183</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_series-1184"><a href="#TypeParser.parse_series-1184"><span class="linenos">1184</span></a><span class="sd">			Parse a series of strings and convert them to their underlying common type</span>
-</span><span id="TypeParser.parse_series-1185"><a href="#TypeParser.parse_series-1185"><span class="linenos">1185</span></a>
-</span><span id="TypeParser.parse_series-1186"><a href="#TypeParser.parse_series-1186"><span class="linenos">1186</span></a><span class="sd">			If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser.parse_series-1187"><a href="#TypeParser.parse_series-1187"><span class="linenos">1187</span></a>
-</span><span id="TypeParser.parse_series-1188"><a href="#TypeParser.parse_series-1188"><span class="linenos">1188</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser.parse_series-1189"><a href="#TypeParser.parse_series-1189"><span class="linenos">1189</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser.parse_series-1190"><a href="#TypeParser.parse_series-1190"><span class="linenos">1190</span></a><span class="sd">			`values`</span>
-</span><span id="TypeParser.parse_series-1191"><a href="#TypeParser.parse_series-1191"><span class="linenos">1191</span></a><span class="sd">			: series of strings to be parsed</span>
-</span><span id="TypeParser.parse_series-1192"><a href="#TypeParser.parse_series-1192"><span class="linenos">1192</span></a>
-</span><span id="TypeParser.parse_series-1193"><a href="#TypeParser.parse_series-1193"><span class="linenos">1193</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.parse_series-1194"><a href="#TypeParser.parse_series-1194"><span class="linenos">1194</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.parse_series-1195"><a href="#TypeParser.parse_series-1195"><span class="linenos">1195</span></a><span class="sd">			converted values</span>
-</span><span id="TypeParser.parse_series-1196"><a href="#TypeParser.parse_series-1196"><span class="linenos">1196</span></a>
-</span><span id="TypeParser.parse_series-1197"><a href="#TypeParser.parse_series-1197"><span class="linenos">1197</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.parse_series-1198"><a href="#TypeParser.parse_series-1198"><span class="linenos">1198</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.parse_series-1199"><a href="#TypeParser.parse_series-1199"><span class="linenos">1199</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.parse_series-1200"><a href="#TypeParser.parse_series-1200"><span class="linenos">1200</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.parse_series-1201"><a href="#TypeParser.parse_series-1201"><span class="linenos">1201</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2&quot;, &quot;3&quot;])        # [1, 2, 3]</span>
-</span><span id="TypeParser.parse_series-1202"><a href="#TypeParser.parse_series-1202"><span class="linenos">1202</span></a><span class="sd">			parser.parse_series([&quot;5&quot;, &quot;6.7&quot;, &quot;8.&quot;])     # [5., 6.7, 8.]</span>
-</span><span id="TypeParser.parse_series-1203"><a href="#TypeParser.parse_series-1203"><span class="linenos">1203</span></a><span class="sd">			parser.parse_series([&quot;true&quot;, &quot;false&quot;, &quot;&quot;])  # [True, False, None]</span>
-</span><span id="TypeParser.parse_series-1204"><a href="#TypeParser.parse_series-1204"><span class="linenos">1204</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])    # [&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;]</span>
-</span><span id="TypeParser.parse_series-1205"><a href="#TypeParser.parse_series-1205"><span class="linenos">1205</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.parse_series-1206"><a href="#TypeParser.parse_series-1206"><span class="linenos">1206</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_series-1207"><a href="#TypeParser.parse_series-1207"><span class="linenos">1207</span></a>		<span class="n">inferred</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_series</span><span class="p">(</span><span class="n">values</span><span class="p">)</span>
-</span><span id="TypeParser.parse_series-1208"><a href="#TypeParser.parse_series-1208"><span class="linenos">1208</span></a>		<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_series-1188"><a href="#TypeParser.parse_series-1188"><span class="linenos">1188</span></a>	<span class="k">def</span> <span class="nf">parse_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]:</span>
+</span><span id="TypeParser.parse_series-1189"><a href="#TypeParser.parse_series-1189"><span class="linenos">1189</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_series-1190"><a href="#TypeParser.parse_series-1190"><span class="linenos">1190</span></a><span class="sd">			Parse a series of strings and convert them to their underlying common type</span>
+</span><span id="TypeParser.parse_series-1191"><a href="#TypeParser.parse_series-1191"><span class="linenos">1191</span></a>
+</span><span id="TypeParser.parse_series-1192"><a href="#TypeParser.parse_series-1192"><span class="linenos">1192</span></a><span class="sd">			If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser.parse_series-1193"><a href="#TypeParser.parse_series-1193"><span class="linenos">1193</span></a>
+</span><span id="TypeParser.parse_series-1194"><a href="#TypeParser.parse_series-1194"><span class="linenos">1194</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser.parse_series-1195"><a href="#TypeParser.parse_series-1195"><span class="linenos">1195</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser.parse_series-1196"><a href="#TypeParser.parse_series-1196"><span class="linenos">1196</span></a><span class="sd">			`values`</span>
+</span><span id="TypeParser.parse_series-1197"><a href="#TypeParser.parse_series-1197"><span class="linenos">1197</span></a><span class="sd">			: series of strings to be parsed</span>
+</span><span id="TypeParser.parse_series-1198"><a href="#TypeParser.parse_series-1198"><span class="linenos">1198</span></a>
+</span><span id="TypeParser.parse_series-1199"><a href="#TypeParser.parse_series-1199"><span class="linenos">1199</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.parse_series-1200"><a href="#TypeParser.parse_series-1200"><span class="linenos">1200</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.parse_series-1201"><a href="#TypeParser.parse_series-1201"><span class="linenos">1201</span></a><span class="sd">			converted values</span>
+</span><span id="TypeParser.parse_series-1202"><a href="#TypeParser.parse_series-1202"><span class="linenos">1202</span></a>
+</span><span id="TypeParser.parse_series-1203"><a href="#TypeParser.parse_series-1203"><span class="linenos">1203</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.parse_series-1204"><a href="#TypeParser.parse_series-1204"><span class="linenos">1204</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.parse_series-1205"><a href="#TypeParser.parse_series-1205"><span class="linenos">1205</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.parse_series-1206"><a href="#TypeParser.parse_series-1206"><span class="linenos">1206</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.parse_series-1207"><a href="#TypeParser.parse_series-1207"><span class="linenos">1207</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2&quot;, &quot;3&quot;])        # [1, 2, 3]</span>
+</span><span id="TypeParser.parse_series-1208"><a href="#TypeParser.parse_series-1208"><span class="linenos">1208</span></a><span class="sd">			parser.parse_series([&quot;5&quot;, &quot;6.7&quot;, &quot;8.&quot;])     # [5., 6.7, 8.]</span>
+</span><span id="TypeParser.parse_series-1209"><a href="#TypeParser.parse_series-1209"><span class="linenos">1209</span></a><span class="sd">			parser.parse_series([&quot;true&quot;, &quot;false&quot;, &quot;&quot;])  # [True, False, None]</span>
+</span><span id="TypeParser.parse_series-1210"><a href="#TypeParser.parse_series-1210"><span class="linenos">1210</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])    # [&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;]</span>
+</span><span id="TypeParser.parse_series-1211"><a href="#TypeParser.parse_series-1211"><span class="linenos">1211</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.parse_series-1212"><a href="#TypeParser.parse_series-1212"><span class="linenos">1212</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_series-1213"><a href="#TypeParser.parse_series-1213"><span class="linenos">1213</span></a>		<span class="n">inferred</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_series</span><span class="p">(</span><span class="n">values</span><span class="p">)</span>
+</span><span id="TypeParser.parse_series-1214"><a href="#TypeParser.parse_series-1214"><span class="linenos">1214</span></a>		<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">]</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Parse a series of strings and convert them to their underlying common type</p>
 
 <p>If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See <code><a href="#reduce_types">parsetypes.reduce_types()</a></code> for more information.</p>
@@ -3094,67 +3036,66 @@
 <span class="n">parser</span><span class="o">.</span><span class="n">parse_series</span><span class="p">([</span><span class="s2">&quot;5&quot;</span><span class="p">,</span> <span class="s2">&quot;6.7&quot;</span><span class="p">,</span> <span class="s2">&quot;8.&quot;</span><span class="p">])</span>     <span class="c1"># [5., 6.7, 8.]</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">parse_series</span><span class="p">([</span><span class="s2">&quot;true&quot;</span><span class="p">,</span> <span class="s2">&quot;false&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">])</span>  <span class="c1"># [True, False, None]</span>
 <span class="n">parser</span><span class="o">.</span><span class="n">parse_series</span><span class="p">([</span><span class="s2">&quot;1&quot;</span><span class="p">,</span> <span class="s2">&quot;2.3&quot;</span><span class="p">,</span> <span class="s2">&quot;abc&quot;</span><span class="p">])</span>    <span class="c1"># [&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;]</span>
 </code></pre>
 </div></div>
 
 
-
                             </div>
                             <div id="TypeParser.parse_table" class="classattr">
                                         <input id="TypeParser.parse_table-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">parse_table</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.parse_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.parse_table"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_table-1211"><a href="#TypeParser.parse_table-1211"><span class="linenos">1211</span></a>	<span class="k">def</span> <span class="nf">parse_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
-</span><span id="TypeParser.parse_table-1212"><a href="#TypeParser.parse_table-1212"><span class="linenos">1212</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_table-1213"><a href="#TypeParser.parse_table-1213"><span class="linenos">1213</span></a><span class="sd">			Parse a table of strings and convert them to the underlying common type of each column</span>
-</span><span id="TypeParser.parse_table-1214"><a href="#TypeParser.parse_table-1214"><span class="linenos">1214</span></a>
-</span><span id="TypeParser.parse_table-1215"><a href="#TypeParser.parse_table-1215"><span class="linenos">1215</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser.parse_table-1216"><a href="#TypeParser.parse_table-1216"><span class="linenos">1216</span></a>
-</span><span id="TypeParser.parse_table-1217"><a href="#TypeParser.parse_table-1217"><span class="linenos">1217</span></a><span class="sd">			Note that the type to which the values should be converted is determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.</span>
-</span><span id="TypeParser.parse_table-1218"><a href="#TypeParser.parse_table-1218"><span class="linenos">1218</span></a>
-</span><span id="TypeParser.parse_table-1219"><a href="#TypeParser.parse_table-1219"><span class="linenos">1219</span></a><span class="sd">			This is a function that computes the entire table and returns it all at once. The generator function `iterate_table()` behaves analogously, except that it computes and yields each row one at a time instead.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_table-1217"><a href="#TypeParser.parse_table-1217"><span class="linenos">1217</span></a>	<span class="k">def</span> <span class="nf">parse_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
+</span><span id="TypeParser.parse_table-1218"><a href="#TypeParser.parse_table-1218"><span class="linenos">1218</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_table-1219"><a href="#TypeParser.parse_table-1219"><span class="linenos">1219</span></a><span class="sd">			Parse a table of strings and convert them to the underlying common type of each column</span>
 </span><span id="TypeParser.parse_table-1220"><a href="#TypeParser.parse_table-1220"><span class="linenos">1220</span></a>
-</span><span id="TypeParser.parse_table-1221"><a href="#TypeParser.parse_table-1221"><span class="linenos">1221</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser.parse_table-1222"><a href="#TypeParser.parse_table-1222"><span class="linenos">1222</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser.parse_table-1223"><a href="#TypeParser.parse_table-1223"><span class="linenos">1223</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser.parse_table-1224"><a href="#TypeParser.parse_table-1224"><span class="linenos">1224</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
-</span><span id="TypeParser.parse_table-1225"><a href="#TypeParser.parse_table-1225"><span class="linenos">1225</span></a>
-</span><span id="TypeParser.parse_table-1226"><a href="#TypeParser.parse_table-1226"><span class="linenos">1226</span></a><span class="sd">			`iterator`</span>
-</span><span id="TypeParser.parse_table-1227"><a href="#TypeParser.parse_table-1227"><span class="linenos">1227</span></a><span class="sd">			: whether the parsed values should be yielded as an iterator. If False, which is the default, the entire table is computed and returned as a list of lists. If True, this function behaves as a generator, and the rows of the table are computed and yielded one at a time. However, note that even when set to True, the type inference requires that inferred type of each individual value must all be able to fit into memory at once.</span>
-</span><span id="TypeParser.parse_table-1228"><a href="#TypeParser.parse_table-1228"><span class="linenos">1228</span></a>
-</span><span id="TypeParser.parse_table-1229"><a href="#TypeParser.parse_table-1229"><span class="linenos">1229</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.parse_table-1230"><a href="#TypeParser.parse_table-1230"><span class="linenos">1230</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.parse_table-1231"><a href="#TypeParser.parse_table-1231"><span class="linenos">1231</span></a><span class="sd">			converted table of values, in row-major order</span>
-</span><span id="TypeParser.parse_table-1232"><a href="#TypeParser.parse_table-1232"><span class="linenos">1232</span></a>
-</span><span id="TypeParser.parse_table-1233"><a href="#TypeParser.parse_table-1233"><span class="linenos">1233</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.parse_table-1234"><a href="#TypeParser.parse_table-1234"><span class="linenos">1234</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.parse_table-1235"><a href="#TypeParser.parse_table-1235"><span class="linenos">1235</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.parse_table-1236"><a href="#TypeParser.parse_table-1236"><span class="linenos">1236</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.parse_table-1237"><a href="#TypeParser.parse_table-1237"><span class="linenos">1237</span></a><span class="sd">			table = parser.parse_table([</span>
-</span><span id="TypeParser.parse_table-1238"><a href="#TypeParser.parse_table-1238"><span class="linenos">1238</span></a><span class="sd">				[&quot;1&quot;, &quot;5&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser.parse_table-1239"><a href="#TypeParser.parse_table-1239"><span class="linenos">1239</span></a><span class="sd">				[&quot;2&quot;, &quot;6.7&quot;, &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser.parse_table-1240"><a href="#TypeParser.parse_table-1240"><span class="linenos">1240</span></a><span class="sd">				[&quot;3&quot;, &quot;8.0&quot;, &quot;&quot;,      &quot;abc&quot;],</span>
-</span><span id="TypeParser.parse_table-1241"><a href="#TypeParser.parse_table-1241"><span class="linenos">1241</span></a><span class="sd">			]):</span>
-</span><span id="TypeParser.parse_table-1242"><a href="#TypeParser.parse_table-1242"><span class="linenos">1242</span></a><span class="sd">			assert table == [</span>
-</span><span id="TypeParser.parse_table-1243"><a href="#TypeParser.parse_table-1243"><span class="linenos">1243</span></a><span class="sd">				[1, 5.,  True,  &quot;1&quot;],</span>
-</span><span id="TypeParser.parse_table-1244"><a href="#TypeParser.parse_table-1244"><span class="linenos">1244</span></a><span class="sd">				[2, 6.7, False, &quot;2.3&quot;],</span>
-</span><span id="TypeParser.parse_table-1245"><a href="#TypeParser.parse_table-1245"><span class="linenos">1245</span></a><span class="sd">				[3, 8.,  None,  &quot;abc&quot;],</span>
-</span><span id="TypeParser.parse_table-1246"><a href="#TypeParser.parse_table-1246"><span class="linenos">1246</span></a><span class="sd">			]</span>
-</span><span id="TypeParser.parse_table-1247"><a href="#TypeParser.parse_table-1247"><span class="linenos">1247</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.parse_table-1248"><a href="#TypeParser.parse_table-1248"><span class="linenos">1248</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_table-1249"><a href="#TypeParser.parse_table-1249"><span class="linenos">1249</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">converted_row</span> <span class="k">for</span> <span class="n">converted_row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">iterate_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)]</span>
+</span><span id="TypeParser.parse_table-1221"><a href="#TypeParser.parse_table-1221"><span class="linenos">1221</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser.parse_table-1222"><a href="#TypeParser.parse_table-1222"><span class="linenos">1222</span></a>
+</span><span id="TypeParser.parse_table-1223"><a href="#TypeParser.parse_table-1223"><span class="linenos">1223</span></a><span class="sd">			Note that the type to which the values should be converted is determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.</span>
+</span><span id="TypeParser.parse_table-1224"><a href="#TypeParser.parse_table-1224"><span class="linenos">1224</span></a>
+</span><span id="TypeParser.parse_table-1225"><a href="#TypeParser.parse_table-1225"><span class="linenos">1225</span></a><span class="sd">			This is a function that computes the entire table and returns it all at once. The generator function `iterate_table()` behaves analogously, except that it computes and yields each row one at a time instead.</span>
+</span><span id="TypeParser.parse_table-1226"><a href="#TypeParser.parse_table-1226"><span class="linenos">1226</span></a>
+</span><span id="TypeParser.parse_table-1227"><a href="#TypeParser.parse_table-1227"><span class="linenos">1227</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser.parse_table-1228"><a href="#TypeParser.parse_table-1228"><span class="linenos">1228</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser.parse_table-1229"><a href="#TypeParser.parse_table-1229"><span class="linenos">1229</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser.parse_table-1230"><a href="#TypeParser.parse_table-1230"><span class="linenos">1230</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
+</span><span id="TypeParser.parse_table-1231"><a href="#TypeParser.parse_table-1231"><span class="linenos">1231</span></a>
+</span><span id="TypeParser.parse_table-1232"><a href="#TypeParser.parse_table-1232"><span class="linenos">1232</span></a><span class="sd">			`iterator`</span>
+</span><span id="TypeParser.parse_table-1233"><a href="#TypeParser.parse_table-1233"><span class="linenos">1233</span></a><span class="sd">			: whether the parsed values should be yielded as an iterator. If False, which is the default, the entire table is computed and returned as a list of lists. If True, this function behaves as a generator, and the rows of the table are computed and yielded one at a time. However, note that even when set to True, the type inference requires that inferred type of each individual value must all be able to fit into memory at once.</span>
+</span><span id="TypeParser.parse_table-1234"><a href="#TypeParser.parse_table-1234"><span class="linenos">1234</span></a>
+</span><span id="TypeParser.parse_table-1235"><a href="#TypeParser.parse_table-1235"><span class="linenos">1235</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.parse_table-1236"><a href="#TypeParser.parse_table-1236"><span class="linenos">1236</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.parse_table-1237"><a href="#TypeParser.parse_table-1237"><span class="linenos">1237</span></a><span class="sd">			converted table of values, in row-major order</span>
+</span><span id="TypeParser.parse_table-1238"><a href="#TypeParser.parse_table-1238"><span class="linenos">1238</span></a>
+</span><span id="TypeParser.parse_table-1239"><a href="#TypeParser.parse_table-1239"><span class="linenos">1239</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.parse_table-1240"><a href="#TypeParser.parse_table-1240"><span class="linenos">1240</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.parse_table-1241"><a href="#TypeParser.parse_table-1241"><span class="linenos">1241</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.parse_table-1242"><a href="#TypeParser.parse_table-1242"><span class="linenos">1242</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.parse_table-1243"><a href="#TypeParser.parse_table-1243"><span class="linenos">1243</span></a><span class="sd">			table = parser.parse_table([</span>
+</span><span id="TypeParser.parse_table-1244"><a href="#TypeParser.parse_table-1244"><span class="linenos">1244</span></a><span class="sd">				[&quot;1&quot;, &quot;5&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser.parse_table-1245"><a href="#TypeParser.parse_table-1245"><span class="linenos">1245</span></a><span class="sd">				[&quot;2&quot;, &quot;6.7&quot;, &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser.parse_table-1246"><a href="#TypeParser.parse_table-1246"><span class="linenos">1246</span></a><span class="sd">				[&quot;3&quot;, &quot;8.0&quot;, &quot;&quot;,      &quot;abc&quot;],</span>
+</span><span id="TypeParser.parse_table-1247"><a href="#TypeParser.parse_table-1247"><span class="linenos">1247</span></a><span class="sd">			]):</span>
+</span><span id="TypeParser.parse_table-1248"><a href="#TypeParser.parse_table-1248"><span class="linenos">1248</span></a><span class="sd">			assert table == [</span>
+</span><span id="TypeParser.parse_table-1249"><a href="#TypeParser.parse_table-1249"><span class="linenos">1249</span></a><span class="sd">				[1, 5.,  True,  &quot;1&quot;],</span>
+</span><span id="TypeParser.parse_table-1250"><a href="#TypeParser.parse_table-1250"><span class="linenos">1250</span></a><span class="sd">				[2, 6.7, False, &quot;2.3&quot;],</span>
+</span><span id="TypeParser.parse_table-1251"><a href="#TypeParser.parse_table-1251"><span class="linenos">1251</span></a><span class="sd">				[3, 8.,  None,  &quot;abc&quot;],</span>
+</span><span id="TypeParser.parse_table-1252"><a href="#TypeParser.parse_table-1252"><span class="linenos">1252</span></a><span class="sd">			]</span>
+</span><span id="TypeParser.parse_table-1253"><a href="#TypeParser.parse_table-1253"><span class="linenos">1253</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.parse_table-1254"><a href="#TypeParser.parse_table-1254"><span class="linenos">1254</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_table-1255"><a href="#TypeParser.parse_table-1255"><span class="linenos">1255</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">converted_row</span> <span class="k">for</span> <span class="n">converted_row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">iterate_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)]</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Parse a table of strings and convert them to the underlying common type of each column</p>
 
 <p>For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See <code><a href="#reduce_types">parsetypes.reduce_types()</a></code> for more information.</p>
@@ -3189,65 +3130,64 @@
 	<span class="p">[</span><span class="mi">2</span><span class="p">,</span> <span class="mf">6.7</span><span class="p">,</span> <span class="kc">False</span><span class="p">,</span> <span class="s2">&quot;2.3&quot;</span><span class="p">],</span>
 	<span class="p">[</span><span class="mi">3</span><span class="p">,</span> <span class="mf">8.</span><span class="p">,</span>  <span class="kc">None</span><span class="p">,</span>  <span class="s2">&quot;abc&quot;</span><span class="p">],</span>
 <span class="p">]</span>
 </code></pre>
 </div></div>
 
 
-
                             </div>
                             <div id="TypeParser.iterate_table" class="classattr">
                                         <input id="TypeParser.iterate_table-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">iterate_table</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="n">Iterator</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.iterate_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.iterate_table"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.iterate_table-1252"><a href="#TypeParser.iterate_table-1252"><span class="linenos">1252</span></a>	<span class="k">def</span> <span class="nf">iterate_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="n">Iterator</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
-</span><span id="TypeParser.iterate_table-1253"><a href="#TypeParser.iterate_table-1253"><span class="linenos">1253</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.iterate_table-1254"><a href="#TypeParser.iterate_table-1254"><span class="linenos">1254</span></a><span class="sd">			Parse a table of strings for the underlying common type of each column, then convert and yield each row</span>
-</span><span id="TypeParser.iterate_table-1255"><a href="#TypeParser.iterate_table-1255"><span class="linenos">1255</span></a>
-</span><span id="TypeParser.iterate_table-1256"><a href="#TypeParser.iterate_table-1256"><span class="linenos">1256</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser.iterate_table-1257"><a href="#TypeParser.iterate_table-1257"><span class="linenos">1257</span></a>
-</span><span id="TypeParser.iterate_table-1258"><a href="#TypeParser.iterate_table-1258"><span class="linenos">1258</span></a><span class="sd">			This is a generator function that computes and yields each row one at a time. However, note that in order to determine the types to which each column should be converted, the individual inferred types of every value in the table must still be able to fit into memory.</span>
-</span><span id="TypeParser.iterate_table-1259"><a href="#TypeParser.iterate_table-1259"><span class="linenos">1259</span></a>
-</span><span id="TypeParser.iterate_table-1260"><a href="#TypeParser.iterate_table-1260"><span class="linenos">1260</span></a><span class="sd">			The function `parse_table()` behaves analogously, except that it computes the entire table and returns it as a list of lists instead.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.iterate_table-1258"><a href="#TypeParser.iterate_table-1258"><span class="linenos">1258</span></a>	<span class="k">def</span> <span class="nf">iterate_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="n">Iterator</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
+</span><span id="TypeParser.iterate_table-1259"><a href="#TypeParser.iterate_table-1259"><span class="linenos">1259</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.iterate_table-1260"><a href="#TypeParser.iterate_table-1260"><span class="linenos">1260</span></a><span class="sd">			Parse a table of strings for the underlying common type of each column, then convert and yield each row</span>
 </span><span id="TypeParser.iterate_table-1261"><a href="#TypeParser.iterate_table-1261"><span class="linenos">1261</span></a>
-</span><span id="TypeParser.iterate_table-1262"><a href="#TypeParser.iterate_table-1262"><span class="linenos">1262</span></a><span class="sd">			Arguments</span>
-</span><span id="TypeParser.iterate_table-1263"><a href="#TypeParser.iterate_table-1263"><span class="linenos">1263</span></a><span class="sd">			---------</span>
-</span><span id="TypeParser.iterate_table-1264"><a href="#TypeParser.iterate_table-1264"><span class="linenos">1264</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser.iterate_table-1265"><a href="#TypeParser.iterate_table-1265"><span class="linenos">1265</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
-</span><span id="TypeParser.iterate_table-1266"><a href="#TypeParser.iterate_table-1266"><span class="linenos">1266</span></a>
-</span><span id="TypeParser.iterate_table-1267"><a href="#TypeParser.iterate_table-1267"><span class="linenos">1267</span></a><span class="sd">			Yields</span>
-</span><span id="TypeParser.iterate_table-1268"><a href="#TypeParser.iterate_table-1268"><span class="linenos">1268</span></a><span class="sd">			------</span>
-</span><span id="TypeParser.iterate_table-1269"><a href="#TypeParser.iterate_table-1269"><span class="linenos">1269</span></a><span class="sd">			each row of converted table values</span>
-</span><span id="TypeParser.iterate_table-1270"><a href="#TypeParser.iterate_table-1270"><span class="linenos">1270</span></a>
-</span><span id="TypeParser.iterate_table-1271"><a href="#TypeParser.iterate_table-1271"><span class="linenos">1271</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.iterate_table-1272"><a href="#TypeParser.iterate_table-1272"><span class="linenos">1272</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.iterate_table-1273"><a href="#TypeParser.iterate_table-1273"><span class="linenos">1273</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.iterate_table-1274"><a href="#TypeParser.iterate_table-1274"><span class="linenos">1274</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.iterate_table-1275"><a href="#TypeParser.iterate_table-1275"><span class="linenos">1275</span></a><span class="sd">			table = parser.iterate_table([</span>
-</span><span id="TypeParser.iterate_table-1276"><a href="#TypeParser.iterate_table-1276"><span class="linenos">1276</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser.iterate_table-1277"><a href="#TypeParser.iterate_table-1277"><span class="linenos">1277</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser.iterate_table-1278"><a href="#TypeParser.iterate_table-1278"><span class="linenos">1278</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
-</span><span id="TypeParser.iterate_table-1279"><a href="#TypeParser.iterate_table-1279"><span class="linenos">1279</span></a><span class="sd">			]):</span>
-</span><span id="TypeParser.iterate_table-1280"><a href="#TypeParser.iterate_table-1280"><span class="linenos">1280</span></a><span class="sd">			assert next(table) == [1.,  1, &quot;1&quot;]</span>
-</span><span id="TypeParser.iterate_table-1281"><a href="#TypeParser.iterate_table-1281"><span class="linenos">1281</span></a><span class="sd">			assert next(table) == [2.,  0, &quot;2.3&quot;]</span>
-</span><span id="TypeParser.iterate_table-1282"><a href="#TypeParser.iterate_table-1282"><span class="linenos">1282</span></a><span class="sd">			assert next(table) == [3.4, 2, &quot;abc&quot;]</span>
-</span><span id="TypeParser.iterate_table-1283"><a href="#TypeParser.iterate_table-1283"><span class="linenos">1283</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.iterate_table-1284"><a href="#TypeParser.iterate_table-1284"><span class="linenos">1284</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.iterate_table-1285"><a href="#TypeParser.iterate_table-1285"><span class="linenos">1285</span></a>		<span class="n">inferred_types</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
-</span><span id="TypeParser.iterate_table-1286"><a href="#TypeParser.iterate_table-1286"><span class="linenos">1286</span></a>
-</span><span id="TypeParser.iterate_table-1287"><a href="#TypeParser.iterate_table-1287"><span class="linenos">1287</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows</span><span class="p">:</span>
-</span><span id="TypeParser.iterate_table-1288"><a href="#TypeParser.iterate_table-1288"><span class="linenos">1288</span></a>			<span class="k">yield</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span><span class="p">,</span> <span class="n">inferred</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">row</span><span class="p">,</span> <span class="n">inferred_types</span><span class="p">)]</span>
+</span><span id="TypeParser.iterate_table-1262"><a href="#TypeParser.iterate_table-1262"><span class="linenos">1262</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser.iterate_table-1263"><a href="#TypeParser.iterate_table-1263"><span class="linenos">1263</span></a>
+</span><span id="TypeParser.iterate_table-1264"><a href="#TypeParser.iterate_table-1264"><span class="linenos">1264</span></a><span class="sd">			This is a generator function that computes and yields each row one at a time. However, note that in order to determine the types to which each column should be converted, the individual inferred types of every value in the table must still be able to fit into memory.</span>
+</span><span id="TypeParser.iterate_table-1265"><a href="#TypeParser.iterate_table-1265"><span class="linenos">1265</span></a>
+</span><span id="TypeParser.iterate_table-1266"><a href="#TypeParser.iterate_table-1266"><span class="linenos">1266</span></a><span class="sd">			The function `parse_table()` behaves analogously, except that it computes the entire table and returns it as a list of lists instead.</span>
+</span><span id="TypeParser.iterate_table-1267"><a href="#TypeParser.iterate_table-1267"><span class="linenos">1267</span></a>
+</span><span id="TypeParser.iterate_table-1268"><a href="#TypeParser.iterate_table-1268"><span class="linenos">1268</span></a><span class="sd">			Arguments</span>
+</span><span id="TypeParser.iterate_table-1269"><a href="#TypeParser.iterate_table-1269"><span class="linenos">1269</span></a><span class="sd">			---------</span>
+</span><span id="TypeParser.iterate_table-1270"><a href="#TypeParser.iterate_table-1270"><span class="linenos">1270</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser.iterate_table-1271"><a href="#TypeParser.iterate_table-1271"><span class="linenos">1271</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
+</span><span id="TypeParser.iterate_table-1272"><a href="#TypeParser.iterate_table-1272"><span class="linenos">1272</span></a>
+</span><span id="TypeParser.iterate_table-1273"><a href="#TypeParser.iterate_table-1273"><span class="linenos">1273</span></a><span class="sd">			Yields</span>
+</span><span id="TypeParser.iterate_table-1274"><a href="#TypeParser.iterate_table-1274"><span class="linenos">1274</span></a><span class="sd">			------</span>
+</span><span id="TypeParser.iterate_table-1275"><a href="#TypeParser.iterate_table-1275"><span class="linenos">1275</span></a><span class="sd">			each row of converted table values</span>
+</span><span id="TypeParser.iterate_table-1276"><a href="#TypeParser.iterate_table-1276"><span class="linenos">1276</span></a>
+</span><span id="TypeParser.iterate_table-1277"><a href="#TypeParser.iterate_table-1277"><span class="linenos">1277</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.iterate_table-1278"><a href="#TypeParser.iterate_table-1278"><span class="linenos">1278</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.iterate_table-1279"><a href="#TypeParser.iterate_table-1279"><span class="linenos">1279</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.iterate_table-1280"><a href="#TypeParser.iterate_table-1280"><span class="linenos">1280</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.iterate_table-1281"><a href="#TypeParser.iterate_table-1281"><span class="linenos">1281</span></a><span class="sd">			table = parser.iterate_table([</span>
+</span><span id="TypeParser.iterate_table-1282"><a href="#TypeParser.iterate_table-1282"><span class="linenos">1282</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser.iterate_table-1283"><a href="#TypeParser.iterate_table-1283"><span class="linenos">1283</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser.iterate_table-1284"><a href="#TypeParser.iterate_table-1284"><span class="linenos">1284</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
+</span><span id="TypeParser.iterate_table-1285"><a href="#TypeParser.iterate_table-1285"><span class="linenos">1285</span></a><span class="sd">			]):</span>
+</span><span id="TypeParser.iterate_table-1286"><a href="#TypeParser.iterate_table-1286"><span class="linenos">1286</span></a><span class="sd">			assert next(table) == [1.,  1, &quot;1&quot;]</span>
+</span><span id="TypeParser.iterate_table-1287"><a href="#TypeParser.iterate_table-1287"><span class="linenos">1287</span></a><span class="sd">			assert next(table) == [2.,  0, &quot;2.3&quot;]</span>
+</span><span id="TypeParser.iterate_table-1288"><a href="#TypeParser.iterate_table-1288"><span class="linenos">1288</span></a><span class="sd">			assert next(table) == [3.4, 2, &quot;abc&quot;]</span>
+</span><span id="TypeParser.iterate_table-1289"><a href="#TypeParser.iterate_table-1289"><span class="linenos">1289</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.iterate_table-1290"><a href="#TypeParser.iterate_table-1290"><span class="linenos">1290</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.iterate_table-1291"><a href="#TypeParser.iterate_table-1291"><span class="linenos">1291</span></a>		<span class="n">inferred_types</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
+</span><span id="TypeParser.iterate_table-1292"><a href="#TypeParser.iterate_table-1292"><span class="linenos">1292</span></a>
+</span><span id="TypeParser.iterate_table-1293"><a href="#TypeParser.iterate_table-1293"><span class="linenos">1293</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows</span><span class="p">:</span>
+</span><span id="TypeParser.iterate_table-1294"><a href="#TypeParser.iterate_table-1294"><span class="linenos">1294</span></a>			<span class="k">yield</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span><span class="p">,</span> <span class="n">inferred</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">row</span><span class="p">,</span> <span class="n">inferred_types</span><span class="p">)]</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Parse a table of strings for the underlying common type of each column, then convert and yield each row</p>
 
 <p>For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See <code><a href="#reduce_types">parsetypes.reduce_types()</a></code> for more information.</p>
@@ -3277,44 +3217,14 @@
 <span class="k">assert</span> <span class="nb">next</span><span class="p">(</span><span class="n">table</span><span class="p">)</span> <span class="o">==</span> <span class="p">[</span><span class="mf">1.</span><span class="p">,</span>  <span class="mi">1</span><span class="p">,</span> <span class="s2">&quot;1&quot;</span><span class="p">]</span>
 <span class="k">assert</span> <span class="nb">next</span><span class="p">(</span><span class="n">table</span><span class="p">)</span> <span class="o">==</span> <span class="p">[</span><span class="mf">2.</span><span class="p">,</span>  <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;2.3&quot;</span><span class="p">]</span>
 <span class="k">assert</span> <span class="nb">next</span><span class="p">(</span><span class="n">table</span><span class="p">)</span> <span class="o">==</span> <span class="p">[</span><span class="mf">3.4</span><span class="p">,</span> <span class="mi">2</span><span class="p">,</span> <span class="s2">&quot;abc&quot;</span><span class="p">]</span>
 </code></pre>
 </div></div>
 
 
-
-                            </div>
-                            <div class="inherited">
-                                <h5>Inherited Members</h5>
-                                <dl>
-                                    <div><dt>builtins.object</dt>
-                                <dd id="TypeParser.__new__" class="function">__new__</dd>
-                <dd id="TypeParser.__repr__" class="function">__repr__</dd>
-                <dd id="TypeParser.__hash__" class="function">__hash__</dd>
-                <dd id="TypeParser.__str__" class="function">__str__</dd>
-                <dd id="TypeParser.__getattribute__" class="function">__getattribute__</dd>
-                <dd id="TypeParser.__setattr__" class="function">__setattr__</dd>
-                <dd id="TypeParser.__delattr__" class="function">__delattr__</dd>
-                <dd id="TypeParser.__lt__" class="function">__lt__</dd>
-                <dd id="TypeParser.__le__" class="function">__le__</dd>
-                <dd id="TypeParser.__eq__" class="function">__eq__</dd>
-                <dd id="TypeParser.__ne__" class="function">__ne__</dd>
-                <dd id="TypeParser.__gt__" class="function">__gt__</dd>
-                <dd id="TypeParser.__ge__" class="function">__ge__</dd>
-                <dd id="TypeParser.__reduce_ex__" class="function">__reduce_ex__</dd>
-                <dd id="TypeParser.__reduce__" class="function">__reduce__</dd>
-                <dd id="TypeParser.__getstate__" class="function">__getstate__</dd>
-                <dd id="TypeParser.__subclasshook__" class="function">__subclasshook__</dd>
-                <dd id="TypeParser.__init_subclass__" class="function">__init_subclass__</dd>
-                <dd id="TypeParser.__format__" class="function">__format__</dd>
-                <dd id="TypeParser.__sizeof__" class="function">__sizeof__</dd>
-                <dd id="TypeParser.__dir__" class="function">__dir__</dd>
-
-            </div>
-                                </dl>
                             </div>
                 </section>
                 <section id="reduce_types">
                             <input id="reduce_types-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
@@ -3389,15 +3299,14 @@
 <pre><span></span><code><span class="n">reduce_types</span><span class="p">([</span><span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">])</span>        <span class="c1"># float</span>
 <span class="n">reduce_types</span><span class="p">([</span><span class="nb">bool</span><span class="p">,</span> <span class="nb">int</span><span class="p">])</span>         <span class="c1"># int</span>
 <span class="n">reduce_types</span><span class="p">([</span><span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="nb">str</span><span class="p">])</span>   <span class="c1"># str</span>
 </code></pre>
 </div></div>
 
 
-
                 </section>
                 <section id="Nullable">
                             <input id="Nullable-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
             
     <span class="def">class</span>
     <span class="name">Nullable</span><wbr>(<span class="base">typing.Generic[~S]</span>):
@@ -3423,58 +3332,11 @@
 <p>Dummy container type that represents a scalar (<code>S</code>) that could also be None</p>
 
 <p>The type annotation <code>Nullable[S]</code> is treated as equivalent to <code>Union[S, types.NoneType]</code>, which will accept either a value of type <code>S</code> or the value <code>None</code>.</p>
 
 <p>This class should not be instantiated.</p></div>
 
 
-
-                            <div id="Nullable.__init__" class="classattr">
-                                <div class="attr function">
-            
-        <span class="name">Nullable</span><span class="signature pdoc-code condensed">()</span>
-
-
-        
-    </div>
-    <a class="headerlink" href="#Nullable.__init__"></a>
-    
-    
-
-                            </div>
-                            <div class="inherited">
-                                <h5>Inherited Members</h5>
-                                <dl>
-                                    <div><dt>typing.Generic</dt>
-                                <dd id="Nullable.__class_getitem__" class="function">__class_getitem__</dd>
-                <dd id="Nullable.__init_subclass__" class="function">__init_subclass__</dd>
-
-            </div>
-            <div><dt>builtins.object</dt>
-                                <dd id="Nullable.__new__" class="function">__new__</dd>
-                <dd id="Nullable.__repr__" class="function">__repr__</dd>
-                <dd id="Nullable.__hash__" class="function">__hash__</dd>
-                <dd id="Nullable.__str__" class="function">__str__</dd>
-                <dd id="Nullable.__getattribute__" class="function">__getattribute__</dd>
-                <dd id="Nullable.__setattr__" class="function">__setattr__</dd>
-                <dd id="Nullable.__delattr__" class="function">__delattr__</dd>
-                <dd id="Nullable.__lt__" class="function">__lt__</dd>
-                <dd id="Nullable.__le__" class="function">__le__</dd>
-                <dd id="Nullable.__eq__" class="function">__eq__</dd>
-                <dd id="Nullable.__ne__" class="function">__ne__</dd>
-                <dd id="Nullable.__gt__" class="function">__gt__</dd>
-                <dd id="Nullable.__ge__" class="function">__ge__</dd>
-                <dd id="Nullable.__reduce_ex__" class="function">__reduce_ex__</dd>
-                <dd id="Nullable.__reduce__" class="function">__reduce__</dd>
-                <dd id="Nullable.__getstate__" class="function">__getstate__</dd>
-                <dd id="Nullable.__subclasshook__" class="function">__subclasshook__</dd>
-                <dd id="Nullable.__format__" class="function">__format__</dd>
-                <dd id="Nullable.__sizeof__" class="function">__sizeof__</dd>
-                <dd id="Nullable.__dir__" class="function">__dir__</dd>
-
-            </div>
-                                </dl>
-                            </div>
                 </section>
     </main>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -20,15 +20,14 @@
           o convert()
           o parse()
           o parse_series()
           o parse_table()
           o iterate_table()
     * reduce_types()
     * Nullable
-          o Nullable
 built_with_pdoc[pdoc_logo]
    Edit_on_GitHub
 ****** parsetypes ******
 This package provides tools for parsing serialised data to recover their
 original underlying types.
 The TypeParser class provides configurable type inference and parsing. This can
 be initialised with different settings to, for example:
@@ -49,15 +48,15 @@
 _6
 - give exact Decimal values instead of floats
 _7
 - detect inline lists
 _8"""
 _9
 10
-11__version__ = "0.3"
+11__version__ = "0.3.1"
 12
 13from ._common import AnyScalar, AnyScalarType, AnyValue, AnyValueType,
 GenericValue, Nullable
 14from ._parser import TypeParser
 15from ._reduce_types import reduce_types
 16
 17__all__ = ('TypeParser', 'reduce_types', 'Nullable')
@@ -981,15 +980,17 @@
 Keyword arguments
 _543
 -----------------
 _544
 _545
 `allow_negative`
 _546
-: whether to accept negative values
+: whether to accept negative values. Since negative values are always indicated
+with a negative sign, `allow_sign` must also be True (which is the default
+setting) for this to have any effect.
 _547
 _548
 `allow_sign`
 _549
 : whether to accept values prepended with a sign character. If False, it
 implies that `allow_negative` is False also.
 _550
@@ -1409,15 +1410,16 @@
 return False
 _761
 _762
 raise ValueError(f"not a boolean: {value}")
 _763
 _764
 _765
-def parse_int(self, value: str, *, allow_scientific: bool=True) -> int:
+def parse_int(self, value: str, *, allow_negative: bool=True, allow_sign:
+bool=True, allow_scientific: bool=True) -> int:
 _766
 """
 _767
 Parse a string and return it as an int if possible
 _768
 _769
 If the string represents a bool, it will be converted to `1` for True and `0`
@@ -1434,1006 +1436,1019 @@
 _775
 _776
 Keyword arguments
 _777
 -----------------
 _778
 _779
-`allow_scientific`
+`allow_negative`
 _780
-: whether to accept scientific notation. If True, strings of the form
-<code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
-<code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
-mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var>
-must be an integer and <var>X</var> must be a non-negative integer, even in
-cases where the expression would evaluate mathematically to an integer.
+: whether to accept negative values. Since negative values are always indicated
+with a negative sign, `allow_sign` must also be True (which is the default
+setting) for this to have any effect.
 _781
 _782
-Returns
+`allow_sign`
 _783
--------
+: whether to accept values prepended with a sign character. If False, it
+implies that `allow_negative` is False also.
 _784
-parsed int value
 _785
+`allow_scientific`
 _786
-Raises
+: whether to accept scientific notation. If True, strings of the form
+<code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
+<code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
+mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var>
+must be an integer and <var>X</var> must be a non-negative integer, even in
+cases where the expression would evaluate mathematically to an integer.
 _787
-------
 _788
-`ValueError` if `value` cannot be parsed
+Returns
 _789
+-------
 _790
-Examples
+parsed int value
 _791
---------
 _792
-```python
+Raises
 _793
-parser = TypeParser()
+------
 _794
-parser.parse_int("0")    # 0
+`ValueError` if `value` cannot be parsed
 _795
-parser.parse_int("-1")   # -1
 _796
-parser.parse_int("2e3")  # 2000
+Examples
 _797
-```
+--------
 _798
-"""
+```python
 _799
-if self._trim:
+parser = TypeParser()
 _800
-value = value.strip()
+parser.parse_int("0")    # 0
 _801
+parser.parse_int("-1")   # -1
 _802
-if self.is_int(value, allow_sign=True, allow_negative=True,
-allow_scientific=allow_scientific):
+parser.parse_int("2e3")  # 2000
 _803
-if allow_scientific:
+```
 _804
-value, exp = _decompose_string_pair(value, self._scientific_char,
-self._int_case_sensitive)
+"""
 _805
-if exp is not None:
+if self._trim:
 _806
-if value[0] in (self._negative_chars - {self._negative_char}):
+value = value.strip()
 _807
-value = self._negative_char + value[1:]
 _808
-return int(value) * (10 ** int(exp))
+if self.is_int(value, allow_negative=allow_negative, allow_sign=allow_sign,
+allow_scientific=allow_scientific):
 _809
+if allow_scientific:
 _810
-if value[0] in (self._negative_chars - {self._negative_char}):
+value, exp = _decompose_string_pair(value, self._scientific_char,
+self._int_case_sensitive)
 _811
-value = self._negative_char + value[1:]
+if exp is not None:
 _812
-return int(value)
+if value[0] in (self._negative_chars - {self._negative_char}):
 _813
+value = self._negative_char + value[1:]
 _814
-elif self.is_bool(value):
+return int(value) * (10 ** int(exp))
 _815
-return int(self.parse_bool(value))
 _816
-else:
+if value[0] in (self._negative_chars - {self._negative_char}):
 _817
-raise ValueError(f"not an integer: {value}")
+value = self._negative_char + value[1:]
 _818
+return int(value)
 _819
 _820
-def _parse_floatlike(self,
+elif self.is_bool(value):
 _821
-value: str,
+return int(self.parse_bool(value))
 _822
-converter: Callable[[Union[str, bool]], _FloatLike],
+else:
 _823
-inf_value: _FloatLike,
+raise ValueError(f"not an integer: {value}")
 _824
-nan_value: _FloatLike,
 _825
-*,
 _826
-allow_scientific: bool=True,
+def _parse_floatlike(self,
 _827
-allow_inf: bool=True,
+value: str,
 _828
-allow_nan: bool=True
+converter: Callable[[Union[str, bool]], _FloatLike],
 _829
-) -> _FloatLike:
+inf_value: _FloatLike,
 _830
-if self._trim:
+nan_value: _FloatLike,
 _831
-value = value.strip()
+*,
 _832
-if self.is_float(value, allow_scientific=allow_scientific, allow_inf=allow_inf,
-allow_nan=allow_nan):
+allow_scientific: bool=True,
 _833
-if self._float_case_sensitive:
+allow_inf: bool=True,
 _834
-special_value = value
+allow_nan: bool=True
 _835
-else:
+) -> _FloatLike:
 _836
-special_value = value.lower()
+if self._trim:
 _837
-if allow_inf and special_value in self._match_inf_values:
+value = value.strip()
 _838
-return inf_value
+if self.is_float(value, allow_scientific=allow_scientific, allow_inf=allow_inf,
+allow_nan=allow_nan):
 _839
-if allow_nan and special_value in self._match_nan_values:
+if self._float_case_sensitive:
 _840
-return nan_value
+special_value = value
 _841
+else:
 _842
-if len(value) > 0 and value[0] in self._sign_chars:
+special_value = value.lower()
 _843
-positive_part = value[1:]
+if allow_inf and special_value in self._match_inf_values:
 _844
-if self._float_case_sensitive:
+return inf_value
 _845
-special_value = positive_part
+if allow_nan and special_value in self._match_nan_values:
 _846
-else:
+return nan_value
 _847
-special_value = positive_part.lower()
 _848
-if allow_inf and special_value in self._match_inf_values:
+if len(value) > 0 and value[0] in self._sign_chars:
 _849
-if value[0] in self._negative_chars:
+positive_part = value[1:]
 _850
-return -1 * inf_value
+if self._float_case_sensitive:
 _851
-else:
+special_value = positive_part
 _852
-return inf_value
+else:
 _853
-if allow_nan and special_value in self._match_nan_values:
+special_value = positive_part.lower()
 _854
-return nan_value
+if allow_inf and special_value in self._match_inf_values:
 _855
-_856
 if value[0] in self._negative_chars:
+_856
+return -1 * inf_value
 _857
-value = self._negative_char + positive_part
+else:
 _858
-return converter(value)
+return inf_value
 _859
-elif self.is_bool(value):
+if allow_nan and special_value in self._match_nan_values:
 _860
-return converter(self.parse_bool(value))
+return nan_value
 _861
-else:
 _862
-raise ValueError(f"not a {_FloatLike.__name__}: {value}")
+if value[0] in self._negative_chars:
 _863
+value = self._negative_char + positive_part
 _864
+return converter(value)
 _865
-def parse_float(self, value: str, *, allow_scientific: bool=True, allow_inf:
-bool=True, allow_nan: bool=True) -> float:
+elif self.is_bool(value):
 _866
-"""
+return converter(self.parse_bool(value))
 _867
-Parse a string and return it as a (non-exact) float if possible
+else:
 _868
+raise ValueError(f"not a {_FloatLike.__name__}: {value}")
 _869
-If the string represents a bool, it will be converted to `1.` for True and `0.`
-for False. If the string represents an int, it will be converted to a float
-also.
 _870
 _871
-Behaves analogously to `parse_decimal()`, except that that returns an exact
-Decimal instead.
+def parse_float(self, value: str, *, allow_scientific: bool=True, allow_inf:
+bool=True, allow_nan: bool=True) -> float:
 _872
+"""
 _873
-Arguments
+Parse a string and return it as a (non-exact) float if possible
 _874
----------
 _875
-`value`
+If the string represents a bool, it will be converted to `1.` for True and `0.`
+for False. If the string represents an int, it will be converted to a float
+also.
 _876
-: string to be parsed
 _877
+Behaves analogously to `parse_decimal()`, except that that returns an exact
+Decimal instead.
 _878
-Keyword arguments
 _879
------------------
+Arguments
 _880
+---------
 _881
-`allow_scientific`
+`value`
 _882
+: string to be parsed
+_883
+_884
+Keyword arguments
+_885
+-----------------
+_886
+_887
+`allow_scientific`
+_888
 : whether to accept scientific notation. If True, strings of the form
 <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
 <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
 mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var>
 must be an integer, but can be negative.
-_883
-_884
+_889
+_890
 `allow_inf`
-_885
+_891
 : whether to accept positive and negative infinity values. If True, strings
 that match the values in <code><var>parser</var>.inf_values</code> (empty set
 by default) are interpreted as infinity, or as negative infinity if prepended
 by a negative sign. The case sensitivity of this matching depends on
 <code><var>parser</var>.float_case_sensitive</code>, which is False by default.
-_886
-_887
+_892
+_893
 `allow_nan`
-_888
+_894
 : whether to accept NaN (not a number) representations. If True, strings that
 match the values in <code><var>parser</var>.nan_values</code> (empty set by
 default) are interpeted as NaN. The case sensitivity of this matching also
 depends on <code><var>parser</var>.float_case_sensitive</code>, which is False
 by default.
-_889
-_890
-Returns
-_891
--------
-_892
-parsed float value
-_893
-_894
-Raises
 _895
-------
 _896
-`ValueError` if `value` cannot be parsed
+Returns
 _897
+-------
 _898
-Examples
+parsed float value
 _899
---------
 _900
-```python
+Raises
 _901
-parser = TypeParser(inf_values=["inf"], nan_values=["nan"])
+------
 _902
-parser.parse_float("1.")       # 1.
+`ValueError` if `value` cannot be parsed
 _903
-parser.parse_float("1.23e2")   # 123.
 _904
-parser.parse_float("1.23e-2")  # 0.0123
+Examples
 _905
-parser.parse_float("inf")      # math.inf
+--------
 _906
-```
+```python
 _907
-"""
+parser = TypeParser(inf_values=["inf"], nan_values=["nan"])
 _908
-return self._parse_floatlike(value, float, math.inf, math.nan,
+parser.parse_float("1.")       # 1.
 _909
-allow_scientific=allow_scientific,
+parser.parse_float("1.23e2")   # 123.
 _910
-allow_inf=allow_inf,
+parser.parse_float("1.23e-2")  # 0.0123
 _911
-allow_nan=allow_nan,
+parser.parse_float("inf")      # math.inf
 _912
-)
+```
 _913
+"""
 _914
+return self._parse_floatlike(value, float, math.inf, math.nan,
 _915
-def parse_decimal(self, value: str, *, allow_scientific: bool=True, allow_inf:
-bool=True, allow_nan: bool=True) -> Decimal:
+allow_scientific=allow_scientific,
 _916
-"""
+allow_inf=allow_inf,
 _917
-Parse a string and return it as an exact Decimal if possible
+allow_nan=allow_nan,
 _918
+)
 _919
-If the string represents a bool, it will be converted to `Decimal(1)` for True
-and `Decimal(0)` for False. If the string represents an int, it will be
-converted to a Decimal also.
 _920
 _921
-Behaves analogously to `parse_float()`, except that that returns a non-exact
-float instead.
+def parse_decimal(self, value: str, *, allow_scientific: bool=True, allow_inf:
+bool=True, allow_nan: bool=True) -> Decimal:
 _922
+"""
 _923
-Arguments
+Parse a string and return it as an exact Decimal if possible
 _924
----------
 _925
-`value`
+If the string represents a bool, it will be converted to `Decimal(1)` for True
+and `Decimal(0)` for False. If the string represents an int, it will be
+converted to a Decimal also.
 _926
-: string to be parsed
 _927
+Behaves analogously to `parse_float()`, except that that returns a non-exact
+float instead.
 _928
-Keyword arguments
 _929
------------------
+Arguments
 _930
+---------
 _931
-`allow_scientific`
+`value`
 _932
+: string to be parsed
+_933
+_934
+Keyword arguments
+_935
+-----------------
+_936
+_937
+`allow_scientific`
+_938
 : whether to accept scientific notation. If True, strings of the form
 <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
 <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
 mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var>
 must be an integer, but can be negative.
-_933
-_934
+_939
+_940
 `allow_inf`
-_935
+_941
 : whether to accept positive and negative infinity values. If True, strings
 that match the values in <code><var>parser</var>.inf_values</code> (empty set
 by default) are interpreted as infinity, or as negative infinity if prepended
 by a negative sign. The case sensitivity of this matching depends on
 <code><var>parser</var>.float_case_sensitive</code>, which is False by default.
-_936
-_937
+_942
+_943
 `allow_nan`
-_938
+_944
 : whether to accept NaN (not a number) representations. If True, strings that
 match the values in <code><var>parser</var>.nan_values</code> (empty set by
 default) are interpeted as NaN. The case sensitivity of this matching also
 depends on <code><var>parser</var>.float_case_sensitive</code>, which is False
 by default.
-_939
-_940
-Returns
-_941
--------
-_942
-parsed Decimal value
-_943
-_944
-Raises
 _945
-------
 _946
-`ValueError` if `value` cannot be parsed
+Returns
 _947
+-------
 _948
-Examples
+parsed Decimal value
 _949
---------
 _950
-```python
+Raises
 _951
-parser = TypeParser(inf_values=["inf"], nan_values=["nan"])
+------
 _952
-parser.parse_decimal("1.")       # Decimal(1)
+`ValueError` if `value` cannot be parsed
 _953
-parser.parse_decimal("1.23e2")   # Decimal(123)
 _954
-parser.parse_decimal("1.23e-2")  # Decimal(123) / Decimal(10000)
+Examples
 _955
-parser.parse_decimal("inf")      # Decimal(math.inf)
+--------
 _956
-```
+```python
 _957
-"""
+parser = TypeParser(inf_values=["inf"], nan_values=["nan"])
 _958
-return self._parse_floatlike(value, Decimal, Decimal(math.inf), Decimal
-(math.nan),
+parser.parse_decimal("1.")       # Decimal(1)
 _959
-allow_scientific=allow_scientific,
+parser.parse_decimal("1.23e2")   # Decimal(123)
 _960
-allow_inf=allow_inf,
+parser.parse_decimal("1.23e-2")  # Decimal(123) / Decimal(10000)
 _961
-allow_nan=allow_nan,
+parser.parse_decimal("inf")      # Decimal(math.inf)
 _962
-)
+```
 _963
+"""
 _964
+return self._parse_floatlike(value, Decimal, Decimal(math.inf), Decimal
+(math.nan),
 _965
-def infer(self, value: str) -> AnyValueType:
+allow_scientific=allow_scientific,
 _966
-"""
+allow_inf=allow_inf,
 _967
-Infer the underlying type of a string
+allow_nan=allow_nan,
 _968
+)
 _969
-Also check for inline lists if <code><var>parser</var>.list_delimiter</code> is
-not None.
 _970
 _971
-Arguments
+def infer(self, value: str) -> AnyValueType:
 _972
----------
+"""
 _973
-`value`
+Infer the underlying type of a string
 _974
-: the string for which the type should be inferred
 _975
+Also check for inline lists if <code><var>parser</var>.list_delimiter</code> is
+not None.
 _976
-Returns
 _977
--------
+Arguments
 _978
-inferred type
+---------
 _979
+`value`
 _980
-Examples
+: the string for which the type should be inferred
 _981
---------
 _982
-```python
+Returns
 _983
-parser = TypeParser()
+-------
 _984
-parser.infer("true")  # bool
+inferred type
 _985
-parser.infer("2.0")   # float
 _986
-parser.infer("abc")   # str
+Examples
 _987
-```
+--------
 _988
-"""
+```python
 _989
-if self.is_none(value):
+parser = TypeParser()
 _990
-return NoneType
+parser.infer("true")  # bool
 _991
-if self.is_bool(value):
+parser.infer("2.0")   # float
 _992
-return bool
+parser.infer("abc")   # str
 _993
-if self.is_int(value):
+```
 _994
-return int
+"""
 _995
-if self.is_float(value):
+if self.is_none(value):
 _996
-if self._use_decimal:
+return NoneType
 _997
-return Decimal
+if self.is_bool(value):
 _998
-else:
+return bool
 _999
-return float
+if self.is_int(value):
 1000
+return int
 1001
-if self._trim:
+if self.is_float(value):
 1002
-value = value.strip()
+if self._use_decimal:
 1003
+return Decimal
 1004
-if self._list_delimiter is not None and self._list_delimiter in value:
+else:
 1005
-subvalues = value.split(self._list_delimiter)
+return float
 1006
-if self._trim:
 1007
-subvalues = [subvalue.strip() for subvalue in subvalues]
+if self._trim:
 1008
-reduced_type = reduce_types(self.infer(subvalue) for subvalue in subvalues)
+value = value.strip()
 1009
-r = list[reduced_type]
 1010
-return r
+if self._list_delimiter is not None and self._list_delimiter in value:
 1011
+subvalues = value.split(self._list_delimiter)
 1012
-return GenericValue
+if self._trim:
 1013
+subvalues = [subvalue.strip() for subvalue in subvalues]
 1014
+reduced_type = reduce_types(self.infer(subvalue) for subvalue in subvalues)
 1015
-def infer_series(self, values: Iterable[str]) -> AnyValueType:
+r = list[reduced_type]
 1016
-"""
+return r
 1017
-Infer the underlying common type of a series of strings
 1018
+return GenericValue
 1019
-If the values in the series do not have the same apparent type, the resulting
-type will be narrowest possible type that will encompass all values in the
-series. See `parsetypes.reduce_types()` for more information.
 1020
 1021
-Arguments
+def infer_series(self, values: Iterable[str]) -> AnyValueType:
 1022
----------
+"""
 1023
-`values`
+Infer the underlying common type of a series of strings
 1024
-: series of strings for which the type should be inferred
 1025
+If the values in the series do not have the same apparent type, the resulting
+type will be narrowest possible type that will encompass all values in the
+series. See `parsetypes.reduce_types()` for more information.
 1026
-Returns
 1027
--------
+Arguments
 1028
-inferred type
+---------
 1029
+`values`
 1030
-Examples
+: series of strings for which the type should be inferred
 1031
---------
 1032
-```python
+Returns
 1033
-parser = TypeParser()
+-------
 1034
-parser.infer_series(["1", "2", "3.4"])       # float
+inferred type
 1035
-parser.infer_series(["true", "false", "2"])  # int
 1036
-parser.infer_series(["1", "2.3", "abc"])     # str
+Examples
 1037
-```
+--------
 1038
-"""
+```python
 1039
-return reduce_types(self.infer(value) for value in values)
+parser = TypeParser()
 1040
+parser.infer_series(["1", "2", "3.4"])       # float
 1041
+parser.infer_series(["true", "false", "2"])  # int
 1042
-def infer_table(self, rows: Iterable[Sequence[str]]) -> list[AnyValueType]:
+parser.infer_series(["1", "2.3", "abc"])     # str
 1043
-"""
+```
 1044
-Infer the underlying common type for each column of a table of strings
+"""
 1045
+return reduce_types(self.infer(value) for value in values)
 1046
-For each column, if the values do not have the same apparent type, the
-resulting type will be narrowest possible type that will encompass all values
-in the column. See `parsetypes.reduce_types()` for more information.
 1047
 1048
-Note that the individual inferred types of every value in the table must be
-able to fit into memory.
+def infer_table(self, rows: Iterable[Sequence[str]]) -> list[AnyValueType]:
 1049
+"""
 1050
-Arguments
+Infer the underlying common type for each column of a table of strings
 1051
----------
 1052
-`rows`
+For each column, if the values do not have the same apparent type, the
+resulting type will be narrowest possible type that will encompass all values
+in the column. See `parsetypes.reduce_types()` for more information.
 1053
-: table of strings for which the types should be inferred, in row-major order
 1054
+Note that the individual inferred types of every value in the table must be
+able to fit into memory.
 1055
-Returns
 1056
--------
+Arguments
 1057
-inferred types
+---------
 1058
+`rows`
 1059
-Examples
+: table of strings for which the types should be inferred, in row-major order
 1060
---------
 1061
-```python
+Returns
 1062
-parser = TypeParser()
+-------
 1063
-parser.infer_table([
+inferred types
 1064
-["1",   "true",  "1"],
 1065
-["2",   "false", "2.3"],
+Examples
 1066
-["3.4", "2",     "abc"],
+--------
 1067
-])
+```python
 1068
-# [float, int, str]
+parser = TypeParser()
 1069
-```
+parser.infer_table([
 1070
-"""
+["1",   "true",  "1"],
 1071
-rows_iter = iter(rows)
+["2",   "false", "2.3"],
 1072
-first_row = next(rows_iter, None)
+["3.4", "2",     "abc"],
 1073
-if first_row is None:
+])
 1074
-return []
+# [float, int, str]
 1075
+```
 1076
-num_cols = len(first_row)
+"""
 1077
-if num_cols == 0:
+rows_iter = iter(rows)
 1078
-return []
+first_row = next(rows_iter, None)
 1079
+if first_row is None:
 1080
-table = _TypeTable([[self.infer(value)] for value in first_row])
+return []
 1081
-for row in rows_iter:
 1082
-table.add_row([self.infer(value) for value in row])
+num_cols = len(first_row)
 1083
+if num_cols == 0:
 1084
-return [reduce_types(col) for col in table.cols]
+return []
 1085
 1086
+table = _TypeTable([[self.infer(value)] for value in first_row])
 1087
-def convert(self, value: str, target_type: AnyValueType) -> AnyValue:
+for row in rows_iter:
 1088
-"""
+table.add_row([self.infer(value) for value in row])
 1089
-Convert a string to the specified target type if possible
 1090
+return [reduce_types(col) for col in table.cols]
 1091
-Valid values for `target_type` include any return value from `infer()`,
-`infer_series()` and `infer_table()`. To infer and convert the string
-automatically, use `parse()`, `parse_series()` or `parse_table()` instead.
 1092
 1093
-Arguments
+def convert(self, value: str, target_type: AnyValueType) -> AnyValue:
 1094
----------
+"""
 1095
-`value`
+Convert a string to the specified target type if possible
 1096
-: the string to be converted
 1097
+Valid values for `target_type` include any return value from `infer()`,
+`infer_series()` and `infer_table()`. To infer and convert the string
+automatically, use `parse()`, `parse_series()` or `parse_table()` instead.
 1098
-`target_type`
 1099
-: type to which the value should be converted
+Arguments
 1100
+---------
 1101
-Returns
+`value`
 1102
--------
+: the string to be converted
 1103
-converted value
 1104
+`target_type`
 1105
-Raises
+: type to which the value should be converted
 1106
--------
 1107
-`ValueError`
+Returns
 1108
-: if `value` cannot be converted to `target_type`
+-------
 1109
+converted value
 1110
-`TypeError`
 1111
-: if `target_type` is not a valid type
+Raises
 1112
+-------
 1113
-Examples
+`ValueError`
 1114
---------
+: if `value` cannot be converted to `target_type`
 1115
-```python
 1116
-parser = TypeParser()
+`TypeError`
 1117
-parser.convert("true", bool)  # True
+: if `target_type` is not a valid type
 1118
-parser.convert("2", int)      # 2
 1119
-parser.convert("2", float)    # 2.
+Examples
 1120
-```
+--------
 1121
-"""
+```python
 1122
-base, type_args = _decompose_type(target_type)
+parser = TypeParser()
 1123
-if base == NoneType:
+parser.convert("true", bool)  # True
 1124
-return self.parse_none(value)
+parser.convert("2", int)      # 2
 1125
-elif base == bool:
+parser.convert("2", float)    # 2.
 1126
-return self.parse_bool(value)
+```
 1127
-elif base == int:
+"""
 1128
-return self.parse_int(value)
+base, type_args = _decompose_type(target_type)
 1129
-elif base == Decimal:
+if base == NoneType:
 1130
-return self.parse_decimal(value)
+return self.parse_none(value)
 1131
-elif base == float:
+elif base == bool:
 1132
-return self.parse_float(value)
+return self.parse_bool(value)
 1133
-elif base == str:
+elif base == int:
 1134
-return value
+return self.parse_int(value)
 1135
-elif base == Nullable:
+elif base == Decimal:
 1136
-if self.is_none(value):
+return self.parse_decimal(value)
 1137
-return None
+elif base == float:
 1138
-else:
+return self.parse_float(value)
 1139
-if type_args is not None and len(type_args) == 1 and type_args[0] != str:
+elif base == str:
 1140
-inner_type = type_args[0]
+return value
 1141
-return self.convert(value, inner_type)
+elif base == Nullable:
 1142
-else:
+if self.is_none(value):
 1143
-return value
+return None
 1144
-elif base == list:
+else:
 1145
-subvalues = value.split(self._list_delimiter)
+if type_args is not None and len(type_args) == 1 and type_args[0] != str:
 1146
-if self._trim:
+inner_type = type_args[0]
 1147
-subvalues = [subvalue.strip() for subvalue in subvalues]
+return self.convert(value, inner_type)
 1148
-if type_args is not None and len(type_args) == 1 and type_args[0] != str:
+else:
 1149
-subtype = type_args[0]
+return value
 1150
-return [self.convert(subvalue, subtype) for subvalue in subvalues]
+elif base == list:
 1151
-else:
+subvalues = value.split(self._list_delimiter)
 1152
-return subvalues
+if self._trim:
 1153
-else:
+subvalues = [subvalue.strip() for subvalue in subvalues]
 1154
-raise TypeError(f"cannot convert to type: {target_type}")
+if type_args is not None and len(type_args) == 1 and type_args[0] != str:
 1155
+subtype = type_args[0]
 1156
+return [self.convert(subvalue, subtype) for subvalue in subvalues]
 1157
-def parse(self, value: str) -> AnyValue:
+else:
 1158
-"""
+return subvalues
 1159
-Parse a string and convert it to its underlying type
+else:
 1160
+raise TypeError(f"cannot convert to type: {target_type}")
 1161
-Arguments
 1162
----------
 1163
-`value`
+def parse(self, value: str) -> AnyValue:
 1164
-: the string to be parsed
+"""
 1165
+Parse a string and convert it to its underlying type
 1166
-Returns
 1167
--------
+Arguments
 1168
-converted value
+---------
 1169
+`value`
 1170
-Examples
+: the string to be parsed
 1171
---------
 1172
-```python
+Returns
 1173
-parser = TypeParser()
+-------
 1174
-parser.parse("true")  # True
+converted value
 1175
-parser.parse("2.0")   # 2.
 1176
-parser.parse("abc")   # "abc"
+Examples
 1177
-```
+--------
 1178
-"""
+```python
 1179
-return self.convert(value, self.infer(value))
+parser = TypeParser()
 1180
+parser.parse("true")  # True
 1181
+parser.parse("2.0")   # 2.
 1182
-def parse_series(self, values: Iterable[str]) -> list[AnyValue]:
+parser.parse("abc")   # "abc"
 1183
-"""
+```
 1184
-Parse a series of strings and convert them to their underlying common type
+"""
 1185
+return self.convert(value, self.infer(value))
 1186
-If the values in the series do not have the same apparent type, the common type
-is taken as the narrowest possible type that will encompass all values in the
-series. See `parsetypes.reduce_types()` for more information.
 1187
 1188
-Arguments
+def parse_series(self, values: Iterable[str]) -> list[AnyValue]:
 1189
----------
+"""
 1190
-`values`
+Parse a series of strings and convert them to their underlying common type
 1191
-: series of strings to be parsed
 1192
+If the values in the series do not have the same apparent type, the common type
+is taken as the narrowest possible type that will encompass all values in the
+series. See `parsetypes.reduce_types()` for more information.
 1193
-Returns
 1194
--------
+Arguments
 1195
-converted values
+---------
 1196
+`values`
 1197
-Examples
+: series of strings to be parsed
 1198
---------
 1199
-```python
+Returns
 1200
-parser = TypeParser()
+-------
 1201
-parser.parse_series(["1", "2", "3"])        # [1, 2, 3]
+converted values
 1202
-parser.parse_series(["5", "6.7", "8."])     # [5., 6.7, 8.]
 1203
-parser.parse_series(["true", "false", ""])  # [True, False, None]
+Examples
 1204
-parser.parse_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
+--------
 1205
-```
+```python
 1206
-"""
+parser = TypeParser()
 1207
-inferred = self.infer_series(values)
+parser.parse_series(["1", "2", "3"])        # [1, 2, 3]
 1208
-return [self.convert(value, inferred) for value in values]
+parser.parse_series(["5", "6.7", "8."])     # [5., 6.7, 8.]
 1209
+parser.parse_series(["true", "false", ""])  # [True, False, None]
 1210
+parser.parse_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
 1211
-def parse_table(self, rows: Iterable[Sequence[str]]) -> list[list[AnyValue]]:
+```
 1212
 """
 1213
-Parse a table of strings and convert them to the underlying common type of each
-column
+inferred = self.infer_series(values)
 1214
+return [self.convert(value, inferred) for value in values]
 1215
+1216
+1217
+def parse_table(self, rows: Iterable[Sequence[str]]) -> list[list[AnyValue]]:
+1218
+"""
+1219
+Parse a table of strings and convert them to the underlying common type of each
+column
+1220
+1221
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See `parsetypes.reduce_types()` for more information.
-1216
-1217
+1222
+1223
 Note that the type to which the values should be converted is determined by
 `infer_table()`, and so the individual inferred types of every value in the
 table must be able to fit into memory.
-1218
-1219
+1224
+1225
 This is a function that computes the entire table and returns it all at once.
 The generator function `iterate_table()` behaves analogously, except that it
 computes and yields each row one at a time instead.
-1220
-1221
+1226
+1227
 Arguments
-1222
+1228
 ---------
-1223
+1229
 `rows`
-1224
+1230
 : table of strings to be parsed, in row-major order
-1225
-1226
+1231
+1232
 `iterator`
-1227
+1233
 : whether the parsed values should be yielded as an iterator. If False, which
 is the default, the entire table is computed and returned as a list of lists.
 If True, this function behaves as a generator, and the rows of the table are
 computed and yielded one at a time. However, note that even when set to True,
 the type inference requires that inferred type of each individual value must
 all be able to fit into memory at once.
-1228
-1229
+1234
+1235
 Returns
-1230
+1236
 -------
-1231
+1237
 converted table of values, in row-major order
-1232
-1233
+1238
+1239
 Examples
-1234
+1240
 --------
-1235
+1241
 ```python
-1236
+1242
 parser = TypeParser()
-1237
+1243
 table = parser.parse_table([
-1238
+1244
 ["1", "5",   "true",  "1"],
-1239
+1245
 ["2", "6.7", "false", "2.3"],
-1240
+1246
 ["3", "8.0", "",      "abc"],
-1241
+1247
 ]):
-1242
+1248
 assert table == [
-1243
+1249
 [1, 5.,  True,  "1"],
-1244
+1250
 [2, 6.7, False, "2.3"],
-1245
+1251
 [3, 8.,  None,  "abc"],
-1246
+1252
 ]
-1247
+1253
 ```
-1248
+1254
 """
-1249
+1255
 return [converted_row for converted_row in self.iterate_table(rows)]
-1250
-1251
-1252
+1256
+1257
+1258
 def iterate_table(self, rows: Iterable[Sequence[str]]) -> Iterator[list
 [AnyValue]]:
-1253
+1259
 """
-1254
+1260
 Parse a table of strings for the underlying common type of each column, then
 convert and yield each row
-1255
-1256
+1261
+1262
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See `parsetypes.reduce_types()` for more information.
-1257
-1258
+1263
+1264
 This is a generator function that computes and yields each row one at a time.
 However, note that in order to determine the types to which each column should
 be converted, the individual inferred types of every value in the table must
 still be able to fit into memory.
-1259
-1260
+1265
+1266
 The function `parse_table()` behaves analogously, except that it computes the
 entire table and returns it as a list of lists instead.
-1261
-1262
+1267
+1268
 Arguments
-1263
+1269
 ---------
-1264
+1270
 `rows`
-1265
+1271
 : table of strings to be parsed, in row-major order
-1266
-1267
+1272
+1273
 Yields
-1268
+1274
 ------
-1269
+1275
 each row of converted table values
-1270
-1271
+1276
+1277
 Examples
-1272
+1278
 --------
-1273
+1279
 ```python
-1274
+1280
 parser = TypeParser()
-1275
+1281
 table = parser.iterate_table([
-1276
+1282
 ["1",   "true",  "1"],
-1277
+1283
 ["2",   "false", "2.3"],
-1278
+1284
 ["3.4", "2",     "abc"],
-1279
+1285
 ]):
-1280
+1286
 assert next(table) == [1.,  1, "1"]
-1281
+1287
 assert next(table) == [2.,  0, "2.3"]
-1282
+1288
 assert next(table) == [3.4, 2, "abc"]
-1283
+1289
 ```
-1284
+1290
 """
-1285
+1291
 inferred_types = self.infer_table(rows)
-1286
-1287
+1292
+1293
 for row in rows:
-1288
+1294
 yield [self.convert(value, inferred) for value, inferred in zip(row,
 inferred_types)]
 A parser that can be used to infer the underlying types of data serialised as
 strings, and to convert them into their original underlying types.
 The behaviour of the parser and the type inference can be configured either in
 the constructor or using mutable properties of a parser instance. See the
 constructor documentation for the list of available options.
@@ -2953,15 +2968,17 @@
 Keyword arguments
 543
 -----------------
 544
 545
 `allow_negative`
 546
-: whether to accept negative values
+: whether to accept negative values. Since negative values are always indicated
+with a negative sign, `allow_sign` must also be True (which is the default
+setting) for this to have any effect.
 547
 548
 `allow_sign`
 549
 : whether to accept values prepended with a sign character. If False, it
 implies that `allow_negative` is False also.
 550
@@ -3073,15 +3090,17 @@
 return False
 604
 return True
 Check if a string represents an int
 ***** Arguments *****
 value : string to be checked
 ***** Keyword arguments *****
-allow_negative : whether to accept negative values
+allow_negative : whether to accept negative values. Since negative values are
+always indicated with a negative sign, allow_sign must also be True (which is
+the default setting) for this to have any effect.
 allow_sign : whether to accept values prepended with a sign character. If
 False, it implies that allow_negative is False also.
 allow_scientific : whether to accept scientific notation. If True, strings of
 the form "MeX" will be interpreted as the expression M * (10 ** X), where M is
 the mantissa/significand and X is the exponent. Note that M must be an integer
 and X must be a non-negative integer, even in cases where the expression would
 evaluate mathematically to an integer.
@@ -3469,18 +3488,24 @@
 ***** Raises *****
 ValueError if value cannot be parsed
 ***** Examples *****
 parser = TypeParser()
 parser.parse_bool("true")   # True
 parser.parse_bool("FALSE")  # False
 ⁰
-def parse_int(self, value: str, *, allow_scientific: bool = True) -> int: View
-Source
+def parse_int(
+self,
+value: str,
+*,
+allow_negative: bool = True,
+allow_sign: bool = True,
+allow_scientific: bool = True) -> int: View Source
 765
-def parse_int(self, value: str, *, allow_scientific: bool=True) -> int:
+def parse_int(self, value: str, *, allow_negative: bool=True, allow_sign:
+bool=True, allow_scientific: bool=True) -> int:
 766
 """
 767
 Parse a string and return it as an int if possible
 768
 769
 If the string represents a bool, it will be converted to `1` for True and `0`
@@ -3497,98 +3522,116 @@
 775
 776
 Keyword arguments
 777
 -----------------
 778
 779
-`allow_scientific`
+`allow_negative`
 780
-: whether to accept scientific notation. If True, strings of the form
-<code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
-<code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
-mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var>
-must be an integer and <var>X</var> must be a non-negative integer, even in
-cases where the expression would evaluate mathematically to an integer.
+: whether to accept negative values. Since negative values are always indicated
+with a negative sign, `allow_sign` must also be True (which is the default
+setting) for this to have any effect.
 781
 782
-Returns
+`allow_sign`
 783
--------
+: whether to accept values prepended with a sign character. If False, it
+implies that `allow_negative` is False also.
 784
-parsed int value
 785
+`allow_scientific`
 786
-Raises
+: whether to accept scientific notation. If True, strings of the form
+<code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
+<code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
+mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var>
+must be an integer and <var>X</var> must be a non-negative integer, even in
+cases where the expression would evaluate mathematically to an integer.
 787
-------
 788
-`ValueError` if `value` cannot be parsed
+Returns
 789
+-------
 790
-Examples
+parsed int value
 791
---------
 792
-```python
+Raises
 793
-parser = TypeParser()
+------
 794
-parser.parse_int("0")    # 0
+`ValueError` if `value` cannot be parsed
 795
-parser.parse_int("-1")   # -1
 796
-parser.parse_int("2e3")  # 2000
+Examples
 797
-```
+--------
 798
-"""
+```python
 799
-if self._trim:
+parser = TypeParser()
 800
-value = value.strip()
+parser.parse_int("0")    # 0
 801
+parser.parse_int("-1")   # -1
 802
-if self.is_int(value, allow_sign=True, allow_negative=True,
-allow_scientific=allow_scientific):
+parser.parse_int("2e3")  # 2000
 803
-if allow_scientific:
+```
 804
-value, exp = _decompose_string_pair(value, self._scientific_char,
-self._int_case_sensitive)
+"""
 805
-if exp is not None:
+if self._trim:
 806
-if value[0] in (self._negative_chars - {self._negative_char}):
+value = value.strip()
 807
-value = self._negative_char + value[1:]
 808
-return int(value) * (10 ** int(exp))
+if self.is_int(value, allow_negative=allow_negative, allow_sign=allow_sign,
+allow_scientific=allow_scientific):
 809
+if allow_scientific:
 810
-if value[0] in (self._negative_chars - {self._negative_char}):
+value, exp = _decompose_string_pair(value, self._scientific_char,
+self._int_case_sensitive)
 811
-value = self._negative_char + value[1:]
+if exp is not None:
 812
-return int(value)
+if value[0] in (self._negative_chars - {self._negative_char}):
 813
+value = self._negative_char + value[1:]
 814
-elif self.is_bool(value):
+return int(value) * (10 ** int(exp))
 815
-return int(self.parse_bool(value))
 816
-else:
+if value[0] in (self._negative_chars - {self._negative_char}):
 817
+value = self._negative_char + value[1:]
+818
+return int(value)
+819
+820
+elif self.is_bool(value):
+821
+return int(self.parse_bool(value))
+822
+else:
+823
 raise ValueError(f"not an integer: {value}")
 Parse a string and return it as an int if possible
 If the string represents a bool, it will be converted to 1 for True and 0 for
 False.
 ***** Arguments *****
 value : string to be parsed
 ***** Keyword arguments *****
+allow_negative : whether to accept negative values. Since negative values are
+always indicated with a negative sign, allow_sign must also be True (which is
+the default setting) for this to have any effect.
+allow_sign : whether to accept values prepended with a sign character. If
+False, it implies that allow_negative is False also.
 allow_scientific : whether to accept scientific notation. If True, strings of
 the form "MeX" will be interpreted as the expression M * (10 ** X), where M is
 the mantissa/significand and X is the exponent. Note that M must be an integer
 and X must be a non-negative integer, even in cases where the expression would
 evaluate mathematically to an integer.
 ***** Returns *****
 parsed int value
@@ -3603,115 +3646,115 @@
 def parse_float(
 self,
 value: str,
 *,
 allow_scientific: bool = True,
 allow_inf: bool = True,
 allow_nan: bool = True) -> float: View Source
-865
+871
 def parse_float(self, value: str, *, allow_scientific: bool=True, allow_inf:
 bool=True, allow_nan: bool=True) -> float:
-866
+872
 """
-867
+873
 Parse a string and return it as a (non-exact) float if possible
-868
-869
+874
+875
 If the string represents a bool, it will be converted to `1.` for True and `0.`
 for False. If the string represents an int, it will be converted to a float
 also.
-870
-871
+876
+877
 Behaves analogously to `parse_decimal()`, except that that returns an exact
 Decimal instead.
-872
-873
+878
+879
 Arguments
-874
+880
 ---------
-875
+881
 `value`
-876
+882
 : string to be parsed
-877
-878
+883
+884
 Keyword arguments
-879
+885
 -----------------
-880
-881
+886
+887
 `allow_scientific`
-882
+888
 : whether to accept scientific notation. If True, strings of the form
 <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
 <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
 mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var>
 must be an integer, but can be negative.
-883
-884
+889
+890
 `allow_inf`
-885
+891
 : whether to accept positive and negative infinity values. If True, strings
 that match the values in <code><var>parser</var>.inf_values</code> (empty set
 by default) are interpreted as infinity, or as negative infinity if prepended
 by a negative sign. The case sensitivity of this matching depends on
 <code><var>parser</var>.float_case_sensitive</code>, which is False by default.
-886
-887
+892
+893
 `allow_nan`
-888
+894
 : whether to accept NaN (not a number) representations. If True, strings that
 match the values in <code><var>parser</var>.nan_values</code> (empty set by
 default) are interpeted as NaN. The case sensitivity of this matching also
 depends on <code><var>parser</var>.float_case_sensitive</code>, which is False
 by default.
-889
-890
+895
+896
 Returns
-891
+897
 -------
-892
+898
 parsed float value
-893
-894
+899
+900
 Raises
-895
+901
 ------
-896
+902
 `ValueError` if `value` cannot be parsed
-897
-898
+903
+904
 Examples
-899
+905
 --------
-900
+906
 ```python
-901
+907
 parser = TypeParser(inf_values=["inf"], nan_values=["nan"])
-902
+908
 parser.parse_float("1.")       # 1.
-903
+909
 parser.parse_float("1.23e2")   # 123.
-904
+910
 parser.parse_float("1.23e-2")  # 0.0123
-905
+911
 parser.parse_float("inf")      # math.inf
-906
+912
 ```
-907
+913
 """
-908
+914
 return self._parse_floatlike(value, float, math.inf, math.nan,
-909
+915
 allow_scientific=allow_scientific,
-910
+916
 allow_inf=allow_inf,
-911
+917
 allow_nan=allow_nan,
-912
+918
 )
 Parse a string and return it as a (non-exact) float if possible
 If the string represents a bool, it will be converted to 1. for True and 0. for
 False. If the string represents an int, it will be converted to a float also.
 Behaves analogously to parse_decimal(), except that that returns an exact
 Decimal instead.
 ***** Arguments *****
@@ -3744,116 +3787,116 @@
 def parse_decimal(
 self,
 value: str,
 *,
 allow_scientific: bool = True,
 allow_inf: bool = True,
 allow_nan: bool = True) -> decimal.Decimal: View Source
-915
+921
 def parse_decimal(self, value: str, *, allow_scientific: bool=True, allow_inf:
 bool=True, allow_nan: bool=True) -> Decimal:
-916
+922
 """
-917
+923
 Parse a string and return it as an exact Decimal if possible
-918
-919
+924
+925
 If the string represents a bool, it will be converted to `Decimal(1)` for True
 and `Decimal(0)` for False. If the string represents an int, it will be
 converted to a Decimal also.
-920
-921
+926
+927
 Behaves analogously to `parse_float()`, except that that returns a non-exact
 float instead.
-922
-923
+928
+929
 Arguments
-924
+930
 ---------
-925
+931
 `value`
-926
+932
 : string to be parsed
-927
-928
+933
+934
 Keyword arguments
-929
+935
 -----------------
-930
-931
+936
+937
 `allow_scientific`
-932
+938
 : whether to accept scientific notation. If True, strings of the form
 <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
 <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
 mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var>
 must be an integer, but can be negative.
-933
-934
+939
+940
 `allow_inf`
-935
+941
 : whether to accept positive and negative infinity values. If True, strings
 that match the values in <code><var>parser</var>.inf_values</code> (empty set
 by default) are interpreted as infinity, or as negative infinity if prepended
 by a negative sign. The case sensitivity of this matching depends on
 <code><var>parser</var>.float_case_sensitive</code>, which is False by default.
-936
-937
+942
+943
 `allow_nan`
-938
+944
 : whether to accept NaN (not a number) representations. If True, strings that
 match the values in <code><var>parser</var>.nan_values</code> (empty set by
 default) are interpeted as NaN. The case sensitivity of this matching also
 depends on <code><var>parser</var>.float_case_sensitive</code>, which is False
 by default.
-939
-940
+945
+946
 Returns
-941
+947
 -------
-942
+948
 parsed Decimal value
-943
-944
+949
+950
 Raises
-945
+951
 ------
-946
+952
 `ValueError` if `value` cannot be parsed
-947
-948
+953
+954
 Examples
-949
+955
 --------
-950
+956
 ```python
-951
+957
 parser = TypeParser(inf_values=["inf"], nan_values=["nan"])
-952
+958
 parser.parse_decimal("1.")       # Decimal(1)
-953
+959
 parser.parse_decimal("1.23e2")   # Decimal(123)
-954
+960
 parser.parse_decimal("1.23e-2")  # Decimal(123) / Decimal(10000)
-955
+961
 parser.parse_decimal("inf")      # Decimal(math.inf)
-956
+962
 ```
-957
+963
 """
-958
+964
 return self._parse_floatlike(value, Decimal, Decimal(math.inf), Decimal
 (math.nan),
-959
+965
 allow_scientific=allow_scientific,
-960
+966
 allow_inf=allow_inf,
-961
+967
 allow_nan=allow_nan,
-962
+968
 )
 Parse a string and return it as an exact Decimal if possible
 If the string represents a bool, it will be converted to Decimal(1) for True
 and Decimal(0) for False. If the string represents an int, it will be converted
 to a Decimal also.
 Behaves analogously to parse_float(), except that that returns a non-exact
 float instead.
@@ -3884,103 +3927,103 @@
 parser.parse_decimal("1.23e-2")  # Decimal(123) / Decimal(10000)
 parser.parse_decimal("inf")      # Decimal(math.inf)
 ⁰
 def infer(
 self,
 value: str) -> Type[Union[str, int, float, decimal.Decimal, bool, NoneType,
 Nullable, list]]: View Source
-_965
-def infer(self, value: str) -> AnyValueType:
-_966
-"""
-_967
-Infer the underlying type of a string
-_968
-_969
-Also check for inline lists if <code><var>parser</var>.list_delimiter</code> is
-not None.
-_970
 _971
-Arguments
+def infer(self, value: str) -> AnyValueType:
 _972
----------
+"""
 _973
-`value`
+Infer the underlying type of a string
 _974
-: the string for which the type should be inferred
 _975
+Also check for inline lists if <code><var>parser</var>.list_delimiter</code> is
+not None.
 _976
-Returns
 _977
--------
+Arguments
 _978
-inferred type
+---------
 _979
+`value`
 _980
-Examples
+: the string for which the type should be inferred
 _981
---------
 _982
-```python
+Returns
 _983
-parser = TypeParser()
+-------
 _984
-parser.infer("true")  # bool
+inferred type
 _985
-parser.infer("2.0")   # float
 _986
-parser.infer("abc")   # str
+Examples
 _987
-```
+--------
 _988
-"""
+```python
 _989
-if self.is_none(value):
+parser = TypeParser()
 _990
-return NoneType
+parser.infer("true")  # bool
 _991
-if self.is_bool(value):
+parser.infer("2.0")   # float
 _992
-return bool
+parser.infer("abc")   # str
 _993
-if self.is_int(value):
+```
 _994
-return int
+"""
 _995
-if self.is_float(value):
+if self.is_none(value):
 _996
-if self._use_decimal:
+return NoneType
 _997
-return Decimal
+if self.is_bool(value):
 _998
-else:
+return bool
 _999
-return float
+if self.is_int(value):
 1000
+return int
 1001
-if self._trim:
+if self.is_float(value):
 1002
-value = value.strip()
+if self._use_decimal:
 1003
+return Decimal
 1004
-if self._list_delimiter is not None and self._list_delimiter in value:
+else:
 1005
-subvalues = value.split(self._list_delimiter)
+return float
 1006
-if self._trim:
 1007
-subvalues = [subvalue.strip() for subvalue in subvalues]
+if self._trim:
 1008
-reduced_type = reduce_types(self.infer(subvalue) for subvalue in subvalues)
+value = value.strip()
 1009
-r = list[reduced_type]
 1010
-return r
+if self._list_delimiter is not None and self._list_delimiter in value:
 1011
+subvalues = value.split(self._list_delimiter)
 1012
+if self._trim:
+1013
+subvalues = [subvalue.strip() for subvalue in subvalues]
+1014
+reduced_type = reduce_types(self.infer(subvalue) for subvalue in subvalues)
+1015
+r = list[reduced_type]
+1016
+return r
+1017
+1018
 return GenericValue
 Infer the underlying type of a string
 Also check for inline lists if parser.list_delimiter is not None.
 ***** Arguments *****
 value : the string for which the type should be inferred
 ***** Returns *****
 inferred type
@@ -3990,61 +4033,61 @@
 parser.infer("2.0")   # float
 parser.infer("abc")   # str
 ⁰
 def infer_series(
 self,
 values: Iterable[str]) -> Type[Union[str, int, float, decimal.Decimal, bool,
 NoneType, Nullable, list]]: View Source
-1015
+1021
 def infer_series(self, values: Iterable[str]) -> AnyValueType:
-1016
+1022
 """
-1017
+1023
 Infer the underlying common type of a series of strings
-1018
-1019
+1024
+1025
 If the values in the series do not have the same apparent type, the resulting
 type will be narrowest possible type that will encompass all values in the
 series. See `parsetypes.reduce_types()` for more information.
-1020
-1021
+1026
+1027
 Arguments
-1022
+1028
 ---------
-1023
+1029
 `values`
-1024
+1030
 : series of strings for which the type should be inferred
-1025
-1026
+1031
+1032
 Returns
-1027
+1033
 -------
-1028
+1034
 inferred type
-1029
-1030
+1035
+1036
 Examples
-1031
+1037
 --------
-1032
+1038
 ```python
-1033
+1039
 parser = TypeParser()
-1034
+1040
 parser.infer_series(["1", "2", "3.4"])       # float
-1035
+1041
 parser.infer_series(["true", "false", "2"])  # int
-1036
+1042
 parser.infer_series(["1", "2.3", "abc"])     # str
-1037
+1043
 ```
-1038
+1044
 """
-1039
+1045
 return reduce_types(self.infer(value) for value in values)
 Infer the underlying common type of a series of strings
 If the values in the series do not have the same apparent type, the resulting
 type will be narrowest possible type that will encompass all values in the
 series. See parsetypes.reduce_types() for more information.
 ***** Arguments *****
 values : series of strings for which the type should be inferred
@@ -4056,94 +4099,94 @@
 parser.infer_series(["true", "false", "2"])  # int
 parser.infer_series(["1", "2.3", "abc"])     # str
 ⁰
 def infer_table(
 self,
 rows: Iterable[Sequence[str]]) -> list[typing.Type[typing.Union[str, int,
 float, decimal.Decimal, bool, NoneType, Nullable, list]]]: View Source
-1042
+1048
 def infer_table(self, rows: Iterable[Sequence[str]]) -> list[AnyValueType]:
-1043
+1049
 """
-1044
+1050
 Infer the underlying common type for each column of a table of strings
-1045
-1046
+1051
+1052
 For each column, if the values do not have the same apparent type, the
 resulting type will be narrowest possible type that will encompass all values
 in the column. See `parsetypes.reduce_types()` for more information.
-1047
-1048
-Note that the individual inferred types of every value in the table must be
-able to fit into memory.
-1049
-1050
-Arguments
-1051
----------
-1052
-`rows`
 1053
-: table of strings for which the types should be inferred, in row-major order
 1054
+Note that the individual inferred types of every value in the table must be
+able to fit into memory.
 1055
-Returns
 1056
--------
+Arguments
 1057
-inferred types
+---------
 1058
+`rows`
 1059
-Examples
+: table of strings for which the types should be inferred, in row-major order
 1060
---------
 1061
-```python
+Returns
 1062
-parser = TypeParser()
+-------
 1063
-parser.infer_table([
+inferred types
 1064
-["1",   "true",  "1"],
 1065
-["2",   "false", "2.3"],
+Examples
 1066
-["3.4", "2",     "abc"],
+--------
 1067
-])
+```python
 1068
-# [float, int, str]
+parser = TypeParser()
 1069
-```
+parser.infer_table([
 1070
-"""
+["1",   "true",  "1"],
 1071
-rows_iter = iter(rows)
+["2",   "false", "2.3"],
 1072
-first_row = next(rows_iter, None)
+["3.4", "2",     "abc"],
 1073
-if first_row is None:
+])
 1074
-return []
+# [float, int, str]
 1075
+```
 1076
-num_cols = len(first_row)
+"""
 1077
-if num_cols == 0:
+rows_iter = iter(rows)
 1078
-return []
+first_row = next(rows_iter, None)
 1079
+if first_row is None:
 1080
-table = _TypeTable([[self.infer(value)] for value in first_row])
+return []
 1081
-for row in rows_iter:
 1082
-table.add_row([self.infer(value) for value in row])
+num_cols = len(first_row)
 1083
+if num_cols == 0:
 1084
+return []
+1085
+1086
+table = _TypeTable([[self.infer(value)] for value in first_row])
+1087
+for row in rows_iter:
+1088
+table.add_row([self.infer(value) for value in row])
+1089
+1090
 return [reduce_types(col) for col in table.cols]
 Infer the underlying common type for each column of a table of strings
 For each column, if the values do not have the same apparent type, the
 resulting type will be narrowest possible type that will encompass all values
 in the column. See parsetypes.reduce_types() for more information.
 Note that the individual inferred types of every value in the table must be
 able to fit into memory.
@@ -4163,144 +4206,144 @@
 ⁰
 def convert(
 self,
 value: str,
 target_type: Type[Union[str, int, float, decimal.Decimal, bool, NoneType,
 Nullable, list]]) -> Union[str, int, float, decimal.Decimal, bool, NoneType,
 list]: View Source
-1087
+1093
 def convert(self, value: str, target_type: AnyValueType) -> AnyValue:
-1088
+1094
 """
-1089
+1095
 Convert a string to the specified target type if possible
-1090
-1091
+1096
+1097
 Valid values for `target_type` include any return value from `infer()`,
 `infer_series()` and `infer_table()`. To infer and convert the string
 automatically, use `parse()`, `parse_series()` or `parse_table()` instead.
-1092
-1093
-Arguments
-1094
----------
-1095
-`value`
-1096
-: the string to be converted
-1097
 1098
-`target_type`
 1099
-: type to which the value should be converted
+Arguments
 1100
+---------
 1101
-Returns
+`value`
 1102
--------
+: the string to be converted
 1103
-converted value
 1104
+`target_type`
 1105
-Raises
+: type to which the value should be converted
 1106
--------
 1107
-`ValueError`
+Returns
 1108
-: if `value` cannot be converted to `target_type`
+-------
 1109
+converted value
 1110
-`TypeError`
 1111
-: if `target_type` is not a valid type
+Raises
 1112
+-------
 1113
-Examples
+`ValueError`
 1114
---------
+: if `value` cannot be converted to `target_type`
 1115
-```python
 1116
-parser = TypeParser()
+`TypeError`
 1117
-parser.convert("true", bool)  # True
+: if `target_type` is not a valid type
 1118
-parser.convert("2", int)      # 2
 1119
-parser.convert("2", float)    # 2.
+Examples
 1120
-```
+--------
 1121
-"""
+```python
 1122
-base, type_args = _decompose_type(target_type)
+parser = TypeParser()
 1123
-if base == NoneType:
+parser.convert("true", bool)  # True
 1124
-return self.parse_none(value)
+parser.convert("2", int)      # 2
 1125
-elif base == bool:
+parser.convert("2", float)    # 2.
 1126
-return self.parse_bool(value)
+```
 1127
-elif base == int:
+"""
 1128
-return self.parse_int(value)
+base, type_args = _decompose_type(target_type)
 1129
-elif base == Decimal:
+if base == NoneType:
 1130
-return self.parse_decimal(value)
+return self.parse_none(value)
 1131
-elif base == float:
+elif base == bool:
 1132
-return self.parse_float(value)
+return self.parse_bool(value)
 1133
-elif base == str:
+elif base == int:
 1134
-return value
+return self.parse_int(value)
 1135
-elif base == Nullable:
+elif base == Decimal:
 1136
-if self.is_none(value):
+return self.parse_decimal(value)
 1137
-return None
+elif base == float:
 1138
-else:
+return self.parse_float(value)
 1139
-if type_args is not None and len(type_args) == 1 and type_args[0] != str:
+elif base == str:
 1140
-inner_type = type_args[0]
+return value
 1141
-return self.convert(value, inner_type)
+elif base == Nullable:
 1142
-else:
+if self.is_none(value):
 1143
-return value
+return None
 1144
-elif base == list:
+else:
 1145
-subvalues = value.split(self._list_delimiter)
+if type_args is not None and len(type_args) == 1 and type_args[0] != str:
 1146
-if self._trim:
+inner_type = type_args[0]
 1147
-subvalues = [subvalue.strip() for subvalue in subvalues]
+return self.convert(value, inner_type)
 1148
-if type_args is not None and len(type_args) == 1 and type_args[0] != str:
+else:
 1149
-subtype = type_args[0]
+return value
 1150
-return [self.convert(subvalue, subtype) for subvalue in subvalues]
+elif base == list:
 1151
-else:
+subvalues = value.split(self._list_delimiter)
 1152
-return subvalues
+if self._trim:
 1153
-else:
+subvalues = [subvalue.strip() for subvalue in subvalues]
 1154
+if type_args is not None and len(type_args) == 1 and type_args[0] != str:
+1155
+subtype = type_args[0]
+1156
+return [self.convert(subvalue, subtype) for subvalue in subvalues]
+1157
+else:
+1158
+return subvalues
+1159
+else:
+1160
 raise TypeError(f"cannot convert to type: {target_type}")
 Convert a string to the specified target type if possible
 Valid values for target_type include any return value from infer(),
 infer_series() and infer_table(). To infer and convert the string
 automatically, use parse(), parse_series() or parse_table() instead.
 ***** Arguments *****
 value : the string to be converted
@@ -4316,56 +4359,56 @@
 parser.convert("2", int)      # 2
 parser.convert("2", float)    # 2.
 ⁰
 def parse(
 self,
 value: str) -> Union[str, int, float, decimal.Decimal, bool, NoneType, list]:
 View Source
-1157
+1163
 def parse(self, value: str) -> AnyValue:
-1158
+1164
 """
-1159
+1165
 Parse a string and convert it to its underlying type
-1160
-1161
+1166
+1167
 Arguments
-1162
+1168
 ---------
-1163
+1169
 `value`
-1164
+1170
 : the string to be parsed
-1165
-1166
+1171
+1172
 Returns
-1167
+1173
 -------
-1168
+1174
 converted value
-1169
-1170
+1175
+1176
 Examples
-1171
+1177
 --------
-1172
+1178
 ```python
-1173
+1179
 parser = TypeParser()
-1174
+1180
 parser.parse("true")  # True
-1175
+1181
 parser.parse("2.0")   # 2.
-1176
+1182
 parser.parse("abc")   # "abc"
-1177
+1183
 ```
-1178
+1184
 """
-1179
+1185
 return self.convert(value, self.infer(value))
 Parse a string and convert it to its underlying type
 ***** Arguments *****
 value : the string to be parsed
 ***** Returns *****
 converted value
 ***** Examples *****
@@ -4374,65 +4417,65 @@
 parser.parse("2.0")   # 2.
 parser.parse("abc")   # "abc"
 ⁰
 def parse_series(
 self,
 values: Iterable[str]) -> list[typing.Union[str, int, float, decimal.Decimal,
 bool, NoneType, list]]: View Source
-1182
+1188
 def parse_series(self, values: Iterable[str]) -> list[AnyValue]:
-1183
+1189
 """
-1184
+1190
 Parse a series of strings and convert them to their underlying common type
-1185
-1186
+1191
+1192
 If the values in the series do not have the same apparent type, the common type
 is taken as the narrowest possible type that will encompass all values in the
 series. See `parsetypes.reduce_types()` for more information.
-1187
-1188
+1193
+1194
 Arguments
-1189
+1195
 ---------
-1190
+1196
 `values`
-1191
+1197
 : series of strings to be parsed
-1192
-1193
+1198
+1199
 Returns
-1194
+1200
 -------
-1195
+1201
 converted values
-1196
-1197
+1202
+1203
 Examples
-1198
+1204
 --------
-1199
+1205
 ```python
-1200
+1206
 parser = TypeParser()
-1201
+1207
 parser.parse_series(["1", "2", "3"])        # [1, 2, 3]
-1202
+1208
 parser.parse_series(["5", "6.7", "8."])     # [5., 6.7, 8.]
-1203
+1209
 parser.parse_series(["true", "false", ""])  # [True, False, None]
-1204
+1210
 parser.parse_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
-1205
+1211
 ```
-1206
+1212
 """
-1207
+1213
 inferred = self.infer_series(values)
-1208
+1214
 return [self.convert(value, inferred) for value in values]
 Parse a series of strings and convert them to their underlying common type
 If the values in the series do not have the same apparent type, the common type
 is taken as the narrowest possible type that will encompass all values in the
 series. See parsetypes.reduce_types() for more information.
 ***** Arguments *****
 values : series of strings to be parsed
@@ -4445,96 +4488,96 @@
 parser.parse_series(["true", "false", ""])  # [True, False, None]
 parser.parse_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
 ⁰
 def parse_table(
 self,
 rows: Iterable[Sequence[str]]) -> list[list[typing.Union[str, int, float,
 decimal.Decimal, bool, NoneType, list]]]: View Source
-1211
+1217
 def parse_table(self, rows: Iterable[Sequence[str]]) -> list[list[AnyValue]]:
-1212
+1218
 """
-1213
+1219
 Parse a table of strings and convert them to the underlying common type of each
 column
-1214
-1215
+1220
+1221
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See `parsetypes.reduce_types()` for more information.
-1216
-1217
+1222
+1223
 Note that the type to which the values should be converted is determined by
 `infer_table()`, and so the individual inferred types of every value in the
 table must be able to fit into memory.
-1218
-1219
+1224
+1225
 This is a function that computes the entire table and returns it all at once.
 The generator function `iterate_table()` behaves analogously, except that it
 computes and yields each row one at a time instead.
-1220
-1221
+1226
+1227
 Arguments
-1222
+1228
 ---------
-1223
+1229
 `rows`
-1224
+1230
 : table of strings to be parsed, in row-major order
-1225
-1226
+1231
+1232
 `iterator`
-1227
+1233
 : whether the parsed values should be yielded as an iterator. If False, which
 is the default, the entire table is computed and returned as a list of lists.
 If True, this function behaves as a generator, and the rows of the table are
 computed and yielded one at a time. However, note that even when set to True,
 the type inference requires that inferred type of each individual value must
 all be able to fit into memory at once.
-1228
-1229
+1234
+1235
 Returns
-1230
+1236
 -------
-1231
+1237
 converted table of values, in row-major order
-1232
-1233
+1238
+1239
 Examples
-1234
+1240
 --------
-1235
+1241
 ```python
-1236
+1242
 parser = TypeParser()
-1237
+1243
 table = parser.parse_table([
-1238
+1244
 ["1", "5",   "true",  "1"],
-1239
+1245
 ["2", "6.7", "false", "2.3"],
-1240
+1246
 ["3", "8.0", "",      "abc"],
-1241
+1247
 ]):
-1242
+1248
 assert table == [
-1243
+1249
 [1, 5.,  True,  "1"],
-1244
+1250
 [2, 6.7, False, "2.3"],
-1245
+1251
 [3, 8.,  None,  "abc"],
-1246
+1252
 ]
-1247
+1253
 ```
-1248
+1254
 """
-1249
+1255
 return [converted_row for converted_row in self.iterate_table(rows)]
 Parse a table of strings and convert them to the underlying common type of each
 column
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See parsetypes.reduce_types() for more information.
 Note that the type to which the values should be converted is determined by
@@ -4566,88 +4609,88 @@
 	[3, 8.,  None,  "abc"],
 ]
 ⁰
 def iterate_table(
 self,
 rows: Iterable[Sequence[str]]) -> Iterator[list[Union[str, int, float,
 decimal.Decimal, bool, NoneType, list]]]: View Source
-1252
+1258
 def iterate_table(self, rows: Iterable[Sequence[str]]) -> Iterator[list
 [AnyValue]]:
-1253
+1259
 """
-1254
+1260
 Parse a table of strings for the underlying common type of each column, then
 convert and yield each row
-1255
-1256
+1261
+1262
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See `parsetypes.reduce_types()` for more information.
-1257
-1258
+1263
+1264
 This is a generator function that computes and yields each row one at a time.
 However, note that in order to determine the types to which each column should
 be converted, the individual inferred types of every value in the table must
 still be able to fit into memory.
-1259
-1260
+1265
+1266
 The function `parse_table()` behaves analogously, except that it computes the
 entire table and returns it as a list of lists instead.
-1261
-1262
+1267
+1268
 Arguments
-1263
+1269
 ---------
-1264
+1270
 `rows`
-1265
+1271
 : table of strings to be parsed, in row-major order
-1266
-1267
+1272
+1273
 Yields
-1268
+1274
 ------
-1269
+1275
 each row of converted table values
-1270
-1271
+1276
+1277
 Examples
-1272
+1278
 --------
-1273
+1279
 ```python
-1274
+1280
 parser = TypeParser()
-1275
+1281
 table = parser.iterate_table([
-1276
+1282
 ["1",   "true",  "1"],
-1277
+1283
 ["2",   "false", "2.3"],
-1278
+1284
 ["3.4", "2",     "abc"],
-1279
+1285
 ]):
-1280
+1286
 assert next(table) == [1.,  1, "1"]
-1281
+1287
 assert next(table) == [2.,  0, "2.3"]
-1282
+1288
 assert next(table) == [3.4, 2, "abc"]
-1283
+1289
 ```
-1284
+1290
 """
-1285
+1291
 inferred_types = self.infer_table(rows)
-1286
-1287
+1292
+1293
 for row in rows:
-1288
+1294
 yield [self.convert(value, inferred) for value, inferred in zip(row,
 inferred_types)]
 Parse a table of strings for the underlying common type of each column, then
 convert and yield each row
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See parsetypes.reduce_types() for more information.
@@ -4667,15 +4710,14 @@
 	["1",   "true",  "1"],
 	["2",   "false", "2.3"],
 	["3.4", "2",     "abc"],
 ]):
 assert next(table) == [1.,  1, "1"]
 assert next(table) == [2.,  0, "2.3"]
 assert next(table) == [3.4, 2, "abc"]
-** Inherited Members **
   ⁰
 def reduce_types(
 types: Iterable[Type[Union[str, int, float, decimal.Decimal, bool, NoneType,
 Nullable, list]]]) -> Type[Union[str, int, float, decimal.Decimal, bool,
 NoneType, Nullable, list]]: View Source
 156def reduce_types(types: Iterable[AnyValueType]) -> AnyValueType:
 157
@@ -4784,10 +4826,8 @@
 """
 30
 pass
 Dummy container type that represents a scalar (S) that could also be None
 The type annotation Nullable[S] is treated as equivalent to Union[S,
 types.NoneType], which will accept either a value of type S or the value None.
 This class should not be instantiated.
-Nullable()
-** Inherited Members **
```

### Comparing `parsetypes-0.3/docs/html/search.js` & `parsetypes-0.3.1/docs/html/search.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -728,15 +728,15 @@
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.is_int": {
                     "fullname": "parsetypes.TypeParser.is_int",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.is_int",
                     "kind": "function",
-                    "doc": "<p>Check if a string represents an int</p>\n\n<h2 id=\"arguments\">Arguments</h2>\n\n<p><code>value</code>\n: string to be checked</p>\n\n<h2 id=\"keyword-arguments\">Keyword arguments</h2>\n\n<p><code>allow_negative</code>\n: whether to accept negative values</p>\n\n<p><code>allow_sign</code>\n: whether to accept values prepended with a sign character. If False, it implies that <code>allow_negative</code> is False also.</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"<var>M</var>e<var>X</var>\"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var> must be an integer and <var>X</var> must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>whether it is an int</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;0&quot;</span><span class=\"p\">)</span>    <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;-1&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># False</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;&quot;</span><span class=\"p\">)</span>     <span class=\"c1\"># False</span>\n</code></pre>\n</div>\n",
+                    "doc": "<p>Check if a string represents an int</p>\n\n<h2 id=\"arguments\">Arguments</h2>\n\n<p><code>value</code>\n: string to be checked</p>\n\n<h2 id=\"keyword-arguments\">Keyword arguments</h2>\n\n<p><code>allow_negative</code>\n: whether to accept negative values. Since negative values are always indicated with a negative sign, <code>allow_sign</code> must also be True (which is the default setting) for this to have any effect.</p>\n\n<p><code>allow_sign</code>\n: whether to accept values prepended with a sign character. If False, it implies that <code>allow_negative</code> is False also.</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"<var>M</var>e<var>X</var>\"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var> must be an integer and <var>X</var> must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>whether it is an int</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;0&quot;</span><span class=\"p\">)</span>    <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;-1&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># False</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;&quot;</span><span class=\"p\">)</span>     <span class=\"c1\"># False</span>\n</code></pre>\n</div>\n",
                     "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"o\">*</span>,</span><span class=\"param\">\t<span class=\"n\">allow_negative</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_sign</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_scientific</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">bool</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.is_float": {
                     "fullname": "parsetypes.TypeParser.is_float",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.is_float",
@@ -773,16 +773,16 @@
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.parse_int": {
                     "fullname": "parsetypes.TypeParser.parse_int",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.parse_int",
                     "kind": "function",
-                    "doc": "<p>Parse a string and return it as an int if possible</p>\n\n<p>If the string represents a bool, it will be converted to <code>1</code> for True and <code>0</code> for False.</p>\n\n<h2 id=\"arguments\">Arguments</h2>\n\n<p><code>value</code>\n: string to be parsed</p>\n\n<h2 id=\"keyword-arguments\">Keyword arguments</h2>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"<var>M</var>e<var>X</var>\"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var> must be an integer and <var>X</var> must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>parsed int value</p>\n\n<h2 id=\"raises\">Raises</h2>\n\n<p><code>ValueError</code> if <code>value</code> cannot be parsed</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;0&quot;</span><span class=\"p\">)</span>    <span class=\"c1\"># 0</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;-1&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># -1</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;2e3&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># 2000</span>\n</code></pre>\n</div>\n",
-                    "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"o\">*</span>, </span><span class=\"param\"><span class=\"n\">allow_scientific</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">int</span>:</span></span>",
+                    "doc": "<p>Parse a string and return it as an int if possible</p>\n\n<p>If the string represents a bool, it will be converted to <code>1</code> for True and <code>0</code> for False.</p>\n\n<h2 id=\"arguments\">Arguments</h2>\n\n<p><code>value</code>\n: string to be parsed</p>\n\n<h2 id=\"keyword-arguments\">Keyword arguments</h2>\n\n<p><code>allow_negative</code>\n: whether to accept negative values. Since negative values are always indicated with a negative sign, <code>allow_sign</code> must also be True (which is the default setting) for this to have any effect.</p>\n\n<p><code>allow_sign</code>\n: whether to accept values prepended with a sign character. If False, it implies that <code>allow_negative</code> is False also.</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"<var>M</var>e<var>X</var>\"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var> must be an integer and <var>X</var> must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>parsed int value</p>\n\n<h2 id=\"raises\">Raises</h2>\n\n<p><code>ValueError</code> if <code>value</code> cannot be parsed</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;0&quot;</span><span class=\"p\">)</span>    <span class=\"c1\"># 0</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;-1&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># -1</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;2e3&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># 2000</span>\n</code></pre>\n</div>\n",
+                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"o\">*</span>,</span><span class=\"param\">\t<span class=\"n\">allow_negative</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_sign</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_scientific</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">int</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.parse_float": {
                     "fullname": "parsetypes.TypeParser.parse_float",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.parse_float",
                     "kind": "function",
@@ -883,22 +883,14 @@
                 "parsetypes.Nullable": {
                     "fullname": "parsetypes.Nullable",
                     "modulename": "parsetypes",
                     "qualname": "Nullable",
                     "kind": "class",
                     "doc": "<p>Dummy container type that represents a scalar (<code>S</code>) that could also be None</p>\n\n<p>The type annotation <code>Nullable[S]</code> is treated as equivalent to <code>Union[S, types.NoneType]</code>, which will accept either a value of type <code>S</code> or the value <code>None</code>.</p>\n\n<p>This class should not be instantiated.</p>\n",
                     "bases": "typing.Generic[~S]"
-                },
-                "parsetypes.Nullable.__init__": {
-                    "fullname": "parsetypes.Nullable.__init__",
-                    "modulename": "parsetypes",
-                    "qualname": "Nullable.__init__",
-                    "kind": "function",
-                    "doc": "<p></p>\n",
-                    "signature": "<span class=\"signature pdoc-code condensed\">()</span>"
                 }
             },
             "docInfo": {
                 "parsetypes": {
                     "qualname": 0,
                     "fullname": 1,
                     "annotation": 0,
@@ -946,15 +938,15 @@
                 "parsetypes.TypeParser.is_int": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 89,
                     "bases": 0,
-                    "doc": 294
+                    "doc": 324
                 },
                 "parsetypes.TypeParser.is_float": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 89,
@@ -989,17 +981,17 @@
                     "doc": 194
                 },
                 "parsetypes.TypeParser.parse_int": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
-                    "signature": 47,
+                    "signature": 89,
                     "bases": 0,
-                    "doc": 271
+                    "doc": 342
                 },
                 "parsetypes.TypeParser.parse_float": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 89,
@@ -1100,40 +1092,28 @@
                     "qualname": 1,
                     "fullname": 2,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 0,
                     "bases": 2,
                     "doc": 62
-                },
-                "parsetypes.Nullable.__init__": {
-                    "qualname": 3,
-                    "fullname": 4,
-                    "annotation": 0,
-                    "default_value": 0,
-                    "signature": 4,
-                    "bases": 0,
-                    "doc": 3
                 }
             },
-            "length": 24,
+            "length": 23,
             "save": true
         },
         "index": {
             "qualname": {
                 "root": {
                     "docs": {
                         "parsetypes.TypeParser.__init__": {
                             "tf": 1
-                        },
-                        "parsetypes.Nullable.__init__": {
-                            "tf": 1
                         }
                     },
-                    "df": 2,
+                    "df": 1,
                     "t": {
                         "docs": {},
                         "df": 0,
                         "y": {
                             "docs": {},
                             "df": 0,
                             "p": {
@@ -1274,20 +1254,17 @@
                             "i": {
                                 "docs": {},
                                 "df": 0,
                                 "t": {
                                     "docs": {
                                         "parsetypes.TypeParser.__init__": {
                                             "tf": 1
-                                        },
-                                        "parsetypes.Nullable.__init__": {
-                                            "tf": 1
                                         }
                                     },
-                                    "df": 2
+                                    "df": 1
                                 }
                             },
                             "t": {
                                 "docs": {
                                     "parsetypes.TypeParser.is_int": {
                                         "tf": 1
                                     },
@@ -1409,20 +1386,17 @@
                                             "l": {
                                                 "docs": {},
                                                 "df": 0,
                                                 "e": {
                                                     "docs": {
                                                         "parsetypes.Nullable": {
                                                             "tf": 1
-                                                        },
-                                                        "parsetypes.Nullable.__init__": {
-                                                            "tf": 1
                                                         }
                                                     },
-                                                    "df": 2
+                                                    "df": 1
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         }
@@ -1651,20 +1625,17 @@
                 }
             },
             "fullname": {
                 "root": {
                     "docs": {
                         "parsetypes.TypeParser.__init__": {
                             "tf": 1
-                        },
-                        "parsetypes.Nullable.__init__": {
-                            "tf": 1
                         }
                     },
-                    "df": 2,
+                    "df": 1,
                     "p": {
                         "docs": {},
                         "df": 0,
                         "a": {
                             "docs": {},
                             "df": 0,
                             "r": {
@@ -1779,20 +1750,17 @@
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.reduce_types": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.Nullable": {
                                                                     "tf": 1
-                                                                },
-                                                                "parsetypes.Nullable.__init__": {
-                                                                    "tf": 1
                                                                 }
                                                             },
-                                                            "df": 24
+                                                            "df": 23
                                                         }
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
@@ -1943,20 +1911,17 @@
                             "i": {
                                 "docs": {},
                                 "df": 0,
                                 "t": {
                                     "docs": {
                                         "parsetypes.TypeParser.__init__": {
                                             "tf": 1
-                                        },
-                                        "parsetypes.Nullable.__init__": {
-                                            "tf": 1
                                         }
                                     },
-                                    "df": 2
+                                    "df": 1
                                 }
                             },
                             "t": {
                                 "docs": {
                                     "parsetypes.TypeParser.is_int": {
                                         "tf": 1
                                     },
@@ -2078,20 +2043,17 @@
                                             "l": {
                                                 "docs": {},
                                                 "df": 0,
                                                 "e": {
                                                     "docs": {
                                                         "parsetypes.Nullable": {
                                                             "tf": 1
-                                                        },
-                                                        "parsetypes.Nullable.__init__": {
-                                                            "tf": 1
                                                         }
                                                     },
-                                                    "df": 2
+                                                    "df": 1
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         }
@@ -2322,15 +2284,15 @@
                         "parsetypes.TypeParser.parse_none": {
                             "tf": 4.47213595499958
                         },
                         "parsetypes.TypeParser.parse_bool": {
                             "tf": 4.47213595499958
                         },
                         "parsetypes.TypeParser.parse_int": {
-                            "tf": 6.244997998398398
+                            "tf": 8.54400374531753
                         },
                         "parsetypes.TypeParser.parse_float": {
                             "tf": 8.54400374531753
                         },
                         "parsetypes.TypeParser.parse_decimal": {
                             "tf": 8.774964387392123
                         },
@@ -2356,20 +2318,17 @@
                             "tf": 8.888194417315589
                         },
                         "parsetypes.TypeParser.iterate_table": {
                             "tf": 8.660254037844387
                         },
                         "parsetypes.reduce_types": {
                             "tf": 11.489125293076057
-                        },
-                        "parsetypes.Nullable.__init__": {
-                            "tf": 2
                         }
                     },
-                    "df": 21,
+                    "df": 20,
                     "t": {
                         "docs": {},
                         "df": 0,
                         "r": {
                             "docs": {},
                             "df": 0,
                             "i": {
@@ -2398,15 +2357,15 @@
                                         "parsetypes.TypeParser.is_float": {
                                             "tf": 1.7320508075688772
                                         },
                                         "parsetypes.TypeParser.is_decimal": {
                                             "tf": 1.7320508075688772
                                         },
                                         "parsetypes.TypeParser.parse_int": {
-                                            "tf": 1
+                                            "tf": 1.7320508075688772
                                         },
                                         "parsetypes.TypeParser.parse_float": {
                                             "tf": 1.7320508075688772
                                         },
                                         "parsetypes.TypeParser.parse_decimal": {
                                             "tf": 1.7320508075688772
                                         }
@@ -2527,15 +2486,15 @@
                                         "parsetypes.TypeParser.is_decimal": {
                                             "tf": 2
                                         },
                                         "parsetypes.TypeParser.parse_bool": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_int": {
-                                            "tf": 1
+                                            "tf": 1.7320508075688772
                                         },
                                         "parsetypes.TypeParser.parse_float": {
                                             "tf": 1.7320508075688772
                                         },
                                         "parsetypes.TypeParser.parse_decimal": {
                                             "tf": 1.7320508075688772
                                         },
@@ -3094,17 +3053,20 @@
                             "g": {
                                 "docs": {},
                                 "df": 0,
                                 "n": {
                                     "docs": {
                                         "parsetypes.TypeParser.is_int": {
                                             "tf": 1
+                                        },
+                                        "parsetypes.TypeParser.parse_int": {
+                                            "tf": 1
                                         }
                                     },
-                                    "df": 1
+                                    "df": 2
                                 }
                             }
                         },
                         "c": {
                             "docs": {},
                             "df": 0,
                             "i": {
@@ -3268,17 +3230,20 @@
                                             "v": {
                                                 "docs": {},
                                                 "df": 0,
                                                 "e": {
                                                     "docs": {
                                                         "parsetypes.TypeParser.is_int": {
                                                             "tf": 1
+                                                        },
+                                                        "parsetypes.TypeParser.parse_int": {
+                                                            "tf": 1
                                                         }
                                                     },
-                                                    "df": 1
+                                                    "df": 2
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         },
@@ -3609,15 +3574,15 @@
                                             "parsetypes.TypeParser.is_float": {
                                                 "tf": 1.7320508075688772
                                             },
                                             "parsetypes.TypeParser.is_decimal": {
                                                 "tf": 1.7320508075688772
                                             },
                                             "parsetypes.TypeParser.parse_int": {
-                                                "tf": 1
+                                                "tf": 1.7320508075688772
                                             },
                                             "parsetypes.TypeParser.parse_float": {
                                                 "tf": 1.7320508075688772
                                             },
                                             "parsetypes.TypeParser.parse_decimal": {
                                                 "tf": 1.7320508075688772
                                             }
@@ -4118,30 +4083,30 @@
                         "parsetypes.TypeParser.is_none": {
                             "tf": 9.38083151964686
                         },
                         "parsetypes.TypeParser.is_bool": {
                             "tf": 10.677078252031311
                         },
                         "parsetypes.TypeParser.is_int": {
-                            "tf": 12.36931687685298
+                            "tf": 12.489995996796797
                         },
                         "parsetypes.TypeParser.is_float": {
                             "tf": 13.228756555322953
                         },
                         "parsetypes.TypeParser.is_decimal": {
                             "tf": 2.23606797749979
                         },
                         "parsetypes.TypeParser.parse_none": {
                             "tf": 9.797958971132712
                         },
                         "parsetypes.TypeParser.parse_bool": {
                             "tf": 10.198039027185569
                         },
                         "parsetypes.TypeParser.parse_int": {
-                            "tf": 11.704699910719626
+                            "tf": 12.36931687685298
                         },
                         "parsetypes.TypeParser.parse_float": {
                             "tf": 14.696938456699069
                         },
                         "parsetypes.TypeParser.parse_decimal": {
                             "tf": 14.798648586948742
                         },
@@ -4170,20 +4135,17 @@
                             "tf": 15.524174696260024
                         },
                         "parsetypes.reduce_types": {
                             "tf": 9.433981132056603
                         },
                         "parsetypes.Nullable": {
                             "tf": 4.242640687119285
-                        },
-                        "parsetypes.Nullable.__init__": {
-                            "tf": 1.7320508075688772
                         }
                     },
-                    "df": 24,
+                    "df": 23,
                     "t": {
                         "docs": {},
                         "df": 0,
                         "h": {
                             "docs": {},
                             "df": 0,
                             "i": {
@@ -4199,23 +4161,29 @@
                                         },
                                         "parsetypes.TypeParser.is_none": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.is_bool": {
                                             "tf": 1
                                         },
+                                        "parsetypes.TypeParser.is_int": {
+                                            "tf": 1
+                                        },
                                         "parsetypes.TypeParser.is_float": {
                                             "tf": 1.7320508075688772
                                         },
                                         "parsetypes.TypeParser.parse_none": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_bool": {
                                             "tf": 1
                                         },
+                                        "parsetypes.TypeParser.parse_int": {
+                                            "tf": 1
+                                        },
                                         "parsetypes.TypeParser.parse_float": {
                                             "tf": 1.4142135623730951
                                         },
                                         "parsetypes.TypeParser.parse_decimal": {
                                             "tf": 1.4142135623730951
                                         },
                                         "parsetypes.TypeParser.parse_table": {
@@ -4227,15 +4195,15 @@
                                         "parsetypes.reduce_types": {
                                             "tf": 1
                                         },
                                         "parsetypes.Nullable": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 13
+                                    "df": 15
                                 }
                             },
                             "e": {
                                 "docs": {
                                     "parsetypes": {
                                         "tf": 1
                                     },
@@ -4248,27 +4216,27 @@
                                     "parsetypes.TypeParser.is_none": {
                                         "tf": 2
                                     },
                                     "parsetypes.TypeParser.is_bool": {
                                         "tf": 1.7320508075688772
                                     },
                                     "parsetypes.TypeParser.is_int": {
-                                        "tf": 2.23606797749979
+                                        "tf": 2.449489742783178
                                     },
                                     "parsetypes.TypeParser.is_float": {
                                         "tf": 3
                                     },
                                     "parsetypes.TypeParser.parse_none": {
                                         "tf": 2
                                     },
                                     "parsetypes.TypeParser.parse_bool": {
                                         "tf": 1.7320508075688772
                                     },
                                     "parsetypes.TypeParser.parse_int": {
-                                        "tf": 2.449489742783178
+                                        "tf": 2.6457513110645907
                                     },
                                     "parsetypes.TypeParser.parse_float": {
                                         "tf": 3.1622776601683795
                                     },
                                     "parsetypes.TypeParser.parse_decimal": {
                                         "tf": 3.1622776601683795
                                     },
@@ -4371,15 +4339,15 @@
                                         "parsetypes.TypeParser.parse_none": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_bool": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_int": {
-                                            "tf": 1
+                                            "tf": 1.4142135623730951
                                         },
                                         "parsetypes.TypeParser.parse_float": {
                                             "tf": 2.23606797749979
                                         },
                                         "parsetypes.TypeParser.parse_decimal": {
                                             "tf": 2.23606797749979
                                         },
@@ -4423,27 +4391,27 @@
                                 "parsetypes.TypeParser.is_none": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.is_bool": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.is_int": {
-                                    "tf": 2.23606797749979
+                                    "tf": 2.449489742783178
                                 },
                                 "parsetypes.TypeParser.is_float": {
                                     "tf": 2
                                 },
                                 "parsetypes.TypeParser.parse_none": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_bool": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_int": {
-                                    "tf": 2
+                                    "tf": 2.6457513110645907
                                 },
                                 "parsetypes.TypeParser.parse_float": {
                                     "tf": 2.6457513110645907
                                 },
                                 "parsetypes.TypeParser.parse_decimal": {
                                     "tf": 2.6457513110645907
                                 },
@@ -4768,24 +4736,24 @@
                                         "parsetypes.TypeParser.is_none": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.is_bool": {
                                             "tf": 2.23606797749979
                                         },
                                         "parsetypes.TypeParser.is_int": {
-                                            "tf": 1.7320508075688772
+                                            "tf": 2
                                         },
                                         "parsetypes.TypeParser.is_float": {
                                             "tf": 2.449489742783178
                                         },
                                         "parsetypes.TypeParser.parse_bool": {
                                             "tf": 2
                                         },
                                         "parsetypes.TypeParser.parse_int": {
-                                            "tf": 1.4142135623730951
+                                            "tf": 1.7320508075688772
                                         },
                                         "parsetypes.TypeParser.parse_float": {
                                             "tf": 2
                                         },
                                         "parsetypes.TypeParser.parse_decimal": {
                                             "tf": 2
                                         },
@@ -5232,22 +5200,25 @@
                                                             },
                                                             "parsetypes.TypeParser.is_int": {
                                                                 "tf": 1
                                                             },
                                                             "parsetypes.TypeParser.is_float": {
                                                                 "tf": 1
                                                             },
+                                                            "parsetypes.TypeParser.parse_int": {
+                                                                "tf": 1
+                                                            },
                                                             "parsetypes.TypeParser.parse_float": {
                                                                 "tf": 1
                                                             },
                                                             "parsetypes.TypeParser.parse_decimal": {
                                                                 "tf": 1
                                                             }
                                                         },
-                                                        "df": 5
+                                                        "df": 6
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
@@ -5361,16 +5332,19 @@
                                     },
                                     "parsetypes.TypeParser": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.__init__": {
                                         "tf": 2.23606797749979
                                     },
+                                    "parsetypes.TypeParser.is_int": {
+                                        "tf": 1
+                                    },
                                     "parsetypes.TypeParser.parse_int": {
-                                        "tf": 1.4142135623730951
+                                        "tf": 1.7320508075688772
                                     },
                                     "parsetypes.TypeParser.parse_float": {
                                         "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.parse_decimal": {
                                         "tf": 1.4142135623730951
                                     },
@@ -5392,15 +5366,15 @@
                                     "parsetypes.TypeParser.parse_table": {
                                         "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.iterate_table": {
                                         "tf": 1.7320508075688772
                                     }
                                 },
-                                "df": 13,
+                                "df": 14,
                                 "m": {
                                     "docs": {
                                         "parsetypes.TypeParser.is_int": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.is_float": {
                                             "tf": 1
@@ -5528,15 +5502,15 @@
                                             "parsetypes.TypeParser.parse_none": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.parse_bool": {
                                                 "tf": 2.23606797749979
                                             },
                                             "parsetypes.TypeParser.parse_int": {
-                                                "tf": 1
+                                                "tf": 1.7320508075688772
                                             },
                                             "parsetypes.TypeParser.parse_float": {
                                                 "tf": 1.7320508075688772
                                             },
                                             "parsetypes.TypeParser.parse_decimal": {
                                                 "tf": 1.7320508075688772
                                             },
@@ -5728,17 +5702,23 @@
                                         "n": {
                                             "docs": {},
                                             "df": 0,
                                             "g": {
                                                 "docs": {
                                                     "parsetypes.TypeParser.__init__": {
                                                         "tf": 1
+                                                    },
+                                                    "parsetypes.TypeParser.is_int": {
+                                                        "tf": 1
+                                                    },
+                                                    "parsetypes.TypeParser.parse_int": {
+                                                        "tf": 1
                                                     }
                                                 },
-                                                "df": 1,
+                                                "df": 3,
                                                 "s": {
                                                     "docs": {
                                                         "parsetypes": {
                                                             "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.__init__": {
                                                             "tf": 1
@@ -6253,32 +6233,50 @@
                                 "df": 0,
                                 "n": {
                                     "docs": {
                                         "parsetypes.TypeParser.__init__": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.is_int": {
-                                            "tf": 1.4142135623730951
+                                            "tf": 2
                                         },
                                         "parsetypes.TypeParser.is_float": {
                                             "tf": 1
                                         },
+                                        "parsetypes.TypeParser.parse_int": {
+                                            "tf": 2
+                                        },
                                         "parsetypes.TypeParser.parse_float": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_decimal": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 5
+                                    "df": 6
                                 }
                             },
                             "n": {
                                 "docs": {},
                                 "df": 0,
+                                "c": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "e": {
+                                        "docs": {
+                                            "parsetypes.TypeParser.is_int": {
+                                                "tf": 1
+                                            },
+                                            "parsetypes.TypeParser.parse_int": {
+                                                "tf": 1
+                                            }
+                                        },
+                                        "df": 2
+                                    }
+                                },
                                 "g": {
                                     "docs": {},
                                     "df": 0,
                                     "l": {
                                         "docs": {},
                                         "df": 0,
                                         "e": {
@@ -6588,34 +6586,40 @@
                                                 "docs": {
                                                     "parsetypes.TypeParser.is_none": {
                                                         "tf": 1.4142135623730951
                                                     },
                                                     "parsetypes.TypeParser.is_bool": {
                                                         "tf": 1.4142135623730951
                                                     },
+                                                    "parsetypes.TypeParser.is_int": {
+                                                        "tf": 1
+                                                    },
                                                     "parsetypes.TypeParser.is_float": {
                                                         "tf": 2
                                                     },
                                                     "parsetypes.TypeParser.parse_none": {
                                                         "tf": 1.4142135623730951
                                                     },
                                                     "parsetypes.TypeParser.parse_bool": {
                                                         "tf": 1.4142135623730951
                                                     },
+                                                    "parsetypes.TypeParser.parse_int": {
+                                                        "tf": 1
+                                                    },
                                                     "parsetypes.TypeParser.parse_float": {
                                                         "tf": 2
                                                     },
                                                     "parsetypes.TypeParser.parse_decimal": {
                                                         "tf": 2
                                                     },
                                                     "parsetypes.TypeParser.parse_table": {
                                                         "tf": 1
                                                     }
                                                 },
-                                                "df": 8
+                                                "df": 10
                                             }
                                         }
                                     }
                                 }
                             },
                             "p": {
                                 "docs": {},
@@ -8354,17 +8358,20 @@
                                                 "e": {
                                                     "docs": {},
                                                     "df": 0,
                                                     "r": {
                                                         "docs": {
                                                             "parsetypes.TypeParser.is_int": {
                                                                 "tf": 1
+                                                            },
+                                                            "parsetypes.TypeParser.parse_int": {
+                                                                "tf": 1
                                                             }
                                                         },
-                                                        "df": 1
+                                                        "df": 2
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
@@ -9038,14 +9045,41 @@
                                                             },
                                                             "df": 5
                                                         }
                                                     }
                                                 }
                                             }
                                         }
+                                    },
+                                    "c": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "a": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "t": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "e": {
+                                                    "docs": {},
+                                                    "df": 0,
+                                                    "d": {
+                                                        "docs": {
+                                                            "parsetypes.TypeParser.is_int": {
+                                                                "tf": 1
+                                                            },
+                                                            "parsetypes.TypeParser.parse_int": {
+                                                                "tf": 1
+                                                            }
+                                                        },
+                                                        "df": 2
+                                                    }
+                                                }
+                                            }
+                                        }
                                     }
                                 }
                             },
                             "c": {
                                 "docs": {},
                                 "df": 0,
                                 "l": {
@@ -9094,30 +9128,30 @@
                                 "parsetypes.TypeParser.is_none": {
                                     "tf": 2
                                 },
                                 "parsetypes.TypeParser.is_bool": {
                                     "tf": 2.23606797749979
                                 },
                                 "parsetypes.TypeParser.is_int": {
-                                    "tf": 2.8284271247461903
+                                    "tf": 3
                                 },
                                 "parsetypes.TypeParser.is_float": {
                                     "tf": 3.1622776601683795
                                 },
                                 "parsetypes.TypeParser.is_decimal": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_none": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_bool": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_int": {
-                                    "tf": 1.4142135623730951
+                                    "tf": 2
                                 },
                                 "parsetypes.TypeParser.parse_float": {
                                     "tf": 2
                                 },
                                 "parsetypes.TypeParser.parse_decimal": {
                                     "tf": 2
                                 },
@@ -9210,15 +9244,15 @@
                                 "parsetypes.TypeParser.parse_none": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_bool": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_int": {
-                                    "tf": 1.4142135623730951
+                                    "tf": 1.7320508075688772
                                 },
                                 "parsetypes.TypeParser.parse_float": {
                                     "tf": 1.7320508075688772
                                 },
                                 "parsetypes.TypeParser.parse_decimal": {
                                     "tf": 1.7320508075688772
                                 },
@@ -9313,15 +9347,15 @@
                                 "parsetypes.TypeParser.parse_none": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.TypeParser.parse_bool": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.TypeParser.parse_int": {
-                                    "tf": 2
+                                    "tf": 2.23606797749979
                                 },
                                 "parsetypes.TypeParser.parse_float": {
                                     "tf": 2.8284271247461903
                                 },
                                 "parsetypes.TypeParser.parse_decimal": {
                                     "tf": 2.8284271247461903
                                 },
@@ -9367,17 +9401,20 @@
                                         "e": {
                                             "docs": {},
                                             "df": 0,
                                             "s": {
                                                 "docs": {
                                                     "parsetypes.TypeParser.is_int": {
                                                         "tf": 1
+                                                    },
+                                                    "parsetypes.TypeParser.parse_int": {
+                                                        "tf": 1
                                                     }
                                                 },
-                                                "df": 1
+                                                "df": 2
                                             }
                                         }
                                     }
                                 }
                             }
                         }
                     },
@@ -9395,27 +9432,27 @@
                             "parsetypes.TypeParser.is_none": {
                                 "tf": 1
                             },
                             "parsetypes.TypeParser.is_bool": {
                                 "tf": 1.7320508075688772
                             },
                             "parsetypes.TypeParser.is_int": {
-                                "tf": 1.7320508075688772
+                                "tf": 2
                             },
                             "parsetypes.TypeParser.is_float": {
                                 "tf": 2.449489742783178
                             },
                             "parsetypes.TypeParser.parse_none": {
                                 "tf": 1
                             },
                             "parsetypes.TypeParser.parse_bool": {
                                 "tf": 1.4142135623730951
                             },
                             "parsetypes.TypeParser.parse_int": {
-                                "tf": 1.7320508075688772
+                                "tf": 2.23606797749979
                             },
                             "parsetypes.TypeParser.parse_float": {
                                 "tf": 2.449489742783178
                             },
                             "parsetypes.TypeParser.parse_decimal": {
                                 "tf": 2.449489742783178
                             },
@@ -9533,19 +9570,25 @@
                                 "df": 16
                             },
                             "y": {
                                 "docs": {
                                     "parsetypes.TypeParser.__init__": {
                                         "tf": 1.4142135623730951
                                     },
+                                    "parsetypes.TypeParser.is_int": {
+                                        "tf": 1
+                                    },
+                                    "parsetypes.TypeParser.parse_int": {
+                                        "tf": 1
+                                    },
                                     "parsetypes.TypeParser.convert": {
                                         "tf": 1
                                     }
                                 },
-                                "df": 2
+                                "df": 4
                             },
                             "a": {
                                 "docs": {},
                                 "df": 0,
                                 "l": {
                                     "docs": {},
                                     "df": 0,
@@ -9843,37 +9886,43 @@
                                     },
                                     "parsetypes.TypeParser.is_none": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.is_bool": {
                                         "tf": 1
                                     },
+                                    "parsetypes.TypeParser.is_int": {
+                                        "tf": 1
+                                    },
                                     "parsetypes.TypeParser.is_float": {
                                         "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.parse_none": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_bool": {
                                         "tf": 1
                                     },
+                                    "parsetypes.TypeParser.parse_int": {
+                                        "tf": 1
+                                    },
                                     "parsetypes.TypeParser.parse_float": {
                                         "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.parse_decimal": {
                                         "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.parse_table": {
                                         "tf": 1
                                     },
                                     "parsetypes.reduce_types": {
                                         "tf": 1
                                     }
                                 },
-                                "df": 10
+                                "df": 12
                             }
                         },
                         "p": {
                             "docs": {},
                             "df": 0,
                             "p": {
                                 "docs": {},
@@ -10007,49 +10056,58 @@
                                     "y": {
                                         "docs": {},
                                         "df": 0,
                                         "s": {
                                             "docs": {
                                                 "parsetypes.TypeParser.__init__": {
                                                     "tf": 1
+                                                },
+                                                "parsetypes.TypeParser.is_int": {
+                                                    "tf": 1
+                                                },
+                                                "parsetypes.TypeParser.parse_int": {
+                                                    "tf": 1
                                                 }
                                             },
-                                            "df": 1
+                                            "df": 3
                                         }
                                     }
                                 }
                             },
                             "s": {
                                 "docs": {},
                                 "df": 0,
                                 "o": {
                                     "docs": {
                                         "parsetypes.TypeParser.__init__": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.is_int": {
-                                            "tf": 1
+                                            "tf": 1.4142135623730951
                                         },
                                         "parsetypes.TypeParser.is_float": {
                                             "tf": 1.4142135623730951
                                         },
+                                        "parsetypes.TypeParser.parse_int": {
+                                            "tf": 1.4142135623730951
+                                        },
                                         "parsetypes.TypeParser.parse_float": {
                                             "tf": 1.4142135623730951
                                         },
                                         "parsetypes.TypeParser.parse_decimal": {
                                             "tf": 1.4142135623730951
                                         },
                                         "parsetypes.TypeParser.infer": {
                                             "tf": 1
                                         },
                                         "parsetypes.Nullable": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 7
+                                    "df": 8
                                 }
                             },
                             "l": {
                                 "docs": {
                                     "parsetypes.TypeParser.__init__": {
                                         "tf": 1.4142135623730951
                                     },
@@ -10075,21 +10133,21 @@
                                 "df": 7,
                                 "o": {
                                     "docs": {},
                                     "df": 0,
                                     "w": {
                                         "docs": {
                                             "parsetypes.TypeParser.is_int": {
-                                                "tf": 2
+                                                "tf": 2.23606797749979
                                             },
                                             "parsetypes.TypeParser.is_float": {
                                                 "tf": 1.7320508075688772
                                             },
                                             "parsetypes.TypeParser.parse_int": {
-                                                "tf": 1
+                                                "tf": 2.23606797749979
                                             },
                                             "parsetypes.TypeParser.parse_float": {
                                                 "tf": 1.7320508075688772
                                             },
                                             "parsetypes.TypeParser.parse_decimal": {
                                                 "tf": 1.7320508075688772
                                             }
@@ -10207,15 +10265,15 @@
                                                 "parsetypes.TypeParser.is_int": {
                                                     "tf": 1.7320508075688772
                                                 },
                                                 "parsetypes.TypeParser.is_float": {
                                                     "tf": 1.7320508075688772
                                                 },
                                                 "parsetypes.TypeParser.parse_int": {
-                                                    "tf": 1
+                                                    "tf": 1.7320508075688772
                                                 },
                                                 "parsetypes.TypeParser.parse_float": {
                                                     "tf": 1.7320508075688772
                                                 },
                                                 "parsetypes.TypeParser.parse_decimal": {
                                                     "tf": 1.7320508075688772
                                                 },
@@ -10383,27 +10441,27 @@
                                 "parsetypes.TypeParser.is_none": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.TypeParser.is_bool": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.TypeParser.is_int": {
-                                    "tf": 2
+                                    "tf": 2.23606797749979
                                 },
                                 "parsetypes.TypeParser.is_float": {
                                     "tf": 2
                                 },
                                 "parsetypes.TypeParser.parse_none": {
                                     "tf": 1.7320508075688772
                                 },
                                 "parsetypes.TypeParser.parse_bool": {
                                     "tf": 1.7320508075688772
                                 },
                                 "parsetypes.TypeParser.parse_int": {
-                                    "tf": 2.449489742783178
+                                    "tf": 2.6457513110645907
                                 },
                                 "parsetypes.TypeParser.parse_float": {
                                     "tf": 2.6457513110645907
                                 },
                                 "parsetypes.TypeParser.parse_decimal": {
                                     "tf": 2.6457513110645907
                                 },
@@ -10627,18 +10685,21 @@
                                         "parsetypes": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.__init__": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.is_int": {
-                                            "tf": 1
+                                            "tf": 1.4142135623730951
+                                        },
+                                        "parsetypes.TypeParser.parse_int": {
+                                            "tf": 1.4142135623730951
                                         }
                                     },
-                                    "df": 3
+                                    "df": 4
                                 }
                             },
                             "l": {
                                 "docs": {},
                                 "df": 0,
                                 "l": {
                                     "docs": {
@@ -10727,15 +10788,15 @@
                                                     "parsetypes.TypeParser.is_int": {
                                                         "tf": 2
                                                     },
                                                     "parsetypes.TypeParser.is_float": {
                                                         "tf": 2
                                                     },
                                                     "parsetypes.TypeParser.parse_int": {
-                                                        "tf": 1
+                                                        "tf": 1.7320508075688772
                                                     },
                                                     "parsetypes.TypeParser.parse_float": {
                                                         "tf": 1.7320508075688772
                                                     },
                                                     "parsetypes.TypeParser.parse_decimal": {
                                                         "tf": 1.7320508075688772
                                                     },
@@ -10835,23 +10896,29 @@
                                             },
                                             "parsetypes.TypeParser.is_none": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.is_bool": {
                                                 "tf": 1
                                             },
+                                            "parsetypes.TypeParser.is_int": {
+                                                "tf": 1
+                                            },
                                             "parsetypes.TypeParser.is_float": {
                                                 "tf": 1.4142135623730951
                                             },
                                             "parsetypes.TypeParser.parse_none": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.parse_bool": {
                                                 "tf": 1
                                             },
+                                            "parsetypes.TypeParser.parse_int": {
+                                                "tf": 1
+                                            },
                                             "parsetypes.TypeParser.parse_float": {
                                                 "tf": 1.4142135623730951
                                             },
                                             "parsetypes.TypeParser.parse_decimal": {
                                                 "tf": 1.4142135623730951
                                             },
                                             "parsetypes.TypeParser.infer": {
@@ -10872,15 +10939,15 @@
                                             "parsetypes.TypeParser.iterate_table": {
                                                 "tf": 1
                                             },
                                             "parsetypes.Nullable": {
                                                 "tf": 1
                                             }
                                         },
-                                        "df": 15
+                                        "df": 17
                                     }
                                 }
                             }
                         },
                         "e": {
                             "docs": {},
                             "df": 0,
@@ -11300,14 +11367,41 @@
                                             }
                                         },
                                         "df": 5
                                     }
                                 }
                             }
                         },
+                        "f": {
+                            "docs": {},
+                            "df": 0,
+                            "f": {
+                                "docs": {},
+                                "df": 0,
+                                "e": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "c": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "t": {
+                                            "docs": {
+                                                "parsetypes.TypeParser.is_int": {
+                                                    "tf": 1
+                                                },
+                                                "parsetypes.TypeParser.parse_int": {
+                                                    "tf": 1
+                                                }
+                                            },
+                                            "df": 2
+                                        }
+                                    }
+                                }
+                            }
+                        },
                         "v": {
                             "docs": {},
                             "df": 0,
                             "e": {
                                 "docs": {},
                                 "df": 0,
                                 "n": {
@@ -11738,21 +11832,21 @@
                                                 "df": 0,
                                                 "e": {
                                                     "docs": {
                                                         "parsetypes.TypeParser.__init__": {
                                                             "tf": 1.4142135623730951
                                                         },
                                                         "parsetypes.TypeParser.is_int": {
-                                                            "tf": 2
+                                                            "tf": 2.449489742783178
                                                         },
                                                         "parsetypes.TypeParser.is_float": {
                                                             "tf": 2
                                                         },
                                                         "parsetypes.TypeParser.parse_int": {
-                                                            "tf": 1
+                                                            "tf": 2.449489742783178
                                                         },
                                                         "parsetypes.TypeParser.parse_float": {
                                                             "tf": 2
                                                         },
                                                         "parsetypes.TypeParser.parse_decimal": {
                                                             "tf": 2
                                                         }
@@ -12080,25 +12174,28 @@
                                                 "parsetypes.TypeParser.is_none": {
                                                     "tf": 1.7320508075688772
                                                 },
                                                 "parsetypes.TypeParser.is_bool": {
                                                     "tf": 2
                                                 },
                                                 "parsetypes.TypeParser.is_int": {
-                                                    "tf": 1.4142135623730951
+                                                    "tf": 1.7320508075688772
                                                 },
                                                 "parsetypes.TypeParser.is_float": {
                                                     "tf": 2.23606797749979
                                                 },
                                                 "parsetypes.TypeParser.parse_none": {
                                                     "tf": 1.7320508075688772
                                                 },
                                                 "parsetypes.TypeParser.parse_bool": {
                                                     "tf": 2
                                                 },
+                                                "parsetypes.TypeParser.parse_int": {
+                                                    "tf": 1.7320508075688772
+                                                },
                                                 "parsetypes.TypeParser.parse_float": {
                                                     "tf": 2.6457513110645907
                                                 },
                                                 "parsetypes.TypeParser.parse_decimal": {
                                                     "tf": 2.6457513110645907
                                                 },
                                                 "parsetypes.TypeParser.infer_series": {
@@ -12119,15 +12216,15 @@
                                                 "parsetypes.TypeParser.iterate_table": {
                                                     "tf": 1.7320508075688772
                                                 },
                                                 "parsetypes.reduce_types": {
                                                     "tf": 1
                                                 }
                                             },
-                                            "df": 17
+                                            "df": 18
                                         },
                                         "e": {
                                             "docs": {},
                                             "df": 0,
                                             "r": {
                                                 "docs": {},
                                                 "df": 0,
@@ -12383,21 +12480,21 @@
                             },
                             "s": {
                                 "docs": {},
                                 "df": 0,
                                 "t": {
                                     "docs": {
                                         "parsetypes.TypeParser.is_int": {
-                                            "tf": 1.4142135623730951
+                                            "tf": 1.7320508075688772
                                         },
                                         "parsetypes.TypeParser.is_float": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_int": {
-                                            "tf": 1.4142135623730951
+                                            "tf": 1.7320508075688772
                                         },
                                         "parsetypes.TypeParser.parse_float": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_decimal": {
                                             "tf": 1
                                         },
@@ -12924,45 +13021,31 @@
                                             }
                                         }
                                     }
                                 }
                             }
                         }
                     },
-                    "x": {
-                        "docs": {
-                            "parsetypes.TypeParser.is_int": {
-                                "tf": 2
-                            },
-                            "parsetypes.TypeParser.is_float": {
-                                "tf": 2
-                            },
-                            "parsetypes.TypeParser.parse_int": {
-                                "tf": 2
-                            },
-                            "parsetypes.TypeParser.parse_float": {
-                                "tf": 2
-                            },
-                            "parsetypes.TypeParser.parse_decimal": {
-                                "tf": 2
-                            }
-                        },
-                        "df": 5
-                    },
                     "h": {
                         "docs": {},
                         "df": 0,
                         "a": {
                             "docs": {},
                             "df": 0,
                             "v": {
                                 "docs": {},
                                 "df": 0,
                                 "e": {
                                     "docs": {
+                                        "parsetypes.TypeParser.is_int": {
+                                            "tf": 1
+                                        },
+                                        "parsetypes.TypeParser.parse_int": {
+                                            "tf": 1
+                                        },
                                         "parsetypes.TypeParser.infer_series": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.infer_table": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_series": {
@@ -12974,15 +13057,15 @@
                                         "parsetypes.TypeParser.iterate_table": {
                                             "tf": 1
                                         },
                                         "parsetypes.reduce_types": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 6
+                                    "df": 8
                                 }
                             }
                         },
                         "o": {
                             "docs": {},
                             "df": 0,
                             "w": {
@@ -13010,14 +13093,34 @@
                                             }
                                         }
                                     }
                                 }
                             }
                         }
                     },
+                    "x": {
+                        "docs": {
+                            "parsetypes.TypeParser.is_int": {
+                                "tf": 2
+                            },
+                            "parsetypes.TypeParser.is_float": {
+                                "tf": 2
+                            },
+                            "parsetypes.TypeParser.parse_int": {
+                                "tf": 2
+                            },
+                            "parsetypes.TypeParser.parse_float": {
+                                "tf": 2
+                            },
+                            "parsetypes.TypeParser.parse_decimal": {
+                                "tf": 2
+                            }
+                        },
+                        "df": 5
+                    },
                     "y": {
                         "docs": {},
                         "df": 0,
                         "i": {
                             "docs": {},
                             "df": 0,
                             "e": {
```

### Comparing `parsetypes-0.3/pyproject.toml` & `parsetypes-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parsetypes-0.3/src/parsetypes/__init__.py` & `parsetypes-0.3.1/src/parsetypes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 	The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:
 	- treat `inf` as either a float or a normal string
 	- give exact Decimal values instead of floats
 	- detect inline lists
 """
 
 
-__version__ = "0.3"
+__version__ = "0.3.1"
 
 from ._common import AnyScalar, AnyScalarType, AnyValue, AnyValueType, GenericValue, Nullable
 from ._parser import TypeParser
 from ._reduce_types import reduce_types
 
 __all__ = ('TypeParser', 'reduce_types', 'Nullable')
```

### Comparing `parsetypes-0.3/src/parsetypes/_common.py` & `parsetypes-0.3.1/src/parsetypes/_common.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.3/src/parsetypes/_parser.py` & `parsetypes-0.3.1/src/parsetypes/_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -538,15 +538,15 @@
 			`value`
 			: string to be checked
 
 			Keyword arguments
 			-----------------
 
 			`allow_negative`
-			: whether to accept negative values
+			: whether to accept negative values. Since negative values are always indicated with a negative sign, `allow_sign` must also be True (which is the default setting) for this to have any effect.
 
 			`allow_sign`
 			: whether to accept values prepended with a sign character. If False, it implies that `allow_negative` is False also.
 
 			`allow_scientific`
 			: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var> must be an integer and <var>X</var> must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.
 
@@ -757,28 +757,34 @@
 			return True
 		if special_value in self._match_false_values:
 			return False
 
 		raise ValueError(f"not a boolean: {value}")
 
 
-	def parse_int(self, value: str, *, allow_scientific: bool=True) -> int:
+	def parse_int(self, value: str, *, allow_negative: bool=True, allow_sign: bool=True, allow_scientific: bool=True) -> int:
 		"""
 			Parse a string and return it as an int if possible
 
 			If the string represents a bool, it will be converted to `1` for True and `0` for False.
 
 			Arguments
 			---------
 			`value`
 			: string to be parsed
 
 			Keyword arguments
 			-----------------
 
+			`allow_negative`
+			: whether to accept negative values. Since negative values are always indicated with a negative sign, `allow_sign` must also be True (which is the default setting) for this to have any effect.
+
+			`allow_sign`
+			: whether to accept values prepended with a sign character. If False, it implies that `allow_negative` is False also.
+
 			`allow_scientific`
 			: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var> must be an integer and <var>X</var> must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.
 
 			Returns
 			-------
 			parsed int value
 
@@ -794,15 +800,15 @@
 			parser.parse_int("-1")   # -1
 			parser.parse_int("2e3")  # 2000
 			```
 		"""
 		if self._trim:
 			value = value.strip()
 
-		if self.is_int(value, allow_sign=True, allow_negative=True, allow_scientific=allow_scientific):
+		if self.is_int(value, allow_negative=allow_negative, allow_sign=allow_sign, allow_scientific=allow_scientific):
 			if allow_scientific:
 				value, exp = _decompose_string_pair(value, self._scientific_char, self._int_case_sensitive)
 				if exp is not None:
 					if value[0] in (self._negative_chars - {self._negative_char}):
 						value = self._negative_char + value[1:]
 					return int(value) * (10 ** int(exp))
```

### Comparing `parsetypes-0.3/src/parsetypes/_reduce_types.py` & `parsetypes-0.3.1/src/parsetypes/_reduce_types.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.3/src/parsetypes.egg-info/PKG-INFO` & `parsetypes-0.3.1/src/parsetypes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsetypes
-Version: 0.3
+Version: 0.3.1
 Summary: Parse serialised data to recover their original underlying types
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/parsetypes
 Project-URL: Documentation, https://parsetypes.gnayihs.uy/
 Project-URL: Issues, https://github.com/yushiyangk/parsetypes/issues
 Keywords: python,str,string,types,conversion
@@ -158,14 +158,18 @@
 
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>parsetypes ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>parsetypes ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
+### 0.3.1
+
+- Added the arguments `allow_negative` and `allow_sign` (both `True` by default) to <code><var>parser</var>.parse_int()</code>, for parity with <code><var>parser</var>.is_int()</code> which already had these arguments
+
 ### 0.3
 
 - Made the previously public but undocumented instance variables of TypeParser that corresponded to the constructor arguments private instead
 - Added public properties to TypeParser for accessing or modifying the same settings in a controlled manner
 
 ### 0.2.6
```

### Comparing `parsetypes-0.3/src/parsetypes.egg-info/SOURCES.txt` & `parsetypes-0.3.1/src/parsetypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parsetypes-0.3/tests/test_parser.py` & `parsetypes-0.3.1/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,63 +378,81 @@
 		else:
 			int_result = default_parser.parse_int(value)
 			assert int_result == (1 if expected_bool == True else 0)
 
 
 	@staticmethod
 	@pytest.mark.parametrize(
-		('value', 'is_int_allow_sign_expected', 'is_int_allow_negative_expected', 'is_int_allow_both_expected', 'expected_int'),
+		('value', 'is_int_allow_sign_expected', 'is_int_allow_negative_expected', 'is_int_allow_both_expected', 'allow_sign_expected', 'allow_negative_expected', 'allow_both_expected'),
 		# All test cases expect False when both disallowed
 		[
-			("+0", True, False, True, 0),
-			("-0", False, False, True, 0),
-			("−0", False, False, True, 0),
-			("+1", True, False, True, 1),
-			("+20", True, False, True, 20),
-			("+03", True, False, True, 3),
-			("-4", False, False, True, -4),
-			("-50", False, False, True, -50),
-			("-06", False, False, True, -6),
-			("−7", False, False, True, -7),
-			("−80", False, False, True, -80),
-			("−09", False, False, True, -9),
-			("++10", False, False, False, None),
-			("--10", False, False, False, None),
-			("10+", False, False, False, None),
-			("10-", False, False, False, None),
-			("1+1", False, False, False, None),
-			("1-1", False, False, False, None),
-			("0+1", False, False, False, None),
-			("0-1", False, False, False, None),
+			("+0", True, False, True, 0, None, 0),
+			("-0", False, False, True, None, None, 0),
+			("−0", False, False, True, None, None, 0),
+			("+1", True, False, True, 1, None, 1),
+			("+20", True, False, True, 20, None, 20),
+			("+03", True, False, True, 3, None, 3),
+			("-4", False, False, True, None, None, -4),
+			("-50", False, False, True, None, None, -50),
+			("-06", False, False, True, None, None, -6),
+			("−7", False, False, True, None, None, -7),
+			("−80", False, False, True, None, None, -80),
+			("−09", False, False, True, None, None, -9),
+			("++10", False, False, False, None, None, None),
+			("--10", False, False, False, None, None, None),
+			("10+", False, False, False, None, None, None),
+			("10-", False, False, False, None, None, None),
+			("1+1", False, False, False, None, None, None),
+			("1-1", False, False, False, None, None, None),
+			("0+1", False, False, False, None, None, None),
+			("0-1", False, False, False, None, None, None),
 		]
 	)
 	def test_allow_sign_negative(
 		default_parser: TypeParser,
 		value: str,
 		is_int_allow_sign_expected: bool,
 		is_int_allow_negative_expected: bool,
 		is_int_allow_both_expected: bool,
-		expected_int: int
+		allow_sign_expected: int,
+		allow_negative_expected: int,
+		allow_both_expected: int,
 	):
 		is_int_allow_sign_result = default_parser.is_int(value, allow_sign=True, allow_negative=False)
 		assert is_int_allow_sign_result == is_int_allow_sign_expected
 		is_int_allow_negative_result = default_parser.is_int(value, allow_sign=False, allow_negative=True)
 		assert is_int_allow_negative_result == is_int_allow_negative_expected
 		is_int_allow_both_result = default_parser.is_int(value, allow_sign=True, allow_negative=True)
 		assert is_int_allow_both_result == is_int_allow_both_expected
+		is_int_allow_none_result = default_parser.is_int(value, allow_sign=False, allow_negative=False)
+		assert is_int_allow_none_result == False
 
-		is_int_disallow_negative_result = default_parser.is_int(value, allow_sign=False, allow_negative=False)
-		assert is_int_disallow_negative_result == False
+		if allow_sign_expected is None:
+			with pytest.raises(ValueError):
+				default_parser.parse_int(value, allow_sign=True, allow_negative=False)
+		else:
+			allow_sign_result = default_parser.parse_int(value, allow_sign=True, allow_negative=False)
+			assert allow_sign_result == allow_sign_expected
 
-		if expected_int is None:
+		if allow_negative_expected is None:
+			with pytest.raises(ValueError):
+				default_parser.parse_int(value, allow_sign=False, allow_negative=True)
+		else:
+			allow_negative_result = default_parser.parse_int(value, allow_sign=False, allow_negative=True)
+			assert allow_negative_result == allow_negative_expected
+
+		if allow_both_expected is None:
 			with pytest.raises(ValueError):
-				default_parser.parse_int(value)
+				default_parser.parse_int(value, allow_sign=True, allow_negative=True)
 		else:
-			result = default_parser.parse_int(value)
-			assert result == expected_int
+			allow_both_result = default_parser.parse_int(value, allow_sign=True, allow_negative=True)
+			assert allow_both_result == allow_both_expected
+
+		with pytest.raises(ValueError):
+			default_parser.parse_int(value, allow_sign=False, allow_negative=False)
 
 
 	@staticmethod
 	@pytest.mark.parametrize(
 		('value', 'is_int_allow_scientific_expected', 'allow_scientific_expected'),
 		# All test cases expect False when e disallowed
 		[
@@ -1708,16 +1726,16 @@
 
 class TestConstructorAndProperties:
 	@staticmethod
 	@pytest.mark.parametrize('list_delimiter', [',', '\n'])
 	@pytest.mark.parametrize('none_values', [[], [""], ["none", "n"]])
 	@pytest.mark.parametrize('true_values', [[], ["t", "tru"]])
 	@pytest.mark.parametrize('false_values', [[], ["f", "fa"]])
-	@pytest.mark.parametrize('inf_values', [['inf']])
-	@pytest.mark.parametrize('nan_values', [['nan']])
+	@pytest.mark.parametrize('inf_values', [["inf"]])
+	@pytest.mark.parametrize('nan_values', [["nan"]])
 	def test_args(
 		list_delimiter: str,
 		none_values: list[str],
 		true_values: list[str],
 		false_values: list[str],
 		inf_values: list[str],
 		nan_values: list[str],
```

### Comparing `parsetypes-0.3/tests/test_reduce_types.py` & `parsetypes-0.3.1/tests/test_reduce_types.py`

 * *Files identical despite different names*

