# Comparing `tmp/arabica-1.6.0.tar.gz` & `tmp/arabica-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabica-1.6.0.tar", last modified: Thu Jun 15 19:12:32 2023, max compression
+gzip compressed data, was "arabica-1.6.1.tar", last modified: Sat Jun 17 11:28:02 2023, max compression
```

## Comparing `arabica-1.6.0.tar` & `arabica-1.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 19:12:32.763858 arabica-1.6.0/
--rw-rw-rw-   0        0        0       11 2023-05-18 21:22:46.000000 arabica-1.6.0/LICENSE
--rw-rw-rw-   0        0        0     7527 2023-06-15 19:12:32.763858 arabica-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     6766 2023-04-17 21:14:46.000000 arabica-1.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 19:12:32.749287 arabica-1.6.0/arabica/
--rw-rw-rw-   0        0        0      105 2023-05-18 23:17:32.000000 arabica-1.6.0/arabica/__init__.py
--rw-rw-rw-   0        0        0    12483 2023-05-18 23:09:58.000000 arabica-1.6.0/arabica/arabica_freq.py
--rw-rw-rw-   0        0        0    30721 2023-05-19 20:32:49.000000 arabica-1.6.0/arabica/cappuccino.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.6.0/arabica/clean_ngram.py
--rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.6.0/arabica/clean_numbers.py
--rw-rw-rw-   0        0        0     7819 2023-05-20 10:56:18.000000 arabica-1.6.0/arabica/coffee_break.py
--rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.6.0/arabica/group.py
--rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.6.0/arabica/preprocess.py
--rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.6.0/arabica/sentiment.py
--rw-rw-rw-   0        0        0     1118 2023-05-18 20:28:46.000000 arabica-1.6.0/arabica/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:12:32.763858 arabica-1.6.0/arabica.egg-info/
--rw-rw-rw-   0        0        0     7527 2023-06-15 19:12:32.000000 arabica-1.6.0/arabica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-06-15 19:12:32.000000 arabica-1.6.0/arabica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 19:12:32.000000 arabica-1.6.0/arabica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      165 2023-06-15 19:12:32.000000 arabica-1.6.0/arabica.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 19:12:32.000000 arabica-1.6.0/arabica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      547 2023-06-15 19:12:03.000000 arabica-1.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 19:12:32.763858 arabica-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-06-15 19:12:02.000000 arabica-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:28:02.970941 arabica-1.6.1/
+-rw-rw-rw-   0        0        0       11 2023-05-18 21:22:46.000000 arabica-1.6.1/LICENSE
+-rw-rw-rw-   0        0        0     7777 2023-06-17 11:28:02.972055 arabica-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7011 2023-06-17 11:19:31.000000 arabica-1.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 11:28:02.967045 arabica-1.6.1/arabica/
+-rw-rw-rw-   0        0        0      105 2023-05-18 23:17:32.000000 arabica-1.6.1/arabica/__init__.py
+-rw-rw-rw-   0        0        0    12483 2023-05-18 23:09:58.000000 arabica-1.6.1/arabica/arabica_freq.py
+-rw-rw-rw-   0        0        0    30721 2023-05-19 20:32:49.000000 arabica-1.6.1/arabica/cappuccino.py
+-rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.6.1/arabica/clean_ngram.py
+-rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.6.1/arabica/clean_numbers.py
+-rw-rw-rw-   0        0        0     8246 2023-06-17 08:04:35.000000 arabica-1.6.1/arabica/coffee_break.py
+-rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.6.1/arabica/group.py
+-rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.6.1/arabica/preprocess.py
+-rw-rw-rw-   0        0        0      533 2023-06-17 08:02:21.000000 arabica-1.6.1/arabica/sentiment.py
+-rw-rw-rw-   0        0        0     1118 2023-05-18 20:28:46.000000 arabica-1.6.1/arabica/stopwords.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:28:02.970941 arabica-1.6.1/arabica.egg-info/
+-rw-rw-rw-   0        0        0     7777 2023-06-17 11:28:02.000000 arabica-1.6.1/arabica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-06-17 11:28:02.000000 arabica-1.6.1/arabica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 11:28:02.000000 arabica-1.6.1/arabica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-06-17 11:28:02.000000 arabica-1.6.1/arabica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-17 11:28:02.000000 arabica-1.6.1/arabica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      547 2023-06-17 11:25:22.000000 arabica-1.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-17 11:28:02.972055 arabica-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1111 2023-06-17 11:25:22.000000 arabica-1.6.1/setup.py
```

### Comparing `arabica-1.6.0/PKG-INFO` & `arabica-1.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
@@ -101,23 +101,28 @@
                skip: [] ,                # Remove additional strings
                numbers: bool = False,    # Remove numbers
                lower_case: bool = False  # Lowercase text
 ```
 
 **coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. 
 
-* The implemented model is **VADER** (Valence Aware Dictionary and sEntiment Reasoner), a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See: *Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text.* Available from [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
+The implemented models are:
 
-* Structural breaks in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
+* **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See: *Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text.* Available from [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
+
+* **FinVADER** improves VADER's classification accuracy, including two financial lexicons. Available from [here](https://pypi.org/project/finvader/).
+
+Structural breaks in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
 
 
 ``` python
 def coffee_break(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
+                 model: str,                # Sentiment classifier, 'vader' - general language, 'finvader' - financial text                
                  skip: [] ,                 # Remove additional strings
                  preprocess: bool = False,  # Clean data from numbers and punctuation
                  time_freq: str ='',        # Aggregation period: 'Y'/'M'
                  n_breaks: int =''          # Number of breaks: min. 2
 )
 ```
```

### Comparing `arabica-1.6.0/README.md` & `arabica-1.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -84,23 +84,28 @@
                skip: [] ,                # Remove additional strings
                numbers: bool = False,    # Remove numbers
                lower_case: bool = False  # Lowercase text
 ```
 
 **coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. 
 
-* The implemented model is **VADER** (Valence Aware Dictionary and sEntiment Reasoner), a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See: *Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text.* Available from [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
+The implemented models are:
 
-* Structural breaks in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
+* **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See: *Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text.* Available from [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
+
+* **FinVADER** improves VADER's classification accuracy, including two financial lexicons. Available from [here](https://pypi.org/project/finvader/).
+
+Structural breaks in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
 
 
 ``` python
 def coffee_break(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
+                 model: str,                # Sentiment classifier, 'vader' - general language, 'finvader' - financial text                
                  skip: [] ,                 # Remove additional strings
                  preprocess: bool = False,  # Clean data from numbers and punctuation
                  time_freq: str ='',        # Aggregation period: 'Y'/'M'
                  n_breaks: int =''          # Number of breaks: min. 2
 )
 ```
```

### Comparing `arabica-1.6.0/arabica/arabica_freq.py` & `arabica-1.6.1/arabica/arabica_freq.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.0/arabica/cappuccino.py` & `arabica-1.6.1/arabica/cappuccino.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.0/arabica/clean_ngram.py` & `arabica-1.6.1/arabica/clean_ngram.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.0/arabica/coffee_break.py` & `arabica-1.6.1/arabica/coffee_break.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-
 # Sentiment analysis and structural breaks identification module
 
 import jenkspy
 import matplotlib.pyplot as plt
 from matplotlib.pyplot import figure
 import numpy as np
 import pandas as pd
 import sys
 
 
 from .preprocess import *
 from .group import *
-from .sentiment import sentiment_vader
+from .sentiment import *
+
 
 
 def coffee_break(text: str,                  # Text column
                  time: str,                  # Time column
                  date_format: str,           # Date format: 'eur' - European, 'us' - American
+                 model: str,                 # Sentiment classifier: 'vader' - general language,                               'finvader' - financial texts
                  skip: [ ],                  # Remove additional strings
                  preprocess: bool = False,   # Clean data from numbers and punctuation
                  time_freq: int = '',        # Aggregation period: 'Y'/'M'
                  n_breaks: int = ''):        # Number of breaks: min. 2
 
     date_formats = ["eur", "us"]
     frequencies = ["M", "Y"]
@@ -65,15 +66,19 @@
             data['period']=data['period'].astype(str)
             data['period'] = pd.to_datetime(data['period'], dayfirst=True)
 
         elif date_format == 'us':
             data['period']=data['period'].astype(str)
             data['period'] = pd.to_datetime(data['period'], dayfirst=False)
 
-        data['sentiment'] = np.vectorize(sentiment_vader)(data['text'])
+        if model == 'vader':
+            data['sentiment'] = np.vectorize(sentiment_vader)(data['text'])
+        elif model == 'finvader':
+            data['sentiment'] = np.vectorize(fin_vader)(data['text'])
+
         sentiment_ts = grouper_sentiment(data = data,time_freq='1M')
         sentiment_ts['period'] = pd.to_datetime(sentiment_ts['period'])
         sentiment_ts.set_index(sentiment_ts['period'], inplace = True)
         sentiment_ts.columns = ['period', 'sentiment']
 
 
         if n_breaks is None:
@@ -138,15 +143,19 @@
             data['period']=data['period'].astype(str)
             data['period'] = pd.to_datetime(data['period'], dayfirst=True)
 
         elif date_format == 'us':
             data['period']=data['period'].astype(str)
             data['period'] = pd.to_datetime(data['period'], dayfirst=False)
 
-        data['sentiment'] = np.vectorize(sentiment_vader)(data['text'])
+        if model == 'vader':
+            data['sentiment'] = np.vectorize(sentiment_vader)(data['text'])
+        elif model == 'finvader':
+            data['sentiment'] = np.vectorize(fin_vader)(data['text'])
+
         sentiment_ts = grouper_sentiment(data = data,time_freq='1Y')
         sentiment_ts['period'] = pd.to_datetime(sentiment_ts['period'])
         sentiment_ts.set_index(sentiment_ts['period'], inplace = True)
         sentiment_ts.columns = ['period', 'sentiment']
 
         if n_breaks is None:
             ts = sentiment_ts['sentiment']
```

### Comparing `arabica-1.6.0/arabica/group.py` & `arabica-1.6.1/arabica/group.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.0/arabica/preprocess.py` & `arabica-1.6.1/arabica/preprocess.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.0/arabica/stopwords.py` & `arabica-1.6.1/arabica/stopwords.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.0/arabica.egg-info/PKG-INFO` & `arabica-1.6.1/arabica.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
@@ -101,23 +101,28 @@
                skip: [] ,                # Remove additional strings
                numbers: bool = False,    # Remove numbers
                lower_case: bool = False  # Lowercase text
 ```
 
 **coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. 
 
-* The implemented model is **VADER** (Valence Aware Dictionary and sEntiment Reasoner), a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See: *Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text.* Available from [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
+The implemented models are:
 
-* Structural breaks in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
+* **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See: *Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text.* Available from [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
+
+* **FinVADER** improves VADER's classification accuracy, including two financial lexicons. Available from [here](https://pypi.org/project/finvader/).
+
+Structural breaks in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
 
 
 ``` python
 def coffee_break(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
+                 model: str,                # Sentiment classifier, 'vader' - general language, 'finvader' - financial text                
                  skip: [] ,                 # Remove additional strings
                  preprocess: bool = False,  # Clean data from numbers and punctuation
                  time_freq: str ='',        # Aggregation period: 'Y'/'M'
                  n_breaks: int =''          # Number of breaks: min. 2
 )
 ```
```

### Comparing `arabica-1.6.0/pyproject.toml` & `arabica-1.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "arabica"
-version = "1.6.0"
+version = "1.6.1"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "Python package for exploratory text data analysis"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8, !=3.11"
```

### Comparing `arabica-1.6.0/setup.py` & `arabica-1.6.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="arabica",
-        version="1.6.0",
+        version="1.6.1",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["arabica"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/Arabica",
         python_requires='>=3.8, !=3.11',
-        install_requires = ['pandas == 1.4.0',
+        install_requires = ['pandas >=1.4.0',
                             'nltk == 3.6.2',
                             'regex',
+                            'finvader',
                             'matplotlib == 3.6.0',
                             'matplotlib-inline == 0.1.6',
                             'plotnine == 0.10.1',
                             'wordcloud == 1.8.2.2',
                             'jenkspy == 0.3.2',
                             'vaderSentiment == 3.3.2',
                             'cleantext == 1.1.4'],
```

