# Comparing `tmp/pytorch-supporter-0.0.17.tar.gz` & `tmp/pytorch-supporter-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-supporter-0.0.17.tar", last modified: Fri Jun 16 06:38:52 2023, max compression
+gzip compressed data, was "pytorch-supporter-0.0.18.tar", last modified: Sat Jun 17 05:51:32 2023, max compression
```

## Comparing `pytorch-supporter-0.0.17.tar` & `pytorch-supporter-0.0.18.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 06:38:52.169295 pytorch-supporter-0.0.17/
--rw-r--r--   0 root         (0) root         (0)     2416 2023-06-16 06:38:52.168295 pytorch-supporter-0.0.17/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2154 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 06:38:52.164295 pytorch-supporter-0.0.17/pytorch_supporter/
--rw-r--r--   0 root         (0) root         (0)       41 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 06:38:52.167295 pytorch-supporter-0.0.17/pytorch_supporter/layers/
--rw-r--r--   0 root         (0) root         (0)      984 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/layers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      198 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/layers/dict_to_parameters.py
--rw-r--r--   0 root         (0) root         (0)      425 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/layers/dot_product.py
--rw-r--r--   0 root         (0) root         (0)      644 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/layers/gru_last_hidden_state.py
--rw-r--r--   0 root         (0) root         (0)      801 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/layers/hidden_state_reset_gru.py
--rw-r--r--   0 root         (0) root         (0)      872 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/layers/hidden_state_reset_lstm.py
--rw-r--r--   0 root         (0) root         (0)      801 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/layers/hidden_state_reset_rnn.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/layers/lazily_initialized_linear.py
--rw-r--r--   0 root         (0) root         (0)      655 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/layers/lstm_last_hidden_state.py
--rw-r--r--   0 root         (0) root         (0)      225 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/layers/permute.py
--rw-r--r--   0 root         (0) root         (0)      336 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/layers/reshape.py
--rw-r--r--   0 root         (0) root         (0)      644 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/layers/rnn_last_hidden_state.py
--rw-r--r--   0 root         (0) root         (0)      197 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/layers/select_from_array.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 06:38:52.168295 pytorch-supporter-0.0.17/pytorch_supporter/utils/
--rw-r--r--   0 root         (0) root         (0)      145 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      802 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/utils/text.py
--rw-r--r--   0 root         (0) root         (0)      835 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter/utils/time_series.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 06:38:52.165295 pytorch-supporter-0.0.17/pytorch_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2416 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1000 2023-06-16 06:38:52.000000 pytorch-supporter-0.0.17/pytorch_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/pytorch_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 06:38:52.169295 pytorch-supporter-0.0.17/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-16 06:38:51.000000 pytorch-supporter-0.0.17/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:51:32.349018 pytorch-supporter-0.0.18/
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-06-17 05:51:32.348018 pytorch-supporter-0.0.18/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:51:32.342018 pytorch-supporter-0.0.18/pytorch_supporter/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:51:32.347018 pytorch-supporter-0.0.18/pytorch_supporter/layers/
+-rw-r--r--   0 root         (0) root         (0)      984 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/layers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      198 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/layers/dict_to_parameters.py
+-rw-r--r--   0 root         (0) root         (0)      425 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/layers/dot_product.py
+-rw-r--r--   0 root         (0) root         (0)      644 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/layers/gru_last_hidden_state.py
+-rw-r--r--   0 root         (0) root         (0)      801 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/layers/hidden_state_reset_gru.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/layers/hidden_state_reset_lstm.py
+-rw-r--r--   0 root         (0) root         (0)      801 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/layers/hidden_state_reset_rnn.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/layers/lazily_initialized_linear.py
+-rw-r--r--   0 root         (0) root         (0)      655 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/layers/lstm_last_hidden_state.py
+-rw-r--r--   0 root         (0) root         (0)      225 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/layers/permute.py
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/layers/reshape.py
+-rw-r--r--   0 root         (0) root         (0)      644 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/layers/rnn_last_hidden_state.py
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/layers/select_from_array.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:51:32.348018 pytorch-supporter-0.0.18/pytorch_supporter/utils/
+-rw-r--r--   0 root         (0) root         (0)      145 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      802 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/utils/text.py
+-rw-r--r--   0 root         (0) root         (0)      835 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter/utils/time_series.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:51:32.343018 pytorch-supporter-0.0.18/pytorch_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1000 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/pytorch_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 05:51:32.349018 pytorch-supporter-0.0.18/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-17 05:51:31.000000 pytorch-supporter-0.0.18/setup.py
```

### Comparing `pytorch-supporter-0.0.17/PKG-INFO` & `pytorch-supporter-0.0.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-supporter
-Version: 0.0.17
+Version: 0.0.18
 Summary: Pytorch supporter
 Home-page: https://github.com/automatethem/pytorch-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `pytorch-supporter-0.0.17/README.md` & `pytorch-supporter-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.17/pytorch_supporter/layers/__init__.py` & `pytorch-supporter-0.0.18/pytorch_supporter/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.17/pytorch_supporter/layers/gru_last_hidden_state.py` & `pytorch-supporter-0.0.18/pytorch_supporter/layers/gru_last_hidden_state.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.17/pytorch_supporter/layers/hidden_state_reset_gru.py` & `pytorch-supporter-0.0.18/pytorch_supporter/layers/hidden_state_reset_gru.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.17/pytorch_supporter/layers/hidden_state_reset_lstm.py` & `pytorch-supporter-0.0.18/pytorch_supporter/layers/hidden_state_reset_rnn.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import torch
 
-#이전 시퀀스의 숨은 상태가 다음 시퀀스의 영행을 주기 않게 하기위해 새로운 시퀀스 입력시 이전 숨은 상태 초기화하는 LSTM
-class HiddenStateResetLSTM(torch.nn.Module):
+#이전 시퀀스의 숨은 상태가 다음 시퀀스의 영행을 주기 않게 하기위해 새로운 시퀀스 입력시 이전 숨은 상태 초기화하는 RNN
+class HiddenStateResetRNN(torch.nn.Module):
     def __init__(self, input_size, hidden_size, num_layers=1, **kwargs):
         super().__init__()
-        self.layer = torch.nn.LSTM(input_size=input_size, hidden_size=hidden_size, num_layers=num_layers, **kwargs)
+        self.layer = torch.nn.RNN(input_size=input_size, hidden_size=hidden_size, num_layers=num_layers, **kwargs)
         self.input_size = input_size
         self.hidden_size = hidden_size
         self.num_layers = num_layers
 
     def forward(self, x, **kwargs):
         batch_length = len(x)
         hidden_state = torch.zeros(self.num_layers, batch_length, self.hidden_size)
-        cell_state = torch.zeros(self.num_layers, batch_length, self.hidden_size)
-        x = self.layer(x, hx=(hidden_state, cell_state), **kwargs)
+        print(hidden_state)
+        x = self.layer(x, hx=hidden_state, **kwargs)
         return x
```

### Comparing `pytorch-supporter-0.0.17/pytorch_supporter/layers/lazily_initialized_linear.py` & `pytorch-supporter-0.0.18/pytorch_supporter/layers/lazily_initialized_linear.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.17/pytorch_supporter/layers/lstm_last_hidden_state.py` & `pytorch-supporter-0.0.18/pytorch_supporter/layers/lstm_last_hidden_state.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.17/pytorch_supporter/layers/rnn_last_hidden_state.py` & `pytorch-supporter-0.0.18/pytorch_supporter/layers/rnn_last_hidden_state.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.17/pytorch_supporter/utils/text.py` & `pytorch-supporter-0.0.18/pytorch_supporter/utils/text.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.17/pytorch_supporter/utils/time_series.py` & `pytorch-supporter-0.0.18/pytorch_supporter/utils/time_series.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.17/pytorch_supporter.egg-info/PKG-INFO` & `pytorch-supporter-0.0.18/pytorch_supporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-supporter
-Version: 0.0.17
+Version: 0.0.18
 Summary: Pytorch supporter
 Home-page: https://github.com/automatethem/pytorch-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `pytorch-supporter-0.0.17/pytorch_supporter.egg-info/SOURCES.txt` & `pytorch-supporter-0.0.18/pytorch_supporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.17/setup.py` & `pytorch-supporter-0.0.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='pytorch-supporter',
-	version='0.0.17',
+	version='0.0.18',
 	description='Pytorch supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/pytorch-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

