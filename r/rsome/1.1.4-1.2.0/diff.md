# Comparing `tmp/rsome-1.1.4.tar.gz` & `tmp/rsome-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsome-1.1.4.tar", last modified: Wed Mar  1 06:00:11 2023, max compression
+gzip compressed data, was "rsome-1.2.0.tar", last modified: Sat Jun 17 16:43:27 2023, max compression
```

## Comparing `rsome-1.1.4.tar` & `rsome-1.2.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 pengxiong   (501) staff       (20)        0 2023-03-01 06:00:11.955330 rsome-1.1.4/
--rw-r--r--   0 pengxiong   (501) staff       (20)    35129 2022-11-30 14:30:50.000000 rsome-1.1.4/LICENSE.md
--rw-r--r--   0 pengxiong   (501) staff       (20)     6561 2023-03-01 06:00:11.955399 rsome-1.1.4/PKG-INFO
--rw-r--r--   0 pengxiong   (501) staff       (20)     6066 2023-03-01 05:32:39.000000 rsome-1.1.4/README.md
--rw-r--r--   0 pengxiong   (501) staff       (20)      516 2022-11-30 14:30:50.000000 rsome-1.1.4/pyproject.toml
-drwxr-xr-x   0 pengxiong   (501) staff       (20)        0 2023-03-01 06:00:11.954249 rsome-1.1.4/rsome/
--rw-r--r--   0 pengxiong   (501) staff       (20)      320 2023-02-02 06:05:31.000000 rsome-1.1.4/rsome/__init__.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     3154 2023-03-01 05:52:32.000000 rsome-1.1.4/rsome/clp_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     2028 2022-12-08 14:48:08.000000 rsome-1.1.4/rsome/cpt_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     2772 2022-11-30 14:30:50.000000 rsome-1.1.4/rsome/cpx_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     3654 2022-11-30 14:30:50.000000 rsome-1.1.4/rsome/cvx_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)    17467 2023-03-01 04:31:39.000000 rsome-1.1.4/rsome/deco.py
--rw-r--r--   0 pengxiong   (501) staff       (20)    36064 2023-03-01 04:27:19.000000 rsome-1.1.4/rsome/dro.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     3170 2022-11-30 14:30:50.000000 rsome-1.1.4/rsome/eco_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)    13247 2022-12-01 08:44:24.000000 rsome-1.1.4/rsome/gcp.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     2407 2023-03-01 04:32:16.000000 rsome-1.1.4/rsome/grb_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)   135312 2023-03-01 05:20:28.000000 rsome-1.1.4/rsome/lp.py
--rw-r--r--   0 pengxiong   (501) staff       (20)       33 2022-11-30 14:30:50.000000 rsome-1.1.4/rsome/lpg_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     7075 2023-03-01 05:23:03.000000 rsome-1.1.4/rsome/math.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     5159 2023-03-01 05:22:17.000000 rsome-1.1.4/rsome/msk_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     2270 2022-11-30 14:30:50.000000 rsome-1.1.4/rsome/ort_solver.py
--rw-r--r--   0 pengxiong   (501) staff       (20)        0 2022-11-30 14:30:50.000000 rsome-1.1.4/rsome/py.typed
--rw-r--r--   0 pengxiong   (501) staff       (20)    13760 2023-02-23 03:28:13.000000 rsome-1.1.4/rsome/ro.py
--rw-r--r--   0 pengxiong   (501) staff       (20)    12839 2023-03-01 05:25:34.000000 rsome-1.1.4/rsome/socp.py
--rw-r--r--   0 pengxiong   (501) staff       (20)     6833 2023-03-01 05:26:52.000000 rsome-1.1.4/rsome/subroutines.py
-drwxr-xr-x   0 pengxiong   (501) staff       (20)        0 2023-03-01 06:00:11.955213 rsome-1.1.4/rsome.egg-info/
--rw-r--r--   0 pengxiong   (501) staff       (20)     6561 2023-03-01 06:00:11.000000 rsome-1.1.4/rsome.egg-info/PKG-INFO
--rw-r--r--   0 pengxiong   (501) staff       (20)      552 2023-03-01 06:00:11.000000 rsome-1.1.4/rsome.egg-info/SOURCES.txt
--rw-r--r--   0 pengxiong   (501) staff       (20)        1 2023-03-01 06:00:11.000000 rsome-1.1.4/rsome.egg-info/dependency_links.txt
--rw-r--r--   0 pengxiong   (501) staff       (20)        1 2023-03-01 06:00:11.000000 rsome-1.1.4/rsome.egg-info/not-zip-safe
--rw-r--r--   0 pengxiong   (501) staff       (20)      115 2023-03-01 06:00:11.000000 rsome-1.1.4/rsome.egg-info/requires.txt
--rw-r--r--   0 pengxiong   (501) staff       (20)        6 2023-03-01 06:00:11.000000 rsome-1.1.4/rsome.egg-info/top_level.txt
--rw-r--r--   0 pengxiong   (501) staff       (20)      792 2023-03-01 06:00:11.955681 rsome-1.1.4/setup.cfg
--rw-r--r--   0 pengxiong   (501) staff       (20)      180 2022-11-30 14:30:50.000000 rsome-1.1.4/setup.py
+drwxr-xr-x   0 pengxiong   (501) staff       (20)        0 2023-06-17 16:43:27.169816 rsome-1.2.0/
+-rw-r--r--   0 pengxiong   (501) staff       (20)    35129 2022-11-30 14:30:50.000000 rsome-1.2.0/LICENSE.md
+-rw-r--r--   0 pengxiong   (501) staff       (20)     6536 2023-06-17 16:43:27.169880 rsome-1.2.0/PKG-INFO
+-rw-r--r--   0 pengxiong   (501) staff       (20)     6040 2023-06-16 07:09:38.000000 rsome-1.2.0/README.md
+-rw-r--r--   0 pengxiong   (501) staff       (20)      473 2023-06-17 15:52:57.000000 rsome-1.2.0/pyproject.toml
+drwxr-xr-x   0 pengxiong   (501) staff       (20)        0 2023-06-17 16:43:27.168999 rsome-1.2.0/rsome/
+-rw-r--r--   0 pengxiong   (501) staff       (20)      257 2023-06-07 02:43:40.000000 rsome-1.2.0/rsome/__init__.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     3386 2023-06-17 09:22:45.000000 rsome-1.2.0/rsome/clp_solver.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     4305 2023-06-17 09:24:10.000000 rsome-1.2.0/rsome/cpt_solver.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     2097 2023-06-09 02:04:06.000000 rsome-1.2.0/rsome/cpt_solver_bkp.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     3429 2023-06-17 09:25:07.000000 rsome-1.2.0/rsome/cpx_solver.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)    23484 2023-06-17 10:02:53.000000 rsome-1.2.0/rsome/deco.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)    36908 2023-06-17 09:33:47.000000 rsome-1.2.0/rsome/dro.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     3834 2023-06-17 09:34:22.000000 rsome-1.2.0/rsome/eco_solver.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)    22329 2023-06-17 10:04:18.000000 rsome-1.2.0/rsome/gcp.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     2972 2023-06-17 09:40:05.000000 rsome-1.2.0/rsome/grb_solver.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)   151192 2023-06-17 10:06:04.000000 rsome-1.2.0/rsome/lp.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)       33 2022-11-30 14:30:50.000000 rsome-1.2.0/rsome/lpg_solver.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)    10059 2023-06-17 10:08:04.000000 rsome-1.2.0/rsome/math.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     5379 2023-06-17 12:34:04.000000 rsome-1.2.0/rsome/msk_solver.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     2459 2023-06-09 02:08:38.000000 rsome-1.2.0/rsome/ort_solver.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)        0 2022-11-30 14:30:50.000000 rsome-1.2.0/rsome/py.typed
+-rw-r--r--   0 pengxiong   (501) staff       (20)    15521 2023-06-17 12:35:57.000000 rsome-1.2.0/rsome/ro.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)    12862 2023-06-01 07:57:25.000000 rsome-1.2.0/rsome/socp.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)     7571 2023-06-17 10:12:56.000000 rsome-1.2.0/rsome/subroutines.py
+-rw-r--r--   0 pengxiong   (501) staff       (20)      990 2023-06-17 10:13:09.000000 rsome-1.2.0/rsome/this.py
+drwxr-xr-x   0 pengxiong   (501) staff       (20)        0 2023-06-17 16:43:27.169703 rsome-1.2.0/rsome.egg-info/
+-rw-r--r--   0 pengxiong   (501) staff       (20)     6536 2023-06-17 16:43:26.000000 rsome-1.2.0/rsome.egg-info/PKG-INFO
+-rw-r--r--   0 pengxiong   (501) staff       (20)      570 2023-06-17 16:43:27.000000 rsome-1.2.0/rsome.egg-info/SOURCES.txt
+-rw-r--r--   0 pengxiong   (501) staff       (20)        1 2023-06-17 16:43:26.000000 rsome-1.2.0/rsome.egg-info/dependency_links.txt
+-rw-r--r--   0 pengxiong   (501) staff       (20)        1 2023-06-17 16:43:26.000000 rsome-1.2.0/rsome.egg-info/not-zip-safe
+-rw-r--r--   0 pengxiong   (501) staff       (20)      115 2023-06-17 16:43:27.000000 rsome-1.2.0/rsome.egg-info/requires.txt
+-rw-r--r--   0 pengxiong   (501) staff       (20)        6 2023-06-17 16:43:27.000000 rsome-1.2.0/rsome.egg-info/top_level.txt
+-rw-r--r--   0 pengxiong   (501) staff       (20)      823 2023-06-17 16:43:27.170163 rsome-1.2.0/setup.cfg
+-rw-r--r--   0 pengxiong   (501) staff       (20)      180 2022-11-30 14:30:50.000000 rsome-1.2.0/setup.py
```

### Comparing `rsome-1.1.4/LICENSE.md` & `rsome-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rsome-1.1.4/PKG-INFO` & `rsome-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: rsome
-Version: 1.1.4
+Version: 1.2.0
 Summary: Robust Stochastic Optimization Made Easy
 Author: Peng Xiong
 License: GPL-3.0
 Platform: linux
 Platform: osx
 Platform: win64
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.md
 
 <img src="https://github.com/XiongPengNUS/rsome/blob/master/rsologo.png?raw=true" width=100>
 
 # RSOME: Robust Stochastic Optimization Made Easy
@@ -27,15 +27,15 @@
 [![tests](https://github.com/XiongPengNUS/rsome/actions/workflows/test.yml/badge.svg)](https://github.com/XiongPengNUS/rsome/actions/workflows/test.yml)
 [![Docs](https://github.com/XiongPengNUS/rsome/actions/workflows/pages/pages-build-deployment/badge.svg?label=Docs)](https://github.com/XiongPengNUS/rsome/actions/workflows/pages/pages-build-deployment)
 [![Project Status: Active - The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed/XiongPengNUS/rsome)
 ![GitHub issues](https://img.shields.io/github/issues-raw/XiongPengNUS/rsome)
 
 - Website: [RSOME for Python](https://xiongpengnus.github.io/rsome/)
-- PyPI: [RSOME 1.1.4](https://pypi.org/project/rsome/)
+- PyPI: [RSOME 1.2.0](https://pypi.org/project/rsome/)
 
 RSOME (Robust Stochastic Optimization Made Easy) is an open-source Python package for generic modeling of optimization problems (subject to uncertainty). Models in RSOME are constructed by variables, constraints, and expressions that are formatted as N-dimensional arrays. These arrays are consistent with the NumPy library in terms of syntax and operations, including broadcasting, indexing, slicing, element-wise operations, and matrix calculation rules, among others. In short, RSOME provides a convenient platform to facilitate developments of robust optimization models and their applications.
 
 ## Content
 
 - [Installation](#section2)
 - [Solver interfaces](#section3)
@@ -48,26 +48,26 @@
 The RSOME package can be installed by using the <code>pip</code> command:
 ***
 **`pip install rsome`**
 ***
 
 ### Solver interfaces <a id="section3"></a>
 
-The RSOME package transforms robust or distributionally robust optimization models into deterministic second-order cone or exponential cone programming problems, and solved by external solvers. Details of compatible solvers and their interfaces are presented in the following table.
+The RSOME package transforms robust or distributionally robust optimization models into deterministic linear or conic programming problems, and solved by external solvers. Details of compatible solvers and their interfaces are presented in the following table.
 
-| Solver | License  type | Required version | RSOME interface |Integrality constraints| Second-order cone constraints| Exponential cone constraints
+| Solver | License  type | Required version | RSOME interface | Second-order cone constraints| Exponential cone constraints | Semidefiniteness constraints
 |:-------|:--------------|:-----------------|:----------------|:------------------------|:---------------------|:--------------|
-|[scipy.optimize](https://docs.scipy.org/doc/scipy/reference/optimize.html)| Open-source | >= 1.2.1 | `lpg_solver` | Yes for 1.9.0 or above | No | No |
-|[CyLP](https://github.com/coin-or/cylp)| Open-source | >= 0.9.0 | `clp_solver` | Yes | No | No |
-|[OR-Tools](https://developers.google.com/optimization/install) | Open-source | >= 7.5.7466 | `ort_solver` | Yes | No | No |
-|[ECOS](https://github.com/embotech/ecos-python) | Open-source | >= 2.0.10 | `eco_solver` | Yes | Yes | Yes |
-|[Gurobi](https://www.gurobi.com/documentation/9.0/quickstart_mac/ins_the_anaconda_python_di.html)| Commercial | >= 9.1.0 | `grb_solver` | Yes | Yes | No |
-|[MOSEK](https://docs.mosek.com/9.2/pythonapi/install-interface.html) | Commercial | >= 9.1.11 | `msk_solver` | Yes | Yes | Yes |
-|[CPLEX](https://www.ibm.com/support/knowledgecenter/en/SSSA5P_12.8.0/ilog.odms.cplex.help/CPLEX/GettingStarted/topics/set_up/Python_setup.html) | Commercial | >= 12.9.0.0 | `cpx_solver` | Yes | Yes | No |
-|[COPT](https://www.shanshu.ai/copt) | Commercial | >= 5.0.1 | `cpt_solver` | Yes | Yes | No |
+|[scipy.optimize](https://docs.scipy.org/doc/scipy/reference/optimize.html)| Open-source | >= 1.9.0 | `lpg_solver` | No | No | No |
+|[CyLP](https://github.com/coin-or/cylp)| Open-source | >= 0.9.0 | `clp_solver` | No | No | No |
+|[OR-Tools](https://developers.google.com/optimization/install) | Open-source | >= 7.5.7466 | `ort_solver` | No | No | No |
+|[ECOS](https://github.com/embotech/ecos-python) | Open-source | >= 2.0.10 | `eco_solver` | Yes | Yes | No |
+|[Gurobi](https://www.gurobi.com/documentation/9.0/quickstart_mac/ins_the_anaconda_python_di.html)| Commercial | >= 9.1.0 | `grb_solver` | Yes | No | No |
+|[Mosek](https://docs.mosek.com/9.2/pythonapi/install-interface.html) | Commercial | >= 10.0.44 | `msk_solver` | Yes | Yes | Yes |
+|[CPLEX](https://www.ibm.com/support/knowledgecenter/en/SSSA5P_12.8.0/ilog.odms.cplex.help/CPLEX/GettingStarted/topics/set_up/Python_setup.html) | Commercial | >= 12.9.0.0 | `cpx_solver` | Yes | No | No |
+|[COPT](https://www.shanshu.ai/copt) | Commercial | >= 6.5.3 | `cpt_solver` | Yes | No | No |
 
 ## Getting started <a id="section4"></a>
 
 Documents of RSOME are provided as follows:
 - [RSOME quick start](https://xiongpengnus.github.io/rsome/)
 - [RSOME users guide](https://xiongpengnus.github.io/rsome/user_guide)
 - [Application examples](https://xiongpengnus.github.io/rsome/examples)
@@ -76,26 +76,29 @@
 
 RSOME is a software project supported by Singapore Ministry of Education Tier 3 Grant *Science of Prescriptive Analytics*. It is primarly developed and maintained by [Zhi Chen](https://www.cb.cityu.edu.hk/staff/zchen96/), [Melvyn Sim](https://bizfaculty.nus.edu.sg/faculty-details/?profId=127), and [Peng Xiong](https://bizfaculty.nus.edu.sg/faculty-details/?profId=543). Many other researchers, including Erick Delage, Zhaowei Hao, Long He, Zhenyu Hu, Jun Jiang, Brad Sturt, Qinshen Tang, as well as anonymous users and paper reviewers, have helped greatly in the way of developing RSOME.
 
 ## Citation <a id="section6">
 
 If you use RSOME in your research, please cite our papers:
 
-- Chen, Zhi, and Peng Xiong. 2021. [RSOME in Python: an open-source package for robust stochastic optimization made easy](http://www.optimization-online.org/DB_HTML/2021/06/8443.html). <i>Optimization Online</i>.
+- Chen, Zhi, and Peng Xiong. 2023. [RSOME in Python: an open-source package for robust stochastic optimization made easy](https://pubsonline.informs.org/doi/abs/10.1287/ijoc.2023.1291). Forthcoming in <i>INFORMS Journal on Computing</i>.
 
-- Chen, Zhi, Melvyn Sim, Peng Xiong. 2020. [Robust stochastic optimization made easy with RSOME](https://pubsonline.informs.org/doi/abs/10.1287/mnsc.2020.3603). <i>Management Science</i> <b>66</b>(8) 3329–3339.
+- Chen, Zhi, Melvyn Sim, Peng Xiong. 2020. [Robust stochastic optimization made easy with RSOME](https://pubsonline.informs.org/doi/abs/10.1287/mnsc.2020.3603). <i>Management Science</i> <b>66</b>(8) 3329-3339.
 
 Bibtex entry:
 
 ```
 @article{chen2021rsome,
   title={RSOME in Python: an open-source package for robust stochastic optimization made easy},
   author={Chen, Zhi and Xiong, Peng},
-  journal={Optimization Online. URL: http://www.optimization-online.org/DB_HTML/2021/06/8443.html},
-  year={2021},
+  journal={INFORMS Journal on Computing},
+  year={2023},
+  month={Mar},
+  day={30},
+  publisher={INFORMS}
 }
 ```
 
 ```
 @article{chen2020robust,
   title={Robust stochastic optimization made easy with RSOME},
   author={Chen, Zhi and Sim, Melvyn and Xiong, Peng},
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rsome-1.1.4/README.md` & `rsome-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [![tests](https://github.com/XiongPengNUS/rsome/actions/workflows/test.yml/badge.svg)](https://github.com/XiongPengNUS/rsome/actions/workflows/test.yml)
 [![Docs](https://github.com/XiongPengNUS/rsome/actions/workflows/pages/pages-build-deployment/badge.svg?label=Docs)](https://github.com/XiongPengNUS/rsome/actions/workflows/pages/pages-build-deployment)
 [![Project Status: Active - The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed/XiongPengNUS/rsome)
 ![GitHub issues](https://img.shields.io/github/issues-raw/XiongPengNUS/rsome)
 
 - Website: [RSOME for Python](https://xiongpengnus.github.io/rsome/)
-- PyPI: [RSOME 1.1.4](https://pypi.org/project/rsome/)
+- PyPI: [RSOME 1.2.0](https://pypi.org/project/rsome/)
 
 RSOME (Robust Stochastic Optimization Made Easy) is an open-source Python package for generic modeling of optimization problems (subject to uncertainty). Models in RSOME are constructed by variables, constraints, and expressions that are formatted as N-dimensional arrays. These arrays are consistent with the NumPy library in terms of syntax and operations, including broadcasting, indexing, slicing, element-wise operations, and matrix calculation rules, among others. In short, RSOME provides a convenient platform to facilitate developments of robust optimization models and their applications.
 
 ## Content
 
 - [Installation](#section2)
 - [Solver interfaces](#section3)
@@ -30,26 +30,26 @@
 The RSOME package can be installed by using the <code>pip</code> command:
 ***
 **`pip install rsome`**
 ***
 
 ### Solver interfaces <a id="section3"></a>
 
-The RSOME package transforms robust or distributionally robust optimization models into deterministic second-order cone or exponential cone programming problems, and solved by external solvers. Details of compatible solvers and their interfaces are presented in the following table.
+The RSOME package transforms robust or distributionally robust optimization models into deterministic linear or conic programming problems, and solved by external solvers. Details of compatible solvers and their interfaces are presented in the following table.
 
-| Solver | License  type | Required version | RSOME interface |Integrality constraints| Second-order cone constraints| Exponential cone constraints
+| Solver | License  type | Required version | RSOME interface | Second-order cone constraints| Exponential cone constraints | Semidefiniteness constraints
 |:-------|:--------------|:-----------------|:----------------|:------------------------|:---------------------|:--------------|
-|[scipy.optimize](https://docs.scipy.org/doc/scipy/reference/optimize.html)| Open-source | >= 1.2.1 | `lpg_solver` | Yes for 1.9.0 or above | No | No |
-|[CyLP](https://github.com/coin-or/cylp)| Open-source | >= 0.9.0 | `clp_solver` | Yes | No | No |
-|[OR-Tools](https://developers.google.com/optimization/install) | Open-source | >= 7.5.7466 | `ort_solver` | Yes | No | No |
-|[ECOS](https://github.com/embotech/ecos-python) | Open-source | >= 2.0.10 | `eco_solver` | Yes | Yes | Yes |
-|[Gurobi](https://www.gurobi.com/documentation/9.0/quickstart_mac/ins_the_anaconda_python_di.html)| Commercial | >= 9.1.0 | `grb_solver` | Yes | Yes | No |
-|[MOSEK](https://docs.mosek.com/9.2/pythonapi/install-interface.html) | Commercial | >= 9.1.11 | `msk_solver` | Yes | Yes | Yes |
-|[CPLEX](https://www.ibm.com/support/knowledgecenter/en/SSSA5P_12.8.0/ilog.odms.cplex.help/CPLEX/GettingStarted/topics/set_up/Python_setup.html) | Commercial | >= 12.9.0.0 | `cpx_solver` | Yes | Yes | No |
-|[COPT](https://www.shanshu.ai/copt) | Commercial | >= 5.0.1 | `cpt_solver` | Yes | Yes | No |
+|[scipy.optimize](https://docs.scipy.org/doc/scipy/reference/optimize.html)| Open-source | >= 1.9.0 | `lpg_solver` | No | No | No |
+|[CyLP](https://github.com/coin-or/cylp)| Open-source | >= 0.9.0 | `clp_solver` | No | No | No |
+|[OR-Tools](https://developers.google.com/optimization/install) | Open-source | >= 7.5.7466 | `ort_solver` | No | No | No |
+|[ECOS](https://github.com/embotech/ecos-python) | Open-source | >= 2.0.10 | `eco_solver` | Yes | Yes | No |
+|[Gurobi](https://www.gurobi.com/documentation/9.0/quickstart_mac/ins_the_anaconda_python_di.html)| Commercial | >= 9.1.0 | `grb_solver` | Yes | No | No |
+|[Mosek](https://docs.mosek.com/9.2/pythonapi/install-interface.html) | Commercial | >= 10.0.44 | `msk_solver` | Yes | Yes | Yes |
+|[CPLEX](https://www.ibm.com/support/knowledgecenter/en/SSSA5P_12.8.0/ilog.odms.cplex.help/CPLEX/GettingStarted/topics/set_up/Python_setup.html) | Commercial | >= 12.9.0.0 | `cpx_solver` | Yes | No | No |
+|[COPT](https://www.shanshu.ai/copt) | Commercial | >= 6.5.3 | `cpt_solver` | Yes | No | No |
 
 ## Getting started <a id="section4"></a>
 
 Documents of RSOME are provided as follows:
 - [RSOME quick start](https://xiongpengnus.github.io/rsome/)
 - [RSOME users guide](https://xiongpengnus.github.io/rsome/user_guide)
 - [Application examples](https://xiongpengnus.github.io/rsome/examples)
@@ -58,26 +58,29 @@
 
 RSOME is a software project supported by Singapore Ministry of Education Tier 3 Grant *Science of Prescriptive Analytics*. It is primarly developed and maintained by [Zhi Chen](https://www.cb.cityu.edu.hk/staff/zchen96/), [Melvyn Sim](https://bizfaculty.nus.edu.sg/faculty-details/?profId=127), and [Peng Xiong](https://bizfaculty.nus.edu.sg/faculty-details/?profId=543). Many other researchers, including Erick Delage, Zhaowei Hao, Long He, Zhenyu Hu, Jun Jiang, Brad Sturt, Qinshen Tang, as well as anonymous users and paper reviewers, have helped greatly in the way of developing RSOME.
 
 ## Citation <a id="section6">
 
 If you use RSOME in your research, please cite our papers:
 
-- Chen, Zhi, and Peng Xiong. 2021. [RSOME in Python: an open-source package for robust stochastic optimization made easy](http://www.optimization-online.org/DB_HTML/2021/06/8443.html). <i>Optimization Online</i>.
+- Chen, Zhi, and Peng Xiong. 2023. [RSOME in Python: an open-source package for robust stochastic optimization made easy](https://pubsonline.informs.org/doi/abs/10.1287/ijoc.2023.1291). Forthcoming in <i>INFORMS Journal on Computing</i>.
 
-- Chen, Zhi, Melvyn Sim, Peng Xiong. 2020. [Robust stochastic optimization made easy with RSOME](https://pubsonline.informs.org/doi/abs/10.1287/mnsc.2020.3603). <i>Management Science</i> <b>66</b>(8) 3329–3339.
+- Chen, Zhi, Melvyn Sim, Peng Xiong. 2020. [Robust stochastic optimization made easy with RSOME](https://pubsonline.informs.org/doi/abs/10.1287/mnsc.2020.3603). <i>Management Science</i> <b>66</b>(8) 3329-3339.
 
 Bibtex entry:
 
 ```
 @article{chen2021rsome,
   title={RSOME in Python: an open-source package for robust stochastic optimization made easy},
   author={Chen, Zhi and Xiong, Peng},
-  journal={Optimization Online. URL: http://www.optimization-online.org/DB_HTML/2021/06/8443.html},
-  year={2021},
+  journal={INFORMS Journal on Computing},
+  year={2023},
+  month={Mar},
+  day={30},
+  publisher={INFORMS}
 }
 ```
 
 ```
 @article{chen2020robust,
   title={Robust stochastic optimization made easy with RSOME},
   author={Chen, Zhi and Sim, Melvyn and Xiong, Peng},
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rsome-1.1.4/rsome/clp_solver.py` & `rsome-1.2.0/rsome/clp_solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 
     try:
         if formula.xmat:
             warnings.warn('The LP solver ignores exponential cone constraints.')
     except AttributeError:
         pass
 
+    try:
+        if formula.lmi:
+            warnings.warn('The LP solver ignores semidefinite cone constraints.')
+    except AttributeError:
+        pass
+
     obj = formula.obj.flatten()
     linear = formula.linear
     sense = formula.sense
     const = formula.const
     ub = formula.ub
     lb = formula.lb
     vtype = formula.vtype
@@ -87,15 +93,15 @@
             left += ineq_linear[:, is_int] * iv
         if nbv:
             left += ineq_linear[:, is_bin] * bv
 
         s += (left <= ineq_const)
 
     cbcModel = s.getCbcModel()
-    s.writeLp('blah.lp')
+    # s.writeLp('blah.lp')
 
     if display:
         print('Being solved by CyLP...', flush=True)
         time.sleep(0.2)
     t0 = time.time()
     # status = s.primal()
     cbcModel.solve()
@@ -110,14 +116,14 @@
         if ncv:
             x_sol[is_con] = cbcModel.primalVariableSolution['cv']
         if niv:
             x_sol[is_int] = cbcModel.primalVariableSolution['iv']
         if nbv:
             x_sol[is_bin] = cbcModel.primalVariableSolution['bv']
 
-        solution = Solution(cbcModel.objectiveValue, x_sol, status, stime)
-
+        solution = Solution('CyLP', cbcModel.objectiveValue, x_sol, status, stime)
     else:
         warnings.warn('Fail to find the optimal solution.')
-        solution = None
+        # solution = None
+        solution = Solution('CyLP', np.nan, None, status, stime)
 
     return solution
```

### Comparing `rsome-1.1.4/rsome/cpt_solver.py` & `rsome-1.2.0/rsome/cpt_solver_bkp.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         pass
 
     env = cp.Envr()
     m = env.createModel()
     m.setParam(cp.COPT.Param.Logging, False)
     m.setParam(cp.COPT.Param.LogToConsole, False)
 
-    c = formula.obj[0]
+    c = formula.obj
     A = formula.linear
     vtype = formula.vtype
     lhs = np.array([-cp.COPT.INFINITY]*formula.linear.shape[0])
     index_eq = formula.sense == 1
     lhs[index_eq] = formula.const[index_eq]
     rhs = formula.const
 
@@ -62,14 +62,15 @@
         status = m.getAttr(cp.COPT.attr.MipStatus)
     if display:
         print('Solution status: {0}'.format(status))
         print('Running time: {0:0.4f}s'.format(stime))
 
     try:
         x_sol = np.array(m.getValues())
-        objval = formula.obj[0] @ x_sol
-        solution = Solution(objval, x_sol, status, stime)
+        objval = formula.obj @ x_sol
+        solution = Solution('COPT', objval, x_sol, status, stime)
     except cp.CoptError:
         warnings.warn('Fail to find the optimal solution.')
-        solution = None
+        # solution = None
+        solution = Solution('COPT', np.nan, None, status, stime)
 
     return solution
```

### Comparing `rsome-1.1.4/rsome/cpx_solver.py` & `rsome-1.2.0/rsome/cpx_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,35 +12,37 @@
 
 
 def solve(formula, display=True, params={}):
 
     try:
         if formula.xmat:
             warnings.warn('The SOCP solver ignores exponential cone constraints. ')
+        if formula.lmi:
+            warnings.warn('The SOCP solver ignores semidefinite cone constraints. ')
     except AttributeError:
         pass
 
     cpx = cplex.Cplex()
 
     # obj = formula.obj.flatten()
     linear = formula.linear
-    row = linear.shape[0]
+    row, col = linear.shape
     spmat = [[linear.indices[linear.indptr[i]:linear.indptr[i + 1]].tolist(),
               linear.data[linear.indptr[i]:linear.indptr[i + 1]].tolist()]
              for i in range(row)]
     sense = ['E' if s == 1 else 'L' for s in formula.sense]
     vtype = [cpx.variables.type.integer if vt == 'I' else
              cpx.variables.type.binary if vt == 'B' else
              cpx.variables.type.continuous for vt in formula.vtype]
 
     if all(np.array(vtype) == cpx.variables.type.continuous):
-        cpx.variables.add(obj=formula.obj.flatten(),
+        cpx.variables.add(obj=formula.obj,
                           lb=formula.lb, ub=formula.ub)
     else:
-        cpx.variables.add(obj=formula.obj.flatten(),
+        cpx.variables.add(obj=formula.obj,
                           lb=formula.lb, ub=formula.ub, types=vtype)
     cpx.linear_constraints.add(lin_expr=spmat,
                                senses=sense, rhs=formula.const)
 
     if isinstance(formula, SOCProg):
         for cone in formula.qmat:
             cone_data = [-1] + [1] * (len(cone) - 1)
@@ -61,22 +63,36 @@
     except (TypeError, ValueError, AttributeError):
         raise ValueError('Incorrect parameters or values.')
 
     t0 = time.time()
     cpx.solve()
     stime = time.time() - t0
     status = cpx.solution.get_status()
+    status_string = cpx.solution.get_status_string()
     if display:
-        print('Solution status: {0}'.format(status))
+        print('Solution status: {0}'.format(status_string))
         print('Running time: {0:0.4f}s'.format(stime))
 
     if status in [1, 6, 10, 11, 12, 13,
                   21, 22,
                   101, 102, 105, 107, 109, 111, 113, 116]:
         obj_val = cpx.solution.get_objective_value()
         x_sol = np.array(cpx.solution.get_values())
-        solution = Solution(obj_val, x_sol, status, stime)
+
+        if all(np.array(vtype) == cpx.variables.type.continuous):
+            pi = np.array(cpx.solution.get_dual_values())
+            upi = np.zeros(col)
+            lpi = np.zeros(col)
+            rc = np.array(cpx.solution.get_reduced_costs())
+            upi[rc < 0] = rc[rc < 0]
+            lpi[rc > 0] = rc[rc > 0]
+            y = {'pi': pi, 'upi': upi, 'lpi': lpi}
+        else:
+            y = None
+
+        solution = Solution('CPLEX', obj_val, x_sol, status_string, stime, y=y)
     else:
         warnings.warn('Fail to find the optimal solution.')
-        solution = None
+        # solution = None
+        solution = Solution('CPLEX', np.nan, None, status_string, stime)
 
     return solution
```

### Comparing `rsome-1.1.4/rsome/deco.py` & `rsome-1.2.0/rsome/ro.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,517 +1,486 @@
 from .gcp import Model as GCPModel
-from .gcp import GCProg
-from .lp import LinConstr, Bounds, CvxConstr, ExpConstr
+from .lp import LinConstr, Bounds, CvxConstr, ConeConstr, ExpConstr, KLConstr, LMIConstr
 from .lp import Vars, VarSub, Affine, Convex
-from .lp import def_sol
-from .socp import Model as SOCModel
-from .socp import SOCProg
-from collections.abc import Iterable
-from numbers import Real
-from scipy.sparse import csr_matrix
-
+from .lp import DecRule
+from .lp import RoAffine, RoConstr
+from .lp import PiecewiseConvex, PWConstr
+from .lp import Solution, def_sol
 import numpy as np
-import scipy.sparse as sp
+from numbers import Real
+from collections.abc import Iterable
+# from .subroutines import *
 
 
 class Model:
+    """
+    The Model class creates an object of robust optimization models
+    """
 
     def __init__(self, name=None):
 
-        self.master = GCPModel(nobj=False, mtype='R', name=name, top=self)
-        self.here_now_index = []
-        self.wait_see_index = []
-        self.all_here_now_index = []
-        self.rand_index = []
-
-        self.subs = []
+        self.rc_model = GCPModel(mtype='R', top=self)
+        self.sup_model = GCPModel(nobj=True, mtype='S', top=self)
 
-        self.exact_bounds = []
-        self.relaxed_bounds = []
-        self.solutions = []
+        self.all_constr = []
 
-    def dvar(self, shape=(), vtype='C', name=None):
+        self.obj = None
+        self.obj_support = None
+        self.sign = 1
 
-        new_var = self.master.dvar(shape, vtype, name, aux=False)
-        index = range(new_var.first, new_var.last)
-        self.here_now_index.extend(index)
+        self.primal = None
+        self.dual = None
+        self.solution = None
+        self.pupdate = True
+        self.dupdate = True
+
+        self.solution = None
+
+        self.name = name
+
+    def reset(self):
+
+        self.all_constr = []
+        self.pupdate = True
+        self.dupdate = True
+        self.primal = None
+        self.dual = None
+        self.rc_model.reset()
+
+    def dvar(self, shape=(), vtype='C', name=None, aux=False):
+        """
+        Returns an array of decision variables with the given shape
+        and variable type.
+
+        Parameters
+        ----------
+        shape : int or tuple
+            Shape of the variable array. The variable is a scalar if
+            the shape is unspecified.
+        vtype : {'C', 'B', 'I'}
+            Type of the decision variables. 'C' means continuous; 'B'
+            means binary, and 'I" means integer.
+        name : str
+            Name of the variable array
+        aux : leave it unspecified.
+
+        Returns
+        -------
+        new_var : rsome.lp.Vars
+            An array of new decision variables
+        """
 
-        return HaNVar(new_var)
+        new_var = self.rc_model.dvar(shape, vtype, name, aux)
+        return new_var
 
     def rvar(self, shape=(), name=None):
 
-        new_var = self.master.dvar(shape, 'C', name, aux=False)
-        index = range(new_var.first, new_var.last)
-        self.rand_index.extend(index)
+        """
+        Returns an array of random variables with the given shape.
 
-        return RandVar(new_var)
+        Parameters
+        ----------
+        shape : int or tuple
+            Shape of the variable array.
+        name : str
+            Name of the variable array
+
+        Returns
+        -------
+        new_var : rsome.lp.Vars
+            An array of new random variables
+        """
 
-    def min(self, obj):
-
-        if isinstance(obj, (Vars, VarSub, Affine)):
-            affine = obj.to_affine()
-            if affine.linear[:, self.wait_see_index].nnz > 0:
-                msg = 'No wait-and-see decision is allowed in master problem objective.'
-                raise ValueError(msg)
-            if affine.linear[:, self.rand_index].nnz > 0:
-                msg = 'No random variable is allowed in master problem objective.'
-                raise ValueError(msg)
-        elif isinstance(obj, Convex):
-            cond1 = obj.affine_in.linear[:, self.wait_see_index].nnz > 0
-            cond2 = obj.affine_out.linear[:, self.wait_see_index].nnz > 0
-            if cond1 or cond2:
-                msg = 'No wait-and-see decision is allowed in master problem objective.'
-                raise ValueError(msg)
-            cond1 = obj.affine_in.linear[:, self.rand_index].nnz > 0
-            cond2 = obj.affine_out.linear[:, self.rand_index].nnz > 0
-            if cond1 or cond2:
-                msg = 'No random variable is allowed in master problem objective.'
-                raise ValueError(msg)
-        else:
-            raise TypeError('Unsupported objective function.')
-
-        self.master.min(obj)
+        new_var = self.sup_model.dvar(shape, 'C', name)
+        return new_var
 
-    def max(self, obj):
+    def ldr(self, shape=(), name=None):
 
-        if isinstance(obj, (Vars, VarSub, Affine)):
-            affine = obj.to_affine()
-            if affine.linear[:, self.wait_see_index].nnz > 0:
-                msg = 'No wait-and-see decision is allowed in master problem objective.'
-                raise ValueError(msg)
-            if affine.linear[:, self.rand_index].nnz > 0:
-                msg = 'No random variable is allowed in master problem objective.'
-                raise ValueError(msg)
-        elif isinstance(obj, Convex):
-            cond1 = obj.affine_in.linear[:, self.wait_see_index].nnz > 0
-            cond2 = obj.affine_out.linear[:, self.wait_see_index].nnz > 0
-            if cond1 or cond2:
-                msg = 'No wait-and-see decision is allowed in master problem objective.'
-                raise ValueError(msg)
-            cond1 = obj.affine_in.linear[:, self.rand_index].nnz > 0
-            cond2 = obj.affine_out.linear[:, self.rand_index].nnz > 0
-            if cond1 or cond2:
-                msg = 'No random variable is allowed in master problem objective.'
-                raise ValueError(msg)
-        else:
-            raise TypeError('Unsupported objective function.')
+        """
+        Returns an array with the given shape of linear decision rule
+        variables.
+
+        Parameters
+        ----------
+        shape : int or tuple
+            Shape of the variable array.
+        name : str
+            Name of the variable array
+
+        Returns
+        -------
+        new_var : rsome.ro.DecRule
+            An array of new linear decision rule variables
+        """
 
-        self.master.max(obj)
+        new_ldr = DecRule(self, shape, name)
+        return new_ldr
 
-    def st(self, *arg):
+    def min(self, obj):
+        """
+        Minimize the given objective function.
 
-        for constr in arg:
-            if isinstance(constr, Iterable):
-                for item in constr:
-                    self.st(item)
+        Parameters
+        ----------
+        obj : RSOME expression, numeric constant
+            An objective function
+
+        Notes
+        -----
+        The objective function given as an array must have the size
+        to be one.
+        """
+
+        if self.obj is not None:
+            raise SyntaxError('Redefinition of the objective is not allowed.')
+
+        if not isinstance(obj, (Real, PiecewiseConvex)):
+            if isinstance(obj, VarSub):
+                if obj.indices.size > 1:
+                    raise ValueError('Incorrect function dimension.')
             else:
-                if isinstance(constr, LinConstr):
-                    if constr.linear[:, self.wait_see_index].nnz > 0:
-                        msg = 'No wait-and-see decision is allowed in master problem.'
-                        raise ValueError(msg)
-                    if constr.linear[:, self.rand_index].nnz > 0:
-                        msg = 'No random variable is allowed in master problem.'
-                        raise ValueError(msg)
-
-                elif isinstance(constr, CvxConstr):
-                    cond1 = constr.affine_in.linear[:, self.wait_see_index].nnz > 0
-                    cond2 = constr.affine_out.linear[:, self.wait_see_index].nnz > 0
-                    if cond1 or cond2:
-                        msg = 'No wait-and-see decision is allowed in master problem.'
-                        raise ValueError(msg)
-                    cond1 = constr.affine_in.linear[:, self.rand_index].nnz > 0
-                    cond2 = constr.affine_out.linear[:, self.rand_index].nnz > 0
-                    if cond1 or cond2:
-                        msg = 'No random variable is allowed in master problem.'
-                        raise ValueError(msg)
-
-                elif isinstance(constr, Bounds):
-                    if set(constr.indices).intersection(self.wait_see_index):
-                        msg = 'No wait-and-see decision is allowed in master problem.'
-                        raise ValueError(msg)
-                    if set(constr.indices).intersection(self.rand_index):
-                        msg = 'No random variable is allowed in master problem.'
-                        raise ValueError(msg)
-
-                elif isinstance(constr, ExpConstr):
-                    print('TODO!')
-                    raise ValueError('Not yet.')
-
-                else:
-                    raise TypeError('Unsupported constraints.')
-
-                self.master.st(constr)
-
-    def subprob(self, size=1):
-
-        sub_models = SubModel(self, size)
-        new_var = self.master.dvar(size)
-        sub_models.values = new_var
-        sub_models.value_index = list(range(new_var.first, new_var.last))
-
-        self.subs.append(sub_models)
-
-        return sub_models
-
-    def do_math(self):
-
-        formula = self.master.do_math()
-        all_indices = np.arange(0, formula.linear.shape[1])
-        indices = np.setxor1d(all_indices,
-                              np.array(self.wait_see_index + self.rand_index),
-                              assume_unique=True)
+                if obj.size > 1:
+                    raise ValueError('Incorrect function dimension.')
 
-        formula = GCProg(formula.linear[:, indices], formula.const, formula.sense,
-                         formula.vtype[indices],
-                         formula.ub[indices], formula.lb[indices],
-                         formula.qmat, formula.xmat, formula.obj[:, indices])
-
-        self.all_here_now_index = indices
-
-        return formula
-
-    def solve(self, solver=None, display=True, params={}):
-
-        self.master.solve(solver, display, params)
-        # self.relaxed_bounds.append(self.master.get())
-        self.solutions.append(self.master.solution)
-
-    def add_cut(self, cuts):
-
-        add_linear = sp.vstack([cut.linear for cut in cuts])
-        add_const = np.concatenate([cut.const for cut in cuts])
-        add_sense = np.zeros(len(cuts))
-
-        formula = self.master.primal
-        formula.linear = sp.vstack((formula.linear, add_linear), format='csr')
-        formula.const = np.concatenate((formula.const, add_const))
-        formula.sense = np.concatenate((formula.sense, add_sense))
-        self.master.primal = formula
-
-    def update(self, solver=None, master_display=True, sub_display=False,
-               master_params={}, sub_params={}):
-
-        self.solve(solver, master_display, master_params)
-        self.relaxed_bounds.append(self.master.get())
-        obj_linear = self.master.obj.linear.toarray()[0]
-        obj_const = self.master.obj.const
-        indices = self.here_now_index
-        x_current = self.master.solution.x[indices]
-        exact_obj = obj_linear[self.here_now_index] @ x_current + obj_const
-
-        for sub in self.subs:
-            sol = sub.solve(solver, sub_display, sub_params)
-            objvals = sol['objval']
-            exact_obj += obj_linear[sub.value_index] @ np.array(objvals)
-
-            self.add_cut(sol['cut'])
-
-        self.exact_bounds.append(exact_obj.reshape(()))
-
-    def get_bounds(self):
-
-        if self.master.sign > 0:
-            lower = max(self.relaxed_bounds)
-            upper = min(self.exact_bounds)
-        else:
-            lower = max(self.exact_bounds)
-            upper = min(self.relaxed_bounds)
-
-        return lower, upper
-
-    def get_gap(self, relative=True):
-
-        lower, upper = self.get_bounds()
-
-        if relative:
-            return (upper - lower) / lower
-        else:
-            return upper - lower
+        self.obj = obj
+        self.sign = 1
+        self.pupdate = True
+        self.dupdate = True
 
-    def get(self):
+    def max(self, obj):
+        """
+        Maximize the given objective function.
 
-        if self.exact_bounds == []:
-            raise RuntimeError('The model is unsolved or no solution is obtained.')
-        else:
-            if self.master.sign > 0:
-                return min(self.exact_bounds)
+        Parameters
+        ----------
+        obj : RSOME expression, numeric constant
+            The objective function
+
+        Notes
+        -----
+        The objective function given as an array must have the size
+        to be one.
+        """
+
+        if self.obj is not None:
+            raise SyntaxError('Redefinition of the objective is not allowed.')
+
+        if not isinstance(obj, (Real, PiecewiseConvex)):
+            if isinstance(obj, VarSub):
+                if obj.indices.size > 1:
+                    raise ValueError('Incorrect function dimension.')
             else:
-                return max(self.exact_bounds)
-
-
-class SubModel:
-
-    def __init__(self, model, size):
-
-        self.model = model
-        self.obj = None
-        self.sign = None
-        self.size = size
-        self.lin_constr = []
-        self.bounds = []
-        self.values = None
-        self.value_index = None
-        self.wait_see_index = []
-        self.uset = [None] * size
-
-        self.formula = None
-        self.update = True
-
-    def __getitem__(self, item):
-
-        return SubModelIter(self, item)
-
-    def def_obj(self, obj, sign):
-
-        if isinstance(obj, (Vars, VarSub, Affine)):
-            affine = obj.to_affine()
-            if affine.linear[:, self.model.here_now_index].nnz > 0:
-                msg = 'Here-and-now decisions are not allowed in sub-problem objective.'
-                raise ValueError(msg)
-            if affine.linear[:, self.model.rand_index].nnz > 0:
-                msg = 'Random variables are not allowed in sub-problem objective.'
-                raise ValueError(msg)
-            value_index = list(range(self.values.first, self.values.last))
-            if affine.linear[:, value_index].nnz > 0:
-                msg = 'Sub-problem values are not allowed in sub-problem objective.'
-                raise ValueError(msg)
-        else:
-            raise TypeError('Unsupported objective function')
+                if obj.size > 1:
+                    raise ValueError('Incorrect function dimension.')
 
         self.obj = obj
-        self.sign = sign
-
-    def dvar(self, shape=(), name=None):
-
-        new_var = self.model.master.dvar(shape, 'C', name, aux=False)
-        index = range(new_var.first, new_var.last)
-        self.model.wait_see_index.extend(index)
-        self.wait_see_index.extend(index)
-
-        self.update = True
-
-        return new_var
-
-    def min(self, obj):
-
-        self.def_obj(obj, 1)
+        self.sign = - 1
+        self.pupdate = True
+        self.dupdate = True
+
+    def minmax(self, obj, *args):
+
+        """
+        Minimize the maximum objective value over the given uncertainty set.
+
+        Parameters
+        ----------
+        obj : RSOME expression, numeric constant
+            Objective function involving random variables
+        *args
+            Constraints or collections of constraints of random variables
+            used for defining the uncertainty set
+
+        Notes
+        -----
+        The uncertainty set defined for the objective function is considered
+        the default uncertainty set for the robust model.
+        """
+
+        if self.obj is not None:
+            raise SyntaxError('Redefinition of the objective is not allowed.')
+
+        if not isinstance(obj, (Real, PiecewiseConvex)):
+            if obj.size > 1:
+                raise ValueError('Incorrect function dimension.')
+
+        constraints = []
+        for items in args:
+            if isinstance(items, Iterable):
+                constraints.extend(list(items))
+            else:
+                constraints.append(items)
 
-        self.update = True
+        sup_model = self.sup_model
+        sup_model.reset()
+        for item in constraints:
+            if item.model is not sup_model:
+                raise ValueError('Models mismatch.')
+            sup_model.st(item)
 
-    def max(self, obj):
+        self.obj = obj
+        self.obj_support = sup_model.do_math(primal=False, obj=False)
+        self.sign = 1
+        self.pupdate = True
+        self.dupdate = True
+
+    def maxmin(self, obj, *args):
+
+        """
+        Maximize the minimum objective value over the given uncertainty set.
+
+        Parameters
+        ----------
+        obj : RSOME expression, numeric constant
+            Objective function involving random variables
+        *args
+            Constraints or collections of constraints of random variables
+            used for defining the uncertainty set
+
+        Notes
+        -----
+        The uncertainty set defined for the objective function is considered
+        the default uncertainty set for the robust model.
+        """
+
+        if self.obj is not None:
+            raise SyntaxError('Redefinition of the objective is not allowed.')
+
+        if not isinstance(obj, (Real, PiecewiseConvex)):
+            if obj.size > 1:
+                raise ValueError('Incorrect function dimension.')
+
+        constraints = []
+        for items in args:
+            if isinstance(items, Iterable):
+                constraints.extend(list(items))
+            else:
+                constraints.append(items)
 
-        self.def_obj(obj, -1)
+        sup_model = self.sup_model
+        sup_model.reset()
+        for item in constraints:
+            if item.model is not sup_model:
+                raise ValueError('Models mismatch.')
+            sup_model.st(item)
 
-        self.update = True
+        self.obj = obj
+        self.obj_support = sup_model.do_math(primal=False, obj=False)
+        self.sign = - 1
+        self.pupdate = True
+        self.dupdate = True
 
     def st(self, *arg):
+        """
+        Define constraints that an optimization model subject to.
+
+        Parameters
+        ----------
+        *args : RSOME constraints, iterables
+            Constraints or collections of constraints that the model
+            subject to.
+
+        Notes
+        -----
+        Multiple constraints can be defined altogether as the argument
+        of the st method.
+        """
 
         for constr in arg:
             if isinstance(constr, Iterable):
                 for item in constr:
                     self.st(item)
-            else:
-                value_index = list(range(self.values.first, self.values.last))
-                if isinstance(constr, LinConstr):
-                    if constr.linear[:, value_index].nnz > 0:
-                        msg = 'Sub-problem values are not allowed in sub-problem.'
-                        raise ValueError(msg)
-                    if constr.linear[:, self.model.wait_see_index].nnz == 0:
-                        msg = 'No wait-and-see decision appears in the constraint.'
-                        raise ValueError(msg)
-                    self.lin_constr.append(constr)
-                elif isinstance(constr, Bounds):
-                    if not set(constr.indices).intersection(self.model.wait_see_index):
-                        msg = 'No wait-and-see decision appears in the constraint.'
-                        raise ValueError(msg)
-                    self.bounds.append(constr)
+            elif isinstance(constr, PWConstr):
+                for piece in constr.pieces:
+                    self.st(piece)
+            elif isinstance(constr, (LinConstr, Bounds, CvxConstr,
+                                     ConeConstr, ExpConstr, KLConstr, LMIConstr)):
+                if (constr.model is not self.rc_model) or \
+                        (constr.model.mtype != 'R'):
+                    raise ValueError('Models mismatch.')
+                self.all_constr.append(constr)
+            elif isinstance(constr, RoConstr):
+                if (constr.dec_model is not self.rc_model) or \
+                        (constr.rand_model is not self.sup_model):
+                    raise ValueError('Models mismatch.')
+                sense = (constr.sense[0] if isinstance(constr.sense,
+                                                       np.ndarray)
+                         else constr.sense)
+                if sense == 0:
+                    self.all_constr.append(constr)
                 else:
-                    raise TypeError('Unsupported constraints.')
-
-        self.update = True
-
-    def uncertain(self, uncertainty):
-
-        self.uset = [uncertainty] * self.size
-
-    def do_math(self):
-
-        if self.update is False and self.formula is not None:
-            return self.formula
-
-        sub_model = SOCModel(nobj=True, mtype='R')
-
-        vars = []
-        for var in self.model.master.vars:
-            if var.vtype == 'C':
-                vars.append(var)
+                    left = RoAffine(constr.raffine, constr.affine,
+                                    constr.rand_model)
+                    right = RoAffine(-constr.raffine, -constr.affine,
+                                     constr.rand_model)
+                    left_constr = RoConstr(left, sense=0)
+                    left_constr.support = constr.support
+                    right_constr = RoConstr(right, sense=0)
+                    right_constr.support = constr.support
+                    self.all_constr.append(left_constr)
+                    self.all_constr.append(right_constr)
             else:
-                new_var = Vars(var.model, var.first, var.shape, 'C',
-                               var.name, var.sparray)
-                vars.append(new_var)
-        sub_model.vars = vars + self.model.master.auxs
-        sub_model.lin_constr = self.lin_constr
-        sub_model.bounds = self.bounds
-
-        dual = sub_model.do_math(primal=False, obj=False)
-        dual.const = self.obj.linear.toarray()[0] * dual.const * self.sign
-
-        vtype = dual.vtype
-        ub = dual.ub
-        lb = dual.lb
-        qmat = dual.qmat
-        obj = dual.obj
-
-        linear = dual.linear[self.wait_see_index, :]
-        const = dual.const[self.wait_see_index]
-        sense = dual.sense[self.wait_see_index]
-
-        cmat = dual.linear[self.model.rand_index, :].T
-        if self.model.all_here_now_index == []:
-            all_indices = np.arange(0, dual.linear.shape[0])
-            not_here_now = self.model.wait_see_index + self.model.rand_index
-            indices = np.setxor1d(all_indices, np.array(not_here_now),
-                                  assume_unique=True)
-            self.model.all_here_now_index = indices
-        else:
-            indices = self.model.all_here_now_index
-
-        amat = dual.linear[indices, :].T
-
-        self.update = False
-
-        return SubProg(linear, const, sense, vtype, ub, lb,
-                       qmat, amat, cmat, obj)
-
-    def solve(self, solver=None, display=False, params={}):
-
-        formula = self.do_math()
-
-        indices = self.model.all_here_now_index
-        x_here_now = self.model.master.solution.x[indices]
+                raise TypeError('Unknown type of constraints')
 
-        cuts = []
-        pis = []
-        objvals = []
-        for i, uncertainty in enumerate(self.uset):
-            z_values = uncertainty.center
-            z_values = z_values.reshape((z_values.size, ))
+        self.pupdate = True
+        self.dupdate = True
 
-            obj = formula.obj + formula.amat@x_here_now
-            obj += formula.cmat @ z_values
-            obj = obj.reshape((1, obj.size))
-
-            sub_formula = SOCProg(formula.linear, formula.const, formula.sense,
-                                  formula.vtype, formula.ub, formula.lb,
-                                  formula.qmat, obj)
+        if len(arg) == 1:
+            return arg[0]
+        else:
+            return arg
 
-            if solver is None:
-                sub_sol = def_sol(sub_formula, display, params)
+    def do_math(self, primal=True):
+        """
+        Return the linear, or conic programming problem as the standard
+        formula or deterministic counterpart of the model.
+
+        Parameters
+        ----------
+        primal : bool, default True
+            Specify whether return the primal formula of the model.
+            If primal=False, the method returns the dual formula.
+
+        Returns
+        -------
+        prog : GCProg
+            A conic programming problem.
+        """
+
+        if primal:
+            if self.primal is not None and not self.pupdate:
+                return self.primal
+        else:
+            if self.dual is not None and not self.dupdate:
+                return self.dual
             else:
-                sub_sol = solver.solve(sub_formula, display, params)
-
-            pi = sub_sol.x
-            pis.append(pi)
-            objvals.append(-sub_sol.objval * self.sign)
-
-            cut_linear = - (pi @ formula.amat)
-            cut_linear = csr_matrix(cut_linear.reshape((1, cut_linear.size)))
-            cut_const = (formula.obj - formula.cmat@z_values) @ pi
-            left = Affine(self.model.master, cut_linear, cut_const)
-            right = self.values[i]
-            cut = left <= self.sign * right
-            cuts.append(cut)
-
-        return {'pi': pis, 'objval': objvals, 'cut': cuts}
-
+                self.do_math(primal=True)
+                return self.rc_model.do_math(False, obj=True)
 
-class SubModelIter:
-
-    def __init__(self, submodel, item):
-
-        self.submodel = submodel
-        self.item = item
-
-    def uncertain(self, uncertainty):
-
-        if isinstance(uncertainty, Uncertainty):
-            self.submodel.uset[self.item] = uncertainty
+        self.rc_model.reset()
+        if isinstance(self.obj, (Vars, VarSub, Affine, Convex, Real)):
+            self.rc_model.obj = self.obj
+            self.rc_model.sign = self.sign
+            more_roc = []
+        elif isinstance(self.obj, RoAffine):
+            obj_constr = (self.rc_model.vars[0] >= self.sign * self.obj)
+            obj_constr.support = self.obj_support
+            more_roc = [obj_constr]
+        elif isinstance(self.obj, PiecewiseConvex):
+            more_roc = []
+            pw_constr = self.rc_model.vars[0] >= self.sign * self.obj
+            more_roc = pw_constr.pieces
         else:
-            raise TypeError('Unsupported uncertainty set.')
-
-
-class SubProg(SOCProg):
-
-    def __init__(self, linear, const, sense, vtype, ub, lb,
-                 qmat, amat, cmat, obj):
-
-        super().__init__(linear, const, sense, vtype, ub, lb, qmat, obj)
-        self.amat = amat
-        self.cmat = cmat
-
-
-class RandVar(Vars):
-
-    def __init__(self, vars):
-
-        super().__init__(vars.model, vars.first, vars.shape, vars.vtype,
-                         vars.name, vars.sparray)
-
-    def __repr__(self):
-
-        string = super().__repr__()
-
-        return string.replace('continuous ', '').replace('decision', 'random')
+            raise TypeError('Incorrect type for the objective function.')
 
-    def singleton(self, center):
+        for constr in self.all_constr + more_roc:
+            if isinstance(constr, (LinConstr, Bounds, CvxConstr,
+                                   ExpConstr, KLConstr, LMIConstr)):
+                self.rc_model.st(constr)
+            if isinstance(constr, RoConstr):
+                if constr.support:
+                    rc_constrs = constr.le_to_rc()
+                else:
+                    rc_constrs = constr.le_to_rc(self.obj_support)
+                for rc_constr in rc_constrs:
+                    self.rc_model.st(rc_constr)
+
+        formula = self.rc_model.do_math(primal, obj=True)
+
+        if primal:
+            self.primal = formula
+            self.pupdate = False
+        else:
+            self.dual = formula
+            self.dupdate = False
 
-        if isinstance(center, Real):
-            center = np.array([center])
+        return formula
 
-        center = center.reshape(self.shape)
+    def solve(self, solver=None, display=True, params={}):
+        """
+        Solve the model with the selected solver interface.
 
-        return Uncertainty(self, center, 0, utype='S')
+        Parameters
+        ----------
+        solver : {None, lpg_solver, clp_solver, ort_solver, eco_solver
+                  cpx_solver, grb_solver, msk_solver, cpt_solver}
+            Solver interface used for model solution. Use the default
+            solver if solver=None.
+        display : bool
+            Display option of the solver interface.
+        params : dict
+            A dictionary that specifies parameters of the selected solver.
+            So far the argument only applies to Gurobi, CPLEX, and Mosek.
+        """
 
-    def get(self):
+        if solver is None:
+            solution = def_sol(self.do_math(), display, params)
+        else:
+            solution = solver.solve(self.do_math(), display, params)
 
-        raise TypeError('Cannot access the solution of random variables')
+        if isinstance(solution, Solution):
+            self.rc_model.solution = solution
+        else:
+            self.rc_model.solution = None
 
+        self.solution = self.rc_model.solution
 
-class HaNVar(Vars):
+    def soc_solve(self, solver=None, degree=4, cuts=(-30, 60), display=True, params={}):
+        """
+        Solve the approximated SOC model with the selected solver interface.
+
+        Parameters
+        ----------
+            solver : {None, lpg_solver, clp_solver, ort_solver, eco_solver
+                      cpx_solver, grb_solver, msk_solver}
+                Solver interface used for model solution. Use default solver
+                if solver=None.
+            degree : int
+                The L-degree value for approximating exponential cone
+                constraints.
+            cuts : tuple of two integers
+                The lower and upper cut-off values for the SOC approximation
+                of exponential constraints.
+            display : bool
+                Display option of the solver interface.
+            params : dict
+                A dictionary that specifies parameters of the selected solver.
+                So far the argument only applies to Gurobi, CPLEX, and Mosek.
+        """
+
+        formula = self.do_math().to_socp(degree, cuts)
+        if solver is None:
+            solution = def_sol(formula, display, params)
+        else:
+            solution = solver.solve(formula, display, params)
 
-    def __init__(self, vars):
+        if isinstance(solution, Solution):
+            self.rc_model.solution = solution
+        else:
+            self.rc_model.solution = None
 
-        super().__init__(vars.model, vars.first, vars.shape, vars.vtype,
-                         vars.name, vars.sparray)
+        self.solution = self.rc_model.solution
 
     def get(self):
+        """
+        Return the optimal objective value of the solved model.
 
-        top = self.model.top
-        exact_bounds = np.array(top.exact_bounds)
-        index = np.argmin(top.master.sign * exact_bounds)
-
-        xvec = top.solutions[index].x[self.first:self.last]
-
-        return xvec.reshape(self.shape)
-
-
-class Uncertainty:
-
-    def __init__(self, vars, center, radius, utype):
+        Notes
+        -----
+        An error message is given if the model is unsolved or no solution
+        is obtained.
+        """
 
-        self.vars = vars
-        self.center = center
-        self.radius = radius
-        self.utype = utype
+        if self.rc_model.solution is None:
+            raise RuntimeError('The model is unsolved.')
 
-    def __repr__(self):
+        solution = self.rc_model.solution
+        if np.isnan(solution.objval):
+            msg = 'No solution available. '
+            msg += f'{solution.solver} solution status: {solution.status}'
+            raise RuntimeError(msg)
 
-        utypes = {'S': 'singleton',
-                  '1': 'one-norm',
-                  '2': 'two-norm',
-                  'I': 'infinite-norm'}
+        return self.sign * self.rc_model.solution.objval
 
-        article = 'an' if self.utype == 'I' else 'a'
-        string = f'{article} {utypes[self.utype].lower()} uncertainty set '
-        string += f'for {self.vars.__repr__()}'
+    def optimal(self):
 
-        return string
+        return self.solution is not None
```

### Comparing `rsome-1.1.4/rsome/dro.py` & `rsome-1.2.0/rsome/dro.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from .gcp import Model as GCPModel
 from .ro import Model as ROModel
 from .lp import DecBounds, DecExpConstr, LinConstr
-from .lp import ConeConstr, PCvxConstr, CvxConstr, ExpConstr
+from .lp import ConeConstr, PCvxConstr, CvxConstr, ExpConstr, LMIConstr
 from .lp import Vars, Affine
 from .lp import RoAffine, RoConstr
 from .lp import DecVar, RandVar, DecLinConstr, DecCvxConstr, DecPCvxConstr
 from .lp import DecRoConstr
-from .lp import PiecewiseConvex, ExpPiecewiseConvex, PWConstr, ExpPWConstr
+from .lp import PiecewiseConvex, PWConstr, ExpPWConstr, DecLMIConstr
 from .lp import Scen
 from .lp import Solution, def_sol
 from .subroutines import event_dict
 import numpy as np
 import pandas as pd
 import scipy.sparse as sp
 from numbers import Real
@@ -364,15 +364,15 @@
         for constr in arg:
             if isinstance(constr, Iterable):
                 for item in constr:
                     self.st(item)
             else:
                 if isinstance(constr, (DecLinConstr, DecBounds,
                                        DecCvxConstr, DecPCvxConstr,
-                                       DecExpConstr)):
+                                       DecExpConstr, DecLMIConstr)):
                     if constr.model is not self.vt_model:
                         raise ValueError('Models mismatch.')
                 elif isinstance(constr, DecRoConstr):
                     if constr.dec_model is not self.vt_model or \
                        constr.rand_model is not self.sup_model:
                         raise ValueError('Models mismatch.')
                 elif isinstance(constr, (PWConstr, ExpPWConstr)):
@@ -629,14 +629,26 @@
                     affine3 = constr.expr3.to_affine()
                     linear3 = affine3.linear
                     const3 = affine3.const
                     expr3 = linear3@drule_affine + const3
 
                 ew_constr = ExpConstr(expr1.model, expr1, expr2, expr3)
 
+            elif isinstance(constr, DecLMIConstr):
+                if isinstance(drule, RoAffine):
+                    drule_affine = drule.affine
+                else:
+                    drule_affine = drule
+
+                lmi_left = constr.linear @ drule_affine - constr.const.flatten()
+                lmi_linear = lmi_left.linear
+                lmi_const = (-lmi_left.const).reshape((constr.dim, constr.dim))
+
+                ew_constr = LMIConstr(lmi_left.model, lmi_linear, lmi_const, constr.dim)
+
             else:
                 raise TypeError('Unknown constraint type.')
 
             if isinstance(ew_constr, RoConstr):
                 if (ew_constr.raffine.linear.nnz > 0 or
                         np.any(ew_constr.raffine.const)):
                     if constr.ambset is None:
@@ -757,22 +769,23 @@
 
     def solve(self, solver=None, display=True, params={}):
         """
         Solve the model with the selected solver interface.
 
         Parameters
         ----------
-            solver : {None, lpg_solver, grb_solver, msk_solver}
+            solver : {None, lpg_solver, clp_solver, ort_solver, eco_solver
+                      cpx_solver, grb_solver, msk_solver, cpt_solver}
                 Solver interface used for model solution. Use default solver
                 if solver=None.
             display : bool
                 Display option of the solver interface.
             params : dict
                 A dictionary that specifies parameters of the selected solver.
-                So far the argument only applies to Gurobi and MOSEK.
+                So far the argument only applies to Gurobi, CPLEX, and Mosek.
         """
 
         if solver is None:
             solution = def_sol(self.do_math(), display, params)
         else:
             solution = solver.solve(self.do_math(), display, params)
 
@@ -792,14 +805,21 @@
         -----
         An error message is given if the model is unsolved or no solution
         is obtained.
         """
 
         if self.solution is None:
             raise RuntimeError('The model is unsolved or no solution is obtained')
+
+        solution = self.solution
+        if np.isnan(solution.objval):
+            msg = 'No solution available. '
+            msg += f'{solution.solver} solution status: {solution.status}'
+            raise RuntimeError(msg)
+
         return self.sign * self.solution.objval
 
     def optimal(self):
 
         return self.solution is not None
```

### Comparing `rsome-1.1.4/rsome/eco_solver.py` & `rsome-1.2.0/rsome/eco_solver.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,23 +11,29 @@
 from .socp import SOCProg
 from .gcp import GCProg
 from .lp import Solution
 
 
 def solve(formula, display=True, params={}):
 
+    try:
+        if formula.lmi:
+            warnings.warn('The solver ignores semidefinite cone constraints. ')
+    except AttributeError:
+        pass
+
     bool_idx = [i for i in range(len(formula.vtype)) if formula.vtype[i] == 'B']
     int_idx = [i for i in range(len(formula.vtype)) if formula.vtype[i] == 'I']
 
     cols = formula.linear.shape[1]
     eq_idx = np.argwhere(formula.sense == 1).flatten()
     ineq_idx = np.argwhere(formula.sense == 0).flatten()
     num_ineq = len(ineq_idx)
 
-    c = formula.obj.flatten()
+    c = formula.obj
 
     Gl = formula.linear[ineq_idx]
 
     zlb_idx = np.argwhere(formula.lb > -np.inf).flatten()
     num_zlb = len(zlb_idx)
     Glb = sp.csr_matrix((-np.ones(num_zlb),
                          (np.arange(num_zlb, dtype='int'), zlb_idx)),
@@ -73,27 +79,42 @@
 
     if display:
         print('Being solved by ECOS...', flush=True)
         time.sleep(0.2)
 
     if len(bool_idx) + len(int_idx) == 0:
         sol = ecos.solve(c, G, h, dims, A, b)
+
+        num_constr, num_var = formula.linear.shape
+        pi = np.ones(num_constr) * np.nan
+        upi = np.zeros(num_var)
+        lpi = np.zeros(num_var)
+
+        pi[eq_idx] = - sol['y']
+        pi[ineq_idx] = - sol['z'][:num_ineq]
+        lpi[zlb_idx] = sol['z'][num_ineq + np.arange(num_zlb)]
+        upi[zub_idx] = - sol['z'][num_ineq + num_zlb + np.arange(num_zub)]
+
+        y = {'pi': pi, 'upi': upi, 'lpi': lpi}
     else:
         sol = ecos.solve(c, G, h, dims, A, b,
                          bool_vars_idx=bool_idx, int_vars_idx=int_idx,
                          mi_max_iters=100000000)
+        y = None
+
     info = sol['info']
     stime = info['timing']['runtime']
     status = info['infostring']
 
     if display:
         print('Solution status: {0}'.format(status))
         print('Running time: {0:0.4f}s'.format(stime))
 
     if info['exitFlag'] in [0, 10]:
         x_vec = sol['x']
-        solution = Solution(info['pcost'], x_vec, status, stime)
+        solution = Solution('ECOS', info['pcost'], x_vec, status, stime, y=y)
     else:
         warnings.warn('Fail to find the optimal solution.')
-        solution = None
+        # solution = None
+        solution = Solution('ECOS', np.nan, None, status, stime)
 
     return solution
```

### Comparing `rsome-1.1.4/rsome/gcp.py` & `rsome-1.2.0/rsome/socp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,79 @@
-from .lp import CvxConstr, PCvxConstr, ExpConstr, KLConstr
-from .socp import Model as SOCModel
-from .socp import SOCProg
+from .lp import Model as LPModel
+from .lp import LinConstr, Bounds, CvxConstr, ConeConstr
+from .lp import LinProg
 import numpy as np
 import pandas as pd
 import scipy.sparse as sp
 from collections.abc import Iterable
-from .subroutines import flat, rso_broadcast
 
 
-class Model(SOCModel):
+class Model(LPModel):
+    """
+    The Model class creates an SOCP model object
+    """
 
     def __init__(self, nobj=False, mtype='R', name=None, top=None):
 
         super().__init__(nobj, mtype, name, top)
-        self.exp_constr = []
-        self.other_constr = []
+        self.cvx_constr = []
+        self.cone_constr = []
+        # self.avar_indices = []
 
     def reset(self):
 
         self.lin_constr = []
         self.pws_constr = []
         self.cone_constr = []
-        self.exp_constr = []
-        self.other_constr = []
         self.bounds = []
         self.aux_constr = []
         self.aux_bounds = []
         self.cvx_constr = []
 
     def st(self, constr):
+        """
+        Define constraints that an optimization model subject to.
+
+        Parameters
+        ----------
+        constr
+            Constraints or collections of constraints that the model
+            subject to.
+        """
 
         if isinstance(constr, Iterable):
             for item in constr:
                 self.st(item)
-        elif isinstance(constr, ExpConstr):
-            self.exp_constr.append(constr)
+        elif isinstance(constr, (LinConstr, Bounds)):
+            super().st(constr)
         elif isinstance(constr, CvxConstr):
-            if constr.xtype in 'XLP':
-                self.other_constr.append(constr)
-            else:
+            if constr.model is not self:
+                raise ValueError('Constraints are not defined for this model.')
+            if constr.xtype in 'AMI':
                 super().st(constr)
-        elif isinstance(constr, KLConstr):
-            self.other_constr.append(constr)
+            elif constr.xtype in 'ESQ':
+                self.cvx_constr.append(constr)
+            else:
+                raise ValueError('Unsupported convex constraints.')
+        elif isinstance(constr, ConeConstr):
+            if constr.model is not self:
+                raise ValueError('Constraints are not defined for this model.')
+            self.cone_constr.append(constr)
         else:
-            super().st(constr)
+            raise TypeError('Unknown constraint type.')
+
+        self.pupdate = True
+        self.dupdate = True
+
+        return constr
 
     def do_math(self, primal=True, refresh=True, obj=True):
         """
-        Return the linear, second-order cone, or exponential
-        cone programming problem as the standard formula of
-        the model.
+        Return the linear or second-order cone programming problem
+        as the standard formula of the model.
 
         Parameters
         ----------
         primal : bool, default True
             Specify whether return the primal formula of the model.
             If primal=False, the method returns the daul formula.
 
@@ -61,233 +81,218 @@
             Leave the argument unspecified.
 
         obj : bool
             Leave the argument unspecified.
 
         Returns
         -------
-        prog : GCProg
-            An exponential cone programming problem.
+        prog : SOCProg
+            A second-order cone programming problem.
         """
 
         if primal:
             if self.primal is not None and not self.pupdate:
                 return self.primal
 
             if refresh:
                 self.auxs = []
                 self.aux_constr = []
                 self.aux_bounds = []
                 self.last = self.vars[-1].first + self.vars[-1].size
 
-            more_exp = []
+            more_cvx = []
             if self.obj is not None:
                 obj_constr = (self.vars[0] - self.sign * self.obj >= 0)
                 if isinstance(obj_constr, CvxConstr):
-                    constr = obj_constr
-                    """
-                    if constr.xtype == 'X':
-                        affine_out = constr.affine_out * (1/constr.multiplier)
-                        exp_cone_constr = ExpConstr(constr.model,
-                                                    constr.affine_in,
-                                                    -constr.affine_out, 1)
-                        more_exp.append(exp_cone_constr)
-                    elif constr.xtype == 'L':
-                        affine_out = constr.affine_out * (1/constr.multiplier)
-                        exp_cone_constr = ExpConstr(constr.model,
-                                                    affine_out,
-                                                    constr.affine_in, 1)
-                        more_exp.append(exp_cone_constr)
-                    """
-                    if constr.xtype in 'XLP':
-                        self.other_constr.append(constr)
-
-            for constr in self.other_constr:
-                if isinstance(constr, KLConstr):
-                    ns = constr.p.size
-                    aux_var = self.dvar(ns, aux=True)
-                    self.aux_constr.append(aux_var.sum() <= constr.r)
-                    for s in range(ns):
-                        ps = constr.phat[s]
-                        p = constr.p[s]
-
-                        entro_constr = aux_var[s] * (1/ps) >= -(p * (1/ps)).entropy()
-                        exp_constr = ExpConstr(entro_constr.model,
-                                               entro_constr.affine_out,
-                                               1, entro_constr.affine_in)
-
-                        more_exp.append(exp_constr)
-                elif isinstance(constr, PCvxConstr):
-                    if constr.xtype == 'X':
-                        affine_out = constr.affine_out * (1/constr.multiplier)
-                        exprs_list = rso_broadcast(constr.affine_in,
-                                                   constr.affine_scale,
-                                                   affine_out)
-                        for exprs in exprs_list:
-                            exp_cone_constr = ExpConstr(constr.model,
-                                                        exprs[0],
-                                                        -exprs[2], exprs[1])
-                            self.exp_constr.append(exp_cone_constr)
-                    elif constr.xtype == 'L':
-                        affine_out = constr.affine_out * (1/constr.multiplier)
-                        exprs_list = rso_broadcast(constr.affine_in,
-                                                   constr.affine_scale,
-                                                   affine_out)
-                        for exprs in exprs_list:
-                            exp_cone_constr = ExpConstr(constr.model,
-                                                        exprs[2], exprs[0], exprs[1])
-                            self.exp_constr.append(exp_cone_constr)
-                elif isinstance(constr, CvxConstr):
-                    if constr.xtype == 'P':
-                        affine_out = constr.affine_out * (1/constr.multiplier)
-                        aux_var = self.dvar(constr.affine_in.shape)
-                        self.aux_constr.append(aux_var.sum() >= affine_out)
-                        ns = constr.affine_in.size
-                        affine_in = constr.affine_in.reshape(ns)
-                        affine_aux = aux_var.to_affine().reshape(ns)
-                        for s in range(ns):
-                            exp_cone_constr = ExpConstr(constr.model,
-                                                        affine_aux[s],
-                                                        1, affine_in[s])
-                            more_exp.append(exp_cone_constr)
-                    elif constr.xtype == 'X':
-                        affine_out = constr.affine_out * (1/constr.multiplier)
-                        exprs_list = rso_broadcast(constr.affine_in, affine_out)
-                        for exprs in exprs_list:
-                            exp_cone_constr = ExpConstr(constr.model,
-                                                        exprs[0], -exprs[1], 1)
-                            self.exp_constr.append(exp_cone_constr)
-                    elif constr.xtype == 'L':
-                        affine_out = constr.affine_out * (1/constr.multiplier)
-                        exprs_list = rso_broadcast(constr.affine_in, affine_out)
-                        for exprs in exprs_list:
-                            exp_cone_constr = ExpConstr(constr.model,
-                                                        exprs[1], exprs[0], 1)
-                            self.exp_constr.append(exp_cone_constr)
-
-            xmat = []
-            for constr in self.exp_constr + more_exp:
-                aux_var = self.dvar(3, aux=True)
-                self.aux_constr.append(aux_var[0] - constr.expr1 == 0)
-                self.aux_constr.append(aux_var[1] - constr.expr2 <= 0)
-                self.aux_constr.append(aux_var[2] - constr.expr3 == 0)
-                xmat.append(list(range(aux_var.first, aux_var.first + 3)))
+                    more_cvx.append(obj_constr)
+
+            qmat = []
+            for constr in self.cvx_constr + more_cvx:
+                if constr.xtype == 'E':
+                    aux_left = self.dvar(constr.affine_in.shape, aux=True)
+                    aux_right = self.dvar(1, aux=True)
+                    affine_in = constr.affine_in * constr.multiplier
+                    self.aux_constr.append(affine_in - aux_left == 0)
+                    self.aux_constr.append(constr.affine_out + aux_right <= 0)
+                    bounds = (aux_right >= 0)
+                    if isinstance(bounds, Bounds):
+                        self.aux_bounds.append(bounds)
+                    else:
+                        self.aux_constr.append(bounds)
+                    qmat.append([aux_right.first] +
+                                list([aux_left.first + index
+                                      for index in range(aux_left.size)]))
+                elif constr.xtype == 'S':
+                    aux1 = self.dvar(constr.affine_out.shape, aux=True)
+                    aux2 = self.dvar(constr.affine_in.shape, aux=True)
+                    aux3 = self.dvar(constr.affine_out.shape, aux=True)
+                    affine_in = constr.affine_in * constr.multiplier
+                    self.aux_constr.append(aux1 - 0.5*(1+constr.affine_out) == 0)
+                    self.aux_constr.append(aux2 - affine_in == 0)
+                    self.aux_constr.append(aux3 - 0.5 * (1-constr.affine_out) == 0)
+                    bounds = (aux3 >= 0)
+                    if isinstance(bounds, Bounds):
+                        self.aux_bounds.append(bounds)
+                    else:
+                        self.aux_constr.append(bounds)
+                    for i in range(constr.affine_in.size):
+                        qmat.append([aux3.first + i] +
+                                    [aux1.first + i, aux2.first + i])
+                elif constr.xtype == 'Q':
+                    # aux1 = self.dvar(constr.affine_out.shape, aux=True)
+                    aux1 = self.dvar(1, aux=True)
+                    aux2 = self.dvar(constr.affine_in.shape, aux=True)
+                    # aux3 = self.dvar(constr.affine_out.shape, aux=True)
+                    aux3 = self.dvar(1, aux=True)
+                    aux4 = self.dvar(1, aux=True)
+                    affine_in = constr.affine_in * constr.multiplier
+                    self.aux_constr.append(aux1 - 0.5 * (1-aux4) == 0)
+                    self.aux_constr.append(aux2 - affine_in == 0)
+                    self.aux_constr.append(aux3 - 0.5 * (1+aux4) == 0)
+                    self.aux_constr.append(aux4 + constr.affine_out <= 0)
+                    bounds = (aux3 >= 0)
+                    if isinstance(bounds, Bounds):
+                        self.aux_bounds.append(bounds)
+                    else:
+                        self.aux_constr.append(bounds)
+                    qmat.append([aux3.first] + [aux1.first] +
+                                list(aux2.first + np.arange(aux2.size)))
+
+            for constr in self.cone_constr:
+                qmat.append([constr.right_var.first + constr.right_index] +
+                            [constr.left_var.first + index
+                             for index in constr.left_index])
 
             formula = super().do_math(primal=True, refresh=False, obj=obj)
-            formula = GCProg(formula.linear, formula.const, formula.sense,
-                             formula.vtype, formula.ub, formula.lb,
-                             formula.qmat, xmat, formula.obj)
+            formula = SOCProg(formula.linear, formula.const, formula.sense,
+                              formula.vtype, formula.ub, formula.lb,
+                              qmat, formula.obj)
             self.primal = formula
             self.pupdate = False
 
             return formula
-
         else:
             if self.dual is not None and not self.dupdate:
                 return self.dual
 
             primal = self.do_math(obj=obj)
 
-            dual_socp = super().do_math(primal=False, refresh=False, obj=obj)
-
-            if len(primal.xmat) == 0:
-                formula = GCProg(dual_socp.linear, dual_socp.const, dual_socp.sense,
-                                 dual_socp.vtype, dual_socp.ub, dual_socp.lb,
-                                 dual_socp.qmat, [], dual_socp.obj)
+            dual_lp = super().do_math(primal=False, refresh=False, obj=obj)
+            if len(primal.qmat) == 0:
+                formula = SOCProg(dual_lp.linear, dual_lp.const, dual_lp.sense,
+                                  dual_lp.vtype, dual_lp.ub, dual_lp.lb,
+                                  [], dual_lp.obj)
                 self.dual = formula
                 return formula
 
-            if len(primal.qmat) == 0:
-                pxmat = primal.xmat
+            eye_indices = [item for inner in primal.qmat for item in inner]
+            eye_block = dual_lp.linear[eye_indices, :]
+            if len(eye_block.data) + 1 == len(eye_block.indptr):
+                lin_indices = [ind for ind in range(primal.linear.shape[1])
+                               if ind not in eye_indices]
+                linear = dual_lp.linear[lin_indices, :]
+                const = dual_lp.const[lin_indices]
+                sense = dual_lp.sense[lin_indices]
+                obj = dual_lp.obj
+                vtype = dual_lp.vtype
+                ub = dual_lp.ub
+                lb = dual_lp.lb
+                qmat = []
+                for qc in primal.qmat:
+                    lbz_index = dual_lp.linear[qc[0], :].indices
+                    ub[lbz_index] = - lb[lbz_index]
+                    lb[lbz_index] = 0
+                    linear[:, lbz_index] = - linear[:, lbz_index]
+                    obj[lbz_index] = - obj[lbz_index]
+                    qmat.append(list(dual_lp.linear[qc, :].indices))
+
+                formula = SOCProg(linear, const, sense,
+                                  vtype, ub, lb, qmat, obj)
+
             else:
-                num_exp = len(primal.xmat)
-                i_idx = np.array([range(num_exp)] * 3).T.flatten()
-                j_idx = flat(primal.xmat)
-                sp_xmat = sp.csr_matrix(([1, 1, 1] * num_exp,
-                                         (i_idx, j_idx)),
-                                        (num_exp, primal.linear.shape[1]))
-                socp_idx = flat(primal.qmat)
-                keep_idx = [i for i in range(primal.linear.shape[1])
-                            if i not in socp_idx]
-                sp_xmat = sp_xmat[:, keep_idx]
-                pxmat = [list(sp_xmat[i].indices) for i in range(num_exp)]
-
-            # eye_indices = [item for inner in pxmat for item in inner]
-            # eye_block = dual_socp.linear[eye_indices, :]
-            # if len(eye_block.data) + 1 == len(eye_block.indptr):
-
-            linear = dual_socp.linear
-            const = dual_socp.const
-            sense = dual_socp.sense
-            obj = dual_socp.obj
-            vtype = dual_socp.vtype
-            ub = dual_socp.ub
-            lb = dual_socp.lb
-            qmat = dual_socp.qmat
-
-            num_xc = len(pxmat)
-            count_col = np.arange(0, 3*num_xc, 3).reshape((num_xc, 1))
-            xmat = count_col + np.array([[0, 1, 2]]*num_xc)
-            xmat = list((linear.shape[1] + xmat))
-            data = [-1, 1, -1, -1] * num_xc
-            i_idx = np.array([ex + ex[-1:] for ex in pxmat]).flatten()
-            j_idx = (count_col + np.array([2, 1, 0, 2])).flatten()
-            extra_block = sp.csr_matrix((data, (i_idx, j_idx)),
-                                        (linear.shape[0], 3*num_xc))
-            linear = sp.hstack((linear, extra_block))
-            obj = np.hstack((obj, np.zeros(3*num_xc)))
-            ub = np.hstack((ub, np.inf*np.ones(3*num_xc)))
-            lb = np.hstack((lb, -np.inf*np.ones(3*num_xc)))
-            vtype = np.hstack((vtype, np.array(['C']*3*num_xc)))
-            formula = GCProg(sp.csr_matrix(linear), const, sense,
-                             vtype, ub, lb, qmat, xmat, obj)
+                linear = dual_lp.linear
+                num_constr = dual_lp.linear.shape[1]
+                extra_nvar = len(eye_indices)
+                extra_block = sp.csr_matrix((np.ones(extra_nvar),
+                                             (eye_indices, np.arange(extra_nvar))),
+                                            shape=(linear.shape[0], extra_nvar))
+                linear = sp.csr_matrix(sp.hstack((linear, extra_block)))
+                const = dual_lp.const
+                sense = dual_lp.sense
+
+                obj = np.concatenate((dual_lp.obj, np.zeros(extra_nvar)))
+                vtype = np.concatenate((dual_lp.vtype, np.array(['C']*extra_nvar)))
+
+                ub = np.concatenate((dual_lp.ub, np.ones(extra_nvar)*np.infty))
+                extra_lb = - np.ones(extra_nvar)*np.infty
+                ind_pos = 0
+                for qc in primal.qmat:
+                    extra_lb[ind_pos] = 0
+                    ind_pos += len(qc)
+                lb = np.concatenate((dual_lp.lb, extra_lb))
+
+                qmat = []
+                ind_pos = 0
+                for qc in primal.qmat:
+                    qmat.append([ind_pos+num_constr] +
+                                [k+ind_pos+num_constr for k in range(1, len(qc))])
+                    ind_pos += len(qc)
+
+                formula = SOCProg(linear, const, sense,
+                                  vtype, ub, lb, qmat, obj)
 
             self.dual = formula
             self.dupdate = False
+
             return formula
 
 
-class GCProg(SOCProg):
+class SOCProg(LinProg):
+    """
+    The SOCProg class creates an second-order cone program
+    """
 
-    def __init__(self, linear, const, sense, vtype, ub, lb, qmat, xmat, obj=None):
+    def __init__(self, linear, const, sense, vtype, ub, lb, qmat, obj=None):
 
-        super().__init__(linear, const, sense, vtype, ub, lb, qmat, obj)
-        self.xmat = xmat
+        super().__init__(linear, const, sense, vtype, ub, lb, obj)
+        self.qmat = qmat
 
     def __repr__(self):
 
-        xmat = self.xmat
-        string = 'Conic program object:\n'
-        socp_str = super().__repr__()
-        string += socp_str[socp_str.find('\n')+1:]
+        qmat = self.qmat
+        string = 'Second order cone program object:\n'
+        string += super().__repr__()
         string += '---------------------------------------------\n'
-        string += 'Number of ExpCone constraints: {0}\n'.format(len(xmat))
+        string += 'Number of SOC constraints:     {0}\n'.format(len(qmat))
 
         return string
 
-    def showec(self):
+    def showqc(self):
 
-        n = len(self.xmat)
+        n = len(self.qmat)
 
         if n == 0:
             return None
 
-        indices = np.concatenate([item for item in self.xmat])
-        values = [1, 2, 3] * n
-        indptr = range(0, 3*n+1, 3)
+        indices = np.concatenate([item for item in self.qmat])
+        values = np.concatenate([[-1.0] + [1.0]*(len(item)-1)
+                                 for item in self.qmat])
+        indptr = [0] * (n + 1)
+        for i in range(n):
+            indptr[i+1] = indptr[i] + len(self.qmat[i])
 
         var_names = ['x{0}'.format(i)
                      for i in range(1, self.linear.shape[1] + 1)]
-        constr_names = ['EC{0}'.format(j)
+        constr_names = ['QC{0}'.format(j)
                         for j in range(1, n + 1)]
         table = pd.DataFrame(sp.csr_matrix((values, indices, indptr),
                              (n, self.linear.shape[1])).todense(),
                              index=constr_names, columns=var_names)
-        table['sense'] = ['-'] * n
-        table['constant'] = ['-'] * n
+        table['sense'] = ['<='] * n
+        table['constant'] = [0.0] * n
 
         return table
 
     def show(self):
         """
         Returns a pandas.DataFrame that summarizes the information on the
         optimization problem.
@@ -297,20 +302,31 @@
         obj_row = pd.DataFrame(self.obj.reshape((1, self.obj.size)),
                                columns=table.columns[:-2], index=['Obj'])
         table = pd.concat([obj_row, table], axis=0)
 
         table_qc = self.showqc()
         if table_qc is not None:
             table = pd.concat([table, table_qc], axis=0)
-        table_ec = self.showec()
-        if table_ec is not None:
-            table = pd.concat([table, table_ec], axis=0)
 
         ub = pd.DataFrame(self.ub.reshape((1, self.ub.size)),
                           columns=table.columns[:-2], index=['UB'])
         lb = pd.DataFrame(self.lb.reshape((1, self.lb.size)),
                           columns=table.columns[:-2], index=['LB'])
         vtype = pd.DataFrame(self.vtype.reshape((1, self.vtype.size)),
                              columns=table.columns[:-2], index=['Type'])
         table = pd.concat([table, ub, lb, vtype], axis=0)
 
         return table.fillna('-')
+
+    def lp_export(self):
+
+        string = super().lp_export()
+        index_st = string.find('Subject To')
+        s1 = string[:index_st+11]
+        s2 = string[index_st+11:]
+        sq = ''
+        for i, qc in enumerate(self.qmat):
+            sq += ' q{}: [ '.format(i+1)
+            sq += ' + '.join(['x{} ^2'.format(j+1) for j in qc[1:]])
+            sq += ' - x{} ^2 ] <= 0\n'.format(qc[0]+1)
+
+        return s1 + sq + s2
```

### Comparing `rsome-1.1.4/rsome/grb_solver.py` & `rsome-1.2.0/rsome/grb_solver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """
 This module is used as an interface to call the Gurobi solver for solving
 (mixed-integer) linear or second-order cone programs.
 """
 
+from gurobipy import GurobiError
 import gurobipy as gp
 import numpy as np
 import warnings
 import time
 from .socp import SOCProg
 from .lp import Solution
 
 
 def solve(formula, display=True, params={}):
 
     try:
         if formula.xmat:
             warnings.warn('The SOCP solver ignores exponential cone constraints. ')
+        if formula.lmi:
+            warnings.warn('The SOCP solver ignores semidefinite cone constraints. ')
     except AttributeError:
         pass
 
     nv = formula.linear.shape[1]
     vtype = list(formula.vtype)
 
     grb = gp.Model()
@@ -28,18 +31,18 @@
     indices_eq = (formula.sense == 1)
     indices_ineq = (formula.sense == 0)
     linear_eq = formula.linear[indices_eq, :]
     linear_ineq = formula.linear[indices_ineq, :]
     const_eq = formula.const[indices_eq]
     const_ineq = formula.const[indices_ineq]
     if len(indices_eq) > 0:
-        grb.addMConstr(linear_eq, x, '=', const_eq)
+        c_eq = grb.addMConstr(linear_eq, x, '=', const_eq)
         # grb.addMConstrs(linear_eq, x, '=', const_eq)
     if len(indices_ineq) > 0:
-        grb.addMConstr(linear_ineq, x, '<', const_ineq)
+        c_ineq = grb.addMConstr(linear_ineq, x, '<', const_ineq)
         # grb.addMConstrs(linear_ineq, x, '<', const_ineq)
 
     if isinstance(formula, SOCProg):
         for constr in formula.qmat:
             index_right = constr[0:1]
             index_left = constr[1:]
             A = np.eye(len(index_left))
@@ -61,18 +64,29 @@
         print('Being solved by Gurobi...', flush=True)
         time.sleep(0.2)
     grb.optimize()
     if display:
         print('Solution status: {0}'.format(grb.Status))
         print('Running time: {0:0.4f}s'.format(grb.Runtime))
 
-    # if export:
-    #     grb.write("out.lp")
+    try:
+        pi = np.ones(formula.linear.shape[0]) * np.nan
+        upi = np.zeros(nv)
+        lpi = np.zeros(nv)
+        pi[indices_eq] = c_eq.pi
+        pi[indices_ineq] = c_ineq.pi
+        rc = x.rc
+        upi[rc < 0] = rc[rc < 0]
+        lpi[rc > 0] = rc[rc > 0]
+        y = {'pi': pi, 'upi': upi, 'lpi': lpi}
+    except GurobiError:
+        y = None
 
     try:
-        solution = Solution(grb.ObjVal, np.array(grb.getAttr('X')),
-                            grb.Status, grb.Runtime)
+        solution = Solution('Gurobi', grb.ObjVal, np.array(grb.getAttr('X')),
+                            grb.Status, grb.Runtime, y=y)
     except AttributeError:
         warnings.warn('Fail to find the optimal solution.')
-        solution = None
+        # solution = None
+        solution = Solution('Gurobi', np.nan, None, grb.Status, grb.Runtime)
 
     return solution
```

### Comparing `rsome-1.1.4/rsome/lp.py` & `rsome-1.2.0/rsome/lp.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 import numpy as np
 import pandas as pd
 import scipy.sparse as sp
 import warnings
 import time
 import scipy.optimize as opt
 from numbers import Real
-from scipy.sparse import csr_matrix
-from scipy.sparse import coo_matrix
+from scipy.sparse import csr_matrix, coo_matrix, lil_matrix
 from scipy.linalg import sqrtm, eigh
 from collections.abc import Iterable, Sized
-from typing import List
+# from typing import List
 
 
 def def_sol(formula, display=True, params={}):
     """
     This is the default solver of RSOME.
     """
 
@@ -26,23 +25,69 @@
             warnings.warn('the LP solver ignores SOC constraints.')
     except AttributeError:
         pass
 
     try:
         if formula.xmat:
             warnings.warn('The LP solver ignores exponential cone constraints.')
+        if formula.lmi:
+            warnings.warn('The LP solver ignores semidefinite cone constraints.')
     except AttributeError:
         pass
 
-    if hasattr(opt, 'milp'):
+    A = formula.linear
+    sense = formula.sense
+    vtype = formula.vtype
+    num_constr = A.shape[0]
 
-        A = formula.linear
-        sense = formula.sense
-        vtype = formula.vtype
+    if all(vtype == 'C'):
+        indices_eq = (formula.sense == 1)
+        indices_ineq = (formula.sense == 0)
+        linear_eq = formula.linear[indices_eq, :] if len(indices_eq) else None
+        linear_ineq = formula.linear[indices_ineq, :] if len(indices_ineq) else None
+        const_eq = formula.const[indices_eq] if len(indices_eq) else None
+        const_ineq = formula.const[indices_ineq] if len(indices_ineq) else None
+
+        bounds = [(lb, ub) for lb, ub in zip(formula.lb, formula.ub)]
 
+        default = {'maxiter': 1000000000}
+
+        if display:
+            print('Being solved by the default LP solver...', flush=True)
+            time.sleep(0.2)
+        t0 = time.time()
+        res = opt.linprog(formula.obj, A_ub=linear_ineq, b_ub=const_ineq,
+                          A_eq=linear_eq, b_eq=const_eq,
+                          bounds=bounds, options=default)
+        stime = time.time() - t0
+        if display:
+            print('Solution status: {0}'.format(res.status))
+            print('Running time: {0:0.4f}s'.format(stime))
+
+        if res.status == 0:
+            objval = formula.obj @ res.x
+
+            pi = np.ones(num_constr) * np.nan
+            upi = res['upper']['marginals']
+            lpi = res['lower']['marginals']
+            pi[indices_eq] = res['eqlin']['marginals']
+            pi[indices_ineq] = res['ineqlin']['marginals']
+            y = {'pi': pi, 'upi': upi, 'lpi': lpi}
+
+            return Solution('SciPy', objval, res.x, res.status, stime, y=y)
+        else:
+            status = res.status
+            msg = 'The optimal solution can not be found, '
+            reasons = ('iteration limit is reached.' if status == 1 else
+                       'the problem appears to be infeasible.' if status == 2 else
+                       'the problem appears to be unbounded.' if status == 3 else
+                       'numerical difficulties encountered.')
+            msg += 'because {}'.format(reasons)
+            return Solution('Scipy', np.nan, None, status, stime)
+    else:
         b_u = formula.const
         b_l = np.ones(A.shape[0]) * (-np.inf)
         bool_eq = (sense == 1)
         b_l[bool_eq] = b_u[bool_eq]
 
         bool_bin = (vtype == 'B')
         lb = formula.lb
@@ -50,80 +95,185 @@
         lb[bool_bin] = 0
         ub[bool_bin] = 1
 
         integrality = np.zeros(A.shape[1])
         integrality[vtype != 'C'] = 1
 
         if display:
-            if all(vtype == 'C'):
-                print('Being solved by the default LP solver...', flush=True)
-            else:
-                print('Being solved by the default MILP solver...', flush=True)
+            print('Being solved by the default MILP solver...', flush=True)
             time.sleep(0.2)
         t0 = time.time()
-        res = opt.milp(formula.obj.squeeze(),
-                       constraints=opt.LinearConstraint(A, b_l, b_u),
-                       bounds=opt.Bounds(lb, ub),
-                       integrality=integrality)
+        if all(vtype == 'C'):
+            linear_ineq = A[sense == 0]
+            const_ineq = formula.const[sense == 0]
+            linear_eq = A[sense == 1]
+            const_eq = formula.const[sense == 1]
+            bounds = [(lb, ub) for lb, ub in zip(formula.lb, formula.ub)]
+            default = {'maxiter': 1000000000}
+            res = opt.linprog(formula.obj, A_ub=linear_ineq, b_ub=const_ineq,
+                              A_eq=linear_eq, b_eq=const_eq,
+                              bounds=bounds, options=default)
+        else:
+            res = opt.milp(formula.obj,
+                           constraints=opt.LinearConstraint(A, b_l, b_u),
+                           bounds=opt.Bounds(lb, ub),
+                           integrality=integrality)
         stime = time.time() - t0
         if display:
             print('Solution status: {0}'.format(res.status))
             print('Running time: {0:0.4f}s'.format(stime))
 
         if res.status == 0:
-            objval = formula.obj[0] @ res.x
-            return Solution(objval, res.x, res.status, stime)
+            objval = formula.obj @ res.x
+            return Solution('SciPy', objval, res.x, res.status, stime)
         else:
             status = res.status
-            msg = 'Fail to find the optimal solution.'
-            warnings.warn(msg)
-        return None
+            # msg = 'Fail to find the optimal solution.'
+            # warnings.warn(msg)
+            return Solution('Scipy', np.nan, None, status, stime)
+
+
+def concat(iters, axis=0):
+    """
+    Join a sequence of arrays of affine expressions along an existing axis.
+
+        Parameters
+        ----------
+        iters : array_like.
+            A sequence of RSOME variables or affine expressions. The arrays must
+            have the same shape, except in the dimension corresponding to `axis`
+            (the first, by default).
+
+        axis : int, optional
+            The axis along which the arrays will be joined.  Default is 0.
+
+        Returns
+        -------
+        out : Affine
+            The concatenated array of affine expressions.
+    """
 
+    linear_each = []
+    const_each = []
+    idx_each = []
+    count = 0
+    model = None
+    event_adapt = None
+    fixed = True
+    ctype = None
+    for item in iters:
+        if not isinstance(item, Affine):
+            item = item.to_affine()
+        if isinstance(item, DecAffine):
+            if event_adapt is None:
+                event_adapt = [list(range(item.model.top.num_scen))]
+            if ctype is None:
+                ctype = item.ctype
+            if ctype != item.ctype:
+                raise ValueError('Cannot concatenate different types of expressions.')
+            event_adapt = comb_set(event_adapt, item.event_adapt)
+            fixed = fixed and item.fixed
+        if model is None:
+            model = item.model
+            num_var = model.last
+        else:
+            if model != item.model:
+                raise ValueError('Model mismatch.')
+
+        if item.linear.shape[1] < num_var:
+            item.linear.resize(item.linear.shape[0], num_var)
+        linear_each.append(item.linear)
+        const_each.append(item.const)
+        idx_each.append(np.arange(count, count+item.size).reshape(item.shape))
+
+        count += item.size
+
+    ndim = max([i.ndim for i in idx_each])
+    idx_each = [i.reshape([1] * ndim) if i.shape == () else i
+                for i in idx_each]
+    const_each = [const.reshape([1] * ndim) if const.shape == () else const
+                  for const in const_each]
+
+    idx_all = np.concatenate(idx_each, axis=axis).flatten()
+    linear_all = sp.vstack(linear_each)[idx_all]
+    const_all = np.concatenate(const_each, axis=axis)
+
+    affine = Affine(item.model, linear_all, const_all)
+    if event_adapt is None:
+        return affine
     else:
+        return DecAffine(item.model.top, affine, event_adapt, fixed, ctype)
 
-        if any(np.array(formula.vtype) != 'C'):
-            warnings.warn('Integrality constraints are ignored in the LP solver. ')
 
-        indices_eq = (formula.sense == 1)
-        indices_ineq = (formula.sense == 0)
-        linear_eq = formula.linear[indices_eq, :] if len(indices_eq) else None
-        linear_ineq = formula.linear[indices_ineq, :] if len(indices_ineq) else None
-        const_eq = formula.const[indices_eq] if len(indices_eq) else None
-        const_ineq = formula.const[indices_ineq] if len(indices_ineq) else None
+def rstack(*args):
+    """
+    Stack a sequence of rows of affine expressions vertically (row wise).
 
-        bounds = [(lb, ub) for lb, ub in zip(formula.lb, formula.ub)]
+        Parameters
+        ----------
+        arg : {list, Affine}.
+            Each arg represents an array of affine expressions. If arg is a list
+            of affine expressions, they will be concatenated horizontally (column
+            wise) first.
 
-        default = {'maxiter': 1000000000,
-                   'sparse': True}
+        Returns
+        -------
+        out : Affine
+            The vertically stacked array of affine expressions.
 
-        if display:
-            print('Being solved by the default LP solver...', flush=True)
-            time.sleep(0.2)
-        t0 = time.time()
-        res = opt.linprog(formula.obj, A_ub=linear_ineq, b_ub=const_ineq,
-                          A_eq=linear_eq, b_eq=const_eq,
-                          bounds=bounds, options=default)
-        stime = time.time() - t0
-        if display:
-            print('Solution status: {0}'.format(res.status))
-            print('Running time: {0:0.4f}s'.format(stime))
+        Notes
+        -----
+        The rstack function is different from the vstack function from the numpy
+        package in 1) the arrays to be stacked together are presented as separate
+        arguments, instead of elements in an array-like sequence; and 2) a list of
+        arrays can be stacked horizontally first before being vertically stacked.
+    """
 
-        if res.status == 0:
-            objval = formula.obj[0] @ res.x
-            return Solution(objval, res.x, res.status, stime)
+    rows = []
+    for arg in args:
+        if isinstance(arg, Iterable):
+            rows.append(concat(arg, axis=1))
         else:
-            status = res.status
-            msg = 'The optimal solution can not be found, '
-            reasons = ('iteration limit is reached.' if status == 1 else
-                       'the problem appears to be infeasible.' if status == 2 else
-                       'the problem appears to be unbounded.' if status == 3 else
-                       'numerical difficulties encountered.')
-            msg += 'because {}'.format(reasons)
-            warnings.warn(msg)
-            return None
+            rows.append(arg)
+
+    return concat(rows, axis=0)
+
+
+def cstack(*args):
+    """
+    Stack a sequence of rows of affine expressions horizontally (column wise).
+
+        Parameters
+        ----------
+        arg : {list, Affine}.
+            Each arg represents an array of affine expressions. If arg is a list
+            of affine expressions, they will be concatenated vertically (row wise)
+            first.
+
+        Returns
+        -------
+        out : Affine
+            The horizontally stacked array of affine expressions.
+
+        Notes
+        -----
+        The cstack function is different from the hstack function from the numpy
+        package in 1) the arrays to be stacked together are presented as separate
+        arguments, instead of elements in an array-like sequence; and 2) a list of
+        arrays can be stacked vertically first before being horizontally stacked.
+    """
+
+    cols = []
+    for arg in args:
+        if isinstance(arg, Iterable):
+            cols.append(concat(arg, axis=0))
+        else:
+            cols.append(arg)
+
+    return concat(cols, axis=1)
 
 
 class Model:
     """
     The Model class creates an LP model object.
     """
 
@@ -133,14 +283,16 @@
         self.top = top
         self.nobj = nobj
         self.name = name
 
         self.vars = []
         self.auxs = []
         self.last = 0
+        self.constr_idx = 0
+        self.ciarray = None
         self.lin_constr = []
         self.pws_constr = []
         self.bounds = []
         self.aux_constr = []
         self.aux_bounds = []
         self.obj = None
         self.sign = 1
@@ -195,26 +347,32 @@
                 self.st(item)
         else:
             if not isinstance(constr, (LinConstr, CvxConstr, Bounds)):
                 raise TypeError('Unknown constraint type.')
             if constr.model is not self:
                 raise ValueError('Constraints are not defined for this model.')
             if isinstance(constr, LinConstr):
+                constr.index = self.constr_idx
+                self.constr_idx += 1
                 self.lin_constr.append(constr)
             elif isinstance(constr, CvxConstr):
                 if constr.xtype in 'AMI':
                     self.pws_constr.append(constr)
                 else:
                     raise TypeError('Incorrect constraint type.')
             elif isinstance(constr, Bounds):
+                # onstr.index = self.constr_idx
+                # self.constr_idx += 1
                 self.bounds.append(constr)
 
         self.pupdate = True
         self.dupdate = True
 
+        return constr
+
     def min(self, obj):
         """
         Minimize the given objective function.
 
         Parameters
         ----------
         obj
@@ -332,26 +490,30 @@
                     aux = self.dvar(1, aux=True)
                     self.aux_constr.append(affine_in <= aux)
                     self.aux_constr.append(-affine_in <= aux)
                     self.aux_constr.append(aux + constr.affine_out <= 0)
             if obj:
                 obj = np.array(csr_matrix(([1.0], ([0], [0])),
                                           (1, self.last)).todense())
+                obj = obj.reshape(obj.size)
             else:
-                obj = np.ones((1, self.last))
+                # obj = np.ones((1, self.last))
+                obj = np.ones(self.last)
 
             data_list = []
             indices_list = []
             indptr = [0]
             last = 0
 
             data_list += [item.linear.data
                           for item in self.lin_constr + self.aux_constr]
             indices_list += [item.linear.indices
                              for item in self.lin_constr + self.aux_constr]
+            constr_idx_list = [np.array([item.index] * item.linear.shape[0])
+                               for item in self.lin_constr + self.aux_constr]
 
             if data_list:
                 data = np.concatenate(tuple(data_list))
                 indices = np.concatenate(tuple(indices_list))
                 for item in self.lin_constr + self.aux_constr:
                     indptr.extend(list(item.linear.indptr[1:] + last))
                     last += item.linear.indptr[-1]
@@ -389,14 +551,19 @@
                     lb[b.indices] = np.maximum(b.values, lb[b.indices])
 
             formula = LinProg(linear, const, sense,
                               vtype, ub, lb, obj)
             self.primal = formula
             self.pupdate = False
 
+            if constr_idx_list:
+                self.ciarray = np.concatenate(constr_idx_list)
+            else:
+                self.ciarray = []
+
             return formula
 
         else:
             if self.dual is not None and not self.dupdate:
                 return self.dual
 
             primal = self.do_math(obj=obj)
@@ -463,22 +630,22 @@
     def solve(self, solver=None, display=True, params={}):
         """
         Solve the model with the selected solver interface.
 
         Parameters
         ----------
             solver : {None, lpg_solver, clp_solver, ort_solver, eco_solver
-                      cpx_solver, grb_solver, msk_solver}
+                      cpx_solver, grb_solver, msk_solver, cpt_solver}
                 Solver interface used for model solution. Use default solver
                 if solver=None.
             display : bool
                 Display option of the solver interface.
             params : dict
                 A dictionary that specifies parameters of the selected solver.
-                So far the argument only applies to Gurobi, CPLEX,and MOSEK.
+                So far the argument only applies to Gurobi, CPLEX, and Mosek.
         """
 
         if solver is None:
             solution = def_sol(self.do_math(obj=True), display, params)
         else:
             solution = solver.solve(self.do_math(obj=True), display, params)
 
@@ -494,15 +661,22 @@
         Notes
         -----
         An error message is given if the model is unsolved or no solution
         is obtained.
         """
 
         if self.solution is None:
-            raise RuntimeError('The model is unsolved or no solution is obtained.')
+            raise RuntimeError('The model is unsolved.')
+
+        solution = self.solution
+        if np.isnan(solution.objval):
+            msg = 'No solution available. '
+            msg += f'{solution.solver} solution status: {solution.status}.'
+            raise RuntimeError(msg)
+
         return self.sign * self.solution.objval
 
     def optimal(self):
 
         return self.solution is not None
 
 
@@ -606,14 +780,30 @@
 
         return np.array(range(self.first, self.first + self.size))
 
     def reshape(self, shape):
 
         return self.to_affine().reshape(shape)
 
+    def flatten(self):
+
+        return self.to_affine().flatten()
+
+    def diag(self, k=0, fill=False):
+
+        return self.to_affine().diag(k, fill)
+
+    def tril(self, k=0):
+
+        return self.to_affine().tril(k)
+
+    def triu(self, k=0):
+
+        return self.to_affine().triu(k)
+
     def abs(self):
 
         return self.to_affine().abs()
 
     def norm(self, degree):
         """
         Return the first, second, or infinity norm of a 1-D array.
@@ -662,14 +852,18 @@
         See Also
         --------
         rso.quad : equivalent function
         """
 
         return self.to_affine().quad(qmat)
 
+    def rsocone(self, y, z):
+
+        return self.to_affine().rsocone(y, z)
+
     def expcone(self, x, z):
         """
         Return the exponential cone constraint z*exp(x/z) <= var.
 
         Refer to `rsome.expcone` for full documentation.
 
         See Also
@@ -742,26 +936,30 @@
         See Also
         --------
         rso.entropy : equivalent function
         """
 
         return self.to_affine().entropy()
 
-    def kldiv(self, phat, r):
+    def kldiv(self, q, r):
         """
-        Return the KL divergence constraints sum(var*log(var/phat)) <= r.
+        Return the KL divergence constraints sum(var*log(var/q)) <= r.
 
         Refer to `rsome.kldiv` for full documentation.
 
         See Also
         --------
         rso.kldiv : equivalent function
         """
 
-        return self.to_affine().kldiv(phat, r)
+        return self.to_affine().kldiv(q, r)
+
+    def trace(self):
+
+        return self.to_affine().trace()
 
     def get(self):
         """
         Return the optimal solution of the decision variable.
 
         Notes
         -----
@@ -773,18 +971,24 @@
         infeasibility, unboundedness, or numeric issues.
         """
 
         if self.model.mtype not in 'VR':
             raise TypeError('Not a decision variable.')
 
         if self.model.solution is None:
-            raise RuntimeError('The model is unsolved or no solution is obtained.')
+            raise RuntimeError('The model is unsolved.')
+
+        solution = self.model.solution
+        if np.isnan(solution.objval):
+            msg = 'No solution available. '
+            msg += f'{solution.solver} solution status: {solution.status}.'
+            raise RuntimeError(msg)
 
         indices = range(self.first, self.first + self.size)
-        var_sol = np.array(self.model.solution.x)[indices]
+        var_sol = np.array(solution.x)[indices]
         if self.shape == ():
             var_sol = var_sol[0]
         else:
             var_sol = var_sol.reshape(self.shape)
 
         return var_sol
 
@@ -871,14 +1075,22 @@
         else:
             return self.to_affine() >= other
 
     def __eq__(self, other):
 
         return self.to_affine() == other
 
+    def __rshift__(self, other):
+
+        return self.to_affine().__rshift__(other)
+
+    def __lshift__(self, other):
+
+        return self.to_affine().__lshift__(other)
+
     def assign(self, values):
 
         if self.model.mtype != 'S':
             raise ValueError('Unsupported variables.')
         else:
             if not isinstance(values, (np.ndarray, Real)):
                 raise TypeError('The second argument must be numerical values.')
@@ -1087,26 +1299,98 @@
 
         if isinstance(self.const, np.ndarray):
             new_const = self.const.reshape(shape)
         else:
             new_const = np.array([self.const]).reshape(shape)
         return Affine(self.model, self.linear, new_const)
 
+    def flatten(self):
+
+        return self.reshape((self.size, ))
+
+    def diag(self, k=0, fill=False):
+
+        if len(self.shape) != 2:
+            raise ValueError('The diag function can only be applied to 2D arrays.')
+
+        num = min(self.shape)
+        if k >= 0:
+            idx_row = np.arange(num - k)
+            idx_col = np.arange(k, num)
+        else:
+            idx_row = np.arange(-k, num)
+            idx_col = np.arange(num + k)
+
+        if fill:
+            bool_mat = np.ones(self.shape, dtype=bool)
+            bool_mat[idx_row, idx_col] = False
+            bool_idx = bool_mat.flatten()
+
+            affine = self + 0
+            affine.linear = lil_matrix(affine.linear)
+            affine.linear[bool_idx] = 0.0
+            affine.linear = csr_matrix(affine.linear)
+            affine.const = np.diag(np.diag(affine.const, k), k)
+
+            return affine
+        else:
+            return self[idx_row, idx_col]
+
+    def tril(self, k=0):
+
+        if len(self.shape) != 2:
+            raise ValueError('The tril function can only be applied to 2D arrays.')
+
+        bool_idx = (~np.tril(np.ones(self.shape, dtype=bool), k)).flatten()
+
+        affine = self + 0
+        affine.linear = lil_matrix(affine.linear)
+        affine.linear[bool_idx] = 0.0
+        affine.linear = csr_matrix(affine.linear)
+        affine.const = np.tril(affine.const, k)
+
+        return affine
+
+    def triu(self, k=0):
+
+        if len(self.shape) != 2:
+            raise ValueError('The tril function can only be applied to 2D arrays.')
+
+        bool_idx = (~np.triu(np.ones(self.shape, dtype=bool), k)).flatten()
+
+        affine = self + 0
+        affine.linear = lil_matrix(affine.linear)
+        affine.linear[bool_idx] = 0.0
+        affine.linear = csr_matrix(affine.linear)
+        affine.const = np.triu(affine.const, k)
+
+        return affine
+
     def sum(self, axis=None):
 
         if self.sparray is None:
             self.sparray = self.sv_array()
 
         indices = self.sparray.sum(axis=axis)
 
         linear = sv_to_csr(indices) @ self.linear
         const = self.const.sum(axis=axis)
 
         return Affine(self.model, linear, const)
 
+    def trace(self):
+
+        if len(self.shape) != 2:
+            raise ValueError('The trace function only applies to two-dimensional arrays')
+        dim = min(self.shape)
+
+        out = self[range(dim), range(dim)].sum()
+
+        return out
+
     def __abs__(self):
 
         return Convex(self, np.zeros(self.shape), 'A', 1)
 
     def abs(self):
 
         return self.__abs__()
@@ -1206,14 +1490,47 @@
         affine = sqrt_mat @ self.reshape(self.size)
 
         if sign == 1:
             return affine.sumsqr()
         else:
             return - affine.sumsqr()
 
+    def rsocone(self, y, z):
+
+        if self.size > 1:
+            if self.size != max(self.shape):
+                err = 'Improper number of dimensions to norm. '
+                err += 'The array must be a vector.'
+                raise ValueError(err)
+
+        if isinstance(y, (Vars, VarSub, Affine)):
+            y = y.to_affine()
+            if y.size > 1:
+                raise ValueError('The expression of x must be a scalar.')
+        else:
+            raise TypeError('Unsupoorted type for rotated cone. ')
+        if isinstance(y, (Vars, VarSub, Affine)):
+            if self.model is not y.model:
+                raise ValueError('Models mismatch.')
+
+        if isinstance(z, (Vars, VarSub, Affine)):
+            z = z.to_affine()
+            if z.size > 1:
+                raise ValueError('The expression of z must be a scalar.')
+        else:
+            raise TypeError('Unsupoorted type for rotated cone. ')
+        if isinstance(z, (Vars, VarSub, Affine)):
+            if self.model is not z.model:
+                raise ValueError('Models mismatch.')
+
+        affine_in = concat((((y-z)*0.5).reshape((1,)), self))
+        affine_out = - ((y+z)*0.5).reshape((1,))
+
+        return CvxConstr(self.model, affine_in, affine_out, multiplier=1, xtype='E')
+
     def expcone(self, x, z):
         """
         Return the exponential cone constraint z*exp(x/z) <= affine.
 
         Refer to `rsome.expcone` for full documentation.
 
         See Also
@@ -1310,43 +1627,63 @@
 
         if self.shape != ():
             if self.size != max(self.shape):
                 raise ValueError('The expression must be a vector.')
 
         return Convex(self, np.float64(0), 'P', -1)
 
-    def kldiv(self, phat, r):
+    def kldiv(self, q, r):
         """
-        Return the KL divergence constraints sum(var*log(var/phat)) <= r.
+        Return the KL divergence constraints sum(affine*log(affine/q)) <= r.
 
         Refer to `rsome.kldiv` for full documentation.
 
         See Also
         --------
         rso.kldiv : equivalent function
         """
 
         affine = self.to_affine().reshape((self.size, ))
 
-        if isinstance(phat, Real):
-            phat = np.array([phat]*self.size)
-        elif isinstance(phat, np.ndarray):
-            if phat.size == 1:
-                phat = np.array([phat.flatten()[0]] * self.size)
+        if isinstance(q, Real):
+            q = np.array([q]*self.size)
+        elif isinstance(q, np.ndarray):
+            if q.size == 1:
+                q = np.array([q.flatten()[0]] * self.size)
             else:
-                phat = phat.reshape(affine.shape)
-        elif isinstance(phat, (Vars, VarSub, Affine)):
-            if affine.model is not phat.model:
+                q = q.reshape(affine.shape)
+        elif isinstance(q, (Vars, VarSub, Affine)):
+            if affine.model is not q.model:
                 raise ValueError('Models mismatch.')
-            if phat.size == 1:
-                phat = phat * np.ones(affine.shape)
+            if q.size == 1:
+                q = q * np.ones(affine.shape)
             else:
-                phat = phat.reshape(affine.shape)
+                q = q.reshape(affine.shape)
+
+        return KLConstr(affine, q, r)
+
+    def concat(self, other, axis=0):
 
-        return KLConstr(affine, phat, r)
+        if not isinstance(other, Affine):
+            raise TypeError('Incorrect type in concatenation.')
+        if self.model != other.model:
+            raise ValueError('Model mismatch.')
+
+        idx_left = np.arange(self.size).reshape(self.shape)
+        idx_other = np.arange(self.size, self.size + other.size).reshape(other.shape)
+        idx_all = np.concatenate((idx_left, idx_other), axis=axis).flatten()
+
+        if self.linear.shape[1] < other.linear.shape[1]:
+            self.linear.resize(self.linear.shape[0], other.linear.shape[1])
+        if self.linear.shape[1] > other.linear.shape[1]:
+            other.linear.resize(other.linear.shape[0], self.linear.shape[1])
+        linear_all = sp.vstack((self.linear, other.linear))[idx_all]
+        const_all = np.concatenate((self.const, other.const), axis=axis)
+
+        return Affine(self.model, linear_all, const_all)
 
     def __mul__(self, other):
 
         if isinstance(other, (Vars, VarSub, Affine)):
             other = other.to_affine()
             if self.model.mtype == other.model.mtype:
                 raise TypeError('Bi-linear expressions are not supported.')
@@ -1576,14 +1913,32 @@
         if isinstance(left, Affine) and not isinstance(left, DecAffine):
             return LinConstr(left.model, left.linear,
                              -left.const.reshape((left.const.size,)),
                              np.ones(left.const.size))
         else:
             return left.__eq__(0)
 
+    def __rshift__(self, other):
+
+        left = self - other
+        if len((left.shape)) != 2:
+            msg = """Only two-dimensional arrays can be used to construct linear
+            matrix equality constraints."""
+            raise ValueError(msg)
+        if left.shape[0] != left.shape[1]:
+            msg = """Only two-dimensional square arrays can be used to construct
+            linear matrix equality constraints."""
+            raise ValueError(msg)
+
+        return LMIConstr(left.model, left.linear, -left.const, left.shape[0])
+
+    def __lshift__(self, other):
+
+        return (-self).__rshift__(-other)
+
     def __call__(self):
 
         if self.model.mtype != 'R':
             raise ValueError('Unsupported affine expression.')
 
         if self.model.solution is None:
             raise SyntaxError('No available solution!')
@@ -2166,23 +2521,64 @@
     def __init__(self, model, linear, const, sense, sign=1):
 
         self.model = model
         self.linear = linear
         self.const = const
         self.sense = sense
         self.sign = sign
+        self.index = None
 
     def __repr__(self):
 
         size = self.linear.shape[0]
         if size == 1:
             return '1 linear constraint'
         else:
             return '{} linear constraints'.format(size)
 
+    def dual(self):
+
+        if self.model.solution is None:
+            raise RuntimeError('The model is unsolved. ')
+
+        cidx = self.index
+        if cidx is None:
+            raise RuntimeError('The constraint is not a part of any model. ')
+
+        solution = self.model.solution
+        if solution.y is None:
+            msg = 'The dual solution is not available. '
+            msg += f'{solution.solver} solution status: {solution.status}.'
+            warnings.warn(msg)
+        else:
+            dual_sol = solution.y['pi'][self.model.ciarray == cidx] * self.model.sign
+            if dual_sol.size == 1:
+                dual_sol = dual_sol.item()
+
+            return dual_sol
+
+
+class LMIConstr:
+    """
+    The LMIConstr class creates an object of linear matrix inequality
+    constraints.
+    """
+
+    def __init__(self, model, linear, const, dim):
+
+        self.model = model
+        self.linear = linear
+        self.const = const
+        self.dim = dim
+
+    def __repr__(self):
+
+        dim = int(self.linear.shape[0] ** 0.5)
+        return f'{dim}x{dim} linear matrix inequliaty constraint'
+
 
 class CvxConstr:
     """
     The CvxConstr class creates an object of convex constraints.
     """
 
     def __init__(self, model, affine_in, affine_out, multiplier, xtype):
@@ -2242,14 +2638,42 @@
     def __init__(self, model, indices, values, btype):
 
         self.model = model
         self.indices = indices
         self.values = values
         self.btype = btype
 
+    def dual(self):
+
+        if self.model.solution is None:
+            raise RuntimeError('The model is unsolved. ')
+
+        solution = self.model.solution
+        if solution.y is None:
+            msg = 'The dual solution is not available. '
+            msg += f'{solution.solver} solution status: {solution.status}.'
+            warnings.warn(msg)
+        else:
+            primal = self.model.primal
+            if self.btype == 'U':
+                pi = self.model.solution.y['upi'] * self.model.sign
+                output = pi[self.indices]
+                output[primal.ub[self.indices] < self.values] = 0
+            elif self.btype == 'L':
+                pi = self.model.solution.y['lpi'] * self.model.sign
+                output = pi[self.indices]
+                output[primal.lb[self.indices] > self.values] = 0
+            else:
+                raise ValueError('Unknown bounds. ')
+
+            if output.size == 1:
+                output = output.item()
+
+            return output
+
 
 class ConeConstr:
     """
     The ConeConstr class creates an object of second-order cone constraints.
     """
 
     def __init__(self, model, left_var, left_index, right_var, right_index):
@@ -2299,14 +2723,17 @@
 
         ns = self.p.size
         suffix = 's' if ns > 1 else ''
 
         return "KL divergence constraint for {} scenario{}".format(ns, suffix)
 
 
+# class RQCone
+
+
 class RoConstr:
     """
     The Roaffine class creats an object of uncertain affine functions.
     """
 
     def __init__(self, roaffine, sense):
 
@@ -2408,14 +2835,19 @@
             for xconstr in support.xmat:
                 indices = xconstr
                 cone_constr = ExpConstr(self.dec_model,
                                         dual_var[n, indices[0]],
                                         dual_var[n, indices[1]],
                                         dual_var[n, indices[2]])
                 constr_list.append(cone_constr)
+            for pconstr in support.lmi:
+                dim = pconstr['dim']
+                symat = (pconstr['linear']@dual_var[n]).reshape((dim, dim))
+                symat -= pconstr['const']
+                constr_list.append(symat >> 0)
 
         return constr_list
 
 
 class DecVar(Vars):
     """
     The DecVar class creates an object of generic variable array
@@ -2548,15 +2980,21 @@
         1. The variable is not a decision variable.
         2. The model is unsolved, or no solution is obtained due to
         infeasibility, unboundedness, or numeric issues.
         """
 
         dro_model = self.dro_model
         if dro_model.solution is None:
-            raise RuntimeError('The model is unsolved or infeasible')
+            raise RuntimeError('The model is unsolved.')
+
+        solution = dro_model.solution
+        if np.isnan(solution.objval):
+            msg = 'No solution available. '
+            msg += f'{solution.solver} solution status: {solution.status}.'
+            raise RuntimeError(msg)
 
         var_sol = dro_model.ro_model.rc_model.vars[1].get()
         edict = event_dict(self.event_adapt)
         if rvar is None:
             outputs = []
             for eindex in range(len(self.event_adapt)):
                 indices = (self.ro_first + eindex*self.size +
@@ -3014,14 +3452,20 @@
 
     def sum(self, axis=None):
 
         expr = super().sum(axis)
 
         return DecAffine(self.dro_model, expr, self.event_adapt, self.fixed)
 
+    def trace(self):
+
+        expr = super().trace()
+
+        return DecAffine(expr.dro_model, expr, self.event_adapt, self.fixed)
+
     def expcone(self, x, z):
         """
         Return the exponential cone constraint z*exp(x/z) <= affine.
 
         Refer to `rsome.expcone` for full documentation.
 
         See Also
@@ -3120,16 +3564,14 @@
         Refer to `rsome.entropy` for full documentation.
 
         See Also
         --------
         rso.entropy : equivalent function
         """
 
-        # if self.size > 1:
-        #     raise ValueError('The expression must be a scalar')
         if self.shape != ():
             if self.size != max(self.shape):
                 raise ValueError('The expression must be a vector.')
 
         return DecConvex(Convex(self, np.float64(0), 'P', -1), self.event_adapt)
 
     def __le__(self, other):
@@ -3194,14 +3636,28 @@
         if isinstance(left, DecAffine):
             return DecLinConstr(left.model, left.linear, -left.const,
                                 np.ones(left.size), left.event_adapt,
                                 left.fixed, left.ctype)
         elif isinstance(left, DecRoAffine):
             return DecRoConstr(left, 1, left.event_adapt, left.ctype)
 
+    def __rshift__(self, other):
+
+        left = self - other
+        if isinstance(left, DecAffine):
+            constr = super().__rshift__(other)
+            return DecLMIConstr(constr, left.event_adapt)
+        else:
+            msg = 'Linear matrix inequalities only apply to affine expressions.'
+            raise TypeError(msg)
+
+    def __lshift__(self, other):
+
+        return (-self).__rshift__(-other)
+
     @property
     def E(self):
 
         affine = Affine(self.model, self.linear, self.const)
         return DecAffine(self.dro_model, affine, fixed=self.fixed, ctype='E')
 
     def __call__(self, *args):
@@ -3770,14 +4226,23 @@
             if self.dec_model.top is not ambset.model:
                 raise ValueError('Models mismatch.')
 
             self.ambset = ambset
             return self
 
 
+class DecLMIConstr(LMIConstr):
+
+    def __init__(self, constr, event_adapt, ctype='R'):
+
+        super().__init__(constr.model, constr.linear, constr.const, constr.dim)
+        self.event_adapt = event_adapt
+        self.ctype = ctype
+
+
 class DecRule:
     """
     The DecRule class creats an object of decision rules for RO models.
     """
 
     __array_priority__ = 102
 
@@ -3969,15 +4434,21 @@
         An error message is raised if:
         1. The variable is not a decision variable.
         2. The model is unsolved, or no solution is obtained due to
         infeasibility, unboundedness, or numeric issues.
         """
 
         if self.model.solution is None:
-            raise RuntimeError('The model is unsolved or infeasible')
+            raise RuntimeError('The model is unsolved. ')
+
+        solution = self.model.solution
+        if np.isnan(solution.objval):
+            msg = 'No solution available. '
+            msg += f'{solution.solver} solution status: {solution.status}.'
+            raise RuntimeError(msg)
 
         if rvar is None:
             return self.fixed.get()
         else:
             if rvar.model.mtype != 'S':
                 raise ValueError('The input is not a random variable.')
             ldr_row, ldr_col = self.size, self.model.rc_model.vars[-1].last
@@ -4154,15 +4625,15 @@
 
     def lp_export(self):
 
         string = 'Minimize\n'
         string += ' obj: '
         obj_str = ' '.join(['{} {} x{}'.format('-' if coeff < 0 else '+',
                                                abs(coeff), i+1)
-                            for i, coeff in enumerate(self.obj[0]) if coeff])
+                            for i, coeff in enumerate(self.obj) if coeff])
         string += obj_str[2:] if obj_str[:2] == '+ ' else obj_str
 
         string += '\nSubject To\n'
         for i in range(self.linear.shape[0]):
             row = self.linear[i]
             coeffs = row.data
             indices = row.indices
@@ -4229,22 +4700,38 @@
 
 
 class Solution:
     """
     The Solution class creats an object summarizing solution information.
     """
 
-    def __init__(self, objval, x, status, time, xs=None):
+    def __init__(self, solver, objval, x, status, time, xs=None, y=None):
 
+        self.solver = solver
         self.objval = objval
         self.x = x
         self.xs = xs
+        self.y = y
         self.status = status
         self.time = time
 
+    def __repr__(self):
+
+        msg = f"Solver:          {self.solver}\n"
+        msg += f"Solution status: {self.status}\n"
+        msg += f"Solution time:   {self.time:.4f}s\n"
+        msg += "-------------------------------------\n"
+        msg += f"Objective value: {self.objval}\n"
+        primal_available = "Available" if self.x is not None else "Unavailable"
+        dual_available = "Available" if self.y is not None else "Unavailable"
+        msg += f"Primal solution: {primal_available}\n"
+        msg += f"Dual solution:   {dual_available}"
+
+        return msg
+
 
 class Scen:
     """
     The Scen class creats an object of scenarios for the ambiguity set and
     scenario-wise decision adaptive rules.
     """
 
@@ -4296,15 +4783,15 @@
         args = flat(args)
         if len(args) == 0:
             return
 
         for arg in args:
             if arg.model is not self.ambset.model.sup_model:
                 raise ValueError('Constraints are not for this support.')
-            if not isinstance(arg, (LinConstr, CvxConstr, Bounds, ConeConstr)):
+            if not isinstance(arg, (LinConstr, CvxConstr, Bounds, ConeConstr, LMIConstr)):
                 raise TypeError('Invalid constraint type.')
 
         # for i in self.series:
         indices = (self.series if isinstance(self.series, pd.Series)
                    else [self.series])
         for i in indices:
             self.ambset.sup_constr[i] = tuple(args)
```

### Comparing `rsome-1.1.4/rsome/math.py` & `rsome-1.2.0/rsome/math.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,20 +12,20 @@
     Return the first, second, or infinity norm of a 1-D array.
 
     Parameters
     ----------
     affine : an array of variables or affine expressions.
         Input array. The array must be 1-D.
     degree : {1, 2, numpy.inf}, optional
-        Order of the norm function. It can only be 1, 2, or infinity. The
-        default value is 2, i.e., the Euclidean norm.
+        Order of the norm function. It can only be 1, 2, or infinity.
+        The default value is 2, i.e., the Euclidean norm.
 
     Returns
     -------
-    n : Convex
+    out : Convex
         The norm of the given array.
     """
 
     return affine.norm(degree)
 
 
 def square(affine):
@@ -35,71 +35,93 @@
     Parameters
     ----------
     affine : an array of variables or affine expression
         Input array.
 
     Returns
     -------
-    n : Convex
+    out : Convex
         The element-wise squares of the given array
     """
 
     return affine.to_affine().square()
 
 
 def sumsqr(affine):
     """
-    Return the sum of squares of an array.
+    Return the sum of squares of a 1-D array.
 
     Parameters
     ----------
     affine : an array of variables or affine expression
         Input array. The array must be 1-D.
 
     Returns
     -------
-    n : Convex
+    out : Convex
         The sum of squares of the given array
     """
 
     return affine.to_affine().sumsqr()
 
 
-def quad(affine, qmat):
+def quad(x, qmat):
     """
-    Return the quadratic expression affine @ qmat @ affine.
+    Return the quadratic expression x @ qmat @ x.
 
     Parameters
     ----------
-    affine : an array of variables or affine expression
+    x : an array of variables or affine expressions
         Input array. The array must be 1-D.
     qmat : a positive or negative semidefinite matrix.
 
     Returns
     -------
-    q : Convex
+    out : Convex
         The quadratic expression affine @ qmat affine
     """
 
-    return affine.to_affine().quad(qmat)
+    return x.to_affine().quad(qmat)
+
+
+def rsocone(x, y, z):
+    """
+    Return a rotated cone constraint sumsqr(x) <= y*z.
+
+    Parameters
+    ----------
+    x : an array of variables or affine expressions
+        Input array. The array must be a vector.
+    y : {Real, Vars, VarSub, Affine}
+        The y value in the constraint. It must be a scalar.
+    z : {Real, Vars, VarSub, Affine}
+        The z value in the constraint. It must be a scalar.
+
+    Returns
+    -------
+    output : CvxConstr
+        The rotated cone constraint
+    """
+
+    return x.to_affine().rsocone(y, z)
 
 
 def exp(affine):
     """
     Return the element-wise natural exponential function
     exp(affine).
 
     Parameters
     ----------
     affine : an array of variables or affine expression
         Input array.
 
     Returns
     -------
-    a : Convex
+    out : Convex
         The natural exponential function exp(affine)
     """
 
     return affine.exp()
 
 
 def log(affine):
@@ -110,15 +132,15 @@
     Parameters
     ----------
     affine : an array of variables or affine expression
         Input array.
 
     Returns
     -------
-    a : Convex
+    out : Convex
         The natural logarithm function log(affine)
     """
 
     return affine.log()
 
 
 def pexp(affine, scale):
@@ -127,17 +149,21 @@
     function scale * exp(affine/scale).
 
     Parameters
     ----------
     affine : an array of variables or affine expression
         Input array.
 
+    scale : {Real, Vars, VarSub, Affine}
+        The scale value in the perspective function. It must be a
+        scalar.
+
     Returns
     -------
-    a : PerspConvex
+    out : PerspConvex
         The perspective of natural exponential function
         scale * exp(affine/scale)
     """
 
     return affine.pexp(scale)
 
 
@@ -147,17 +173,21 @@
     function scale * log(affine/scale).
 
     Parameters
     ----------
     affine : an array of variables or affine expression
         Input array.
 
+    scale : {Real, Vars, VarSub, Affine}
+        The scale value in the perspective function. It must be a
+        scalar.
+
     Returns
     -------
-    a : PerspConvex
+    out : PerspConvex
         The perspective of natural logarithm function
         scale * log(affine/scale)
     """
 
     return affine.plog(scale)
 
 
@@ -168,15 +198,15 @@
     Parameters
     ----------
     affine : an array of variables or affine expression
         Input array. It must be a vector.
 
     Returns
     -------
-    a : Convex
+    out : Convex
         The entropy expression sum(affine*log(affine))
     """
 
     return affine.entropy()
 
 
 def expcone(y, x, z):
@@ -197,53 +227,71 @@
     constr : ExpConstr
         The exponential cone constraint z*exp(x/z) <= y
     """
 
     return y.expcone(x, z)
 
 
-def kldiv(p, phat, r):
+def kldiv(p, q, r):
     """
     Return an KL divergence constraint sum(p*log(p/phat)) <= r.
 
     Parameters
     ----------
     p : an array of variables or affine expression
         The array of probabilities. It must be a vector.
-    phat : {Real, Vars, VarSub, Affine}
+    q : {Real, Vars, VarSub, Affine}
         The array of empirical probabilities. It must a vector with
         the same shape as p.
     r : {Real, Vars, VarSub, Affine}
         The ambiguity constant. It must be a scalar.
 
     Returns
     -------
     constr : ExpConstr
-        The KL divergence constraint sum(p*log(p/phat)) <= r.
+        The KL divergence constraint sum(p*log(p/q)) <= r.
     """
 
-    return p.kldiv(phat, r)
+    return p.kldiv(q, r)
+
+
+def trace(affine):
+    """
+    Return the trace of a 2-D array.
+
+    Parameters
+    ----------
+    affine : an array of variables or affine expressions.
+        Input array. It must be a 2-D array.
+
+    Returns
+    -------
+    out : Affine
+        Output array as the trace of the 2-D array.
+    """
+
+    return affine.trace()
 
 
 def maxof(*args):
     """
     Return a piecewise function of the maximum of a number of
     expressions.
 
-        Parameters
-        ----------
-        *args : RSOME affine or bi-affine expressions, real numbers
-            Expressions or numerical values used to define the piecewise
-            function.
+    Parameters
+    ----------
+    *args : RSOME affine or bi-affine expressions, real numbers
+        Expressions or numerical values used to define the piecewise
+        function.
 
-        Returns
-        -------
-        piecewise : PiecewiseConvex
-            The piecewise function defined to be the maximum of a number
-            of given expressions or numerical values.
+    Returns
+    -------
+    piecewise : PiecewiseConvex
+        The piecewise function defined to be the maximum of a number
+        of given expressions or numerical values.
     """
 
     pieces = flat(args)
     this_model = None
     for arg in pieces:
         if isinstance(arg, (Vars, VarSub, Affine)):
             arg = arg.to_affine()
@@ -273,27 +321,102 @@
 
 
 def minof(*args):
     """
     Return a piecewise function of the minimum of a number of
     expressions.
 
-        Parameters
-        ----------
-        *args : RSOME affine or bi-affine expressions, real numbers
-            Expressions or numerical values used to define the piecewise
-            function.
+    Parameters
+    ----------
+    *args : RSOME affine or bi-affine expressions, real numbers
+        Expressions or numerical values used to define the piecewise
+        function.
 
-        Returns
-        -------
-        piecewise : PiecewiseConvex
-            The piecewise function defined to be the minimum of a number
-            of given expressions or numerical values.
+    Returns
+    -------
+    piecewise : PiecewiseConvex
+        The piecewise function defined to be the minimum of a number
+        of given expressions or numerical values.
     """
 
     piecewise = maxof(*args)
     piecewise.pieces = [-piece for piece in piecewise.pieces]
 
     piecewise.sign = -1
     piecewise.add_sign = -1
 
     return piecewise
+
+
+def diag(affine, k=0, fill=False):
+    """
+    Return the diagonal elements of a 2-D array.
+
+    Parameters
+    ----------
+    affine : an array of variables or affine expressions.
+        Input array. It must be a 2-D array.
+
+    k : int, optional
+        Diagonal in question. The default is 0. Use `k>0` for diagonals
+        above the main diagonal, and `k<0` for diagonals below the main
+        diagonal.
+
+    fill : bool
+        If True, return a 2-D array where the non-diagonal elements are
+        filled with zeros. Otherwise, return the diagonal elements as a
+        1-D array
+
+        Returns
+        -------
+        out : Affine
+            The diagonal elements of a given 2-D array.
+    """
+
+    return affine.diag(k, fill)
+
+
+def tril(affine, k=0):
+    """
+    Return the lower triangular elements of a 2-D array. The remaining
+    elements are filled with zeros.
+
+        Parameters
+        ----------
+        affine : an array of variables or affine expressions.
+            Input array. It must be a 2-D array.
+
+        k : int, optional
+            Diagonal above which to zero elements.  `k = 0` (the
+            default) is the main diagonal, `k < 0` is below it and
+            `k > 0` is above.
+
+        Returns
+        -------
+        out : Affine
+            The lower triangular elements of the given 2-D array.
+    """
+
+    return affine.tril(k)
+
+
+def triu(affine, k):
+    """
+    Return the upper triangular elements of a 2-D array. The remaining
+    elements are filled with zeros.
+
+    Parameters
+    ----------
+    affine : an array of variables or affine expressions.
+        Input array. It must be a 2-D array.
+
+    k : int, optional
+        Diagonal above which to zero elements.  `k = 0` (the default)
+        is the main diagonal, `k < 0` is below it and `k > 0` is above.
+
+    Returns
+    -------
+        out : Affine
+        The upper triangular elements of the given 2-D array.
+    """
+
+    return affine.triu(k)
```

### Comparing `rsome-1.1.4/rsome/ort_solver.py` & `rsome-1.2.0/rsome/ort_solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
             warnings.warn('the LP solver ignores SOC constriants.')
     except AttributeError:
         pass
 
     try:
         if formula.xmat:
             warnings.warn('The LP solver ignores exponential cone constraints.')
+        if formula.lmi:
+            warnings.warn('The LP solver ignores semidefinite cone constraints.')
     except AttributeError:
         pass
 
     obj = formula.obj.flatten()
     linear = formula.linear
     sense = formula.sense
     const = formula.const
@@ -67,13 +69,14 @@
     stime = time.time() - t0
     if display:
         print('Solution status: {0}'.format(status))
         print('Running time: {0:0.4f}s'.format(stime))
 
     if status == pywraplp.Solver.OPTIMAL:
         x_sol = np.array([xs[i].solution_value() for i in range(col)])
-        solution = Solution(solver.Objective().Value(), x_sol, status, stime)
+        solution = Solution('OR-Tools', solver.Objective().Value(), x_sol, status, stime)
     else:
         warnings.warn('Fail to find the optimal solution.')
-        solution = None
+        # solution = None
+        solution = Solution('OR-Tools', np.nan, None, status, stime)
 
     return solution
```

### Comparing `rsome-1.1.4/rsome/subroutines.py` & `rsome-1.2.0/rsome/subroutines.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import scipy.sparse as sp
 from numbers import Real
 from scipy.sparse import csr_matrix
 from collections.abc import Iterable
-from typing import List
 
 
 def flat(a_list):
     flat_list = []
     for item in a_list:
         if isinstance(item, Iterable):
             flat_list.extend(flat(item))
@@ -28,14 +27,34 @@
 
     size = index.size
 
     return csr_matrix((values, (np.arange(size), index)),
                       shape=(size, affine.size))
 
 
+def diag_comb(upper, lower):
+
+    data = np.concatenate((upper.data, lower.data))
+    indices = np.concatenate((upper.indices, upper.shape[1] + lower.indices))
+    indptr = np.concatenate((upper.indptr[:-1], upper.indptr[-1] + lower.indptr))
+
+    return csr_matrix((data, indices, indptr),
+                      shape=np.array(upper.shape)+np.array(lower.shape))
+
+
+def vert_comb(upper, lower):
+
+    data = np.concatenate((upper.data, lower.data))
+    indices = np.concatenate((upper.indices, lower.indices))
+    indptr = np.concatenate((upper.indptr[:-1], upper.indptr[-1] + lower.indptr))
+
+    shape = upper.shape[0] + lower.shape[0], max([upper.shape[1], lower.shape[1]])
+    return csr_matrix((data, indices, indptr), shape=shape)
+
+
 def sp_matmul(ndarray, affine, shape):
 
     size = int(np.prod(shape))
 
     if len(shape) < 1:
         return csr_matrix(ndarray)
     else:
@@ -176,15 +195,15 @@
         raise TypeError('Incorrect data type of arrays.')
 
     return array
 
 
 def rso_broadcast(*args):
 
-    arrays = [np.array(arg) if isinstance(arg, Real) else arg
+    arrays = [np.array(arg) if isinstance(arg, (Real, np.ndarray)) else arg.to_affine()
               for arg in args]
 
     indices = [np.arange(array.size).reshape(array.shape) for
                array in arrays]
 
     arrays = [array.reshape(array.size) for array in arrays]
```

### Comparing `rsome-1.1.4/rsome.egg-info/PKG-INFO` & `rsome-1.2.0/rsome.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: rsome
-Version: 1.1.4
+Version: 1.2.0
 Summary: Robust Stochastic Optimization Made Easy
 Author: Peng Xiong
 License: GPL-3.0
 Platform: linux
 Platform: osx
 Platform: win64
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.md
 
 <img src="https://github.com/XiongPengNUS/rsome/blob/master/rsologo.png?raw=true" width=100>
 
 # RSOME: Robust Stochastic Optimization Made Easy
@@ -27,15 +27,15 @@
 [![tests](https://github.com/XiongPengNUS/rsome/actions/workflows/test.yml/badge.svg)](https://github.com/XiongPengNUS/rsome/actions/workflows/test.yml)
 [![Docs](https://github.com/XiongPengNUS/rsome/actions/workflows/pages/pages-build-deployment/badge.svg?label=Docs)](https://github.com/XiongPengNUS/rsome/actions/workflows/pages/pages-build-deployment)
 [![Project Status: Active - The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed/XiongPengNUS/rsome)
 ![GitHub issues](https://img.shields.io/github/issues-raw/XiongPengNUS/rsome)
 
 - Website: [RSOME for Python](https://xiongpengnus.github.io/rsome/)
-- PyPI: [RSOME 1.1.4](https://pypi.org/project/rsome/)
+- PyPI: [RSOME 1.2.0](https://pypi.org/project/rsome/)
 
 RSOME (Robust Stochastic Optimization Made Easy) is an open-source Python package for generic modeling of optimization problems (subject to uncertainty). Models in RSOME are constructed by variables, constraints, and expressions that are formatted as N-dimensional arrays. These arrays are consistent with the NumPy library in terms of syntax and operations, including broadcasting, indexing, slicing, element-wise operations, and matrix calculation rules, among others. In short, RSOME provides a convenient platform to facilitate developments of robust optimization models and their applications.
 
 ## Content
 
 - [Installation](#section2)
 - [Solver interfaces](#section3)
@@ -48,26 +48,26 @@
 The RSOME package can be installed by using the <code>pip</code> command:
 ***
 **`pip install rsome`**
 ***
 
 ### Solver interfaces <a id="section3"></a>
 
-The RSOME package transforms robust or distributionally robust optimization models into deterministic second-order cone or exponential cone programming problems, and solved by external solvers. Details of compatible solvers and their interfaces are presented in the following table.
+The RSOME package transforms robust or distributionally robust optimization models into deterministic linear or conic programming problems, and solved by external solvers. Details of compatible solvers and their interfaces are presented in the following table.
 
-| Solver | License  type | Required version | RSOME interface |Integrality constraints| Second-order cone constraints| Exponential cone constraints
+| Solver | License  type | Required version | RSOME interface | Second-order cone constraints| Exponential cone constraints | Semidefiniteness constraints
 |:-------|:--------------|:-----------------|:----------------|:------------------------|:---------------------|:--------------|
-|[scipy.optimize](https://docs.scipy.org/doc/scipy/reference/optimize.html)| Open-source | >= 1.2.1 | `lpg_solver` | Yes for 1.9.0 or above | No | No |
-|[CyLP](https://github.com/coin-or/cylp)| Open-source | >= 0.9.0 | `clp_solver` | Yes | No | No |
-|[OR-Tools](https://developers.google.com/optimization/install) | Open-source | >= 7.5.7466 | `ort_solver` | Yes | No | No |
-|[ECOS](https://github.com/embotech/ecos-python) | Open-source | >= 2.0.10 | `eco_solver` | Yes | Yes | Yes |
-|[Gurobi](https://www.gurobi.com/documentation/9.0/quickstart_mac/ins_the_anaconda_python_di.html)| Commercial | >= 9.1.0 | `grb_solver` | Yes | Yes | No |
-|[MOSEK](https://docs.mosek.com/9.2/pythonapi/install-interface.html) | Commercial | >= 9.1.11 | `msk_solver` | Yes | Yes | Yes |
-|[CPLEX](https://www.ibm.com/support/knowledgecenter/en/SSSA5P_12.8.0/ilog.odms.cplex.help/CPLEX/GettingStarted/topics/set_up/Python_setup.html) | Commercial | >= 12.9.0.0 | `cpx_solver` | Yes | Yes | No |
-|[COPT](https://www.shanshu.ai/copt) | Commercial | >= 5.0.1 | `cpt_solver` | Yes | Yes | No |
+|[scipy.optimize](https://docs.scipy.org/doc/scipy/reference/optimize.html)| Open-source | >= 1.9.0 | `lpg_solver` | No | No | No |
+|[CyLP](https://github.com/coin-or/cylp)| Open-source | >= 0.9.0 | `clp_solver` | No | No | No |
+|[OR-Tools](https://developers.google.com/optimization/install) | Open-source | >= 7.5.7466 | `ort_solver` | No | No | No |
+|[ECOS](https://github.com/embotech/ecos-python) | Open-source | >= 2.0.10 | `eco_solver` | Yes | Yes | No |
+|[Gurobi](https://www.gurobi.com/documentation/9.0/quickstart_mac/ins_the_anaconda_python_di.html)| Commercial | >= 9.1.0 | `grb_solver` | Yes | No | No |
+|[Mosek](https://docs.mosek.com/9.2/pythonapi/install-interface.html) | Commercial | >= 10.0.44 | `msk_solver` | Yes | Yes | Yes |
+|[CPLEX](https://www.ibm.com/support/knowledgecenter/en/SSSA5P_12.8.0/ilog.odms.cplex.help/CPLEX/GettingStarted/topics/set_up/Python_setup.html) | Commercial | >= 12.9.0.0 | `cpx_solver` | Yes | No | No |
+|[COPT](https://www.shanshu.ai/copt) | Commercial | >= 6.5.3 | `cpt_solver` | Yes | No | No |
 
 ## Getting started <a id="section4"></a>
 
 Documents of RSOME are provided as follows:
 - [RSOME quick start](https://xiongpengnus.github.io/rsome/)
 - [RSOME users guide](https://xiongpengnus.github.io/rsome/user_guide)
 - [Application examples](https://xiongpengnus.github.io/rsome/examples)
@@ -76,26 +76,29 @@
 
 RSOME is a software project supported by Singapore Ministry of Education Tier 3 Grant *Science of Prescriptive Analytics*. It is primarly developed and maintained by [Zhi Chen](https://www.cb.cityu.edu.hk/staff/zchen96/), [Melvyn Sim](https://bizfaculty.nus.edu.sg/faculty-details/?profId=127), and [Peng Xiong](https://bizfaculty.nus.edu.sg/faculty-details/?profId=543). Many other researchers, including Erick Delage, Zhaowei Hao, Long He, Zhenyu Hu, Jun Jiang, Brad Sturt, Qinshen Tang, as well as anonymous users and paper reviewers, have helped greatly in the way of developing RSOME.
 
 ## Citation <a id="section6">
 
 If you use RSOME in your research, please cite our papers:
 
-- Chen, Zhi, and Peng Xiong. 2021. [RSOME in Python: an open-source package for robust stochastic optimization made easy](http://www.optimization-online.org/DB_HTML/2021/06/8443.html). <i>Optimization Online</i>.
+- Chen, Zhi, and Peng Xiong. 2023. [RSOME in Python: an open-source package for robust stochastic optimization made easy](https://pubsonline.informs.org/doi/abs/10.1287/ijoc.2023.1291). Forthcoming in <i>INFORMS Journal on Computing</i>.
 
-- Chen, Zhi, Melvyn Sim, Peng Xiong. 2020. [Robust stochastic optimization made easy with RSOME](https://pubsonline.informs.org/doi/abs/10.1287/mnsc.2020.3603). <i>Management Science</i> <b>66</b>(8) 3329–3339.
+- Chen, Zhi, Melvyn Sim, Peng Xiong. 2020. [Robust stochastic optimization made easy with RSOME](https://pubsonline.informs.org/doi/abs/10.1287/mnsc.2020.3603). <i>Management Science</i> <b>66</b>(8) 3329-3339.
 
 Bibtex entry:
 
 ```
 @article{chen2021rsome,
   title={RSOME in Python: an open-source package for robust stochastic optimization made easy},
   author={Chen, Zhi and Xiong, Peng},
-  journal={Optimization Online. URL: http://www.optimization-online.org/DB_HTML/2021/06/8443.html},
-  year={2021},
+  journal={INFORMS Journal on Computing},
+  year={2023},
+  month={Mar},
+  day={30},
+  publisher={INFORMS}
 }
 ```
 
 ```
 @article{chen2020robust,
   title={Robust stochastic optimization made easy with RSOME},
   author={Chen, Zhi and Sim, Melvyn and Xiong, Peng},
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rsome-1.1.4/rsome.egg-info/SOURCES.txt` & `rsome-1.2.0/rsome.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 rsome/__init__.py
 rsome/clp_solver.py
 rsome/cpt_solver.py
+rsome/cpt_solver_bkp.py
 rsome/cpx_solver.py
-rsome/cvx_solver.py
 rsome/deco.py
 rsome/dro.py
 rsome/eco_solver.py
 rsome/gcp.py
 rsome/grb_solver.py
 rsome/lp.py
 rsome/lpg_solver.py
 rsome/math.py
 rsome/msk_solver.py
 rsome/ort_solver.py
 rsome/py.typed
 rsome/ro.py
 rsome/socp.py
 rsome/subroutines.py
+rsome/this.py
 rsome.egg-info/PKG-INFO
 rsome.egg-info/SOURCES.txt
 rsome.egg-info/dependency_links.txt
 rsome.egg-info/not-zip-safe
 rsome.egg-info/requires.txt
 rsome.egg-info/top_level.txt
```

### Comparing `rsome-1.1.4/setup.cfg` & `rsome-1.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [metadata]
 name = rsome
-version = 1.1.4
+version = 1.2.0
 description = Robust Stochastic Optimization Made Easy
 long_description = file: README.rst
 author = Peng Xiong
 license = GPL-3.0
 license_file = LICENSE.md
 platforms = linux, osx, win64
 classifiers = 
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 packages = 
 	rsome
 install_requires = 
 	numpy >= 1.20.0
-	scipy >= 1.2.1
+	scipy >= 1.9.0
 	pandas >= 0.25.0
-python_requires = >=3.7
+python_requires = >=3.8
 zip_safe = no
 
 [options.extras_require]
 testing = 
 	pytest>=6.0
 	pytest-cov>=2.0
 	mypy>=0.910
@@ -35,12 +35,15 @@
 rsome = py.typed
 
 [flake8]
 max-line-length = 90
 exclude = 
 	*__init__.py
 	*lpg_solver.py
+extend-ignore = 
+	F403,
+	F405
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

