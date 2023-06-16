# Comparing `tmp/theseus-ai-0.1.4.tar.gz` & `tmp/theseus-ai-0.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theseus-ai-0.1.4.tar", last modified: Thu Jan 19 16:24:55 2023, max compression
+gzip compressed data, was "theseus-ai-0.2.0.dev0.tar", last modified: Fri Jun 16 22:24:47 2023, max compression
```

## Comparing `theseus-ai-0.1.4.tar` & `theseus-ai-0.2.0.dev0.tar`

### file list

```diff
@@ -1,173 +1,149 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.094903 theseus-ai-0.1.4/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       91 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    11630 2023-01-19 16:24:55.094903 theseus-ai-0.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11035 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.070902 theseus-ai-0.1.4/requirements/
--rw-r--r--   0 root         (0) root         (0)      193 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/requirements/dev.txt
--rw-r--r--   0 root         (0) root         (0)      174 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      230 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/requirements/main.txt
--rw-r--r--   0 root         (0) root         (0)      430 2023-01-19 16:24:55.094903 theseus-ai-0.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5292 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.070902 theseus-ai-0.1.4/tests/
--rw-r--r--   0 root         (0) root         (0)      179 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.074902 theseus-ai-0.1.4/tests/core/
--rw-r--r--   0 root         (0) root         (0)      179 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7070 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/core/common.py
--rw-r--r--   0 root         (0) root         (0)    13514 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/core/test_cost_function.py
--rw-r--r--   0 root         (0) root         (0)     4442 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/core/test_cost_weight.py
--rw-r--r--   0 root         (0) root         (0)     2270 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/core/test_manifold.py
--rw-r--r--   0 root         (0) root         (0)    19405 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/core/test_objective.py
--rw-r--r--   0 root         (0) root         (0)     5416 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/core/test_robust_cost.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/core/test_theseus_function.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/core/test_variable.py
--rw-r--r--   0 root         (0) root         (0)    14676 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/core/test_vectorizer.py
--rw-r--r--   0 root         (0) root         (0)      857 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.074902 theseus-ai-0.1.4/tests/extlib/
--rw-r--r--   0 root         (0) root         (0)      179 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/extlib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4777 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/extlib/test_baspacho.py
--rw-r--r--   0 root         (0) root         (0)     3106 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/extlib/test_baspacho_simple.py
--rw-r--r--   0 root         (0) root         (0)     3702 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/extlib/test_cusolver_lu_solver.py
--rw-r--r--   0 root         (0) root         (0)     4409 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/extlib/test_mat_mult.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.074902 theseus-ai-0.1.4/tests/geometry/
--rw-r--r--   0 root         (0) root         (0)      179 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/geometry/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19548 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/geometry/common.py
--rw-r--r--   0 root         (0) root         (0)      792 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/geometry/point_types_mypy_check.py
--rw-r--r--   0 root         (0) root         (0)     4561 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/geometry/test_point_types.py
--rw-r--r--   0 root         (0) root         (0)     8862 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/geometry/test_se2.py
--rw-r--r--   0 root         (0) root         (0)    12861 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/geometry/test_se3.py
--rw-r--r--   0 root         (0) root         (0)     6566 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/geometry/test_so2.py
--rw-r--r--   0 root         (0) root         (0)    10391 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/geometry/test_so3.py
--rw-r--r--   0 root         (0) root         (0)     7443 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/geometry/test_vector.py
--rw-r--r--   0 root         (0) root         (0)     3923 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/test_dlm_perturbation.py
--rw-r--r--   0 root         (0) root         (0)    20461 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/tests/test_theseus_layer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.074902 theseus-ai-0.1.4/theseus/
--rw-r--r--   0 root         (0) root         (0)     2111 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.078902 theseus-ai-0.1.4/theseus/core/
--rw-r--r--   0 root         (0) root         (0)      624 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15935 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/core/cost_function.py
--rw-r--r--   0 root         (0) root         (0)     4984 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/core/cost_weight.py
--rw-r--r--   0 root         (0) root         (0)    29410 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/core/objective.py
--rw-r--r--   0 root         (0) root         (0)     6131 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/core/robust_cost_function.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/core/robust_loss.py
--rw-r--r--   0 root         (0) root         (0)     6417 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/core/theseus_function.py
--rw-r--r--   0 root         (0) root         (0)     4800 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/core/variable.py
--rw-r--r--   0 root         (0) root         (0)    20067 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/core/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.078902 theseus-ai-0.1.4/theseus/embodied/
--rw-r--r--   0 root         (0) root         (0)      548 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/embodied/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.078902 theseus-ai-0.1.4/theseus/embodied/collision/
--rw-r--r--   0 root         (0) root         (0)      329 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/embodied/collision/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3616 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/embodied/collision/collision.py
--rw-r--r--   0 root         (0) root         (0)     4906 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/embodied/collision/eff_obj_contact.py
--rw-r--r--   0 root         (0) root         (0)     8528 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/embodied/collision/signed_distance_field.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.078902 theseus-ai-0.1.4/theseus/embodied/kinematics/
--rw-r--r--   0 root         (0) root         (0)      257 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/embodied/kinematics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3894 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/embodied/kinematics/kinematics_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.078902 theseus-ai-0.1.4/theseus/embodied/measurements/
--rw-r--r--   0 root         (0) root         (0)      301 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/embodied/measurements/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/embodied/measurements/between.py
--rw-r--r--   0 root         (0) root         (0)     2730 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/embodied/measurements/moving_frame_between.py
--rw-r--r--   0 root         (0) root         (0)     4090 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/embodied/measurements/reprojection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.078902 theseus-ai-0.1.4/theseus/embodied/misc/
--rw-r--r--   0 root         (0) root         (0)      213 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/embodied/misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/embodied/misc/local_cost_fn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.082903 theseus-ai-0.1.4/theseus/embodied/motionmodel/
--rw-r--r--   0 root         (0) root         (0)      323 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/embodied/motionmodel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7715 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/embodied/motionmodel/double_integrator.py
--rw-r--r--   0 root         (0) root         (0)    11526 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/embodied/motionmodel/quasi_static_pushing_planar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.082903 theseus-ai-0.1.4/theseus/extlib/
--rw-r--r--   0 root         (0) root         (0)      179 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/extlib/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14114 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/extlib/baspacho_solver.cpp
--rw-r--r--   0 root         (0) root         (0)     3751 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/extlib/baspacho_solver.h
--rw-r--r--   0 root         (0) root         (0)    12381 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/extlib/baspacho_solver_cuda.cu
--rw-r--r--   0 root         (0) root         (0)    16013 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/extlib/cusolver_lu_solver.cpp
--rw-r--r--   0 root         (0) root         (0)     3140 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/extlib/cusolver_sp_defs.cpp
--rw-r--r--   0 root         (0) root         (0)      744 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/extlib/cusolver_sp_defs.h
--rw-r--r--   0 root         (0) root         (0)    14555 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/extlib/mat_mult.cu
--rw-r--r--   0 root         (0) root         (0)     1186 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/extlib/utils.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.082903 theseus-ai-0.1.4/theseus/geometry/
--rw-r--r--   0 root         (0) root         (0)      911 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/geometry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7224 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/geometry/lie_group.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/geometry/lie_group_check.py
--rw-r--r--   0 root         (0) root         (0)     5689 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/geometry/manifold.py
--rw-r--r--   0 root         (0) root         (0)     7322 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/geometry/point_types.py
--rw-r--r--   0 root         (0) root         (0)    16533 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/geometry/se2.py
--rw-r--r--   0 root         (0) root         (0)    29473 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/geometry/se3.py
--rw-r--r--   0 root         (0) root         (0)    11359 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/geometry/so2.py
--rw-r--r--   0 root         (0) root         (0)    25233 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/geometry/so3.py
--rw-r--r--   0 root         (0) root         (0)     2683 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/geometry/utils.py
--rw-r--r--   0 root         (0) root         (0)     9405 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/geometry/vector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.070902 theseus-ai-0.1.4/theseus/labs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.086903 theseus-ai-0.1.4/theseus/labs/lie_functional/
--rw-r--r--   0 root         (0) root         (0)      179 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/labs/lie_functional/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/labs/lie_functional/constants.py
--rw-r--r--   0 root         (0) root         (0)     2131 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/labs/lie_functional/lie_group.py
--rw-r--r--   0 root         (0) root         (0)    10910 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/labs/lie_functional/so3.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/labs/lie_functional/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.086903 theseus-ai-0.1.4/theseus/optimizer/
--rw-r--r--   0 root         (0) root         (0)      505 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.086903 theseus-ai-0.1.4/theseus/optimizer/autograd/
--rw-r--r--   0 root         (0) root         (0)      454 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/autograd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6420 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/autograd/baspacho_sparse_autograd.py
--rw-r--r--   0 root         (0) root         (0)     5391 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/autograd/cholmod_sparse_autograd.py
--rw-r--r--   0 root         (0) root         (0)     8077 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/autograd/lu_cuda_sparse_autograd.py
--rw-r--r--   0 root         (0) root         (0)     2612 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/dense_linearization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.086903 theseus-ai-0.1.4/theseus/optimizer/linear/
--rw-r--r--   0 root         (0) root         (0)      520 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/linear/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5112 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/linear/baspacho_sparse_solver.py
--rw-r--r--   0 root         (0) root         (0)     2600 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/linear/cholmod_sparse_solver.py
--rw-r--r--   0 root         (0) root         (0)     5681 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/linear/dense_solver.py
--rw-r--r--   0 root         (0) root         (0)     2630 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/linear/linear_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     1107 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/linear/linear_solver.py
--rw-r--r--   0 root         (0) root         (0)     6843 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/linear/lu_cuda_sparse_solver.py
--rw-r--r--   0 root         (0) root         (0)     1221 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/linear/utils.py
--rw-r--r--   0 root         (0) root         (0)     1346 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/linear_system.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/linearization.py
--rw-r--r--   0 root         (0) root         (0)     6184 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/manifold_gaussian.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.090903 theseus-ai-0.1.4/theseus/optimizer/nonlinear/
--rw-r--r--   0 root         (0) root         (0)      560 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/nonlinear/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4354 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/nonlinear/dogleg.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/nonlinear/gauss_newton.py
--rw-r--r--   0 root         (0) root         (0)     6991 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/nonlinear/levenberg_marquardt.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/nonlinear/nonlinear_least_squares.py
--rw-r--r--   0 root         (0) root         (0)    24796 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/nonlinear/nonlinear_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     5687 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/nonlinear/trust_region.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     7721 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/sparse_linearization.py
--rw-r--r--   0 root         (0) root         (0)     2068 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/optimizer/variable_ordering.py
--rw-r--r--   0 root         (0) root         (0)    12260 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/theseus_layer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.090903 theseus-ai-0.1.4/theseus/third_party/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/third_party/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28031 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/third_party/easyaug.py
--rw-r--r--   0 root         (0) root         (0)     2040 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/third_party/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.090903 theseus-ai-0.1.4/theseus/utils/
--rw-r--r--   0 root         (0) root         (0)      439 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.090903 theseus-ai-0.1.4/theseus/utils/examples/
--rw-r--r--   0 root         (0) root         (0)     1526 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.090903 theseus-ai-0.1.4/theseus/utils/examples/bundle_adjustment/
--rw-r--r--   0 root         (0) root         (0)      244 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/examples/bundle_adjustment/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12392 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/examples/bundle_adjustment/data.py
--rw-r--r--   0 root         (0) root         (0)     2220 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/examples/bundle_adjustment/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.090903 theseus-ai-0.1.4/theseus/utils/examples/motion_planning/
--rw-r--r--   0 root         (0) root         (0)      435 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/examples/motion_planning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9168 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/examples/motion_planning/misc.py
--rw-r--r--   0 root         (0) root         (0)     9771 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/examples/motion_planning/models.py
--rw-r--r--   0 root         (0) root         (0)    18844 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/examples/motion_planning/motion_planner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.090903 theseus-ai-0.1.4/theseus/utils/examples/pose_graph/
--rw-r--r--   0 root         (0) root         (0)      308 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/examples/pose_graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16392 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/examples/pose_graph/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.094903 theseus-ai-0.1.4/theseus/utils/examples/tactile_pose_estimation/
--rw-r--r--   0 root         (0) root         (0)      510 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/examples/tactile_pose_estimation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10221 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/examples/tactile_pose_estimation/misc.py
--rw-r--r--   0 root         (0) root         (0)    10050 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/examples/tactile_pose_estimation/models.py
--rw-r--r--   0 root         (0) root         (0)     9304 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/examples/tactile_pose_estimation/pose_estimator.py
--rw-r--r--   0 root         (0) root         (0)    12465 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/examples/tactile_pose_estimation/trainer.py
--rw-r--r--   0 root         (0) root         (0)     8649 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/sparse_matrix_utils.py
--rw-r--r--   0 root         (0) root         (0)     5070 2023-01-19 16:24:47.000000 theseus-ai-0.1.4/theseus/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 16:24:55.094903 theseus-ai-0.1.4/theseus_ai.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11630 2023-01-19 16:24:55.000000 theseus-ai-0.1.4/theseus_ai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5034 2023-01-19 16:24:55.000000 theseus-ai-0.1.4/theseus_ai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-19 16:24:55.000000 theseus-ai-0.1.4/theseus_ai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      355 2023-01-19 16:24:55.000000 theseus-ai-0.1.4/theseus_ai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-01-19 16:24:55.000000 theseus-ai-0.1.4/theseus_ai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.675665 theseus-ai-0.2.0.dev0/
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       91 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11635 2023-06-16 22:24:47.675665 theseus-ai-0.2.0.dev0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11035 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.655664 theseus-ai-0.2.0.dev0/requirements/
+-rw-r--r--   0 root         (0) root         (0)      192 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/requirements/dev.txt
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-16 22:24:40.000000 theseus-ai-0.2.0.dev0/requirements/main.txt
+-rw-r--r--   0 root         (0) root         (0)      482 2023-06-16 22:24:47.675665 theseus-ai-0.2.0.dev0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6333 2023-06-16 22:24:40.000000 theseus-ai-0.2.0.dev0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.655664 theseus-ai-0.2.0.dev0/theseus/
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      334 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/_version.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.655664 theseus-ai-0.2.0.dev0/theseus/core/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16303 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/core/cost_function.py
+-rw-r--r--   0 root         (0) root         (0)     4984 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/core/cost_weight.py
+-rw-r--r--   0 root         (0) root         (0)    30933 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/core/objective.py
+-rw-r--r--   0 root         (0) root         (0)     7188 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/core/robust_cost_function.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/core/robust_loss.py
+-rw-r--r--   0 root         (0) root         (0)     6417 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/core/theseus_function.py
+-rw-r--r--   0 root         (0) root         (0)     4800 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/core/variable.py
+-rw-r--r--   0 root         (0) root         (0)    20320 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/core/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.655664 theseus-ai-0.2.0.dev0/theseus/embodied/
+-rw-r--r--   0 root         (0) root         (0)      581 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.659664 theseus-ai-0.2.0.dev0/theseus/embodied/collision/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/collision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3616 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/collision/collision.py
+-rw-r--r--   0 root         (0) root         (0)     4906 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/collision/eff_obj_contact.py
+-rw-r--r--   0 root         (0) root         (0)     9043 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/collision/signed_distance_field.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.659664 theseus-ai-0.2.0.dev0/theseus/embodied/kinematics/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/kinematics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3894 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/kinematics/kinematics_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.659664 theseus-ai-0.2.0.dev0/theseus/embodied/measurements/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/measurements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/measurements/between.py
+-rw-r--r--   0 root         (0) root         (0)     2730 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/measurements/moving_frame_between.py
+-rw-r--r--   0 root         (0) root         (0)     4090 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/measurements/reprojection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.659664 theseus-ai-0.2.0.dev0/theseus/embodied/misc/
+-rw-r--r--   0 root         (0) root         (0)      213 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/misc/local_cost_fn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.659664 theseus-ai-0.2.0.dev0/theseus/embodied/motionmodel/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/motionmodel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7715 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/motionmodel/double_integrator.py
+-rw-r--r--   0 root         (0) root         (0)     6957 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/motionmodel/misc.py
+-rw-r--r--   0 root         (0) root         (0)    11526 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/motionmodel/quasi_static_pushing_planar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.663664 theseus-ai-0.2.0.dev0/theseus/extlib/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14114 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/baspacho_solver.cpp
+-rw-r--r--   0 root         (0) root         (0)     3751 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/baspacho_solver.h
+-rw-r--r--   0 root         (0) root         (0)    12381 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/baspacho_solver_cuda.cu
+-rw-r--r--   0 root         (0) root         (0)    16013 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/cusolver_lu_solver.cpp
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/cusolver_sp_defs.cpp
+-rw-r--r--   0 root         (0) root         (0)      744 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/cusolver_sp_defs.h
+-rw-r--r--   0 root         (0) root         (0)    14555 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/mat_mult.cu
+-rw-r--r--   0 root         (0) root         (0)     1186 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/utils.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.663664 theseus-ai-0.2.0.dev0/theseus/geometry/
+-rw-r--r--   0 root         (0) root         (0)      911 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/geometry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/geometry/lie_group.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/geometry/lie_group_check.py
+-rw-r--r--   0 root         (0) root         (0)     5689 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/geometry/manifold.py
+-rw-r--r--   0 root         (0) root         (0)     7322 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/geometry/point_types.py
+-rw-r--r--   0 root         (0) root         (0)    16493 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/geometry/se2.py
+-rw-r--r--   0 root         (0) root         (0)    10894 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/geometry/se3.py
+-rw-r--r--   0 root         (0) root         (0)    11454 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/geometry/so2.py
+-rw-r--r--   0 root         (0) root         (0)    11324 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/geometry/so3.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/geometry/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9405 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/geometry/vector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.663664 theseus-ai-0.2.0.dev0/theseus/labs/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/labs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.663664 theseus-ai-0.2.0.dev0/theseus/labs/embodied/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/labs/embodied/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.663664 theseus-ai-0.2.0.dev0/theseus/labs/embodied/robot/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/labs/embodied/robot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4922 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/labs/embodied/robot/forward_kinematics.py
+-rw-r--r--   0 root         (0) root         (0)    15442 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/labs/embodied/robot/joint.py
+-rw-r--r--   0 root         (0) root         (0)     8668 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/labs/embodied/robot/robot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.667664 theseus-ai-0.2.0.dev0/theseus/optimizer/
+-rw-r--r--   0 root         (0) root         (0)      505 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.667664 theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/
+-rw-r--r--   0 root         (0) root         (0)      454 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5948 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/baspacho_sparse_autograd.py
+-rw-r--r--   0 root         (0) root         (0)     5365 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/cholmod_sparse_autograd.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/common.py
+-rw-r--r--   0 root         (0) root         (0)     7572 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/lu_cuda_sparse_autograd.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/dense_linearization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.667664 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5161 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/baspacho_sparse_solver.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/cholmod_sparse_solver.py
+-rw-r--r--   0 root         (0) root         (0)     5681 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/dense_solver.py
+-rw-r--r--   0 root         (0) root         (0)     2630 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/linear_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/linear_solver.py
+-rw-r--r--   0 root         (0) root         (0)     6892 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/lu_cuda_sparse_solver.py
+-rw-r--r--   0 root         (0) root         (0)     1221 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear_system.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linearization.py
+-rw-r--r--   0 root         (0) root         (0)     6184 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/manifold_gaussian.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.671664 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8421 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/dcem.py
+-rw-r--r--   0 root         (0) root         (0)     4354 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/dogleg.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/gauss_newton.py
+-rw-r--r--   0 root         (0) root         (0)     7009 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/levenberg_marquardt.py
+-rw-r--r--   0 root         (0) root         (0)    16237 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/nonlinear_least_squares.py
+-rw-r--r--   0 root         (0) root         (0)    10821 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/nonlinear_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     5696 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/trust_region.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     8226 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/sparse_linearization.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/variable_ordering.py
+-rw-r--r--   0 root         (0) root         (0)     2331 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/options.py
+-rw-r--r--   0 root         (0) root         (0)    12958 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/theseus_layer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.671664 theseus-ai-0.2.0.dev0/theseus/third_party/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/third_party/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28031 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/third_party/easyaug.py
+-rwxr-xr-x   0 root         (0) root         (0)     6703 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/third_party/lml.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/third_party/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.671664 theseus-ai-0.2.0.dev0/theseus/utils/
+-rw-r--r--   0 root         (0) root         (0)      499 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.671664 theseus-ai-0.2.0.dev0/theseus/utils/examples/
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.671664 theseus-ai-0.2.0.dev0/theseus/utils/examples/bundle_adjustment/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/bundle_adjustment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12392 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/bundle_adjustment/data.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/bundle_adjustment/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.675665 theseus-ai-0.2.0.dev0/theseus/utils/examples/motion_planning/
+-rw-r--r--   0 root         (0) root         (0)      435 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/motion_planning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9168 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/motion_planning/misc.py
+-rw-r--r--   0 root         (0) root         (0)     9771 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/motion_planning/models.py
+-rw-r--r--   0 root         (0) root         (0)    19745 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/motion_planning/motion_planner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.675665 theseus-ai-0.2.0.dev0/theseus/utils/examples/pose_graph/
+-rw-r--r--   0 root         (0) root         (0)      308 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/pose_graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16407 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/pose_graph/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.675665 theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/
+-rw-r--r--   0 root         (0) root         (0)      510 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10221 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/misc.py
+-rw-r--r--   0 root         (0) root         (0)    10050 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/models.py
+-rw-r--r--   0 root         (0) root         (0)     9304 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/pose_estimator.py
+-rw-r--r--   0 root         (0) root         (0)    12465 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/trainer.py
+-rw-r--r--   0 root         (0) root         (0)     8649 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/sparse_matrix_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8089 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.675665 theseus-ai-0.2.0.dev0/theseus_ai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11635 2023-06-16 22:24:47.000000 theseus-ai-0.2.0.dev0/theseus_ai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-06-16 22:24:47.000000 theseus-ai-0.2.0.dev0/theseus_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 22:24:47.000000 theseus-ai-0.2.0.dev0/theseus_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      424 2023-06-16 22:24:47.000000 theseus-ai-0.2.0.dev0/theseus_ai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-16 22:24:47.000000 theseus-ai-0.2.0.dev0/theseus_ai.egg-info/top_level.txt
```

### Comparing `theseus-ai-0.1.4/LICENSE` & `theseus-ai-0.2.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/PKG-INFO` & `theseus-ai-0.2.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theseus-ai
-Version: 0.1.4
+Version: 0.2.0.dev0
 Summary: A library for differentiable nonlinear optimization.
 Home-page: https://github.com/facebookresearch/theseus
 Author: Meta Research
 Keywords: differentiable optimization,nonlinear least squares,factor graphs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: theseus-ai Version: 0.1.4 Summary: A library for
-differentiable nonlinear optimization. Home-page: https://github.com/
+Metadata-Version: 2.1 Name: theseus-ai Version: 0.2.0.dev0 Summary: A library
+for differentiable nonlinear optimization. Home-page: https://github.com/
 facebookresearch/theseus Author: Meta Research Keywords: differentiable
 optimization,nonlinear least squares,factor graphs Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
 LICENSE ![](https://raw.githubusercontent.com/facebookresearch/theseus/main/
```

### Comparing `theseus-ai-0.1.4/README.md` & `theseus-ai-0.2.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/setup.py` & `theseus-ai-0.2.0.dev0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,25 +21,36 @@
 
     if hasattr(torch_cpp_ext, "CUDA_GCC_VERSIONS"):
         # hack to be able to compile with gcc-8.4.0
         torch_cpp_ext.CUDA_GCC_VERSIONS["10.2"] = (
             torch_cpp_ext.MINIMUM_GCC_VERSION,
             (8, 4, 99),
         )
+
+    torch_version = torch.__version__.split(".")
+    torch_geq_113 = (
+        int(torch_version[0]) > 1
+        or int(torch_version[0]) == 1
+        and int(torch_version[1]) >= 13
+    )
 except ModuleNotFoundError:
     print("Theseus installation requires torch.")
     sys.exit(1)
 
 
 def parse_requirements_file(path):
     with open(path) as f:
         reqs = []
         for line in f:
+            if "functorch" in line and torch_geq_113:
+                # Don't install functorch 0.2.1 if torch 1.13 already
+                # installed
+                continue
             line = line.strip()
-            reqs.append(line.split("==")[0])
+            reqs.append(line)
     return reqs
 
 
 def get_baspacho_info(baspacho_root_dir, has_cuda):
     baspacho_build_dir = Path(baspacho_root_dir) / "build"
     include_dirs = [
         str(baspacho_root_dir),
@@ -79,18 +90,34 @@
     )
 
 
 reqs_main = parse_requirements_file("requirements/main.txt")
 reqs_dev = parse_requirements_file("requirements/dev.txt")
 root_dir = Path(__file__).parent
 
-with open(Path("theseus") / "__init__.py", "r") as f:
-    for line in f:
-        if "__version__" in line:
-            version = line.split("__version__ = ")[1].rstrip().strip('"')
+is_nightly = False
+nightly_date_str = os.environ.get("THESEUS_NIGHTLY", None)
+if nightly_date_str is not None:
+    from datetime import date, datetime
+
+    nightly_date = datetime.strptime(nightly_date_str, "%Y.%m.%d").date()
+    assert nightly_date == date.today(), (
+        f"THESEUS_NIGHTLY must be set to today's date in format %Y.%-m.%-d (stripped) "
+        f"but got {nightly_date_str}."
+    )
+    print(f"Building nightly with date {nightly_date_str}")
+    is_nightly = True
+
+if is_nightly:
+    version = nightly_date_str
+else:
+    with open(Path("theseus") / "_version.py", "r") as f:
+        for line in f:
+            if "__version__ = " in line:
+                version = line.split("__version__ = ")[1].rstrip().strip('"')
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # Add C++ and CUDA extensions
 compile_cuda_flag = os.environ.get("THESEUS_FORCE_CUDA")
 compile_cuda_support = (
@@ -123,20 +150,21 @@
 else:
     print("No CUDA support found. CUDA extensions won't be installed.")
     ext_modules = []
 baspacho_extension = maybe_create_baspacho_extension(compile_cuda_support)
 if baspacho_extension is not None:
     ext_modules.append(baspacho_extension)
 
-excluded_packages = []
-if not os.environ.get("INCLUDE_THESEUS_LABS"):
-    excluded_packages.append("theseus.labs")
+excluded_packages = ["lie", "lie.*", "tests*", "tests", "examples"]
+package_name = "theseus-ai-nightly" if is_nightly else "theseus-ai"
+if not os.environ.get("INCLUDE_THESEUS_LABS") and not is_nightly:
+    excluded_packages.append("theseus.labs*")
     print("Excluding theseus.labs")
 setuptools.setup(
-    name="theseus-ai",
+    name=package_name,
     version=version,
     author="Meta Research",
     description="A library for differentiable nonlinear optimization.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/facebookresearch/theseus",
     keywords="differentiable optimization, nonlinear least squares, factor graphs",
```

### Comparing `theseus-ai-0.1.4/theseus/__init__.py` & `theseus-ai-0.2.0.dev0/theseus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
-__version__ = "0.1.4"
+from ._version import __version__
 
 from .constants import DeviceType as DeviceType
 
 from .core import (  # usort: skip
     AutoDiffCostFunction,
     AutogradMode,
     CostFunction,
@@ -82,14 +82,15 @@
     LinearOptimizer,
     LinearSolver,
     LUCudaSparseSolver,
     LUDenseSolver,
 )
 from .optimizer.nonlinear import (  # usort: skip
     BackwardMode,
+    DCEM,
     Dogleg,
     GaussNewton,
     LevenbergMarquardt,
     NonlinearLeastSquares,
     NonlinearOptimizerInfo,
     NonlinearOptimizerParams,
     NonlinearOptimizerStatus,
```

### Comparing `theseus-ai-0.1.4/theseus/core/__init__.py` & `theseus-ai-0.2.0.dev0/theseus/core/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/core/cost_function.py` & `theseus-ai-0.2.0.dev0/theseus/core/cost_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 import contextlib
 from enum import Enum
 from itertools import chain
 from typing import Callable, List, Optional, Sequence, Tuple, Union, cast
 
 import torch
 import torch.autograd.functional as autogradF
-from functorch import jacrev, vmap
+
+try:
+    from torch.func import jacrev, vmap
+except ModuleNotFoundError:
+    from functorch import jacrev, vmap  # type: ignore
 from typing_extensions import Protocol
 
 from theseus.geometry import Manifold
 from theseus.geometry.lie_group_check import no_lie_group_check
 
 from .cost_weight import CostWeight, ScaleCostWeight
 from .theseus_function import TheseusFunction
@@ -199,16 +203,18 @@
         self,
         optim_vars: Sequence[Manifold],
         err_fn: ErrFnType,
         dim: int,
         cost_weight: Optional[CostWeight] = None,
         aux_vars: Optional[Sequence[Variable]] = None,
         name: Optional[str] = None,
+        autograd_create_graph: bool = True,
         autograd_strict: bool = False,
         autograd_vectorize: bool = False,
+        autograd_strategy: str = "reverse-mode",
         autograd_mode: Union[str, AutogradMode] = AutogradMode.VMAP,
     ):
         if cost_weight is None:
             cost_weight = ScaleCostWeight(1.0)
         super().__init__(cost_weight, name=name)
         # this avoids doing aux_vars=[], which is a bad default since [] is mutable
         aux_vars = aux_vars or []
@@ -218,16 +224,18 @@
                 "AutodiffCostFunction must receive at least one optimization variable."
             )
         self.register_vars(optim_vars, is_optim_vars=True)
         self.register_vars(aux_vars, is_optim_vars=False)
 
         self._err_fn = err_fn
         self._dim = dim
+        self._autograd_create_graph = autograd_create_graph
         self._autograd_strict = autograd_strict
         self._autograd_vectorize = autograd_vectorize
+        self._autograd_strategy = autograd_strategy
 
         # The following are auxiliary Variable objects to hold tensor data
         # during jacobian computation without modifying the original Variable objects
         self._tmp_optim_vars = tuple(v.copy() for v in optim_vars)
         self._tmp_aux_vars = None
         self._tmp_optim_vars_for_loop = None
         self._tmp_aux_vars_for_loop = None
@@ -275,17 +283,18 @@
 
     def _compute_autograd_jacobian(
         self, optim_tensors: Tuple[torch.Tensor, ...], jac_fn: Callable
     ) -> Tuple[torch.Tensor, ...]:
         return autogradF.jacobian(
             jac_fn,
             optim_tensors,
-            create_graph=True,
+            create_graph=self._autograd_create_graph,
             strict=self._autograd_strict,
             vectorize=self._autograd_vectorize,
+            strategy=self._autograd_strategy,
         )
 
     def _make_jac_fn_vmap(
         self, tmp_optim_vars: Tuple[Manifold, ...], tmp_aux_vars: Tuple[Variable, ...]
     ):
         def jac_fn(optim_vars_tensors_, aux_vars_tensors_):
             assert len(optim_vars_tensors_) == len(tmp_optim_vars)
```

### Comparing `theseus-ai-0.1.4/theseus/core/cost_weight.py` & `theseus-ai-0.2.0.dev0/theseus/core/cost_weight.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/core/objective.py` & `theseus-ai-0.2.0.dev0/theseus/core/objective.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,56 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
-
 import itertools
 import warnings
 from collections import OrderedDict
-from typing import Any, Callable, Dict, Iterable, List, Optional, Sequence, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Protocol,
+    Sequence,
+    Union,
+)
 
 import torch
 
 from theseus.constants import DeviceType
 from theseus.core.theseus_function import TheseusFunction
 from theseus.geometry.manifold import Manifold
 
 from .cost_function import CostFunction
 from .cost_weight import CostWeight
 from .variable import Variable
 
 
+class ErrorMetric(Protocol):
+    def __call__(self, error_vector: torch.Tensor) -> torch.Tensor:
+        pass
+
+
+def error_squared_norm_fn(error_vector: torch.Tensor) -> torch.Tensor:
+    return (error_vector**2).sum(dim=1) / 2
+
+
 # If dtype is None, uses torch.get_default_dtype()
 class Objective:
     """An objective function to optimize."""
 
-    def __init__(self, dtype: Optional[torch.dtype] = None):
+    def __init__(
+        self,
+        dtype: Optional[torch.dtype] = None,
+        error_metric_fn: Optional[ErrorMetric] = None,
+        __allow_mixed_optim_aux_vars__: bool = False,  # experimental
+    ):
         # maps variable names to the variable objects
         self.optim_vars: OrderedDict[str, Manifold] = OrderedDict()
 
         # maps variable names to variables objects, for optimization variables
         # that were registered when adding cost weights.
         self.cost_weight_optim_vars: OrderedDict[str, Manifold] = OrderedDict()
 
@@ -96,14 +119,22 @@
         # if vectorization should be updated
         self._num_updates_variables: Dict[str, int] = {}
 
         self._last_vectorization_has_grad = False
 
         self._vectorized = False
 
+        # Computes an aggregation function for the error vector derived from costs
+        # By default, this computes the squared norm of the error vector, divided by 2
+        self._error_metric_fn = (
+            error_metric_fn if error_metric_fn is not None else error_squared_norm_fn
+        )
+
+        self._allow_mixed_optim_aux_vars = __allow_mixed_optim_aux_vars__
+
     def _add_function_variables(
         self,
         function: TheseusFunction,
         optim_vars: bool = True,
         is_cost_weight: bool = False,
     ):
         if optim_vars:
@@ -142,14 +173,17 @@
                 assert variable not in self_var_to_fn_map
                 self_var_to_fn_map[variable] = []
 
             # add to either self.optim_vars,
             # self.cost_weight_optim_vars or self.aux_vars
             self_vars_of_this_type[variable.name] = variable
 
+            if self._allow_mixed_optim_aux_vars and variable not in self_var_to_fn_map:
+                self_var_to_fn_map[variable] = []
+
             # add to list of functions connected to this variable
             self_var_to_fn_map[variable].append(function)
 
     # Adds a cost function to the objective
     # Also adds its optimization variables if they haven't been previously added
     # Throws an error if a new variable has the same name of a previously added
     # variable that is not the same object.
@@ -219,24 +253,25 @@
         ]
         aux_vars_names = [
             var.name
             for var in itertools.chain(
                 cost_function.aux_vars, cost_function.weight.aux_vars
             )
         ]
-        dual_var_err_msg = (
-            "Objective does not support a variable being both "
-            + "an optimization variable and an auxiliary variable."
-        )
-        for optim_name in optim_vars_names:
-            if self.has_aux_var(optim_name):
-                raise ValueError(dual_var_err_msg)
-        for aux_name in aux_vars_names:
-            if self.has_optim_var(aux_name):
-                raise ValueError(dual_var_err_msg)
+        if not self._allow_mixed_optim_aux_vars:
+            dual_var_err_msg = (
+                "Objective does not support a variable being both "
+                + "an optimization variable and an auxiliary variable."
+            )
+            for optim_name in optim_vars_names:
+                if self.has_aux_var(optim_name):
+                    raise ValueError(dual_var_err_msg)
+            for aux_name in aux_vars_names:
+                if self.has_optim_var(aux_name):
+                    raise ValueError(dual_var_err_msg)
 
     # returns a reference to the cost function with the given name
     def get_cost_function(self, name: str) -> CostFunction:
         return self.cost_functions.get(name, None)
 
     # checks if the cost function with the given name is in the objective
     def has_cost_function(self, name: str) -> bool:
@@ -421,22 +456,35 @@
             # This line reverts back to the old tensors if a persistent update wasn't
             # required (i.e., `also_update is False`).
             # In this case, we pass _update_vectorization=False because
             # vectorization wasn't updated in the first call to `update()`.
             self.update(old_tensors, _update_vectorization=False)
         return error_vector
 
+    def error_metric(
+        self,
+        input_tensors: Optional[Dict[str, torch.Tensor]] = None,
+        also_update: bool = False,
+    ) -> torch.Tensor:
+        return self._error_metric_fn(
+            self.error(input_tensors=input_tensors, also_update=also_update)
+        )
+
     def error_squared_norm(
         self,
         input_tensors: Optional[Dict[str, torch.Tensor]] = None,
         also_update: bool = False,
     ) -> torch.Tensor:
-        return (
-            self.error(input_tensors=input_tensors, also_update=also_update) ** 2
-        ).sum(dim=1)
+        warnings.warn(
+            "Objective.error_squared_norm() is deprecated "
+            "and will be removed in future versions. "
+            "Please use Objective.error_metric() instead.",
+            DeprecationWarning,
+        )
+        return self.error_metric(input_tensors=input_tensors, also_update=also_update)
 
     def copy(self) -> "Objective":
         new_objective = Objective(dtype=self.dtype)
 
         # First copy all individual cost weights
         old_to_new_cost_weight_map: Dict[CostWeight, CostWeight] = {}
         for cost_weight in self.cost_functions_for_weights:
```

### Comparing `theseus-ai-0.1.4/theseus/core/robust_cost_function.py` & `theseus-ai-0.2.0.dev0/theseus/core/robust_cost_function.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,25 +37,30 @@
 #   - Note that h != r_e. In general, weighted_jacobians_and_error()
 #       is used by our optimizers, since it allows RobustCostFunction to be coupled
 #       with any Jacobian-based NLS solver w/o modifications. However, if you are
 #       interested in the robust cost value itself, you should use the error returned
 #       by `weighted_error()` and **NOT** the one returned by
 #       `weighted_jacobians_error()`.
 #
-# Finally, since we apply the weight before the robust loss, we adopt the convention
+# Since we apply the weight before the robust loss, we adopt the convention
 # that `robust_cost_fn.jacobians() == robust_cost_fn.weighted_jacobians_error()`, and
 # `robust_cost_fn.error() == robust_cost_fn.weighed_error()`.
+#
+# The flag `flatten_dims` can be used to apply the loss to each dimension of the error
+# as if it was a separate error term (for example, if one writes a regression problem
+# as a single CostFunction with each dimension being a residual term).
 class RobustCostFunction(CostFunction):
     _EPS = 1e-20
 
     def __init__(
         self,
         cost_function: CostFunction,
         loss_cls: Type[RobustLoss],
         log_loss_radius: Variable,
+        flatten_dims: bool = False,
         name: Optional[str] = None,
     ):
         self.cost_function = cost_function
         super().__init__(cost_function.weight, name=name)
 
         # Register optimization variables of the underlying cost function
         for attr in cost_function._optim_vars_attr_names:
@@ -66,27 +71,32 @@
         for attr in cost_function._aux_vars_attr_names:
             setattr(self, attr, getattr(cost_function, attr))
             self.register_aux_var(attr)
 
         self.log_loss_radius = log_loss_radius
         self.register_aux_var("log_loss_radius")
         self.loss = loss_cls()
+        self.flatten_dims = flatten_dims
 
     def error(self) -> torch.Tensor:
         warnings.warn(
             "Computing the robust cost error requires weighting first, so "
             "error() is equivalent to weighted_error()."
         )
         return self.weighted_error()
 
     def weighted_error(self) -> torch.Tensor:
         weighted_error = self.cost_function.weighted_error()
+        if self.flatten_dims:
+            weighted_error = weighted_error.reshape(-1, 1)
         squared_norm = torch.sum(weighted_error**2, dim=1, keepdim=True)
         error_loss = self.loss.evaluate(squared_norm, self.log_loss_radius.tensor)
 
+        if self.flatten_dims:
+            return (error_loss.reshape(-1, self.dim()) + RobustCostFunction._EPS).sqrt()
         # The return value is a hacky way to make it so that
         # ||weighted_error||^2 = error_loss
         # By doing this we avoid having to change the objective's error computation
         # specifically for robust cost functions. The issue for this type of cost
         # function is that the theory requires us to maintain scaled errors/jacobians
         # of dim = robust_fn.cost_function.dim() to do the linearization properly,
         # but the actual error has dim = 1, being the result of loss(||error||^2).
@@ -103,33 +113,44 @@
         return self.weighted_jacobians_error()
 
     def weighted_jacobians_error(self) -> Tuple[List[torch.Tensor], torch.Tensor]:
         (
             weighted_jacobians,
             weighted_error,
         ) = self.cost_function.weighted_jacobians_error()
+        if self.flatten_dims:
+            weighted_error = weighted_error.reshape(-1, 1)
+            for i, wj in enumerate(weighted_jacobians):
+                weighted_jacobians[i] = wj.view(-1, 1, wj.shape[2])
         squared_norm = torch.sum(weighted_error**2, dim=1, keepdim=True)
         rescale = (
             self.loss.linearize(squared_norm, self.log_loss_radius.tensor)
             + RobustCostFunction._EPS
         ).sqrt()
 
-        return [
+        rescaled_jacobians = [
             rescale.view(-1, 1, 1) * jacobian for jacobian in weighted_jacobians
-        ], rescale * weighted_error
+        ]
+        rescaled_error = rescale * weighted_error
+        if self.flatten_dims:
+            return [
+                rj.reshape(-1, self.dim(), rj.shape[2]) for rj in rescaled_jacobians
+            ], rescaled_error.reshape(-1, self.dim())
+        return rescaled_jacobians, rescaled_error
 
     def dim(self) -> int:
         return self.cost_function.dim()
 
     def _copy_impl(self, new_name: Optional[str] = None) -> "RobustCostFunction":
         return RobustCostFunction(
             self.cost_function.copy(),
             type(self.loss),
             self.log_loss_radius.copy(),
             name=new_name,
+            flatten_dims=self.flatten_dims,
         )
 
     @property
     def weight(self) -> CostWeight:
         return self.cost_function.weight
 
     @weight.setter
```

### Comparing `theseus-ai-0.1.4/theseus/core/robust_loss.py` & `theseus-ai-0.2.0.dev0/theseus/core/robust_loss.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/core/theseus_function.py` & `theseus-ai-0.2.0.dev0/theseus/core/theseus_function.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/core/variable.py` & `theseus-ai-0.2.0.dev0/theseus/core/variable.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/core/vectorizer.py` & `theseus-ai-0.2.0.dev0/theseus/core/vectorizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,24 +9,30 @@
 
 import torch
 
 from theseus.geometry.manifold import Manifold
 
 from .cost_function import AutoDiffCostFunction, CostFunction
 from .objective import Objective
+from .robust_cost_function import RobustCostFunction
 from .variable import Variable
 
 _CostFunctionSchema = Tuple[str, ...]
 
 
 def _get_cost_function_schema(cost_function: CostFunction) -> _CostFunctionSchema:
     def _fullname(obj) -> str:
         _name = f"{obj.__module__}.{obj.__class__.__name__}"
         if isinstance(obj, AutoDiffCostFunction):
             _name += f"__{id(obj._err_fn)}"
+        if isinstance(obj, RobustCostFunction):
+            _name += (
+                f"__{_fullname(obj.cost_function)}__"
+                f"{_fullname(obj.loss)}__{obj.flatten_dims}"
+            )
         return _name
 
     def _varinfo(var) -> str:
         return f"{_fullname(var)}{tuple(var.shape[1:])}"
 
     return (
         (_fullname(cost_function),)
```

### Comparing `theseus-ai-0.1.4/theseus/embodied/__init__.py` & `theseus-ai-0.2.0.dev0/theseus/embodied/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,9 +7,11 @@
 from .kinematics import IdentityModel, KinematicsModel, UrdfRobotModel
 from .measurements import Between, MovingFrameBetween, Reprojection
 from .misc import Local
 from .motionmodel import (
     DoubleIntegrator,
     GPCostWeight,
     GPMotionModel,
+    HingeCost,
+    Nonholonomic,
     QuasiStaticPushingPlanar,
 )
```

### Comparing `theseus-ai-0.1.4/theseus/embodied/collision/collision.py` & `theseus-ai-0.2.0.dev0/theseus/embodied/collision/collision.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/embodied/collision/eff_obj_contact.py` & `theseus-ai-0.2.0.dev0/theseus/embodied/collision/eff_obj_contact.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/embodied/collision/signed_distance_field.py` & `theseus-ai-0.2.0.dev0/theseus/embodied/collision/signed_distance_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,36 +18,45 @@
     # sdf_data shape is: batch_size x field_height x field_width
     def __init__(
         self,
         origin: Union[Point2, torch.Tensor],
         cell_size: Union[float, torch.Tensor, Variable],
         sdf_data: Optional[Union[torch.Tensor, Variable]] = None,
         occupancy_map: Optional[Union[torch.Tensor, Variable]] = None,
+        occupancy_threshold: float = 0.75,
+        sdf_boundary_value: float = 0.0,
     ):
         if occupancy_map is not None:
             if sdf_data is not None:
                 raise ValueError(
                     "Only one of sdf_data and occupancy_map should be provided."
                 )
             sdf_data = self._compute_sdf_data_from_map(
-                occupancy_map, SignedDistanceField2D.convert_cell_size(cell_size).tensor
+                occupancy_map,
+                SignedDistanceField2D.convert_cell_size(cell_size).tensor,
+                threshold=occupancy_threshold,
             )
         else:
             if sdf_data is None:
                 raise ValueError(
                     "Either sdf_data or argument occupancy_map should be provided."
                 )
+        self.origin: Point2
+        self.cell_size: Variable
+        self.sdf_data: Variable
         self.update_data(origin, sdf_data, cell_size)
         self._num_rows = sdf_data.shape[1]
         self._num_cols = sdf_data.shape[2]
+        self.sdf_boundary_value = sdf_boundary_value
 
     def _compute_sdf_data_from_map(
         self,
         occupancy_map_batch: Union[Variable, torch.Tensor],
         cell_size: torch.Tensor,
+        threshold: float = 0.75,
     ) -> Variable:
         if isinstance(occupancy_map_batch, Variable):
             occupancy_map_batch = occupancy_map_batch.tensor
         if cell_size.shape[0] != occupancy_map_batch.shape[0]:
             cell_size = cell_size.expand(occupancy_map_batch.shape[0], 1)
 
         # Code from https://github.com/gtrll/gpmp2/
@@ -58,15 +67,15 @@
             )
         num_maps = occupancy_map_batch.shape[0]
         all_sdf_data = []
 
         for i in range(num_maps):
             occupancy_map = occupancy_map_batch[i]
 
-            cur_map = occupancy_map > 0.75
+            cur_map = occupancy_map > threshold
             cur_map = cur_map.int()
 
             if torch.max(cur_map) == 0:
                 map_x, map_y = occupancy_map.size(0), occupancy_map.size(1)
                 max_map_size = 2 * cell_size[i].item() * max(map_x, map_y)
                 sdf_data = (
                     torch.ones(occupancy_map.shape, dtype=occupancy_map.dtype)
@@ -205,15 +214,15 @@
         lcdiff = cols - lc
         dist = (
             hrdiff * hcdiff * gather_sdf(lri, lci)
             + lrdiff * hcdiff * gather_sdf(hri, lci)
             + hrdiff * lcdiff * gather_sdf(lri, hci)
             + lrdiff * lcdiff * gather_sdf(hri, hci)
         )
-        dist[out_of_bounds_idx] = 0
+        dist[out_of_bounds_idx] = self.sdf_boundary_value
 
         # Compute the jacobians
 
         cell_size = (
             self.cell_size.tensor
             if self.cell_size.ndim == 2
             else self.cell_size.tensor.unsqueeze(-1)
@@ -226,7 +235,12 @@
         jac2 = (
             hcdiff * (gather_sdf(hri, lci) - gather_sdf(lri, lci))
             + lcdiff * (gather_sdf(hri, hci) - gather_sdf(lri, hci))
         ) / cell_size
         jac1[out_of_bounds_idx] = 0
         jac2[out_of_bounds_idx] = 0
         return dist, torch.stack([jac1, jac2], dim=2)
+
+    def to(self, *args, **kwargs):
+        self.cell_size.to(*args, **kwargs)
+        self.origin.to(*args, **kwargs)
+        self.sdf_data.to(*args, **kwargs)
```

### Comparing `theseus-ai-0.1.4/theseus/embodied/kinematics/kinematics_model.py` & `theseus-ai-0.2.0.dev0/theseus/embodied/kinematics/kinematics_model.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/embodied/measurements/between.py` & `theseus-ai-0.2.0.dev0/theseus/embodied/measurements/between.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/embodied/measurements/moving_frame_between.py` & `theseus-ai-0.2.0.dev0/theseus/embodied/measurements/moving_frame_between.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/embodied/measurements/reprojection.py` & `theseus-ai-0.2.0.dev0/theseus/embodied/measurements/reprojection.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/embodied/misc/local_cost_fn.py` & `theseus-ai-0.2.0.dev0/theseus/embodied/misc/local_cost_fn.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/embodied/motionmodel/double_integrator.py` & `theseus-ai-0.2.0.dev0/theseus/embodied/motionmodel/double_integrator.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/embodied/motionmodel/quasi_static_pushing_planar.py` & `theseus-ai-0.2.0.dev0/theseus/embodied/motionmodel/quasi_static_pushing_planar.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/extlib/baspacho_solver.cpp` & `theseus-ai-0.2.0.dev0/theseus/extlib/baspacho_solver.cpp`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/extlib/baspacho_solver.h` & `theseus-ai-0.2.0.dev0/theseus/extlib/baspacho_solver.h`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/extlib/baspacho_solver_cuda.cu` & `theseus-ai-0.2.0.dev0/theseus/extlib/baspacho_solver_cuda.cu`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/extlib/cusolver_lu_solver.cpp` & `theseus-ai-0.2.0.dev0/theseus/extlib/cusolver_lu_solver.cpp`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/extlib/cusolver_sp_defs.cpp` & `theseus-ai-0.2.0.dev0/theseus/extlib/cusolver_sp_defs.cpp`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/extlib/cusolver_sp_defs.h` & `theseus-ai-0.2.0.dev0/theseus/extlib/cusolver_sp_defs.h`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/extlib/mat_mult.cu` & `theseus-ai-0.2.0.dev0/theseus/extlib/mat_mult.cu`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/extlib/utils.h` & `theseus-ai-0.2.0.dev0/theseus/extlib/utils.h`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/geometry/__init__.py` & `theseus-ai-0.2.0.dev0/theseus/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/geometry/lie_group.py` & `theseus-ai-0.2.0.dev0/theseus/geometry/lie_group.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/geometry/lie_group_check.py` & `theseus-ai-0.2.0.dev0/theseus/geometry/lie_group_check.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/geometry/manifold.py` & `theseus-ai-0.2.0.dev0/theseus/geometry/manifold.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/geometry/point_types.py` & `theseus-ai-0.2.0.dev0/theseus/geometry/point_types.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/geometry/se2.py` & `theseus-ai-0.2.0.dev0/theseus/geometry/se2.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from typing import List, Optional, Union, cast
 
 import torch
 
 import theseus.constants
 from theseus.geometry.lie_group_check import no_lie_group_check
+from theseus.options import _THESEUS_GLOBAL_OPTIONS
 
 from .lie_group import LieGroup
 from .point_types import Point2
 from .so2 import SO2
 
 
 # If tensor is passed, must be x, y, cos, sin
@@ -30,19 +31,14 @@
             raise ValueError("Please provide only one of x_y_theta or tensor.")
         if x_y_theta is not None:
             dtype = x_y_theta.dtype
         super().__init__(tensor=tensor, name=name, dtype=dtype, strict=strict)
         if x_y_theta is not None:
             self.update_from_x_y_theta(x_y_theta)
 
-        self._resolve_eps()
-
-    def _resolve_eps(self):
-        self._NEAR_ZERO_EPS = theseus.constants._SE2_NEAR_ZERO_EPS[self.tensor.dtype]
-
     @staticmethod
     def rand(
         *size: int,
         generator: Optional[torch.Generator] = None,
         dtype: Optional[torch.dtype] = None,
         device: theseus.constants.DeviceType = None,
         requires_grad: bool = False,
@@ -163,15 +159,17 @@
         self, jacobians: Optional[List[torch.Tensor]] = None
     ) -> torch.Tensor:
         rotation = self.rotation
         theta = rotation.log_map().view(-1)
         cosine, sine = rotation.to_cos_sin()
 
         # Compute the approximations when theta is near to 0
-        small_theta = theta.abs() < self._NEAR_ZERO_EPS
+        small_theta = theta.abs() < _THESEUS_GLOBAL_OPTIONS.get_eps(
+            "se2", "near_zero", theta.dtype
+        )
         non_zero = torch.ones(1, dtype=self.dtype, device=self.device)
         sine_nz = torch.where(small_theta, non_zero, sine)
         half_theta_by_tan_half_theta = (
             0.5
             * (1 + cosine)
             * torch.where(small_theta, 1 + sine**2 / 6, theta / sine_nz)
         )
@@ -232,16 +230,16 @@
         u = tangent_vector[:, :2]
         theta = tangent_vector[:, 2]
         rotation = SO2(theta=theta)
 
         cosine, sine = rotation.to_cos_sin()
 
         # Compute the approximations when theta is near to 0
-        small_theta = (
-            theta.abs() < theseus.constants._SE2_NEAR_ZERO_EPS[tangent_vector.dtype]
+        small_theta = theta.abs() < _THESEUS_GLOBAL_OPTIONS.get_eps(
+            "se2", "near_zero", tangent_vector.dtype
         )
         non_zero = torch.ones(
             1, dtype=tangent_vector.dtype, device=tangent_vector.device
         )
         theta2 = theta**2
         theta3 = theta**3
         theta_nz = torch.where(small_theta, non_zero, theta)
@@ -460,12 +458,11 @@
     # only added to avoid casting downstream
     def copy(self, new_name: Optional[str] = None) -> "SE2":
         return cast(SE2, super().copy(new_name=new_name))
 
     # calls to() on the internal tensors
     def to(self, *args, **kwargs):
         super().to(*args, **kwargs)
-        self._resolve_eps()
 
 
 rand_se2 = SE2.rand
 randn_se2 = SE2.randn
```

### Comparing `theseus-ai-0.1.4/theseus/geometry/so2.py` & `theseus-ai-0.2.0.dev0/theseus/geometry/so2.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import warnings
 from typing import List, Optional, Tuple, Union, cast
 
 import torch
 
 import theseus.constants
+from theseus.options import _THESEUS_GLOBAL_OPTIONS
 
 from .lie_group import LieGroup
 from .lie_group_check import _LieGroupCheckContext
 from .point_types import Point2
 
 
 class SO2(LieGroup):
@@ -122,15 +123,15 @@
 
     @staticmethod
     def _check_tensor_impl(tensor: torch.Tensor) -> bool:
         with torch.no_grad():
             if tensor.ndim != 2 or tensor.shape[1] != 2:
                 raise ValueError("SO2 data tensors can only be 2D vectors.")
 
-            MATRIX_EPS = theseus.constants._SO2_MATRIX_EPS[tensor.dtype]
+            MATRIX_EPS = _THESEUS_GLOBAL_OPTIONS.get_eps("so2", "matrix", tensor.dtype)
             if tensor.dtype != torch.float64:
                 tensor = tensor.double()
 
             _check = (
                 torch.linalg.norm(tensor, dim=1) - 1
             ).abs().max().item() <= MATRIX_EPS
 
@@ -178,15 +179,17 @@
 
     @staticmethod
     def normalize(tensor: torch.Tensor) -> torch.Tensor:
         if tensor.ndim != 2 or tensor.shape[1] != 2:
             raise ValueError("SO2 data tensors can only be 2D vectors.")
 
         data_norm = torch.norm(tensor, dim=1, keepdim=True)
-        near_zero = data_norm < theseus.constants._SO2_NORMALIZATION_EPS[tensor.dtype]
+        near_zero = data_norm < _THESEUS_GLOBAL_OPTIONS.get_eps(
+            "so2", "norm", tensor.dtype
+        )
         data_norm_nz = torch.where(
             near_zero,
             torch.tensor(1.0, dtype=tensor.dtype, device=tensor.device),
             data_norm,
         )
         default_data = torch.tensor(
             [1, 0], dtype=tensor.dtype, device=tensor.device
```

### Comparing `theseus-ai-0.1.4/theseus/geometry/utils.py` & `theseus-ai-0.2.0.dev0/theseus/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/geometry/vector.py` & `theseus-ai-0.2.0.dev0/theseus/geometry/vector.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/optimizer/autograd/baspacho_sparse_autograd.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/baspacho_sparse_autograd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 from typing import Any, Tuple, Optional
 import torch
 
+from .common import compute_A_grad
 from ..linear_system import SparseStructure
 from theseus.utils.sparse_matrix_utils import mat_vec, tmat_vec
 
 _BaspachoSolveFunctionBwdReturnType = Tuple[
-    torch.Tensor, torch.Tensor, None, None, None, None, None, None
+    torch.Tensor, torch.Tensor, None, None, None, None, None, None, None
 ]
 
 
 class BaspachoSolveFunction(torch.autograd.Function):
     @staticmethod
     def forward(  # type: ignore
         ctx: Any,
         A_val: torch.Tensor,
         b: torch.Tensor,
         sparse_structure: SparseStructure,
         A_row_ptr: torch.Tensor,
         A_col_ind: torch.Tensor,
         symbolic_decomposition: Any,  # actually SymbolicDecomposition
         damping_alpha_beta: Optional[Tuple[torch.Tensor, torch.Tensor]],
+        detach_hessian: bool = False,
     ) -> torch.Tensor:
         from theseus.extlib.baspacho_solver import SymbolicDecomposition
 
         assert isinstance(symbolic_decomposition, SymbolicDecomposition)
 
         batch_size = A_val.shape[0]
 
@@ -52,14 +54,15 @@
         ctx.x = x
         ctx.A_val_double = A_val_double
         ctx.A_row_ptr = A_row_ptr
         ctx.A_col_ind = A_col_ind
         ctx.sparse_structure = sparse_structure
         ctx.numeric_decomposition = numeric_decomposition
         ctx.damping_alpha_beta = damping_alpha_beta
+        ctx.detach_hessian = detach_hessian
 
         return x.to(A_val.dtype)
 
     # Let v row vector, and w column vector of dimension n, m, and
     # A an nxm matrix. Then
     #   v * A * w = Sum(v_i * A_ij * w_j) = [v (X) w] . A
     # Where by [v (X) w] we mean the nxm matrix which is the
@@ -130,39 +133,34 @@
         # now we fill values of a matrix with structure identical to A with
         # selected entries from the difference of tensor products:
         #   b_Ax (X) H - AH (X) x
         # NOTE: this row-wise manipulation can be much faster in C++ or Cython
         A_col_ind = ctx.sparse_structure.col_ind
         A_row_ptr = ctx.sparse_structure.row_ptr
         batch_size = grad_output.shape[0]
-        A_grad = torch.empty(
-            size=(batch_size, len(A_col_ind)),
-            dtype=torch.double,
-            device=grad_output.device,
-        )  # return value, A's grad
-        for r in range(len(A_row_ptr) - 1):
-            start, end = A_row_ptr[r], A_row_ptr[r + 1]
-            columns = A_col_ind[start:end]  # col indices, for this row
-            A_grad[:, start:end] = (
-                b_Ax[:, r].unsqueeze(1) * H_double[:, columns]
-                - AH[:, r].unsqueeze(1) * ctx.x[:, columns]
-            )
 
-        # apply correction if there is a multiplicative damping
-        if (
-            ctx.damping_alpha_beta is not None
-            and (ctx.damping_alpha_beta[0] > 0.0).any()
-        ):
-            alpha = ctx.damping_alpha_beta[0].view(-1, 1)
-            alpha2Hx = (alpha * 2.0) * H_double * ctx.x  # componentwise product
-            A_grad -= ctx.A_val_double * alpha2Hx[:, ctx.A_col_ind.type(torch.long)]
+        A_grad = compute_A_grad(
+            batch_size,
+            A_row_ptr,
+            A_col_ind,
+            ctx.b,
+            ctx.x,
+            b_Ax,
+            H_double,
+            AH,
+            ctx.damping_alpha_beta,
+            ctx.A_val_double,
+            ctx.A_col_ind,
+            ctx.detach_hessian,
+        )
 
         return (
             A_grad.to(dtype=grad_output.dtype),
             AH.to(dtype=grad_output.dtype),
             None,
             None,
             None,
             None,
             None,
             None,
+            None,
         )
```

### Comparing `theseus-ai-0.1.4/theseus/optimizer/autograd/cholmod_sparse_autograd.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/cholmod_sparse_autograd.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,32 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 from typing import Any, Tuple
 
 import torch
 from sksparse.cholmod import Factor as CholeskyDecomposition
 
+from .common import compute_A_grad
 from ..linear_system import SparseStructure
 
-_CholmodSolveFunctionBwdReturnType = Tuple[torch.Tensor, torch.Tensor, None, None, None]
+_CholmodSolveFunctionBwdReturnType = Tuple[
+    torch.Tensor, torch.Tensor, None, None, None, None
+]
 
 
 class CholmodSolveFunction(torch.autograd.Function):
     @staticmethod
     def forward(  # type: ignore
         ctx: Any,
         At_val: torch.Tensor,
         b: torch.Tensor,
         sparse_structure: SparseStructure,
         symbolic_decomposition: CholeskyDecomposition,
         damping: float,
+        detach_hessian: bool = False,
     ) -> torch.Tensor:
         At_val_cpu = At_val.cpu().double()
         b_cpu = b.cpu().double()
         batch_size = At_val.shape[0]
         x_cpu = torch.empty(
             size=(batch_size, sparse_structure.num_cols),
             dtype=At_val.dtype,
@@ -43,14 +47,15 @@
             cholesky_decompositions.append(cholesky_decomposition)
 
         ctx.b_cpu = b_cpu
         ctx.x_cpu = x_cpu
         ctx.At_val_cpu = At_val_cpu
         ctx.sparse_structure = sparse_structure
         ctx.cholesky_decompositions = cholesky_decompositions
+        ctx.detach_hessian = detach_hessian
 
         return x_cpu.to(device=At_val.device, dtype=At_val.dtype)
 
     # Let v row vector, and w column vector of dimension n, m, and
     # A an nxm matrix. Then
     #   v * A * w = Sum(v_i * A_ij * w_j) = [v (X) w] . A
     # Where by [v (X) w] we mean the nxm matrix which is the
@@ -119,20 +124,24 @@
         # now we fill values of a matrix with structure identical to A with
         # selected entries from the difference of tensor products:
         #   b_Ax (X) H - AH (X) x
         # NOTE: this row-wise manipulation can be much faster in C++ or Cython
         A_col_ind = ctx.sparse_structure.col_ind
         A_row_ptr = ctx.sparse_structure.row_ptr
         batch_size = grad_output.shape[0]
-        A_grad = torch.empty(
-            size=(batch_size, len(A_col_ind))
-        )  # return value, A's grad
-        for r in range(len(A_row_ptr) - 1):
-            start, end = A_row_ptr[r], A_row_ptr[r + 1]
-            columns = A_col_ind[start:end]  # col indices, for this row
-            A_grad[:, start:end] = (
-                b_Ax[:, r].unsqueeze(1) * H[:, columns]
-                - AH[:, r].unsqueeze(1) * ctx.x_cpu[:, columns]
-            )
 
+        A_grad = compute_A_grad(
+            batch_size,
+            A_row_ptr,
+            A_col_ind,
+            ctx.b_cpu,
+            ctx.x_cpu,
+            b_Ax,
+            H,
+            AH,
+            None,
+            None,
+            None,
+            ctx.detach_hessian,
+        )
         dev = grad_output.device
-        return A_grad.to(device=dev), AH.to(device=dev), None, None, None
+        return A_grad.to(device=dev), AH.to(device=dev), None, None, None, None
```

### Comparing `theseus-ai-0.1.4/theseus/optimizer/autograd/lu_cuda_sparse_autograd.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/lu_cuda_sparse_autograd.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 from typing import Any, Optional, Tuple
 import torch
 
 from ..linear_system import SparseStructure
+from .common import compute_A_grad
 
 _LUCudaSolveFunctionBwdReturnType = Tuple[
-    torch.Tensor, torch.Tensor, None, None, None, None, None, None
+    torch.Tensor, torch.Tensor, None, None, None, None, None, None, None
 ]
 
 
 class LUCudaSolveFunction(torch.autograd.Function):
     @staticmethod
     def forward(  # type: ignore
         ctx: Any,
@@ -20,14 +21,15 @@
         b: torch.Tensor,
         sparse_structure: SparseStructure,
         A_row_ptr: torch.Tensor,
         A_col_ind: torch.Tensor,
         solver_context: Any,  # actually CusolverLUSolver,
         damping_alpha_beta: Optional[Tuple[torch.Tensor, torch.Tensor]],
         check_factor_id,
+        detach_hessian: bool = False,
     ) -> torch.Tensor:
         if not torch.cuda.is_available():
             raise RuntimeError("Cuda not available, LUCudaSolveFunction cannot be used")
 
         try:
             from theseus.extlib.cusolver_lu_solver import CusolverLUSolver
             from theseus.extlib.mat_mult import apply_damping, mult_MtM, tmat_vec
@@ -68,14 +70,15 @@
         ctx.x = x
         ctx.A_val_double = A_val_double
         ctx.A_row_ptr = A_row_ptr
         ctx.A_col_ind = A_col_ind
         ctx.sparse_structure = sparse_structure
         ctx.solver_context = solver_context
         ctx.damping_alpha_beta = damping_alpha_beta
+        ctx.detach_hessian = detach_hessian
 
         # HACK: allows to check if the context has been reused (and overwritten)
         ctx.factor_id = solver_context.factor_id if check_factor_id else None
 
         return x.to(A_val.dtype)
 
     # Let v row vector, and w column vector of dimension n, m, and
@@ -168,40 +171,34 @@
         # now we fill values of a matrix with structure identical to A with
         # selected entries from the difference of tensor products:
         #   b_Ax (X) H - AH (X) x
         # NOTE: this row-wise manipulation can be much faster in C++ or Cython
         A_col_ind = ctx.sparse_structure.col_ind
         A_row_ptr = ctx.sparse_structure.row_ptr
         batch_size = grad_output.shape[0]
-        A_grad = torch.empty(
-            size=(batch_size, len(A_col_ind)), dtype=torch.double, device="cuda"
-        )  # return value, A's grad
-        for r in range(len(A_row_ptr) - 1):
-            start, end = A_row_ptr[r], A_row_ptr[r + 1]
-            columns = A_col_ind[start:end]  # col indices, for this row
-            A_grad[:, start:end] = (
-                b_Ax[:, r].unsqueeze(1) * H_double[:, columns]
-                - AH[:, r].unsqueeze(1) * ctx.x[:, columns]
-            )
 
-        # apply correction if there is a multiplicative damping
-        if (
-            ctx.damping_alpha_beta is not None
-            and (ctx.damping_alpha_beta[0] > 0.0).any()
-        ):
-            alpha = ctx.damping_alpha_beta[0].view(-1, 1)
-            alpha2Hx = (alpha * 2.0) * H_double * ctx.x  # componentwise product
-            A_grad -= (
-                ctx.A_val_double.to(grad_output.dtype)
-                * alpha2Hx[:, ctx.A_col_ind.type(torch.long)]
-            )
+        A_grad = compute_A_grad(
+            batch_size,
+            A_row_ptr,
+            A_col_ind,
+            ctx.b,
+            ctx.x,
+            b_Ax,
+            H_double,
+            AH,
+            ctx.damping_alpha_beta,
+            ctx.A_val_double,
+            ctx.A_col_ind,
+            ctx.detach_hessian,
+        )
 
         return (
             A_grad.to(dtype=grad_output.dtype),
             AH.to(dtype=grad_output.dtype),
             None,
             None,
             None,
             None,
             None,
             None,
+            None,
         )
```

### Comparing `theseus-ai-0.1.4/theseus/optimizer/dense_linearization.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/dense_linearization.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,18 +51,18 @@
                 row_slice = slice(err_row_idx, err_row_idx + num_rows)
                 col_slice = slice(var_start_col, var_start_col + num_cols)
                 self.A[:, row_slice, col_slice] = var_jacobian
 
             self.b[:, row_slice] = -error
             err_row_idx += cost_function.dim()
 
-    def _linearize_hessian_impl(self):
+    def _linearize_hessian_impl(self, _detach_hessian: bool = False):
         self._linearize_jacobian_impl()
         At = self.A.transpose(1, 2)
-        self._AtA = At.bmm(self.A)
+        self._AtA = At.bmm(self.A).detach() if _detach_hessian else At.bmm(self.A)
         self._Atb = At.bmm(self.b.unsqueeze(2))
 
     def hessian_approx(self):
         return self._AtA
 
     def _ata_impl(self) -> torch.Tensor:
         return self._AtA
```

### Comparing `theseus-ai-0.1.4/theseus/optimizer/linear/__init__.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/linear/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/optimizer/linear/baspacho_sparse_solver.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/linear/baspacho_sparse_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,8 +126,9 @@
             self.linearization.A_val,
             self.linearization.b,
             self.linearization.structure(),
             self.A_row_ptr,
             self.A_col_ind,
             self.symbolic_decomposition,
             damping_alpha_beta,
+            self.linearization.detached_hessian,
         )
```

### Comparing `theseus-ai-0.1.4/theseus/optimizer/linear/cholmod_sparse_solver.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/linear/cholmod_sparse_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class CholmodSparseSolver(LinearSolver):
     def __init__(
         self,
         objective: Objective,
         linearization_cls: Optional[Type[Linearization]] = None,
         linearization_kwargs: Optional[Dict[str, Any]] = None,
-        damping: float = 1e-6,
+        damping: float = 0.0,
         **kwargs,
     ):
         linearization_cls = linearization_cls or SparseLinearization
         if not linearization_cls == SparseLinearization:
             raise RuntimeError(
                 "CholmodSparseSolver only works with theseus.optimizer.SparseLinearization,"
                 + f" got {type(self.linearization)}"
@@ -60,8 +60,9 @@
 
         return CholmodSolveFunction.apply(
             self.linearization.A_val,
             self.linearization.b,
             self.linearization.structure(),
             self._symbolic_cholesky_decomposition,
             damping,
+            self.linearization.detached_hessian,
         )
```

### Comparing `theseus-ai-0.1.4/theseus/optimizer/linear/dense_solver.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/linear/dense_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/optimizer/linear/linear_optimizer.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/linear/linear_optimizer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/optimizer/linear/linear_solver.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/linear/linear_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/optimizer/linear/lu_cuda_sparse_solver.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/linear/lu_cuda_sparse_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,8 +164,9 @@
             self.linearization.b,
             self.linearization.structure(),
             self.A_row_ptr,
             self.A_col_ind,
             self._solver_contexts[self._last_solver_context],
             damping_alpha_beta,
             True,
+            self.linearization.detached_hessian,
         )
```

### Comparing `theseus-ai-0.1.4/theseus/optimizer/linear/utils.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/linear/utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/optimizer/linear_system.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/linear_system.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/optimizer/linearization.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/linearization.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,23 +41,23 @@
         self.num_rows = self.objective.dim()
 
     @abc.abstractmethod
     def _linearize_jacobian_impl(self):
         pass
 
     @abc.abstractmethod
-    def _linearize_hessian_impl(self):
+    def _linearize_hessian_impl(self, _detach_hessian: bool = False):
         pass
 
-    def linearize(self):
+    def linearize(self, _detach_hessian: bool = False):
         if not self.ordering.complete:
             raise RuntimeError(
                 "Attempted to linearize an objective with an incomplete variable order."
             )
-        self._linearize_hessian_impl()
+        self._linearize_hessian_impl(_detach_hessian=_detach_hessian)
 
     def hessian_approx(self):
         raise NotImplementedError(
             f"hessian_approx is not implemented for {self.__class__.__name__}"
         )
 
     @abc.abstractmethod
```

### Comparing `theseus-ai-0.1.4/theseus/optimizer/manifold_gaussian.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/manifold_gaussian.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/optimizer/nonlinear/dogleg.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/dogleg.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/optimizer/nonlinear/gauss_newton.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/gauss_newton.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/optimizer/nonlinear/levenberg_marquardt.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/levenberg_marquardt.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         **kwargs,
     ) -> None:
         super().reset(**kwargs)
         if adaptive_damping and not self._allows_adaptive:
             raise NotImplementedError(
                 f"Adaptive damping is only supported by solvers with type "
                 f"[{_ADAPT_DAMP_SOLVERS_STR}], but got solver of type "
-                f"{type(self.linear_solver)}."
+                f"{type(self.linear_solver).__name__}."
             )
         if adaptive_damping:
             self._damping = damping * torch.ones(
                 self.objective.batch_size,
                 device=self.objective.device,
                 dtype=self.objective.dtype,
             )
@@ -145,15 +145,15 @@
         down_damping_ratio: float = 9.0,
         up_damping_ratio: float = 11.0,
         damping_accept: float = 0.1,
         ellipsoidal_damping: bool = False,
         **kwargs,
     ) -> Optional[torch.Tensor]:
         # "err" tensors passed as input refer to the squared norm of the
-        # error vector, as returned by self._error_metric()
+        # error vector, as returned by self.objective.error_metric()
         if adaptive_damping:
             return self._check_accept(
                 delta,
                 new_err,
                 previous_err,
                 damping_accept,
                 down_damping_ratio,
```

### Comparing `theseus-ai-0.1.4/theseus/optimizer/nonlinear/trust_region.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/trust_region.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         shrink_ratio: float = 0.25,
         expand_ratio: float = 2.0,
         min_trust_region: float = 1.0e-5,
         max_trust_region: float = 1.0e5,
         **kwargs,
     ) -> Optional[torch.Tensor]:
         # "err" tensors passed as input refer to the squared norm of the
-        # error vector, as returned by self._error_metric()
+        # error vector, as returned by self.objective.error_metric()
         good_params = (0.0 < shrink_ratio <= 1.0) and (expand_ratio >= 1.0)
         good_params &= (shrink_threshold < expand_threshold) and (
             accept_threshold < shrink_threshold
         )
         if not good_params:
             raise ValueError(
                 "Invalid parameters for TrustRegionMethod. "
```

### Comparing `theseus-ai-0.1.4/theseus/optimizer/optimizer.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/optimizer/sparse_linearization.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/sparse_linearization.py`

 * *Files 8% similar despite different names*

```diff
@@ -91,15 +91,20 @@
         # self._linearize_jacobian_impl()
         self._Atb: torch.Tensor = None
 
         # computed lazily by self.diagonal_scaling() and reset to None by
         # self._linearize_jacobian_impl()
         self._AtA_diag: torch.Tensor = None
 
+        # If true, it signals to linear solvers that any computation resulting from
+        # matrix (At * A) must be detached from the compute graph
+        self.detached_hessian = False
+
     def _linearize_jacobian_impl(self):
+        self._detached_hessian = False
         self._Atb = None
         self._AtA_diag = None
 
         # those will be fully overwritten, no need to zero:
         self.A_val = torch.empty(
             size=(self.objective.batch_size, len(self.A_col_ind)),
             device=self.objective.device,
@@ -139,16 +144,20 @@
             self.A_col_ind,
             self.A_row_ptr,
             self.num_rows,
             self.num_cols,
             dtype=np.float64 if self.objective.dtype == torch.double else np.float32,
         )
 
-    def _linearize_hessian_impl(self):
+    def _linearize_hessian_impl(self, _detach_hessian: bool = False):
+        # Some of our sparse solvers don't require explicitly computing the
+        # hessian approximation, so we only compute the jacobian here and let each
+        # solver handle this as needed
         self._linearize_jacobian_impl()
+        self.detached_hessian = _detach_hessian
 
     def _ata_impl(self) -> torch.Tensor:
         raise NotImplementedError("AtA is not yet implemented for SparseLinearization.")
 
     def _atb_impl(self) -> torch.Tensor:
         if self._Atb is None:
             A_row_ptr = torch.tensor(self.A_row_ptr, dtype=torch.int32).to(
```

### Comparing `theseus-ai-0.1.4/theseus/optimizer/variable_ordering.py` & `theseus-ai-0.2.0.dev0/theseus/optimizer/variable_ordering.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/theseus_layer.py` & `theseus-ai-0.2.0.dev0/theseus/theseus_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Vectorize,
 )
 from theseus.constants import __FROM_THESEUS_LAYER_TOKEN__, DeviceType
 from theseus.geometry import LieGroup, Manifold
 from theseus.optimizer import Optimizer, OptimizerInfo
 from theseus.optimizer.linear import LinearSolver
 from theseus.optimizer.nonlinear import BackwardMode, GaussNewton
+from theseus.utils import check_jacobians
 
 
 class TheseusLayer(nn.Module):
     def __init__(
         self,
         optimizer: Optimizer,
         vectorize: bool = True,
@@ -142,14 +143,26 @@
     def device(self) -> DeviceType:
         return self.objective.device
 
     @property
     def dtype(self) -> torch.dtype:
         return self.objective.dtype
 
+    def verify_jacobians(self, num_checks: int = 1, tol: float = 1.0e-3):
+        success = True
+        for cf in self.objective.cost_functions.values():
+            try:
+                check_jacobians(cf, num_checks=num_checks, tol=tol)
+            except RuntimeError as e:
+                print(f"Jacobians check for cost function named {cf.name} failed.")
+                print(e)
+                success = False
+        if success:
+            print("Jacobians check were successful!")
+
 
 def _forward(
     objective: Objective,
     optimizer: Optimizer,
     optimizer_kwargs: Dict[str, Any],
     input_tensors: Dict[str, torch.Tensor],
 ):
@@ -197,15 +210,15 @@
             ctx.bwd_objective = bwd_objective
             ctx.bwd_optimizer = bwd_optimizer
             ctx.epsilon = epsilon
 
             # Precompute and cache this.
             with torch.enable_grad():
                 grad_sol = torch.autograd.grad(
-                    objective.error_squared_norm().sum(),
+                    objective.error_metric().sum(),
                     differentiable_tensors,
                     allow_unused=True,
                 )
             ctx.save_for_backward(
                 *input_vals, *grad_sol, *differentiable_tensors, *optim_tensors
             )
         return (*optim_tensors, info)
@@ -249,15 +262,15 @@
             bwd_optimizer.objective.retract_vars_sequence(
                 delta, bwd_optimizer.linear_solver.linearization.ordering
             )
 
         # Compute gradients.
         with torch.enable_grad():
             grad_perturbed = torch.autograd.grad(
-                bwd_objective.error_squared_norm().sum(),
+                bwd_objective.error_metric().sum(),
                 differentiable_tensors,
                 allow_unused=True,
             )
 
         nones = [None] * (ctx.n * 2)
         grads = [
             (gs - gp) / epsilon if gs is not None else None
@@ -285,24 +298,26 @@
         self.var = var
         self.epsilon = epsilon
         self.grad = grad
         self.register_optim_var("var")
         self.register_aux_vars(["epsilon", "grad"])
 
     def error(self) -> torch.Tensor:
-        err = (
+        # Theseus optimizes SUM(err ** 2) / 2. We add sqrt(2) so
+        # that when expanding the objective is SUM(err_orig) /2 + ||dlm_error||**2
+        err = np.sqrt(2) * (
             self.epsilon.tensor.view((-1,) + (1,) * (self.var.ndim - 1))
             * self.var.tensor
             - 0.5 * self.grad.tensor
         )
         return err.flatten(start_dim=1)
 
     def jacobians(self) -> Tuple[List[torch.Tensor], torch.Tensor]:
         d = self.dim()
-        aux = (
+        aux = np.sqrt(2) * (
             torch.eye(d, dtype=self.epsilon.dtype, device=self.epsilon.device)
             .unsqueeze(0)
             .expand(self.var.shape[0], d, d)
         )
         euclidean_grad_flat = self.epsilon.tensor.view(-1, 1, 1) * aux
         euclidean_grad = euclidean_grad_flat.unflatten(2, self.var.shape[1:])
         return [self.var.project(euclidean_grad, is_sparse=True)], self.error()
```

### Comparing `theseus-ai-0.1.4/theseus/third_party/easyaug.py` & `theseus-ai-0.2.0.dev0/theseus/third_party/easyaug.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/third_party/utils.py` & `theseus-ai-0.2.0.dev0/theseus/third_party/utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/utils/examples/__init__.py` & `theseus-ai-0.2.0.dev0/theseus/utils/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/utils/examples/bundle_adjustment/data.py` & `theseus-ai-0.2.0.dev0/theseus/utils/examples/bundle_adjustment/data.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/utils/examples/bundle_adjustment/util.py` & `theseus-ai-0.2.0.dev0/theseus/utils/examples/bundle_adjustment/util.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/utils/examples/motion_planning/misc.py` & `theseus-ai-0.2.0.dev0/theseus/utils/examples/motion_planning/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,31 +137,31 @@
 
     def _append(new_theta, scale=1.0):
         x_new = x + radius * np.cos(new_theta) * scale
         y_new = y + radius * np.sin(new_theta) * scale
         triangle_pts.append((x_new, y_new))
 
     _append(theta, 1.0)
-    _append(theta + np.pi / 2, 0.5)
-    _append(theta - np.pi / 2, 0.5)
+    _append(theta + np.pi / 2, 0.3)
+    _append(theta - np.pi / 2, 0.3)
     return triangle_pts
 
 
 def _add_robot_to_trajectory(
     x_list, y_list, radius, color="magenta", alpha=0.05, theta=None
 ):
     patches = []
     for i in range(x_list.shape[0]):
         if theta is None:
             patches.append(mpl.patches.Circle((x_list[i], y_list[i]), radius))
             alpha_ = alpha
         else:
             triangle_pts = _get_triangle_pts(x_list[i], y_list[i], theta[i], radius)
             patches.append(mpl.patches.Polygon(triangle_pts))
-            alpha_ = 2 * alpha
+            alpha_ = 4 * alpha
     patch_collection = mpl.collections.PatchCollection(
         patches, alpha=alpha_, color=color
     )
     return patch_collection
 
 
 def generate_trajectory_figs(
```

### Comparing `theseus-ai-0.1.4/theseus/utils/examples/motion_planning/models.py` & `theseus-ai-0.2.0.dev0/theseus/utils/examples/motion_planning/models.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/utils/examples/motion_planning/motion_planner.py` & `theseus-ai-0.2.0.dev0/theseus/utils/examples/motion_planning/motion_planner.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import copy
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import torch
 
 import theseus as th
+from theseus.embodied import HingeCost, Nonholonomic
 
 
 class _XYDifference(th.CostFunction):
     def __init__(
         self,
         var: th.SE2,
         target: th.Point2,
@@ -56,19 +57,21 @@
 class MotionPlannerObjective(th.Objective):
     def __init__(
         self,
         map_size: int,
         epsilon_dist: float,
         total_time: float,
         collision_weight: float,
-        Qc_inv: List[List[int]],
+        Qc_inv: Union[List[List[float]], torch.Tensor],
         num_time_steps: int,
         use_single_collision_weight: bool = True,
         pose_type: Union[Type[th.Point2], Type[th.SE2]] = th.Point2,
         dtype: torch.dtype = torch.double,
+        nonholonomic_w: float = 0.0,
+        positive_vel_w: float = 0.0,
     ):
         for v in [
             map_size,
             epsilon_dist,
             total_time,
             collision_weight,
             Qc_inv,
@@ -111,15 +114,16 @@
             torch.tensor(total_time / num_time_steps, dtype=dtype).view(1, 1), name="dt"
         )
 
         # --------------------------------------------------------------------------- #
         # ------------------------------- Cost weights ------------------------------ #
         # --------------------------------------------------------------------------- #
         # For the GP cost functions, we create a single GPCost weight
-        gp_cost_weight = th.eb.GPCostWeight(torch.tensor(Qc_inv, dtype=dtype), dt)
+        qc_inv_tensor = torch.as_tensor(Qc_inv, dtype=dtype)
+        gp_cost_weight = th.eb.GPCostWeight(qc_inv_tensor.to(dtype=dtype), dt)
 
         # Now we create cost weights for the collision-avoidance cost functions
         # Each of this is a scalar cost weight with a named auxiliary variable.
         # Before running the motion planner, each cost weight value can be updated
         # by passing {name: new_cost_weight_tensor} to the forward method
         collision_cost_weights = []
         if use_single_collision_weight:
@@ -131,15 +135,16 @@
                 )
             )
         else:
             for i in range(1, self.trajectory_len):
                 collision_cost_weights.append(
                     th.ScaleCostWeight(
                         th.Variable(
-                            torch.tensor(collision_weight), name=f"collision_w_{i}"
+                            torch.tensor(collision_weight, dtype=dtype),
+                            name=f"collision_w_{i}",
                         )
                     )
                 )
 
         # For hard-constraints (end points pos/vel) we use a single scalar weight
         # with high value
         boundary_cost_weight = th.ScaleCostWeight(torch.tensor(100.0, dtype=dtype))
@@ -187,14 +192,22 @@
                 velocities[-1],
                 th.Vector(tensor=torch.zeros(1, velocities[-1].dof(), dtype=dtype)),
                 boundary_cost_weight,
                 name="vel_N",
             )
         )
 
+        if nonholonomic_w > 0.0:
+            assert pose_type == th.SE2
+            nhw = th.ScaleCostWeight(nonholonomic_w, name="nonholonomic_w")
+
+        if positive_vel_w > 0.0:
+            assert pose_type == th.SE2
+            pvw = th.ScaleCostWeight(positive_vel_w, name="positive_vel_w")
+
         # Next we add 2-D collisions and GP cost functions, and associate them with the
         # cost weights created above. We need a separate cost function for each time
         # step
         for i in range(1, self.trajectory_len):
             self.add(
                 th.eb.Collision2D(
                     poses[i],
@@ -217,75 +230,83 @@
                         velocities[i],
                         dt,
                         gp_cost_weight,
                         name=f"gp_{i}",
                     )
                 )
             )
+            if nonholonomic_w > 0.0:
+                self.add(
+                    Nonholonomic(
+                        poses[i],  # type: ignore
+                        velocities[i],
+                        nhw,
+                        name=f"nonholonomic_{i}",
+                    )
+                )
+            if positive_vel_w:
+                self.add(
+                    HingeCost(
+                        velocities[i - 1],
+                        torch.tensor([0.0, -torch.inf, -torch.inf]).view(1, 3),
+                        torch.tensor([torch.inf, torch.inf, torch.inf]).view(1, 3),
+                        1.0,
+                        pvw,
+                        name=f"positive_vel_{i}",
+                    ),
+                )
 
 
 class MotionPlanner:
     # If objective is given, this overrides problem arguments
     def __init__(
         self,
-        optim_method: str,
-        max_optim_iters: int,
-        step_size: float = 1.0,
+        optimizer_config: Tuple[str, Dict[str, Any]],
         objective: Optional[MotionPlannerObjective] = None,
         device: th.DeviceType = "cpu",
         dtype: torch.dtype = torch.double,
         # The following are only used if objective is None
         map_size: Optional[int] = None,
         epsilon_dist: Optional[float] = None,
         total_time: Optional[float] = None,
         collision_weight: Optional[float] = None,
-        Qc_inv: Optional[List[List[int]]] = None,
+        Qc_inv: Optional[Union[List[List[float]], torch.Tensor]] = None,
         num_time_steps: Optional[int] = None,
         use_single_collision_weight: bool = True,
         pose_type: Union[Type[th.Point2], Type[th.SE2]] = th.Point2,
+        nonholonomic_w: float = 0.0,
+        positive_vel_w: float = 0.0,
     ):
         if objective is None:
             self.objective = MotionPlannerObjective(
                 map_size,
                 epsilon_dist,
                 total_time,
                 collision_weight,
                 Qc_inv,
                 num_time_steps,
                 use_single_collision_weight=use_single_collision_weight,
                 pose_type=pose_type,
                 dtype=dtype,
+                nonholonomic_w=nonholonomic_w,
+                positive_vel_w=positive_vel_w,
             )
         else:
             self.objective = objective
 
-        self.optim_method = optim_method
-        self.max_optim_iters = max_optim_iters
-        self.step_size = step_size
+        self.optimizer_config = optimizer_config
         self.device = device
         self.dtype = dtype
 
         # Finally, create the Nonlinear Least Squares optimizer for this objective
         # and wrap both into a TheseusLayer
         optimizer: th.NonlinearLeastSquares
-        if optim_method == "gauss_newton":
-            optimizer = th.GaussNewton(
-                self.objective,
-                th.CholeskyDenseSolver,
-                max_iterations=max_optim_iters,
-                step_size=step_size,
-            )
-        elif optim_method == "levenberg_marquardt":
-            optimizer = th.LevenbergMarquardt(
-                self.objective,
-                th.CholeskyDenseSolver,
-                max_iterations=max_optim_iters,
-                step_size=step_size,
-            )
-
+        optimizer_cls = getattr(th, optimizer_config[0])
+        assert issubclass(optimizer_cls, th.NonlinearLeastSquares)
+        optimizer = optimizer_cls(self.objective, **optimizer_config[1])
         self.layer = th.TheseusLayer(optimizer)
         self.layer.to(device=device, dtype=dtype)
 
         # A call to motion_planner.layer.forward(input_dict) will run the NLLS optimizer
         # to solve for a trajectory given the input data. The input dictionary, supports
         # the keys and values illustrated below, where ':' represents a batch dimension.
         #
@@ -391,39 +412,39 @@
             input_dict[f"pose_{i}"] = trajectory[:, :pose_numel, i]
             input_dict[f"vel_{i}"] = trajectory[:, pose_numel:, i]
         return input_dict
 
     def error(self) -> float:
         # Returns the current MSE of the optimization problem
         with torch.no_grad():
-            return self.objective.error_squared_norm().mean().item()
+            return self.objective.error_metric().mean().item()
 
     def get_trajectory(
         self,
         values_dict: Optional[Dict[str, torch.Tensor]] = None,
         detach: bool = False,
     ) -> torch.Tensor:
         # Returns the a tensor with the trajectory that the given variable
         # values represent. If no dictionary is passed, it will used the latest
         # values stored in the objective's variables.
         pose_numel = 2 if self.objective.pose_type == th.Point2 else 4
         vel_numel = 2 if self.objective.pose_type == th.Point2 else 3
-        trajectory = torch.empty(
+        trajectory = torch.zeros(
             self.objective.batch_size,
             pose_numel + vel_numel,
             self.objective.trajectory_len,
             device=self.objective.device,
         )
-        variables = self.objective.optim_vars
+        if values_dict is None:
+            values_dict = {
+                k: t.tensor.clone() for (k, t) in self.objective.optim_vars.items()
+            }
         for i in range(self.objective.trajectory_len):
-            if values_dict is None:
-                trajectory[:, :pose_numel, i] = variables[f"pose_{i}"].tensor.clone()
-                trajectory[:, pose_numel:, i] = variables[f"vel_{i}"].tensor.clone()
-            else:
-                trajectory[:, :pose_numel, i] = values_dict[f"pose_{i}"]
+            trajectory[:, :pose_numel, i] = values_dict[f"pose_{i}"]
+            if f"vel_{i}" in values_dict:
                 trajectory[:, pose_numel:, i] = values_dict[f"vel_{i}"]
         return trajectory.detach() if detach else trajectory
 
     def get_total_squared_errors(self) -> Tuple[torch.Tensor, torch.Tensor]:
         gp_error: torch.Tensor = 0  # type: ignore
         collision_error: torch.Tensor = 0  # type: ignore
         for name, cf in self.objective.cost_functions.items():
@@ -431,17 +452,15 @@
                 gp_error += cf.error().square().mean()
             if "collision" in name:
                 collision_error += cf.error().square().mean()
         return gp_error, collision_error
 
     def copy(self, collision_weight: Optional[float] = None) -> "MotionPlanner":
         return MotionPlanner(
-            self.optim_method,
-            self.max_optim_iters,
-            step_size=self.step_size,
+            self.optimizer_config,
             map_size=self.objective.map_size,
             epsilon_dist=self.objective.epsilon_dist,
             total_time=self.objective.total_time,
             collision_weight=collision_weight or self.objective.collision_weight,
             Qc_inv=self.objective.Qc_inv,
             num_time_steps=self.objective.num_time_steps,
             use_single_collision_weight=self.objective.use_single_collision_weight,
```

### Comparing `theseus-ai-0.1.4/theseus/utils/examples/pose_graph/dataset.py` & `theseus-ai-0.2.0.dev0/theseus/utils/examples/pose_graph/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                 ).to(dtype)
                 relative_pose = th.SE2(
                     x_y_theta=x_y_theta, name="EDGE_SE2__{}".format(n)
                 )
 
                 sel = [0, 3, 5]
                 weight = th.Variable(
-                    torch.from_numpy(np.array(tokens[6:], dtype=np.float64)[sel])
+                    torch.from_numpy(np.array(1, tokens[6:], dtype=np.float64)[sel])
                     .to(dtype)
                     .sqrt()
                     .view(1, -1)
                 )
 
                 edges.append(
                     PoseGraphEdge(
@@ -263,15 +263,15 @@
                 tensor=torch.tile(torch.eye(3, 4, dtype=dtype), [dataset_size, 1, 1]),
                 name="VERTEX_SE3_GT__0",
             )
         )
 
         info = torch.tensor(
             [1 / translation_noise] * 3 + [1 / rotation_noise] * 3, dtype=dtype
-        )
+        ).view(1, -1)
 
         for n in range(1, num_poses):
             gt_relative_pose = th.SE3.exp_map(
                 torch.cat(
                     [
                         torch.rand(dataset_size, 3, dtype=dtype) - 0.5,
                         2.0 * torch.rand(dataset_size, 3, dtype=dtype) - 1,
```

### Comparing `theseus-ai-0.1.4/theseus/utils/examples/tactile_pose_estimation/misc.py` & `theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/misc.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/utils/examples/tactile_pose_estimation/models.py` & `theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/models.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/utils/examples/tactile_pose_estimation/pose_estimator.py` & `theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/pose_estimator.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/utils/examples/tactile_pose_estimation/trainer.py` & `theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/trainer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus/utils/sparse_matrix_utils.py` & `theseus-ai-0.2.0.dev0/theseus/utils/sparse_matrix_utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.1.4/theseus_ai.egg-info/PKG-INFO` & `theseus-ai-0.2.0.dev0/theseus_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theseus-ai
-Version: 0.1.4
+Version: 0.2.0.dev0
 Summary: A library for differentiable nonlinear optimization.
 Home-page: https://github.com/facebookresearch/theseus
 Author: Meta Research
 Keywords: differentiable optimization,nonlinear least squares,factor graphs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: theseus-ai Version: 0.1.4 Summary: A library for
-differentiable nonlinear optimization. Home-page: https://github.com/
+Metadata-Version: 2.1 Name: theseus-ai Version: 0.2.0.dev0 Summary: A library
+for differentiable nonlinear optimization. Home-page: https://github.com/
 facebookresearch/theseus Author: Meta Research Keywords: differentiable
 optimization,nonlinear least squares,factor graphs Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
 LICENSE ![](https://raw.githubusercontent.com/facebookresearch/theseus/main/
```

### Comparing `theseus-ai-0.1.4/theseus_ai.egg-info/SOURCES.txt` & `theseus-ai-0.2.0.dev0/theseus_ai.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -2,44 +2,18 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 requirements/dev.txt
 requirements/docs.txt
 requirements/main.txt
-tests/__init__.py
-tests/decorators.py
-tests/test_dlm_perturbation.py
-tests/test_theseus_layer.py
-tests/core/__init__.py
-tests/core/common.py
-tests/core/test_cost_function.py
-tests/core/test_cost_weight.py
-tests/core/test_manifold.py
-tests/core/test_objective.py
-tests/core/test_robust_cost.py
-tests/core/test_theseus_function.py
-tests/core/test_variable.py
-tests/core/test_vectorizer.py
-tests/extlib/__init__.py
-tests/extlib/test_baspacho.py
-tests/extlib/test_baspacho_simple.py
-tests/extlib/test_cusolver_lu_solver.py
-tests/extlib/test_mat_mult.py
-tests/geometry/__init__.py
-tests/geometry/common.py
-tests/geometry/point_types_mypy_check.py
-tests/geometry/test_point_types.py
-tests/geometry/test_se2.py
-tests/geometry/test_se3.py
-tests/geometry/test_so2.py
-tests/geometry/test_so3.py
-tests/geometry/test_vector.py
 theseus/__init__.py
+theseus/_version.py
 theseus/constants.py
+theseus/options.py
 theseus/theseus_layer.py
 theseus/core/__init__.py
 theseus/core/cost_function.py
 theseus/core/cost_weight.py
 theseus/core/objective.py
 theseus/core/robust_cost_function.py
 theseus/core/robust_loss.py
@@ -57,14 +31,15 @@
 theseus/embodied/measurements/between.py
 theseus/embodied/measurements/moving_frame_between.py
 theseus/embodied/measurements/reprojection.py
 theseus/embodied/misc/__init__.py
 theseus/embodied/misc/local_cost_fn.py
 theseus/embodied/motionmodel/__init__.py
 theseus/embodied/motionmodel/double_integrator.py
+theseus/embodied/motionmodel/misc.py
 theseus/embodied/motionmodel/quasi_static_pushing_planar.py
 theseus/extlib/__init__.py
 theseus/extlib/baspacho_solver.cpp
 theseus/extlib/baspacho_solver.h
 theseus/extlib/baspacho_solver_cuda.cu
 theseus/extlib/cusolver_lu_solver.cpp
 theseus/extlib/cusolver_sp_defs.cpp
@@ -78,48 +53,52 @@
 theseus/geometry/point_types.py
 theseus/geometry/se2.py
 theseus/geometry/se3.py
 theseus/geometry/so2.py
 theseus/geometry/so3.py
 theseus/geometry/utils.py
 theseus/geometry/vector.py
-theseus/labs/lie_functional/__init__.py
-theseus/labs/lie_functional/constants.py
-theseus/labs/lie_functional/lie_group.py
-theseus/labs/lie_functional/so3.py
-theseus/labs/lie_functional/utils.py
+theseus/labs/__init__.py
+theseus/labs/embodied/__init__.py
+theseus/labs/embodied/robot/__init__.py
+theseus/labs/embodied/robot/forward_kinematics.py
+theseus/labs/embodied/robot/joint.py
+theseus/labs/embodied/robot/robot.py
 theseus/optimizer/__init__.py
 theseus/optimizer/dense_linearization.py
 theseus/optimizer/linear_system.py
 theseus/optimizer/linearization.py
 theseus/optimizer/manifold_gaussian.py
 theseus/optimizer/optimizer.py
 theseus/optimizer/sparse_linearization.py
 theseus/optimizer/variable_ordering.py
 theseus/optimizer/autograd/__init__.py
 theseus/optimizer/autograd/baspacho_sparse_autograd.py
 theseus/optimizer/autograd/cholmod_sparse_autograd.py
+theseus/optimizer/autograd/common.py
 theseus/optimizer/autograd/lu_cuda_sparse_autograd.py
 theseus/optimizer/linear/__init__.py
 theseus/optimizer/linear/baspacho_sparse_solver.py
 theseus/optimizer/linear/cholmod_sparse_solver.py
 theseus/optimizer/linear/dense_solver.py
 theseus/optimizer/linear/linear_optimizer.py
 theseus/optimizer/linear/linear_solver.py
 theseus/optimizer/linear/lu_cuda_sparse_solver.py
 theseus/optimizer/linear/utils.py
 theseus/optimizer/nonlinear/__init__.py
+theseus/optimizer/nonlinear/dcem.py
 theseus/optimizer/nonlinear/dogleg.py
 theseus/optimizer/nonlinear/gauss_newton.py
 theseus/optimizer/nonlinear/levenberg_marquardt.py
 theseus/optimizer/nonlinear/nonlinear_least_squares.py
 theseus/optimizer/nonlinear/nonlinear_optimizer.py
 theseus/optimizer/nonlinear/trust_region.py
 theseus/third_party/__init__.py
 theseus/third_party/easyaug.py
+theseus/third_party/lml.py
 theseus/third_party/utils.py
 theseus/utils/__init__.py
 theseus/utils/sparse_matrix_utils.py
 theseus/utils/utils.py
 theseus/utils/examples/__init__.py
 theseus/utils/examples/bundle_adjustment/__init__.py
 theseus/utils/examples/bundle_adjustment/data.py
```

