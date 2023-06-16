# Comparing `tmp/american_options-0.1.2.tar.gz` & `tmp/american_options-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\american_options-0.1.2.tar", last modified: Mon Jun 12 10:11:25 2023, max compression
+gzip compressed data, was "dist\american_options-0.1.3.tar", last modified: Fri Jun 16 11:52:50 2023, max compression
```

## Comparing `american_options-0.1.2.tar` & `american_options-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 10:11:25.000000 american_options-0.1.2/
--rw-rw-rw-   0        0        0     2510 2023-06-12 10:11:25.000000 american_options-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1777 2023-06-12 01:21:26.000000 american_options-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 10:11:25.000000 american_options-0.1.2/american_options/
--rw-rw-rw-   0        0        0    34934 2023-06-12 10:08:26.000000 american_options-0.1.2/american_options/AMoption.py
--rw-rw-rw-   0        0        0      191 2023-06-12 00:46:34.000000 american_options-0.1.2/american_options/__init__.py
--rw-rw-rw-   0        0        0     4524 2023-06-11 22:01:15.000000 american_options-0.1.2/american_options/jump_diffusion.py
--rw-rw-rw-   0        0        0     4198 2023-06-11 22:50:46.000000 american_options-0.1.2/american_options/payoffs.py
--rw-rw-rw-   0        0        0     2333 2023-06-10 14:04:25.000000 american_options-0.1.2/american_options/próby.py
--rw-rw-rw-   0        0        0     2638 2023-06-11 17:41:22.000000 american_options-0.1.2/american_options/sobol.py
--rw-rw-rw-   0        0        0    10287 2023-06-11 22:52:35.000000 american_options-0.1.2/american_options/underlying.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:11:25.000000 american_options-0.1.2/american_options.egg-info/
--rw-rw-rw-   0        0        0     2510 2023-06-12 10:11:25.000000 american_options-0.1.2/american_options.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-06-12 10:11:25.000000 american_options-0.1.2/american_options.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 10:11:25.000000 american_options-0.1.2/american_options.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-12 10:11:25.000000 american_options-0.1.2/american_options.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-12 10:11:25.000000 american_options-0.1.2/american_options.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 10:11:25.000000 american_options-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1425 2023-06-12 10:08:26.000000 american_options-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:52:50.000000 american_options-0.1.3/
+-rw-rw-rw-   0        0        0     2514 2023-06-16 11:52:50.000000 american_options-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1777 2023-06-12 01:21:26.000000 american_options-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 11:52:50.000000 american_options-0.1.3/american_options/
+-rw-rw-rw-   0        0        0    38860 2023-06-16 11:47:37.000000 american_options-0.1.3/american_options/AMoption.py
+-rw-rw-rw-   0        0        0      191 2023-06-12 00:46:34.000000 american_options-0.1.3/american_options/__init__.py
+-rw-rw-rw-   0        0        0     4524 2023-06-11 22:01:15.000000 american_options-0.1.3/american_options/jump_diffusion.py
+-rw-rw-rw-   0        0        0    13623 2023-06-14 22:10:53.000000 american_options-0.1.3/american_options/payoffs.py
+-rw-rw-rw-   0        0        0     3844 2023-06-13 18:24:10.000000 american_options-0.1.3/american_options/próby.py
+-rw-rw-rw-   0        0        0     2638 2023-06-11 17:41:22.000000 american_options-0.1.3/american_options/sobol.py
+-rw-rw-rw-   0        0        0    10501 2023-06-16 11:25:20.000000 american_options-0.1.3/american_options/underlying.py
+-rw-rw-rw-   0        0        0     2859 2023-06-16 10:33:51.000000 american_options-0.1.3/american_options/xd.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:52:50.000000 american_options-0.1.3/american_options.egg-info/
+-rw-rw-rw-   0        0        0     2514 2023-06-16 11:52:50.000000 american_options-0.1.3/american_options.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-06-16 11:52:50.000000 american_options-0.1.3/american_options.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 11:52:50.000000 american_options-0.1.3/american_options.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-16 11:52:50.000000 american_options-0.1.3/american_options.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-16 11:52:50.000000 american_options-0.1.3/american_options.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 11:52:50.000000 american_options-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1429 2023-06-16 11:52:03.000000 american_options-0.1.3/setup.py
```

### Comparing `american_options-0.1.2/PKG-INFO` & `american_options-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: american_options
-Version: 0.1.2
-Summary: library T-28h
+Version: 0.1.3
+Summary: Added new payoffs
 Home-page: https://american_options.readthedocs.io/
 Author: Przemysław Adamski, Katarzyna Hasal, Kacper Toczek
 Author-email: kat.hasal99@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `american_options-0.1.2/README.md` & `american_options-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `american_options-0.1.2/american_options/AMoption.py` & `american_options-0.1.3/american_options/AMoption.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
 
     def __init__(self, underlyings, payoff_func, T):
         self.ssp_representative = None
         if isinstance(underlyings, tuple):
             self.underlyings = underlyings
         else:
-            self.underlyings = (underlyings,)  # Tak się tworzy jednoelementową krotkę
+            self.underlyings = (underlyings,)
         self.payoff_func = payoff_func
         self.T = T
 
     def european(self, n_sims=100000, mode='GBM'):
         """
         Get a price of European option using Monte Carlo simulations.
 
@@ -176,17 +176,17 @@
             TF = Sim_Payoffs > 0
             indices = np.arange(0, n_sims)
 
             Final_Results = pd.DataFrame(data=0, index=range(n_sims),
                                          columns=range(round(values_per_year * self.T) + 1))
             Final_Results[round(values_per_year * self.T)] = Sim_Payoffs.iloc[:, -1]
 
-            Execution_Times = pd.DataFrame(data=0, index=range(n_sims),
+            Exercise_Times = pd.DataFrame(data=0, index=range(n_sims),
                                            columns=range(round(values_per_year * self.T) + 1))
-            Execution_Times[round(values_per_year * self.T)] = 1 * (Sim_Payoffs.iloc[:, -1] > 0)
+            Exercise_Times[round(values_per_year * self.T)] = 1 * (Sim_Payoffs.iloc[:, -1] > 0)
 
             for j in tqdm(np.arange(2, round(self.T * values_per_year) + 1)):
                 TF_j = indices[TF.iloc[:, -j]]
                 if len(TF_j) >= 3:
                     try:
                         def f_j(S_t):
                             H = pd.DataFrame({'S_t': Simulations.iloc[TF_j, -j], 'PO_t': (
@@ -210,28 +210,28 @@
                         model_j.fit(X_j, Y_j)
                         estimations_j = model_j.predict(X_j)
 
                     choose_to_exercise_indices = TF_j[estimations_j < Sim_Payoffs.iloc[TF_j, -j]]
 
                     Final_Results.iloc[choose_to_exercise_indices, -j] = Sim_Payoffs.iloc[
                         choose_to_exercise_indices, -j]
-                    Execution_Times.iloc[choose_to_exercise_indices, -j] = 1
+                    Exercise_Times.iloc[choose_to_exercise_indices, -j] = 1
                     Final_Results.iloc[choose_to_exercise_indices, (-j + 1):] = 0
 
                 elif len(TF_j) == 2 or len(TF_j) == 1:
                     estimations_j = (np.exp(
                         -self.underlyings[0].r * np.arange(1, j) / round(values_per_year * self.T)) * Final_Results.iloc[TF_j,
                                                                                           (-j + 1):]).sum(axis=1)
                     choose_to_exercise_indices = TF_j[estimations_j < Sim_Payoffs.iloc[TF_j, -j]]
                     Final_Results.iloc[choose_to_exercise_indices, -j] = Sim_Payoffs.iloc[
                         choose_to_exercise_indices, -j]
-                    Execution_Times.iloc[choose_to_exercise_indices, -j] = 1
+                    Exercise_Times.iloc[choose_to_exercise_indices, -j] = 1
                     Final_Results.iloc[choose_to_exercise_indices, (-j + 1):] = 0
 
-            self.ET_LS = Execution_Times
+            self.ET_LS = Exercise_Times.to_numpy()
 
             if mode == "GBM":
                 self.price_GBM_LS = np.mean(
                     (np.exp(-self.underlyings[0].r * np.arange(0, round(
                         values_per_year * self.T) + 1) / round(
                         values_per_year * self.T)) * Final_Results).sum(axis=1))
                 return self.price_GBM_LS
@@ -242,14 +242,15 @@
                         values_per_year * self.T)) * Final_Results).sum(axis=1))
                 return self.price_Bootstrap_LS
             elif mode == 'JD':
                 self.price_JD_LS = np.mean(
                     (np.exp(-self.underlyings[0].r * np.arange(0, round(
                         values_per_year * self.T) + 1) / round(
                         values_per_year * self.T)) * Final_Results).sum(axis=1))
+
                 return self.price_JD_LS
         else:
             if mode == "GBM":
                 if all(u.values_per_year_GBM == self.underlyings[0].values_per_year_GBM for u in self.underlyings):
                     values_per_year = self.underlyings[0].values_per_year_GBM
                 else:
                     raise Exception('Underlyings are calibrated for different values_per_year_GBM.')
@@ -273,26 +274,32 @@
                 warnings.warn(
                     'Underlyings assume different interest rates! Interest rate from the first underlying will be used')
 
             sims_list = []
             for u in self.underlyings:
                 sims_list.append(u.simulate(mode=mode, size=n_sims, T=self.T))
 
+            self.LS_price_trajectories = sims_list
+
             Sim_Payoffs = self.payoff_func(sims_list)
 
-            if type(Sim_Payoffs) != pandas.DataFrame:
+            if type(Sim_Payoffs) != pd.DataFrame:
                 Sim_Payoffs = pd.DataFrame(Sim_Payoffs)
 
             TF = Sim_Payoffs > 0
             indices = np.arange(0, n_sims)
 
             Final_Results = pd.DataFrame(data=0, index=range(n_sims),
                                          columns=range(round(values_per_year * self.T) + 1))
             Final_Results[round(values_per_year * self.T)] = Sim_Payoffs.iloc[:, -1]
 
+            Exercise_Times = pd.DataFrame(data=0, index=range(n_sims),
+                                         columns=range(round(values_per_year * self.T) + 1))
+            Exercise_Times[round(values_per_year * self.T)] = 1 * (Sim_Payoffs.iloc[:, -1] > 0)
+
             m = len(self.underlyings)
             powers = set(product(range(4), repeat=m)) - set([tuple(np.zeros(m)), tuple(3 * np.ones(m))])
 
             for j in tqdm(np.arange(2, round(self.T * values_per_year) + 1)):
                 TF_j = indices[TF.iloc[:, -j]]
                 if len(TF_j) >= 3:
                     Sims_j = np.column_stack(list(map(itemgetter(int(values_per_year*self.T) - j + 1), sims_list)))
@@ -307,25 +314,29 @@
                     model_j.fit(X_j, Y_j)
 
                     estimations_j = model_j.predict(X_j)
                     choose_to_exercise_indices = TF_j[estimations_j < Sim_Payoffs.iloc[TF_j, -j]]
 
                     Final_Results.iloc[choose_to_exercise_indices, -j] = Sim_Payoffs.iloc[
                         choose_to_exercise_indices, -j]
+                    Exercise_Times.iloc[choose_to_exercise_indices, -j] = 1
                     Final_Results.iloc[choose_to_exercise_indices, (-j + 1):] = 0
 
                 elif len(TF_j) == 2 or len(TF_j) == 1:
                     estimations_j = (np.exp(
                         -self.underlyings[0].r * np.arange(1, j) / round(255 * self.T)) * Final_Results.iloc[TF_j,
                                                                                           (-j + 1):]).sum(axis=1)
                     choose_to_exercise_indices = TF_j[estimations_j < Sim_Payoffs.iloc[TF_j, -j]]
                     Final_Results.iloc[choose_to_exercise_indices, -j] = Sim_Payoffs.iloc[
                         choose_to_exercise_indices, -j]
+                    Exercise_Times.iloc[choose_to_exercise_indices, -j] = 1
                     Final_Results.iloc[choose_to_exercise_indices, (-j + 1):] = 0
 
+            self.ET_LS = Exercise_Times.to_numpy()
+
             if mode == "GBM":
                 self.price_GBM_LS = np.mean(
                     (np.exp(-self.underlyings[0].r * np.arange(0, round(
                         values_per_year * self.T) + 1) / round(
                         values_per_year * self.T)) * Final_Results).sum(axis=1))
                 return self.price_GBM_LS
             elif mode == "Bootstrap":
@@ -352,31 +363,30 @@
         discounted average of payoffs from next timestep weighted by probabilities of moving to them.
         Calling this method for the first time on the Option on specific Underlying, takes a bit longer as we create
         3-dimensional transition probabilities matrix for the underlying.
         Calling the other options on the same Underlying is then much faster as we recycle once calculated probabilities.
 
         Method supports path-dependent options.
 
-        Parameters
+        Parameters:
         ----------
-        :param n_sims: Number of simulations for pricing
-        :type n_sims: int
-        :param mode: mode of underlying(s) that is desired to be used for simulations. Only 'GBM', 'JD' and 'Bootstrapping' are supported.
-        :type mode: str
-        :param approach: which algorithm of pricing to use. Default: 'sobol_sequence' can calucale all types of options,
-                        while 'basic_1d' can calculate only one-dimensional options,
-                        although after calling it first time, next calls are much faster.
-        :type approach: str
+        n_sims : int
+            number of simulations for pricing
+        mode : str
+            mode of underlying(s) that is desired to be used for simulations. Only 'GBM', 'JD' and 'Bootstrapping' are supported.
+        approach : str
+            which algorithm of pricing to use. Default: 'sobol_sequence' can calucale all types of options,
+            while 'basic_1d' can calculate only one-dimensional options,
+            although after calling it first time, next calls are much faster.
 
-        Returns
+        Returns:
         -------
-        :return: Value of specified option calculated using ssp method
-        :rtype: float
+        float : Value of specified option calculated using ssp method
 
-        Examples
+        Examples:
         --------
         Price one dimensional put option, based on underlying asset modelled with geometric Brownian motion:
 
         >>> import numpy as np
         >>> asset = Underlying(spot_price=100, r=0.06)
         >>> asset.calibrate_GBM(sigma=0.6,values_per_year_GBM=255)
         >>> option = Option(underlyings=asset, payoff_func=lambda trajectory: np.maximum(100-trajectory,0), T=1)
@@ -413,35 +423,36 @@
                 values_per_year = asset.values_per_year_Bootstrap
             elif mode == "JD":
                 values_per_year = asset.values_per_year_JD
             else:
                 raise Exception(
                     'Longstaff-Schwartz method (LS) is supported only for GBM, JD and Boostrapping at this moment')
 
-            ti = int(values_per_year * T)
+            ti = round(values_per_year * T)
             disc = np.exp(- asset.r * T / ti)
 
-            exercise = np.zeros((n_sims, ti))
+            #exercise = np.zeros((n_bins, ti+1))
+            #H = np.zeros((n_bins, ti+1))
             # n of paths in a bin
             n_paths = int(n_sims / n_bins)
             sorted_steps = np.argsort(paths, axis=0)
 
             all_payoffs = self.payoff_func(paths)
             # all_payoffs = self.payoff_func(paths)
 
             if not asset.ssp_calibrated:
                 probs_matrix = np.zeros((n_bins, n_bins, ti))
 
             for i in tqdm(range(ti + 1)):
                 cur_bins = sorted_steps[:, ti - i]
                 hi = all_payoffs[cur_bins, ti - i]
-                hi = np.mean(hi.reshape(-1, n_paths), axis=1)  # payoffy w danym kroku
+                hi_bins = np.mean(hi.reshape(-1, n_paths), axis=1)  # payoffy w danym kroku
 
                 if i == 0:
-                    V_i = hi
+                    V_i = hi_bins
 
                 else:
                     V_i1 = V_i
                     next_bins = sorted_steps[:, ti - i + 1]
 
                     if asset.ssp_calibrated:
                         probs = asset.probs_matrix[:, :, ti - i]
@@ -461,25 +472,29 @@
                                 # print(res)
                                 s += len(res)
                                 if s == n_paths:
                                     break
                         probs_matrix[:, :, ti - i] = probs
 
                     # print(probs)
-                    V_i = np.maximum(hi, probs @ V_i1 * disc)
-                    exercise[:, ti - i] = V_i <= hi
+                    V_i = np.maximum(hi_bins, probs @ V_i1 * disc)
+
+                #exercise[:, ti - i] = V_i <= hi_bins
+                #H[:,ti-i] = hi_bins
             if not asset.ssp_calibrated:
                 asset.probs_matrix = probs_matrix
                 asset.ssp_calibrated = True
 
-            Yt = hi * np.exp(- np.tile(np.arange(0, ti + 1), (n_sims, 1)) * (T/values_per_year) * asset.r)
-            exercise_time = np.argmax(exercise, axis=1)
-            res = np.mean(Yt[np.arange(len(Yt)), exercise_time])
-            self.upper_bound_price_ssp = np.mean(V_i)
-            self.ET_ssp = exercise.astype(int)
+            #Yt = H * np.exp(- np.tile(np.arange(0, ti + 1), (n_bins, 1)) * (T/values_per_year) * asset.r)
+            #exercise_time = np.argmax(exercise, axis=1)
+            #res = np.mean(Yt[np.arange(len(Yt)), exercise_time])
+            #self.upper_bound_price_ssp = np.mean(V_i)
+            #self.ET_ssp = exercise.astype(int)
+            res = np.mean(V_i)
+            self.ET_ssp = res
         else:
             # trying the approach as for one asset, but instead of creating bins for simulated paths of the underlying,
             # TODO: introduce possibility of simulating correlated assets
 
             if mode == "GBM":
                 if all(u.values_per_year_GBM == self.underlyings[0].values_per_year_GBM for u in self.underlyings):
                     values_per_year = self.underlyings[0].values_per_year_GBM
@@ -501,15 +516,15 @@
                     'State space partitioning method method (ssp) is supported only for GBM, JD and Boostrapping at this moment')
 
             if any(u.r != self.underlyings[0].r for u in self.underlyings):
                 warnings.warn(
                     'Underlyings assume different interest rates! Interest rate from the first underlying will be used')
 
             n_assets = len(self.underlyings)
-            ti = int(values_per_year * T)
+            ti = round(values_per_year * T)
             r = self.underlyings[0].r
             dt = T / ti
             disc = np.exp(- r * dt)
 
             # generating Sobol sequence
             # uniform
             np.random.seed(1)
@@ -663,48 +678,107 @@
                                     'high est': [np.mean(high_estimators)],
                                     'left high': [np.mean(high_estimators) - np.std(high_estimators) / np.sqrt(
                                         n_sims) * stats.norm.ppf(0.95)],
                                     'righ high': [np.mean(high_estimators) + np.std(high_estimators) / np.sqrt(
                                         n_sims) * stats.norm.ppf(0.95)]})
         return results
 
+    def plot_exercise_times(self, method, plot_trajectories_ratio = 0.02):
+        if len(self.underlyings) == 1:
+            if method == 'RTM':
+                raise Exception('plot of RTM exercise times is not supported')
+            elif not hasattr(self, 'ET_' + method):
+                raise Exception('''You haven't calculated price with .''' + method + ''' yet or chosen pricing method doesn't exist''')
+
+            if method == 'LS':
+                time_moments = np.argwhere(self.ET_LS == 1)[:, 1]
+                asset_prices = self.LS_price_trajectories.to_numpy()[self.ET_LS.astype(bool)]
+                price_traj = self.LS_price_trajectories.to_numpy()
+            elif method == 'ssp':
+                time_moments = np.argwhere(self.ET_ssp == 1)[:, 1]
+                asset_prices = self.ssp_price_trajectories[self.ET_ssp.astype(bool)]
+                price_traj = self.ssp_price_trajectories
+
+            plt.scatter(time_moments, asset_prices)
+
+            if plot_trajectories_ratio == 0:
+                pass
+            else:
+                for k in np.arange(0, np.shape(price_traj)[0], int(plot_trajectories_ratio*np.shape(price_traj)[0])):
+                    plt.plot(np.arange(0, np.shape(price_traj)[1] , 1), price_traj[k, :], alpha=0.3)
+            plt.show()
+
+        elif len(self.underlyings) == 2:
+            if method == 'RTM':
+                raise Exception('plot of RTM exercise times is not supported')
+            elif not hasattr(self, 'ET_' + method):
+                raise Exception('''You haven't calculated price with .''' + method + ''' yet or chosen pricing method doesn't exist''')
+
+            if method == 'LS':
+                rows, cols = np.shape(self.LS_price_trajectories)[1:3]
+                ET_TF = self.ET_LS.astype(bool)
+                t = np.reshape(np.tile(np.arange(0, cols), rows), (rows, cols))[ET_TF]
+                X = self.LS_price_trajectories[0].to_numpy()[ET_TF]
+                Y = self.LS_price_trajectories[1].to_numpy()[ET_TF]
+                price_traj = self.LS_price_trajectories
+            elif method == 'ssp':
+                rows, cols = np.shape(self.ssp_price_trajectories)[1:3]
+                ET_TF = self.ET_ssp.astype(bool)
+                np.reshape(np.tile(np.arange(0, cols), rows), (rows, cols))
+                t = np.reshape(np.tile(np.arange(0, cols), rows), (rows, rows))[ET_TF]
+                X = self.LS_price_trajectories[0][ET_TF]
+                Y = self.LS_price_trajectories[1][ET_TF]
+                price_traj = self.ssp_price_trajectories
+
+            fig1 = plt.figure(1)
+            ax1 = fig1.add_subplot(111, projection='3d')
+            ax1.scatter(t, X, Y, color='green', alpha=0.1)
+
+            # Increase the size of the axes
+            ax1.xaxis._axinfo['juggled'] = (0, 0, 2)
+            ax1.yaxis._axinfo['juggled'] = (1, 1, 2)
+            ax1.zaxis._axinfo['juggled'] = (2, 2, 2)
+
+            # Add labels to the axes
+            ax1.set_xlabel('t')
+            ax1.set_ylabel('S2')
+            ax1.set_zlabel('S1')
+
+            #Plot trajectories
+            if plot_trajectories_ratio == 0:
+                pass
+            else:
+                for k in np.arange(0, np.shape(price_traj)[1], int(plot_trajectories_ratio*np.shape(price_traj)[1])):
+                    plt.plot(np.arange(0, cols, 1), price_traj[0].to_numpy()[k, :],price_traj[1].to_numpy()[k, :], alpha=0.5)
+            plt.show()
+        else:
+            raise Exception('Exercise times for options based on 3 or more assets cannot be visualized')
+
+    def hist_optimal_exercise(self, method):
+        if method == 'RTM':
+            raise Exception('plot of RTM exercise times is not supported')
+        elif not hasattr(self, 'ET_' + method):
+            raise Exception(
+                '''You haven't calculated price with .''' + method + ''' yet or chosen pricing method doesn't exist''')
+
+        if len(self.underlyings) == 1:
+            if method == 'LS':
+                price_traj = self.LS_price_trajectories
+            elif method == 'ssp':
+                price_traj = self.ssp_price_trajectories
+        else:
+            if method == 'LS':
+                price_traj = self.LS_price_trajectories[0]
+            elif method == 'ssp':
+                price_traj = self.ssp_price_trajectories[0]
+
+        if method == 'LS':
+            density, bins = np.histogram(np.argmax(self.ET_LS, axis=1), bins=np.shape(price_traj)[1])
+        elif method == 'ssp':
+            density, bins = np.histogram(np.argmax(self.ET_ssp, axis=1), bins=np.shape(price_traj)[1])
+
+        plt.hist(density, bins)
+        plt.show()
+
 
-if __name__ == '__main__':
 
-    n = 10000
-    T = 0.5
-    sigma1 = 0.4
-    sigma2 = 0.8
-    r = 0.06
-    N = 250
-    spot1 = 100
-    spot2 = 120
-    K1 = 100
-    K2 = 110
-    K = 100
-    irr = 0.06
-    N = 255
-
-    asset1 = Underlying(spot_price=100, r=0.07)
-    asset1.calibrate_GBM(sigma=0.4, values_per_year_GBM=N)
-    asset1.calibrate_JD(sigma=0.4, jump_intensity=1/3)
-    asset2 = Underlying(spot_price=120, r=0.07)
-    asset2.calibrate_GBM(sigma=0.4, values_per_year_GBM=N)
-    asset2.calibrate_JD(sigma=0.2, jump_intensity=1/2)
-
-    from payoffs import payoff_creator_1d
-    def Call_Payoff(trajektoria,K):
-        return np.maximum(trajektoria-K,0)
-
-    option = Option(underlyings=asset1, payoff_func=lambda trajectory: payoff_creator_1d(trajectory, Call_Payoff, K=100, barrier=True, barrier_level=140), T=1)
-    print(option.ssp(10000, mode='JD'))
-    #20.33463726670842 z permutacją 11s, 20.536608834016505
-    print(option.LS(10000, mode = 'JD'))
-    #20.92430225200415 15s, 20.65867517809142
-    def double_max_put(sims_list, K):
-        return np.maximum(np.maximum(K - sims_list[0], K - sims_list[1]), 0)
-
-    option = Option(underlyings=(asset1, asset2), payoff_func=lambda trajectories: double_max_put(trajectories, 100), T=1)
-    option.european(10000)
-    option.ssp(10000, 'JD')
-    option.LS(10000, 'JD')
```

### Comparing `american_options-0.1.2/american_options/jump_diffusion.py` & `american_options-0.1.3/american_options/jump_diffusion.py`

 * *Files identical despite different names*

### Comparing `american_options-0.1.2/american_options/sobol.py` & `american_options-0.1.3/american_options/sobol.py`

 * *Files identical despite different names*

### Comparing `american_options-0.1.2/american_options/underlying.py` & `american_options-0.1.3/american_options/underlying.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,16 @@
         Creation of an asset
         >>> asset = Underlying(spot_price=100, r=0.06)
         >>> asset.calibrate_GBM(0.4, 255)
         """
         self.sigma = sigma
         self.values_per_year_GBM = values_per_year_GBM
         self.GBM_calibrated = True
+        self.ssp_calibrated=False
+
 
     def calibrate_Bootstrap(self, Historical_Data, values_per_year_Bootstrap=255):
         """
         Method needs to be called when one wants to simulate with Bootstrap
 
         Parameters
         ----------
@@ -68,14 +70,16 @@
         >>> asset.calibrate_Bootstrap(Historical_Data = hist_data, values_per_year_Bootstrap = 255)
 
         """
 
         self.Historical_Data = Historical_Data
         self.values_per_year_Bootstrap = values_per_year_Bootstrap
         self.Bootstrap_calibrated = True
+        self.ssp_calibrated=False
+
 
     def calibrate_RT_GBM(self, sigma, time_steps, successors):
         """
         Method needs to be called when one wants to simulate with random tree
 
         Parameters
         ----------
@@ -94,14 +98,15 @@
         >>> asset.calibrate_RT_GBM(0.4, 4, 3)
         """
 
         self.sigma = sigma
         self.time_steps = time_steps
         self.successors = successors
         self.RT_GBM_calibrated = True
+        self.ssp_calibrated=False
 
     def calibrate_JD(self, sigma, jump_intensity, values_per_year_JD=255, a=0.2, b=0.25):
         """
         Method needs to be called when one wants to simulate with jump-diffusion model \n
 
         Parameters a and b are chosen so that ln(Yi) ~ N(a, b^2),
         with Yi being random variable describing multiplicative jumps ($Yi = S_{\tau_i}/S_{\tau_i-}$)
@@ -128,14 +133,15 @@
 
         self.sigma = sigma
         self.jump_intensity = jump_intensity
         self.values_per_year_JD = values_per_year_JD
         self.a = a
         self.b = b
         self.JD_calibrated = True
+        self.ssp_calibrated=False
 
     def simulate(self, mode, size, T=1):
         """
         Method that simulates asset development paths used in pricing
 
         Parameters
         ----------
@@ -215,17 +221,18 @@
                 simulated_paths = np.zeros([size, ti + 1])
 
                 simulated_paths[:, 0] = self.spot_price
 
                 Z_1 = np.random.normal(size=[size, ti])
                 Z_2 = np.random.normal(size=[size, ti])
                 Poisson = np.random.poisson(l * dt, [size, ti])
+                drift = self.r - l * np.exp(self.a + self.b ** 2 / 2)
 
                 for i in range(ti):
-                    simulated_paths[:, i + 1] = simulated_paths[:, i] * np.exp((self.r - self.sigma ** 2 / 2) * dt +
+                    simulated_paths[:, i + 1] = simulated_paths[:, i] * np.exp((drift - self.sigma ** 2 / 2) * dt +
                                                                                self.sigma * np.sqrt(dt) * Z_1[:, i] + self.a * Poisson[:, i]
                                                                                + np.sqrt(self.b ** 2) * np.sqrt(Poisson[:, i]) * Z_2[:, i])
 
                 return pd.DataFrame(simulated_paths)
             else:
                 raise Exception(
                     "Jump diffusion model has not been calibrated yet. Calibrate it with calibrate_JD method first")
```

### Comparing `american_options-0.1.2/american_options.egg-info/PKG-INFO` & `american_options-0.1.3/american_options.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: american-options
-Version: 0.1.2
-Summary: library T-28h
+Version: 0.1.3
+Summary: Added new payoffs
 Home-page: https://american_options.readthedocs.io/
 Author: Przemysław Adamski, Katarzyna Hasal, Kacper Toczek
 Author-email: kat.hasal99@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `american_options-0.1.2/setup.py` & `american_options-0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # Get the long description on pypi from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="american_options",
-    version="0.1.2",
-    description="library T-28h",
+    version="0.1.3",
+    description="Added new payoffs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://american_options.readthedocs.io/",
     author="Przemysław Adamski, Katarzyna Hasal, Kacper Toczek",
     author_email="kat.hasal99@gmail.com",
     classifiers=[
         "Intended Audience :: Developers",
```

