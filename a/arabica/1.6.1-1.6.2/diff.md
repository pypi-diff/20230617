# Comparing `tmp/arabica-1.6.1.tar.gz` & `tmp/arabica-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabica-1.6.1.tar", last modified: Sat Jun 17 11:28:02 2023, max compression
+gzip compressed data, was "arabica-1.6.2.tar", last modified: Sat Jun 17 11:47:24 2023, max compression
```

## Comparing `arabica-1.6.1.tar` & `arabica-1.6.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 11:28:02.970941 arabica-1.6.1/
--rw-rw-rw-   0        0        0       11 2023-05-18 21:22:46.000000 arabica-1.6.1/LICENSE
--rw-rw-rw-   0        0        0     7777 2023-06-17 11:28:02.972055 arabica-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     7011 2023-06-17 11:19:31.000000 arabica-1.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 11:28:02.967045 arabica-1.6.1/arabica/
--rw-rw-rw-   0        0        0      105 2023-05-18 23:17:32.000000 arabica-1.6.1/arabica/__init__.py
--rw-rw-rw-   0        0        0    12483 2023-05-18 23:09:58.000000 arabica-1.6.1/arabica/arabica_freq.py
--rw-rw-rw-   0        0        0    30721 2023-05-19 20:32:49.000000 arabica-1.6.1/arabica/cappuccino.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.6.1/arabica/clean_ngram.py
--rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.6.1/arabica/clean_numbers.py
--rw-rw-rw-   0        0        0     8246 2023-06-17 08:04:35.000000 arabica-1.6.1/arabica/coffee_break.py
--rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.6.1/arabica/group.py
--rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.6.1/arabica/preprocess.py
--rw-rw-rw-   0        0        0      533 2023-06-17 08:02:21.000000 arabica-1.6.1/arabica/sentiment.py
--rw-rw-rw-   0        0        0     1118 2023-05-18 20:28:46.000000 arabica-1.6.1/arabica/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-06-17 11:28:02.970941 arabica-1.6.1/arabica.egg-info/
--rw-rw-rw-   0        0        0     7777 2023-06-17 11:28:02.000000 arabica-1.6.1/arabica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-06-17 11:28:02.000000 arabica-1.6.1/arabica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 11:28:02.000000 arabica-1.6.1/arabica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-06-17 11:28:02.000000 arabica-1.6.1/arabica.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-17 11:28:02.000000 arabica-1.6.1/arabica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      547 2023-06-17 11:25:22.000000 arabica-1.6.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-17 11:28:02.972055 arabica-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1111 2023-06-17 11:25:22.000000 arabica-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:47:24.333771 arabica-1.6.2/
+-rw-rw-rw-   0        0        0       11 2023-05-18 21:22:46.000000 arabica-1.6.2/LICENSE
+-rw-rw-rw-   0        0        0     7741 2023-06-17 11:47:24.333771 arabica-1.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6974 2023-06-17 11:44:35.000000 arabica-1.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 11:47:24.328769 arabica-1.6.2/arabica/
+-rw-rw-rw-   0        0        0      105 2023-05-18 23:17:32.000000 arabica-1.6.2/arabica/__init__.py
+-rw-rw-rw-   0        0        0    12483 2023-05-18 23:09:58.000000 arabica-1.6.2/arabica/arabica_freq.py
+-rw-rw-rw-   0        0        0    30721 2023-05-19 20:32:49.000000 arabica-1.6.2/arabica/cappuccino.py
+-rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.6.2/arabica/clean_ngram.py
+-rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.6.2/arabica/clean_numbers.py
+-rw-rw-rw-   0        0        0     8246 2023-06-17 08:04:35.000000 arabica-1.6.2/arabica/coffee_break.py
+-rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.6.2/arabica/group.py
+-rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.6.2/arabica/preprocess.py
+-rw-rw-rw-   0        0        0      533 2023-06-17 08:02:21.000000 arabica-1.6.2/arabica/sentiment.py
+-rw-rw-rw-   0        0        0     1118 2023-05-18 20:28:46.000000 arabica-1.6.2/arabica/stopwords.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:47:24.333771 arabica-1.6.2/arabica.egg-info/
+-rw-rw-rw-   0        0        0     7741 2023-06-17 11:47:24.000000 arabica-1.6.2/arabica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-06-17 11:47:24.000000 arabica-1.6.2/arabica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 11:47:24.000000 arabica-1.6.2/arabica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-06-17 11:47:24.000000 arabica-1.6.2/arabica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-17 11:47:24.000000 arabica-1.6.2/arabica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      547 2023-06-17 11:46:58.000000 arabica-1.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-17 11:47:24.334771 arabica-1.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1111 2023-06-17 11:46:58.000000 arabica-1.6.2/setup.py
```

### Comparing `arabica-1.6.1/PKG-INFO` & `arabica-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
@@ -41,15 +41,16 @@
 
 
 ## Installation
 
 Arabica requires [Python 3.8 - 3.10](https://www.python.org/downloads/), [NLTK](http://www.nltk.org) - stop words removal,
 [cleantext](https://pypi.org/project/cleantext/#description) - text cleaning, [wordcloud](https://pypi.org/project/wordcloud) - word cloud visualization,
 [plotnine](https://pypi.org/project/plotnine) - heatmaps and line graphs, [matplotlib](https://pypi.org/project/matplotlib/) - word clouds and graphical operations,
-[vaderSentiment](https://pypi.org/project/vaderSentiment) - sentiment analysis, and [jenskpy](https://pypi.org/project/jenkspy/) for breakpoint identification.
+[vaderSentiment](https://pypi.org/project/vaderSentiment) - sentiment analysis, [finvader](https://pypi.org/project/finvader) - financial sentiment analysis,
+and [jenskpy](https://pypi.org/project/jenkspy/) for breakpoint identification.
 
 To install using pip, use:
 
 `pip install arabica`
 
 
 
@@ -103,15 +104,15 @@
                lower_case: bool = False  # Lowercase text
 ```
 
 **coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. 
 
 The implemented models are:
 
-* **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See: *Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text.* Available from [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
+* **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. Available from [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
 
 * **FinVADER** improves VADER's classification accuracy, including two financial lexicons. Available from [here](https://pypi.org/project/finvader/).
 
 Structural breaks in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
 
 
 ``` python
```

### Comparing `arabica-1.6.1/README.md` & `arabica-1.6.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 
 
 ## Installation
 
 Arabica requires [Python 3.8 - 3.10](https://www.python.org/downloads/), [NLTK](http://www.nltk.org) - stop words removal,
 [cleantext](https://pypi.org/project/cleantext/#description) - text cleaning, [wordcloud](https://pypi.org/project/wordcloud) - word cloud visualization,
 [plotnine](https://pypi.org/project/plotnine) - heatmaps and line graphs, [matplotlib](https://pypi.org/project/matplotlib/) - word clouds and graphical operations,
-[vaderSentiment](https://pypi.org/project/vaderSentiment) - sentiment analysis, and [jenskpy](https://pypi.org/project/jenkspy/) for breakpoint identification.
+[vaderSentiment](https://pypi.org/project/vaderSentiment) - sentiment analysis, [finvader](https://pypi.org/project/finvader) - financial sentiment analysis,
+and [jenskpy](https://pypi.org/project/jenkspy/) for breakpoint identification.
 
 To install using pip, use:
 
 `pip install arabica`
 
 
 
@@ -86,15 +87,15 @@
                lower_case: bool = False  # Lowercase text
 ```
 
 **coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. 
 
 The implemented models are:
 
-* **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See: *Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text.* Available from [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
+* **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. Available from [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
 
 * **FinVADER** improves VADER's classification accuracy, including two financial lexicons. Available from [here](https://pypi.org/project/finvader/).
 
 Structural breaks in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
 
 
 ``` python
```

### Comparing `arabica-1.6.1/arabica/arabica_freq.py` & `arabica-1.6.2/arabica/arabica_freq.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.1/arabica/cappuccino.py` & `arabica-1.6.2/arabica/cappuccino.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.1/arabica/clean_ngram.py` & `arabica-1.6.2/arabica/clean_ngram.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.1/arabica/coffee_break.py` & `arabica-1.6.2/arabica/coffee_break.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.1/arabica/group.py` & `arabica-1.6.2/arabica/group.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.1/arabica/preprocess.py` & `arabica-1.6.2/arabica/preprocess.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.1/arabica/sentiment.py` & `arabica-1.6.2/arabica/sentiment.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.1/arabica/stopwords.py` & `arabica-1.6.2/arabica/stopwords.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.1/arabica.egg-info/PKG-INFO` & `arabica-1.6.2/arabica.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
@@ -41,15 +41,16 @@
 
 
 ## Installation
 
 Arabica requires [Python 3.8 - 3.10](https://www.python.org/downloads/), [NLTK](http://www.nltk.org) - stop words removal,
 [cleantext](https://pypi.org/project/cleantext/#description) - text cleaning, [wordcloud](https://pypi.org/project/wordcloud) - word cloud visualization,
 [plotnine](https://pypi.org/project/plotnine) - heatmaps and line graphs, [matplotlib](https://pypi.org/project/matplotlib/) - word clouds and graphical operations,
-[vaderSentiment](https://pypi.org/project/vaderSentiment) - sentiment analysis, and [jenskpy](https://pypi.org/project/jenkspy/) for breakpoint identification.
+[vaderSentiment](https://pypi.org/project/vaderSentiment) - sentiment analysis, [finvader](https://pypi.org/project/finvader) - financial sentiment analysis,
+and [jenskpy](https://pypi.org/project/jenkspy/) for breakpoint identification.
 
 To install using pip, use:
 
 `pip install arabica`
 
 
 
@@ -103,15 +104,15 @@
                lower_case: bool = False  # Lowercase text
 ```
 
 **coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. 
 
 The implemented models are:
 
-* **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See: *Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text.* Available from [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
+* **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. Available from [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
 
 * **FinVADER** improves VADER's classification accuracy, including two financial lexicons. Available from [here](https://pypi.org/project/finvader/).
 
 Structural breaks in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
 
 
 ``` python
```

### Comparing `arabica-1.6.1/pyproject.toml` & `arabica-1.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "arabica"
-version = "1.6.1"
+version = "1.6.2"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "Python package for exploratory text data analysis"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8, !=3.11"
```

### Comparing `arabica-1.6.1/setup.py` & `arabica-1.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="arabica",
-        version="1.6.1",
+        version="1.6.2",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["arabica"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/Arabica",
```

