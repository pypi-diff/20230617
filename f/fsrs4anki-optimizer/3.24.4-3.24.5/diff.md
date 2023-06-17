# Comparing `tmp/fsrs4anki_optimizer-3.24.4.tar.gz` & `tmp/fsrs4anki_optimizer-3.24.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.24.4.tar", last modified: Fri Jun 16 06:52:24 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.24.5.tar", last modified: Sat Jun 17 12:29:47 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.24.4.tar` & `fsrs4anki_optimizer-3.24.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:52:24.694740 fsrs4anki_optimizer-3.24.4/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 06:52:24.694740 fsrs4anki_optimizer-3.24.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:52:24.690740 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 06:52:14.000000 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-16 06:52:14.000000 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43530 2023-06-16 06:52:14.000000 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:52:24.690740 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 06:52:24.000000 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-16 06:52:24.000000 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:52:24.000000 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-16 06:52:24.000000 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 06:52:24.000000 fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-16 06:52:14.000000 fsrs4anki_optimizer-3.24.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:52:24.694740 fsrs4anki_optimizer-3.24.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 06:52:14.000000 fsrs4anki_optimizer-3.24.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:29:47.885665 fsrs4anki_optimizer-3.24.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-17 12:29:47.885665 fsrs4anki_optimizer-3.24.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:29:47.885665 fsrs4anki_optimizer-3.24.5/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-17 12:29:34.000000 fsrs4anki_optimizer-3.24.5/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-17 12:29:34.000000 fsrs4anki_optimizer-3.24.5/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43615 2023-06-17 12:29:34.000000 fsrs4anki_optimizer-3.24.5/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:29:47.885665 fsrs4anki_optimizer-3.24.5/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-17 12:29:47.000000 fsrs4anki_optimizer-3.24.5/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-17 12:29:47.000000 fsrs4anki_optimizer-3.24.5/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 12:29:47.000000 fsrs4anki_optimizer-3.24.5/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-17 12:29:47.000000 fsrs4anki_optimizer-3.24.5/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-17 12:29:47.000000 fsrs4anki_optimizer-3.24.5/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-17 12:29:34.000000 fsrs4anki_optimizer-3.24.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 12:29:47.885665 fsrs4anki_optimizer-3.24.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-17 12:29:34.000000 fsrs4anki_optimizer-3.24.5/setup.py
```

### Comparing `fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.24.5/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.24.4/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.24.5/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         self.train_data_loader = DataLoader(self.train_set, batch_sampler=sampler, collate_fn=collate_fn)
 
         self.test_set = RevlogDataset(test_set)
         sampler = RevlogSampler(self.test_set, batch_size=self.batch_size)
         self.test_data_loader = DataLoader(self.test_set, batch_sampler=sampler, collate_fn=collate_fn)
         print("dataset built")
 
-    def train(self):
+    def train(self, verbose: bool=True):
         # pretrain
         best_loss = np.inf
         weighted_loss, w = self.eval()
         if weighted_loss < best_loss:
             best_loss = weighted_loss
             best_w = w
 
@@ -214,15 +214,15 @@
                 loss.backward()
                 self.optimizer.step()
                 self.model.apply(self.clipper)
                 pbar.update(n=real_batch_size)
 
         pbar.close()
         for name, param in self.model.named_parameters():
-            print(f"{name}: {list(map(lambda x: round(float(x), 4),param))}")
+            tqdm.write(f"{name}: {list(map(lambda x: round(float(x), 4),param))}")
 
         epoch_len = len(self.next_train_data_loader)
         pbar = tqdm(desc="train", colour="red", total=epoch_len*self.n_epoch)
         print_len = max(self.batch_nums*self.n_epoch // 10, 1)
         for k in range(self.n_epoch):
             weighted_loss, w = self.eval()
             if weighted_loss < best_loss:
@@ -242,15 +242,15 @@
                 for param in self.model.parameters():
                     param.grad[:2] = torch.zeros(2)
                 self.optimizer.step()
                 self.scheduler.step()
                 self.model.apply(self.clipper)
                 pbar.update(real_batch_size)
 
-                if (k * self.batch_nums + i + 1) % print_len == 0:
+                if verbose and (k * self.batch_nums + i + 1) % print_len == 0:
                     tqdm.write(f"iteration: {k * epoch_len + (i + 1) * self.batch_size}")
                     for name, param in self.model.named_parameters():
                         tqdm.write(f"{name}: {list(map(lambda x: round(float(x), 4),param))}")
         pbar.close()
 
         weighted_loss, w = self.eval()
         if weighted_loss < best_loss:
@@ -416,15 +416,15 @@
         df = df.groupby(by=['r_history'], group_keys=False).progress_apply(cal_stability)
         print("Stability calculated.")
         df.reset_index(drop = True, inplace = True)
         df.drop_duplicates(inplace=True)
         df.sort_values(by=['r_history'], inplace=True, ignore_index=True)
 
         if df.shape[0] > 0:
-            for idx in tqdm(df.index):
+            for idx in tqdm(df.index, desc="analysis"):
                 item = df.loc[idx]
                 index = df[(df['i'] == item['i'] + 1) & (df['r_history'].str.startswith(item['r_history']))].index
                 df.loc[index, 'last_stability'] = item['stability']
             df['factor'] = round(df['stability'] / df['last_stability'], 2)
             df = df[(df['i'] >= 2) & (df['group_cnt'] >= 100)].copy()
             df['last_recall'] = df['r_history'].map(lambda x: x[-1])
             df = df[df.groupby(['i', 'r_history'], group_keys=False)['group_cnt'].transform(max) == df['group_cnt']]
@@ -602,15 +602,15 @@
                 return self.w[9] * np.power(d, self.w[10]) * np.power(s, self.w[11]) * np.exp((1 - r) * self.w[12])
 
 
         stability_list = np.array([np.power(base, i - index_offset) for i in range(index_len)])
         print(f"terminal stability: {stability_list.max(): .2f}")
         df = pd.DataFrame(columns=["retention", "difficulty", "time"])
 
-        for percentage in tqdm(range(96, 66, -2)):
+        for percentage in tqdm(range(96, 66, -2), desc="find optimal retention"):
             recall = percentage / 100
             time_list = np.zeros((d_range, index_len))
             time_list[:,:-1] = max_time
             for d in range(d_range, 0, -1):
                 s0 = init_stability(d)
                 s0_index = stability2index(s0)
                 diff = max_time
```

