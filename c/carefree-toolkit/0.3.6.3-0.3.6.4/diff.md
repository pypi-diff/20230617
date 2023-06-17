# Comparing `tmp/carefree-toolkit-0.3.6.3.tar.gz` & `tmp/carefree-toolkit-0.3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-toolkit-0.3.6.3.tar", last modified: Fri Jun  9 06:35:15 2023, max compression
+gzip compressed data, was "carefree-toolkit-0.3.6.4.tar", last modified: Sat Jun 17 03:37:11 2023, max compression
```

## Comparing `carefree-toolkit-0.3.6.3.tar` & `carefree-toolkit-0.3.6.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 heyujian   (501) staff       (20)        0 2023-06-09 06:35:15.863214 carefree-toolkit-0.3.6.3/
--rw-r--r--   0 heyujian   (501) staff       (20)     1069 2022-06-30 09:46:01.000000 carefree-toolkit-0.3.6.3/LICENSE
--rw-r--r--   0 heyujian   (501) staff       (20)     8557 2023-06-09 06:35:15.862929 carefree-toolkit-0.3.6.3/PKG-INFO
--rw-r--r--   0 heyujian   (501) staff       (20)     8138 2022-06-30 09:46:01.000000 carefree-toolkit-0.3.6.3/README.md
-drwxr-xr-x   0 heyujian   (501) staff       (20)        0 2023-06-09 06:35:15.855573 carefree-toolkit-0.3.6.3/carefree_toolkit.egg-info/
--rw-r--r--   0 heyujian   (501) staff       (20)     8557 2023-06-09 06:35:15.000000 carefree-toolkit-0.3.6.3/carefree_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 heyujian   (501) staff       (20)      463 2023-06-09 06:35:15.000000 carefree-toolkit-0.3.6.3/carefree_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 heyujian   (501) staff       (20)        1 2023-06-09 06:35:15.000000 carefree-toolkit-0.3.6.3/carefree_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 heyujian   (501) staff       (20)       54 2023-06-09 06:35:15.000000 carefree-toolkit-0.3.6.3/carefree_toolkit.egg-info/requires.txt
--rw-r--r--   0 heyujian   (501) staff       (20)        7 2023-06-09 06:35:15.000000 carefree-toolkit-0.3.6.3/carefree_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 heyujian   (501) staff       (20)        0 2023-06-09 06:35:15.861480 carefree-toolkit-0.3.6.3/cftool/
--rw-r--r--   0 heyujian   (501) staff       (20)        0 2022-06-30 09:46:01.000000 carefree-toolkit-0.3.6.3/cftool/__init__.py
--rw-r--r--   0 heyujian   (501) staff       (20)    21981 2023-04-01 16:30:06.000000 carefree-toolkit-0.3.6.3/cftool/array.py
--rw-r--r--   0 heyujian   (501) staff       (20)       56 2023-05-19 06:12:55.000000 carefree-toolkit-0.3.6.3/cftool/constants.py
--rw-r--r--   0 heyujian   (501) staff       (20)     8185 2023-04-01 16:30:06.000000 carefree-toolkit-0.3.6.3/cftool/cv.py
--rw-r--r--   0 heyujian   (501) staff       (20)    16766 2023-06-09 06:23:40.000000 carefree-toolkit-0.3.6.3/cftool/data_structures.py
-drwxr-xr-x   0 heyujian   (501) staff       (20)        0 2023-06-09 06:35:15.862159 carefree-toolkit-0.3.6.3/cftool/dist/
--rw-r--r--   0 heyujian   (501) staff       (20)       27 2023-04-01 16:30:06.000000 carefree-toolkit-0.3.6.3/cftool/dist/__init__.py
--rw-r--r--   0 heyujian   (501) staff       (20)    21300 2022-09-14 03:20:51.000000 carefree-toolkit-0.3.6.3/cftool/dist/core.py
--rw-r--r--   0 heyujian   (501) staff       (20)     9607 2023-05-31 07:35:01.000000 carefree-toolkit-0.3.6.3/cftool/geometry.py
--rw-r--r--   0 heyujian   (501) staff       (20)    24711 2022-06-30 09:59:24.000000 carefree-toolkit-0.3.6.3/cftool/manage.py
--rw-r--r--   0 heyujian   (501) staff       (20)    82529 2023-05-19 06:12:55.000000 carefree-toolkit-0.3.6.3/cftool/misc.py
--rw-r--r--   0 heyujian   (501) staff       (20)     6243 2023-04-01 16:30:06.000000 carefree-toolkit-0.3.6.3/cftool/pipeline.py
--rw-r--r--   0 heyujian   (501) staff       (20)      965 2023-04-01 16:30:06.000000 carefree-toolkit-0.3.6.3/cftool/types.py
--rw-r--r--   0 heyujian   (501) staff       (20)     2163 2023-05-19 06:12:55.000000 carefree-toolkit-0.3.6.3/cftool/web.py
--rw-r--r--   0 heyujian   (501) staff       (20)       38 2023-06-09 06:35:15.863271 carefree-toolkit-0.3.6.3/setup.cfg
--rw-r--r--   0 heyujian   (501) staff       (20)      871 2023-06-09 06:35:03.000000 carefree-toolkit-0.3.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 03:37:11.424605 carefree-toolkit-0.3.6.4/
+-rw-rw-rw-   0        0        0     1090 2019-09-25 20:51:10.000000 carefree-toolkit-0.3.6.4/LICENSE
+-rw-rw-rw-   0        0        0     9010 2023-06-17 03:37:11.420615 carefree-toolkit-0.3.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8579 2022-06-27 01:36:51.000000 carefree-toolkit-0.3.6.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 03:37:11.340762 carefree-toolkit-0.3.6.4/carefree_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     9010 2023-06-17 03:37:11.000000 carefree-toolkit-0.3.6.4/carefree_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-06-17 03:37:11.000000 carefree-toolkit-0.3.6.4/carefree_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 03:37:11.000000 carefree-toolkit-0.3.6.4/carefree_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-17 03:37:11.000000 carefree-toolkit-0.3.6.4/carefree_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-17 03:37:11.000000 carefree-toolkit-0.3.6.4/carefree_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 03:37:11.406588 carefree-toolkit-0.3.6.4/cftool/
+-rw-rw-rw-   0        0        0        0 2020-11-05 10:59:33.000000 carefree-toolkit-0.3.6.4/cftool/__init__.py
+-rw-rw-rw-   0        0        0    22677 2023-04-03 14:14:29.000000 carefree-toolkit-0.3.6.4/cftool/array.py
+-rw-rw-rw-   0        0        0       58 2023-05-18 01:18:59.000000 carefree-toolkit-0.3.6.4/cftool/constants.py
+-rw-rw-rw-   0        0        0     8445 2023-04-03 14:14:29.000000 carefree-toolkit-0.3.6.4/cftool/cv.py
+-rw-rw-rw-   0        0        0    17747 2023-06-17 03:34:51.000000 carefree-toolkit-0.3.6.4/cftool/data_structures.py
+drwxrwxrwx   0        0        0        0 2023-06-17 03:37:11.414632 carefree-toolkit-0.3.6.4/cftool/dist/
+-rw-rw-rw-   0        0        0       28 2023-04-03 14:14:29.000000 carefree-toolkit-0.3.6.4/cftool/dist/__init__.py
+-rw-rw-rw-   0        0        0    21842 2022-08-08 17:03:13.000000 carefree-toolkit-0.3.6.4/cftool/dist/core.py
+-rw-rw-rw-   0        0        0     9983 2023-06-05 15:51:28.000000 carefree-toolkit-0.3.6.4/cftool/geometry.py
+-rw-rw-rw-   0        0        0    25320 2022-08-08 17:03:13.000000 carefree-toolkit-0.3.6.4/cftool/manage.py
+-rw-rw-rw-   0        0        0    85083 2023-05-18 01:18:59.000000 carefree-toolkit-0.3.6.4/cftool/misc.py
+-rw-rw-rw-   0        0        0     6451 2023-04-03 14:14:29.000000 carefree-toolkit-0.3.6.4/cftool/pipeline.py
+-rw-rw-rw-   0        0        0     1004 2023-04-03 14:14:29.000000 carefree-toolkit-0.3.6.4/cftool/types.py
+-rw-rw-rw-   0        0        0     2237 2023-05-18 01:18:59.000000 carefree-toolkit-0.3.6.4/cftool/web.py
+-rw-rw-rw-   0        0        0       42 2023-06-17 03:37:11.425601 carefree-toolkit-0.3.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      905 2023-06-17 03:37:04.000000 carefree-toolkit-0.3.6.4/setup.py
```

### Comparing `carefree-toolkit-0.3.6.3/LICENSE` & `carefree-toolkit-0.3.6.4/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2019 carefree0910
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2019 carefree0910
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `carefree-toolkit-0.3.6.3/cftool/array.py` & `carefree-toolkit-0.3.6.4/cftool/array.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,696 +1,696 @@
-import math
-
-import numpy as np
-
-from typing import Any
-from typing import Dict
-from typing import List
-from typing import Tuple
-from typing import Union
-from typing import Callable
-from typing import Optional
-from typing import NamedTuple
-from collections import Counter
-from multiprocessing.shared_memory import SharedMemory
-from numpy.lib.stride_tricks import as_strided
-
-from .misc import random_hash
-from .types import torch
-from .types import torchvision
-from .types import F
-from .types import arr_type
-from .types import tensor_dict_type
-
-
-TNormalizeResponse = Union[arr_type, Tuple[arr_type, Dict[str, Any]]]
-
-
-def is_int(arr: np.ndarray) -> bool:
-    return np.issubdtype(arr.dtype, np.integer)
-
-
-def is_float(arr: np.ndarray) -> bool:
-    return np.issubdtype(arr.dtype, np.floating)
-
-
-def is_string(arr: np.ndarray) -> bool:
-    return np.issubdtype(arr.dtype, str)
-
-
-def sigmoid(arr: arr_type) -> arr_type:
-    if isinstance(arr, np.ndarray):
-        return 1.0 / (1.0 + np.exp(-arr))
-    return torch.sigmoid(arr)
-
-
-def softmax(arr: arr_type) -> arr_type:
-    if isinstance(arr, np.ndarray):
-        logits = arr - np.max(arr, axis=1, keepdims=True)
-        exp = np.exp(logits)
-        return exp / exp.sum(1, keepdims=True)
-    return F.softmax(arr, dim=1)
-
-
-def l2_normalize(arr: arr_type) -> arr_type:
-    if isinstance(arr, np.ndarray):
-        return arr / np.linalg.norm(arr, axis=-1, keepdims=True)
-    return arr / arr.norm(dim=-1, keepdim=True)
-
-
-def normalize(
-    arr: arr_type,
-    *,
-    global_norm: bool = True,
-    return_stats: False,
-    eps: float = 1.0e-8,
-) -> TNormalizeResponse:
-    if global_norm:
-        arr_mean, arr_std = arr.mean().item(), arr.std().item()
-        arr_std = max(eps, arr_std)
-        out = (arr - arr_mean) / arr_std
-        if not return_stats:
-            return out
-        return out, dict(mean=arr_mean, std=arr_std)
-    if isinstance(arr, np.ndarray):
-        arr_mean, arr_std = arr.mean(axis=0), arr.std(axis=0)
-        std = np.maximum(eps, arr_std)
-    else:
-        arr_mean, arr_std = arr.mean(dim=0), arr.std(dim=0)
-        std = torch.clip(arr_std, min=eps)
-    out = (arr - arr_mean) / std
-    if not return_stats:
-        return out
-    return out, dict(mean=arr_mean.tolist(), std=std.tolist())
-
-
-def normalize_from(arr: arr_type, stats: Dict[str, Any]) -> arr_type:
-    mean, std = stats["mean"], stats["std"]
-    return (arr - mean) / std
-
-
-def recover_normalize_from(arr: arr_type, stats: Dict[str, Any]) -> arr_type:
-    mean, std = stats["mean"], stats["std"]
-    return arr * std + mean
-
-
-def min_max_normalize(
-    arr: arr_type,
-    *,
-    global_norm: bool = True,
-    return_stats: False,
-    eps: float = 1.0e-8,
-) -> TNormalizeResponse:
-    if global_norm:
-        arr_min, arr_max = arr.min().item(), arr.max().item()
-        diff = max(eps, arr_max - arr_min)
-        out = (arr - arr_min) / diff
-        if not return_stats:
-            return out
-        return out, dict(min=arr_min, diff=diff)
-    if isinstance(arr, np.ndarray):
-        arr_min, arr_max = arr.min(axis=0), arr.max(axis=0)
-        diff = np.maximum(eps, arr_max - arr_min)
-    else:
-        arr_min, arr_max = arr.min(dim=0).values, arr.max(dim=0).values
-        diff = torch.clip(arr_max - arr_min, min=eps)
-    out = (arr - arr_min) / diff
-    if not return_stats:
-        return out
-    return out, dict(min=arr_min.tolist(), diff=diff.tolist())
-
-
-def min_max_normalize_from(arr: arr_type, stats: Dict[str, Any]) -> arr_type:
-    arr_min, diff = stats["min"], stats["diff"]
-    return (arr - arr_min) / diff
-
-
-def recover_min_max_normalize_from(arr: arr_type, stats: Dict[str, Any]) -> arr_type:
-    arr_min, diff = stats["min"], stats["diff"]
-    return arr * diff + arr_min
-
-
-def quantile_normalize(
-    arr: arr_type,
-    *,
-    q: float = 0.01,
-    global_norm: bool = True,
-    return_stats: False,
-    eps: float = 1.0e-8,
-) -> TNormalizeResponse:
-    # quantiles
-    if isinstance(arr, np.ndarray):
-        kw = {"axis": 0}
-        quantile_fn = np.quantile
-    else:
-        kw = {"dim": 0}
-        quantile_fn = torch.quantile
-    if global_norm:
-        arr_min = quantile_fn(arr, q)
-        arr_max = quantile_fn(arr, 1.0 - q)
-    else:
-        arr_min = quantile_fn(arr, q, **kw)
-        arr_max = quantile_fn(arr, 1.0 - q, **kw)
-    # diff
-    if global_norm:
-        diff = max(eps, arr_max - arr_min)
-    else:
-        if isinstance(arr, np.ndarray):
-            diff = np.maximum(eps, arr_max - arr_min)
-        else:
-            diff = torch.clip(arr_max - arr_min, min=eps)
-    arr = arr.clip(arr_min, arr_max)
-    out = (arr - arr_min) / diff
-    if not return_stats:
-        return out
-    if not global_norm:
-        arr_min = arr_min.item()
-        diff = diff.item()
-    else:
-        arr_min = arr_min.tolist()
-        diff = diff.tolist()
-    return out, dict(min=arr_min, diff=diff)
-
-
-def quantile_normalize_from(arr: arr_type, stats: Dict[str, Any]) -> arr_type:
-    arr_min, diff = stats["min"], stats["diff"]
-    return (arr - arr_min) / diff
-
-
-def recover_quantile_normalize_from(arr: arr_type, stats: Dict[str, Any]) -> arr_type:
-    arr_min, diff = stats["min"], stats["diff"]
-    return arr * diff + arr_min
-
-
-def clip_normalize(arr: arr_type) -> arr_type:
-    fn = np if isinstance(arr, np.ndarray) else torch
-    if arr.dtype == fn.uint8:
-        return arr
-    return fn.clip(arr, 0.0, 1.0)
-
-
-# will return at least 2d
-def squeeze(arr: arr_type) -> arr_type:
-    n = arr.shape[0]
-    arr = arr.squeeze()
-    if n == 1:
-        arr = arr[None, ...]
-    return arr
-
-
-def to_standard(arr: np.ndarray) -> np.ndarray:
-    if is_int(arr):
-        arr = arr.astype(np.int64)
-    elif is_float(arr):
-        arr = arr.astype(np.float32)
-    return arr
-
-
-def to_torch(arr: np.ndarray) -> torch.Tensor:
-    return torch.from_numpy(to_standard(arr))
-
-
-def to_numpy(tensor: torch.Tensor) -> np.ndarray:
-    return tensor.detach().cpu().numpy()
-
-
-def to_device(
-    batch: tensor_dict_type,
-    device: torch.device,
-    **kwargs: Any,
-) -> tensor_dict_type:
-    return {
-        k: v.to(device, **kwargs)
-        if isinstance(v, torch.Tensor)
-        else [
-            vv.to(device, **kwargs) if isinstance(vv, torch.Tensor) else vv for vv in v
-        ]
-        if isinstance(v, list)
-        else v
-        for k, v in batch.items()
-    }
-
-
-def iou(logits: arr_type, labels: arr_type) -> arr_type:
-    is_numpy = isinstance(logits, np.ndarray)
-    num_classes = logits.shape[1]
-    if num_classes == 1:
-        heat_map = sigmoid(logits)
-    elif num_classes == 2:
-        heat_map = softmax(logits)[:, [1]]
-    else:
-        raise ValueError("`IOU` only supports binary situations")
-    intersect = heat_map * labels
-    union = heat_map + labels - intersect
-    kwargs = {"axis" if is_numpy else "dim": tuple(range(1, len(intersect.shape)))}
-    return intersect.sum(**kwargs) / union.sum(**kwargs)
-
-
-def corr(
-    predictions: arr_type,
-    target: arr_type,
-    weights: Optional[arr_type] = None,
-    *,
-    get_diagonal: bool = False,
-) -> arr_type:
-    is_numpy = isinstance(predictions, np.ndarray)
-    keepdim_kw = {"keepdims" if is_numpy else "keepdim": True}
-    norm_fn = np.linalg.norm if is_numpy else torch.norm
-    matmul_fn = np.matmul if is_numpy else torch.matmul
-    sqrt_fn = np.sqrt if is_numpy else torch.sqrt
-    transpose_fn = np.transpose if is_numpy else torch.t
-
-    w_sum = 0.0 if weights is None else weights.sum().item()
-    if weights is None:
-        mean = predictions.mean(0, **keepdim_kw)
-    else:
-        mean = (predictions * weights).sum(0, **keepdim_kw) / w_sum
-    vp = predictions - mean
-    if weights is None:
-        kw = keepdim_kw.copy()
-        kw["axis" if is_numpy else "dim"] = 0
-        vp_norm = norm_fn(vp, 2, **kw)
-    else:
-        vp_norm = sqrt_fn((weights * (vp**2)).sum(0, **keepdim_kw))
-    if predictions is target:
-        vp_norm_t = transpose_fn(vp_norm)
-        if weights is None:
-            mat = matmul_fn(transpose_fn(vp), vp) / (vp_norm * vp_norm_t)
-        else:
-            mat = matmul_fn(transpose_fn(weights * vp), vp) / (vp_norm * vp_norm_t)
-    else:
-        if weights is None:
-            target_mean = target.mean(0, **keepdim_kw)
-        else:
-            target_mean = (target * weights).sum(0, **keepdim_kw) / w_sum
-        vt = transpose_fn(target - target_mean)
-        if weights is None:
-            kw = keepdim_kw.copy()
-            kw["axis" if is_numpy else "dim"] = 1
-            vt_norm = norm_fn(vt, 2, **kw)
-        else:
-            vt_norm = sqrt_fn((transpose_fn(weights) * (vt**2)).sum(1, **keepdim_kw))
-        if weights is None:
-            mat = matmul_fn(vt, vp) / (vp_norm * vt_norm)
-        else:
-            mat = matmul_fn(vt, weights * vp) / (vp_norm * vt_norm)
-    if not get_diagonal:
-        return mat
-    if mat.shape[0] != mat.shape[1]:
-        raise ValueError(
-            "`get_diagonal` is set to True but the correlation matrix "
-            "is not a squared matrix, which is an invalid condition"
-        )
-    return np.diag(mat) if is_numpy else mat.diag()
-
-
-def interpolant(arr: arr_type) -> arr_type:
-    return arr * arr * arr * (arr * (arr * 6.0 - 15.0) + 10.0)
-
-
-def perlin_noise_2d(
-    shape: Tuple[int, int],
-    periods: Tuple[int, int],
-    should_tile: Tuple[bool, bool] = (False, False),
-    interpolant_fn: Callable[[np.ndarray], np.ndarray] = interpolant,
-) -> np.ndarray:
-    delta = periods[0] / shape[0], periods[1] / shape[1]
-    d = (shape[0] // periods[0], shape[1] // periods[1])
-    grid = np.mgrid[: periods[0] : delta[0], : periods[1] : delta[1]] % 1  # type: ignore
-    grid = grid.transpose(1, 2, 0)
-    # gradients
-    angles = 2 * np.pi * np.random.rand(periods[0] + 1, periods[1] + 1)
-    gradients = np.dstack((np.cos(angles), np.sin(angles)))
-    if should_tile[0]:
-        gradients[-1, :] = gradients[0, :]
-    if should_tile[1]:
-        gradients[:, -1] = gradients[:, 0]
-    gradients = gradients.repeat(d[0], 0).repeat(d[1], 1)
-    g00 = gradients[: -d[0], : -d[1]]
-    g10 = gradients[d[0] :, : -d[1]]
-    g01 = gradients[: -d[0], d[1] :]
-    g11 = gradients[d[0] :, d[1] :]
-    # ramps
-    n00 = np.sum(np.dstack((grid[:, :, 0], grid[:, :, 1])) * g00, 2)
-    n10 = np.sum(np.dstack((grid[:, :, 0] - 1, grid[:, :, 1])) * g10, 2)
-    n01 = np.sum(np.dstack((grid[:, :, 0], grid[:, :, 1] - 1)) * g01, 2)
-    n11 = np.sum(np.dstack((grid[:, :, 0] - 1, grid[:, :, 1] - 1)) * g11, 2)
-    # interpolation
-    arr = interpolant_fn(grid)
-    n0 = n00 * (1 - arr[:, :, 0]) + arr[:, :, 0] * n10
-    n1 = n01 * (1 - arr[:, :, 0]) + arr[:, :, 0] * n11
-    return np.sqrt(2) * ((1 - arr[:, :, 1]) * n0 + arr[:, :, 1] * n1)
-
-
-def fractal_noise_2d(
-    shape: Tuple[int, int],
-    periods: Tuple[int, int],
-    octaves: int = 1,
-    persistence: float = 0.5,
-    lacunarity: int = 2,
-    should_tile: Tuple[bool, bool] = (False, False),
-    interpolant_fn: Callable[[np.ndarray], np.ndarray] = interpolant,
-) -> np.ndarray:
-    noise = np.zeros(shape)
-    frequency = 1
-    amplitude = 1.0
-    for _ in range(octaves):
-        noise += amplitude * perlin_noise_2d(
-            shape,
-            (frequency * periods[0], frequency * periods[1]),
-            should_tile,
-            interpolant_fn,
-        )
-        frequency *= lacunarity
-        amplitude *= persistence
-    return noise
-
-
-def contrast_noise(arr: arr_type) -> arr_type:
-    arr = 0.9998 * arr + 0.0001
-    arr = arr / (1.0 - arr)
-    arr = arr**-2
-    arr = 1.0 / (1.0 + arr)
-    return arr
-
-
-def get_one_hot(feature: Union[list, np.ndarray], dim: int) -> np.ndarray:
-    """
-    Get one-hot representation.
-
-    Parameters
-    ----------
-    feature : array-like, source data of one-hot representation.
-    dim : int, dimension of the one-hot representation.
-
-    Returns
-    -------
-    one_hot : np.ndarray, one-hot representation of `feature`
-
-    """
-
-    one_hot = np.zeros([len(feature), dim], np.int64)
-    one_hot[range(len(one_hot)), np.asarray(feature, np.int64).ravel()] = 1
-    return one_hot
-
-
-def get_indices_from_another(base: np.ndarray, segment: np.ndarray) -> np.ndarray:
-    """
-    Get `segment` elements' indices in `base`.
-
-    Warnings
-    ----------
-    All elements in segment should appear in base to ensure validity.
-
-    Parameters
-    ----------
-    base : np.ndarray, base array.
-    segment : np.ndarray, segment array.
-
-    Returns
-    -------
-    indices : np.ndarray, positions where elements in `segment` appear in `base`
-
-    Examples
-    -------
-    >>> import numpy as np
-    >>> base, segment = np.arange(100), np.random.permutation(100)[:10]
-    >>> assert np.allclose(get_indices_from_another(base, segment), segment)
-
-    """
-    base_sorted_args = np.argsort(base)
-    positions = np.searchsorted(base[base_sorted_args], segment)
-    return base_sorted_args[positions]
-
-
-class UniqueIndices(NamedTuple):
-    """
-    unique           : np.ndarray, unique values of the given array (`arr`).
-    unique_cnt       : np.ndarray, counts of each unique value.
-    sorting_indices  : np.ndarray, indices which can (stably) sort the given
-                                   array by its value.
-    split_arr        : np.ndarray, array which can split the `sorting_indices`
-                                   to make sure that. Each portion of the split
-                                   indices belong & only belong to one of the
-                                   unique values.
-    """
-
-    unique: np.ndarray
-    unique_cnt: np.ndarray
-    sorting_indices: np.ndarray
-    split_arr: np.ndarray
-
-    @property
-    def split_indices(self):
-        return np.split(self.sorting_indices, self.split_arr)
-
-
-def get_unique_indices(arr: np.ndarray) -> UniqueIndices:
-    """
-    Get indices for unique values of an array.
-
-    Parameters
-    ----------
-    arr : np.ndarray, target array which we wish to find indices of each unique value.
-
-    Returns
-    -------
-    UniqueIndices
-
-    Examples
-    -------
-    >>> import numpy as np
-    >>> arr = np.array([1, 2, 3, 2, 4, 1, 0, 1], np.int64)
-    >>> # UniqueIndices(
-    >>> #   unique          = array([0, 1, 2, 3, 4], dtype=int64),
-    >>> #   unique_cnt      = array([1, 3, 2, 1, 1], dtype=int64),
-    >>> #   sorting_indices = array([6, 0, 5, 7, 1, 3, 2, 4], dtype=int64),
-    >>> #   split_arr       = array([1, 4, 6, 7], dtype=int64))
-    >>> #   split_indices   = [array([6], dtype=int64), array([0, 5, 7], dtype=int64),
-    >>> #                      array([1, 3], dtype=int64), array([2], dtype=int64),
-    >>> #                      array([4], dtype=int64)]
-    >>> print(get_unique_indices(arr))
-
-    """
-    unique, unique_inv, unique_cnt = np.unique(
-        arr,
-        return_inverse=True,
-        return_counts=True,
-    )
-    sorting_indices, split_arr = (
-        np.argsort(unique_inv, kind="mergesort"),
-        np.cumsum(unique_cnt)[:-1],
-    )
-    return UniqueIndices(unique, unique_cnt, sorting_indices, split_arr)
-
-
-def get_counter_from_arr(arr: np.ndarray) -> Counter:
-    """
-    Get `Counter` of an array.
-
-    Parameters
-    ----------
-    arr : np.ndarray, target array which we wish to get `Counter` from.
-
-    Returns
-    -------
-    Counter
-
-    Examples
-    -------
-    >>> import numpy as np
-    >>> arr = np.array([1, 2, 3, 2, 4, 1, 0, 1], np.int64)
-    >>> # Counter({1: 3, 2: 2, 0: 1, 3: 1, 4: 1})
-    >>> print(get_counter_from_arr(arr))
-
-    """
-    if isinstance(arr, np.ndarray):
-        arr = dict(zip(*np.unique(arr, return_counts=True)))
-    return Counter(arr)
-
-
-def allclose(*arrays: np.ndarray, **kwargs) -> bool:
-    """
-    Perform `np.allclose` to `arrays` one by one.
-
-    Parameters
-    ----------
-    arrays : np.ndarray, target arrays.
-    **kwargs : keyword arguments which will be passed into `np.allclose`.
-
-    Returns
-    -------
-    allclose : bool
-
-    """
-    for i, arr in enumerate(arrays[:-1]):
-        if not np.allclose(arr, arrays[i + 1], **kwargs):
-            return False
-    return True
-
-
-class StrideArray:
-    def __init__(
-        self,
-        arr: np.ndarray,
-        *,
-        copy: bool = False,
-        writable: Optional[bool] = None,
-    ):
-        self.arr = arr
-        self.shape = arr.shape
-        self.num_dim = len(self.shape)
-        self.strides = arr.strides
-        self.copy = copy
-        if writable is None:
-            writable = copy
-        self.writable = writable
-
-    def __str__(self) -> str:
-        return self.arr.__str__()
-
-    def __repr__(self) -> str:
-        return self.arr.__repr__()
-
-    def _construct(
-        self,
-        shapes: Tuple[int, ...],
-        strides: Tuple[int, ...],
-    ) -> np.ndarray:
-        arr = self.arr.copy() if self.copy else self.arr
-        return as_strided(
-            arr,
-            shape=shapes,
-            strides=strides,
-            writeable=self.writable,
-        )
-
-    @staticmethod
-    def _get_output_dim(in_dim: int, window: int, stride: int) -> int:
-        return (in_dim - window) // stride + 1
-
-    def roll(self, window: int, *, stride: int = 1, axis: int = -1) -> np.ndarray:
-        while axis < 0:
-            axis += self.num_dim
-        target_dim = self.shape[axis]
-        rolled_dim = self._get_output_dim(target_dim, window, stride)
-        if rolled_dim <= 0:
-            msg = f"window ({window}) is too large for target dimension ({target_dim})"
-            raise ValueError(msg)
-        # shapes
-        rolled_shapes = tuple(self.shape[:axis]) + (rolled_dim, window)
-        if axis < self.num_dim - 1:
-            rolled_shapes = rolled_shapes + self.shape[axis + 1 :]
-        # strides
-        previous_strides = tuple(self.strides[:axis])
-        target_stride = (self.strides[axis] * stride,)
-        latter_strides = tuple(self.strides[axis:])
-        rolled_strides = previous_strides + target_stride + latter_strides
-        # construct
-        return self._construct(rolled_shapes, rolled_strides)
-
-    def patch(
-        self,
-        patch_w: int,
-        patch_h: Optional[int] = None,
-        *,
-        h_stride: int = 1,
-        w_stride: int = 1,
-        h_axis: int = -2,
-    ) -> np.ndarray:
-        if self.num_dim < 2:
-            raise ValueError("`patch` requires input with at least 2d")
-        while h_axis < 0:
-            h_axis += self.num_dim
-        w_axis = h_axis + 1
-        if patch_h is None:
-            patch_h = patch_w
-        h_shape, w_shape = self.shape[h_axis], self.shape[w_axis]
-        if h_shape < patch_h:
-            msg = f"patch_h ({patch_h}) is too large for target dimension ({h_shape})"
-            raise ValueError(msg)
-        if w_shape < patch_w:
-            msg = f"patch_w ({patch_w}) is too large for target dimension ({w_shape})"
-            raise ValueError(msg)
-        # shapes
-        patched_h_dim = self._get_output_dim(h_shape, patch_h, h_stride)
-        patched_w_dim = self._get_output_dim(w_shape, patch_w, w_stride)
-        patched_dim = (patched_h_dim, patched_w_dim)
-        patched_dim = patched_dim + (patch_h, patch_w)
-        patched_shapes = tuple(self.shape[:h_axis]) + patched_dim
-        if w_axis < self.num_dim - 1:
-            patched_shapes = patched_shapes + self.shape[w_axis + 1 :]
-        # strides
-        arr_h_stride, arr_w_stride = self.strides[h_axis], self.strides[w_axis]
-        previous_strides = tuple(self.strides[:h_axis])
-        target_stride = (arr_h_stride * h_stride, arr_w_stride * w_stride)
-        target_stride = target_stride + (arr_h_stride, arr_w_stride)
-        latter_strides = tuple(self.strides[w_axis + 1 :])
-        patched_strides = previous_strides + target_stride + latter_strides
-        # construct
-        return self._construct(patched_shapes, patched_strides)
-
-    def repeat(self, k: int, axis: int = -1) -> np.ndarray:
-        while axis < 0:
-            axis += self.num_dim
-        target_dim = self.shape[axis]
-        if target_dim != 1:
-            raise ValueError("`repeat` can only be applied on axis with dim == 1")
-        # shapes
-        repeated_shapes = tuple(self.shape[:axis]) + (k,)
-        if axis < self.num_dim - 1:
-            repeated_shapes = repeated_shapes + self.shape[axis + 1 :]
-        # strides
-        previous_strides = tuple(self.strides[:axis])
-        target_stride = (0,)
-        latter_strides = tuple(self.strides[axis + 1 :])
-        repeated_strides = previous_strides + target_stride + latter_strides
-        # construct
-        return self._construct(repeated_shapes, repeated_strides)
-
-
-class SharedArray:
-    def __init__(
-        self,
-        dtype: Union[type, np.dtype],
-        shape: Union[List[int], Tuple[int, ...]],
-        data: Optional[np.ndarray] = None,
-    ):
-        name = random_hash()
-        d_size = np.dtype(dtype).itemsize * np.prod(shape)
-        self._shm = SharedMemory(create=True, size=d_size, name=name)
-        self.value = np.ndarray(shape=shape, dtype=dtype, buffer=self._shm.buf)
-        if data is not None:
-            self.value[:] = data[:]
-
-    def destroy(self) -> None:
-        self._shm.close()
-        self._shm.unlink()
-
-    @classmethod
-    def from_data(cls, data: np.ndarray) -> "SharedArray":
-        return cls(data.dtype, data.shape, data)
-
-
-def get_label_predictions(logits: np.ndarray, threshold: float) -> np.ndarray:
-    # binary classification
-    if logits.shape[-1] == 2:
-        logits = logits[..., [1]] - logits[..., [0]]
-    if logits.shape[-1] == 1:
-        logit_threshold = math.log(threshold / (1.0 - threshold))
-        return (logits > logit_threshold).astype(int)
-    return logits.argmax(1)[..., None]
-
-
-def get_full_logits(logits: np.ndarray) -> np.ndarray:
-    # binary classification
-    if logits.shape[-1] == 1:
-        logits = np.concatenate([-logits, logits], axis=-1)
-    return logits
-
-
-def make_grid(arr: arr_type, n_row: Optional[int] = None) -> torch.Tensor:
-    if isinstance(arr, np.ndarray):
-        arr = to_torch(arr)
-    if n_row is None:
-        n_row = math.ceil(math.sqrt(len(arr)))
-    return torchvision.utils.make_grid(arr, n_row)
+import math
+
+import numpy as np
+
+from typing import Any
+from typing import Dict
+from typing import List
+from typing import Tuple
+from typing import Union
+from typing import Callable
+from typing import Optional
+from typing import NamedTuple
+from collections import Counter
+from multiprocessing.shared_memory import SharedMemory
+from numpy.lib.stride_tricks import as_strided
+
+from .misc import random_hash
+from .types import torch
+from .types import torchvision
+from .types import F
+from .types import arr_type
+from .types import tensor_dict_type
+
+
+TNormalizeResponse = Union[arr_type, Tuple[arr_type, Dict[str, Any]]]
+
+
+def is_int(arr: np.ndarray) -> bool:
+    return np.issubdtype(arr.dtype, np.integer)
+
+
+def is_float(arr: np.ndarray) -> bool:
+    return np.issubdtype(arr.dtype, np.floating)
+
+
+def is_string(arr: np.ndarray) -> bool:
+    return np.issubdtype(arr.dtype, str)
+
+
+def sigmoid(arr: arr_type) -> arr_type:
+    if isinstance(arr, np.ndarray):
+        return 1.0 / (1.0 + np.exp(-arr))
+    return torch.sigmoid(arr)
+
+
+def softmax(arr: arr_type) -> arr_type:
+    if isinstance(arr, np.ndarray):
+        logits = arr - np.max(arr, axis=1, keepdims=True)
+        exp = np.exp(logits)
+        return exp / exp.sum(1, keepdims=True)
+    return F.softmax(arr, dim=1)
+
+
+def l2_normalize(arr: arr_type) -> arr_type:
+    if isinstance(arr, np.ndarray):
+        return arr / np.linalg.norm(arr, axis=-1, keepdims=True)
+    return arr / arr.norm(dim=-1, keepdim=True)
+
+
+def normalize(
+    arr: arr_type,
+    *,
+    global_norm: bool = True,
+    return_stats: False,
+    eps: float = 1.0e-8,
+) -> TNormalizeResponse:
+    if global_norm:
+        arr_mean, arr_std = arr.mean().item(), arr.std().item()
+        arr_std = max(eps, arr_std)
+        out = (arr - arr_mean) / arr_std
+        if not return_stats:
+            return out
+        return out, dict(mean=arr_mean, std=arr_std)
+    if isinstance(arr, np.ndarray):
+        arr_mean, arr_std = arr.mean(axis=0), arr.std(axis=0)
+        std = np.maximum(eps, arr_std)
+    else:
+        arr_mean, arr_std = arr.mean(dim=0), arr.std(dim=0)
+        std = torch.clip(arr_std, min=eps)
+    out = (arr - arr_mean) / std
+    if not return_stats:
+        return out
+    return out, dict(mean=arr_mean.tolist(), std=std.tolist())
+
+
+def normalize_from(arr: arr_type, stats: Dict[str, Any]) -> arr_type:
+    mean, std = stats["mean"], stats["std"]
+    return (arr - mean) / std
+
+
+def recover_normalize_from(arr: arr_type, stats: Dict[str, Any]) -> arr_type:
+    mean, std = stats["mean"], stats["std"]
+    return arr * std + mean
+
+
+def min_max_normalize(
+    arr: arr_type,
+    *,
+    global_norm: bool = True,
+    return_stats: False,
+    eps: float = 1.0e-8,
+) -> TNormalizeResponse:
+    if global_norm:
+        arr_min, arr_max = arr.min().item(), arr.max().item()
+        diff = max(eps, arr_max - arr_min)
+        out = (arr - arr_min) / diff
+        if not return_stats:
+            return out
+        return out, dict(min=arr_min, diff=diff)
+    if isinstance(arr, np.ndarray):
+        arr_min, arr_max = arr.min(axis=0), arr.max(axis=0)
+        diff = np.maximum(eps, arr_max - arr_min)
+    else:
+        arr_min, arr_max = arr.min(dim=0).values, arr.max(dim=0).values
+        diff = torch.clip(arr_max - arr_min, min=eps)
+    out = (arr - arr_min) / diff
+    if not return_stats:
+        return out
+    return out, dict(min=arr_min.tolist(), diff=diff.tolist())
+
+
+def min_max_normalize_from(arr: arr_type, stats: Dict[str, Any]) -> arr_type:
+    arr_min, diff = stats["min"], stats["diff"]
+    return (arr - arr_min) / diff
+
+
+def recover_min_max_normalize_from(arr: arr_type, stats: Dict[str, Any]) -> arr_type:
+    arr_min, diff = stats["min"], stats["diff"]
+    return arr * diff + arr_min
+
+
+def quantile_normalize(
+    arr: arr_type,
+    *,
+    q: float = 0.01,
+    global_norm: bool = True,
+    return_stats: False,
+    eps: float = 1.0e-8,
+) -> TNormalizeResponse:
+    # quantiles
+    if isinstance(arr, np.ndarray):
+        kw = {"axis": 0}
+        quantile_fn = np.quantile
+    else:
+        kw = {"dim": 0}
+        quantile_fn = torch.quantile
+    if global_norm:
+        arr_min = quantile_fn(arr, q)
+        arr_max = quantile_fn(arr, 1.0 - q)
+    else:
+        arr_min = quantile_fn(arr, q, **kw)
+        arr_max = quantile_fn(arr, 1.0 - q, **kw)
+    # diff
+    if global_norm:
+        diff = max(eps, arr_max - arr_min)
+    else:
+        if isinstance(arr, np.ndarray):
+            diff = np.maximum(eps, arr_max - arr_min)
+        else:
+            diff = torch.clip(arr_max - arr_min, min=eps)
+    arr = arr.clip(arr_min, arr_max)
+    out = (arr - arr_min) / diff
+    if not return_stats:
+        return out
+    if not global_norm:
+        arr_min = arr_min.item()
+        diff = diff.item()
+    else:
+        arr_min = arr_min.tolist()
+        diff = diff.tolist()
+    return out, dict(min=arr_min, diff=diff)
+
+
+def quantile_normalize_from(arr: arr_type, stats: Dict[str, Any]) -> arr_type:
+    arr_min, diff = stats["min"], stats["diff"]
+    return (arr - arr_min) / diff
+
+
+def recover_quantile_normalize_from(arr: arr_type, stats: Dict[str, Any]) -> arr_type:
+    arr_min, diff = stats["min"], stats["diff"]
+    return arr * diff + arr_min
+
+
+def clip_normalize(arr: arr_type) -> arr_type:
+    fn = np if isinstance(arr, np.ndarray) else torch
+    if arr.dtype == fn.uint8:
+        return arr
+    return fn.clip(arr, 0.0, 1.0)
+
+
+# will return at least 2d
+def squeeze(arr: arr_type) -> arr_type:
+    n = arr.shape[0]
+    arr = arr.squeeze()
+    if n == 1:
+        arr = arr[None, ...]
+    return arr
+
+
+def to_standard(arr: np.ndarray) -> np.ndarray:
+    if is_int(arr):
+        arr = arr.astype(np.int64)
+    elif is_float(arr):
+        arr = arr.astype(np.float32)
+    return arr
+
+
+def to_torch(arr: np.ndarray) -> torch.Tensor:
+    return torch.from_numpy(to_standard(arr))
+
+
+def to_numpy(tensor: torch.Tensor) -> np.ndarray:
+    return tensor.detach().cpu().numpy()
+
+
+def to_device(
+    batch: tensor_dict_type,
+    device: torch.device,
+    **kwargs: Any,
+) -> tensor_dict_type:
+    return {
+        k: v.to(device, **kwargs)
+        if isinstance(v, torch.Tensor)
+        else [
+            vv.to(device, **kwargs) if isinstance(vv, torch.Tensor) else vv for vv in v
+        ]
+        if isinstance(v, list)
+        else v
+        for k, v in batch.items()
+    }
+
+
+def iou(logits: arr_type, labels: arr_type) -> arr_type:
+    is_numpy = isinstance(logits, np.ndarray)
+    num_classes = logits.shape[1]
+    if num_classes == 1:
+        heat_map = sigmoid(logits)
+    elif num_classes == 2:
+        heat_map = softmax(logits)[:, [1]]
+    else:
+        raise ValueError("`IOU` only supports binary situations")
+    intersect = heat_map * labels
+    union = heat_map + labels - intersect
+    kwargs = {"axis" if is_numpy else "dim": tuple(range(1, len(intersect.shape)))}
+    return intersect.sum(**kwargs) / union.sum(**kwargs)
+
+
+def corr(
+    predictions: arr_type,
+    target: arr_type,
+    weights: Optional[arr_type] = None,
+    *,
+    get_diagonal: bool = False,
+) -> arr_type:
+    is_numpy = isinstance(predictions, np.ndarray)
+    keepdim_kw = {"keepdims" if is_numpy else "keepdim": True}
+    norm_fn = np.linalg.norm if is_numpy else torch.norm
+    matmul_fn = np.matmul if is_numpy else torch.matmul
+    sqrt_fn = np.sqrt if is_numpy else torch.sqrt
+    transpose_fn = np.transpose if is_numpy else torch.t
+
+    w_sum = 0.0 if weights is None else weights.sum().item()
+    if weights is None:
+        mean = predictions.mean(0, **keepdim_kw)
+    else:
+        mean = (predictions * weights).sum(0, **keepdim_kw) / w_sum
+    vp = predictions - mean
+    if weights is None:
+        kw = keepdim_kw.copy()
+        kw["axis" if is_numpy else "dim"] = 0
+        vp_norm = norm_fn(vp, 2, **kw)
+    else:
+        vp_norm = sqrt_fn((weights * (vp**2)).sum(0, **keepdim_kw))
+    if predictions is target:
+        vp_norm_t = transpose_fn(vp_norm)
+        if weights is None:
+            mat = matmul_fn(transpose_fn(vp), vp) / (vp_norm * vp_norm_t)
+        else:
+            mat = matmul_fn(transpose_fn(weights * vp), vp) / (vp_norm * vp_norm_t)
+    else:
+        if weights is None:
+            target_mean = target.mean(0, **keepdim_kw)
+        else:
+            target_mean = (target * weights).sum(0, **keepdim_kw) / w_sum
+        vt = transpose_fn(target - target_mean)
+        if weights is None:
+            kw = keepdim_kw.copy()
+            kw["axis" if is_numpy else "dim"] = 1
+            vt_norm = norm_fn(vt, 2, **kw)
+        else:
+            vt_norm = sqrt_fn((transpose_fn(weights) * (vt**2)).sum(1, **keepdim_kw))
+        if weights is None:
+            mat = matmul_fn(vt, vp) / (vp_norm * vt_norm)
+        else:
+            mat = matmul_fn(vt, weights * vp) / (vp_norm * vt_norm)
+    if not get_diagonal:
+        return mat
+    if mat.shape[0] != mat.shape[1]:
+        raise ValueError(
+            "`get_diagonal` is set to True but the correlation matrix "
+            "is not a squared matrix, which is an invalid condition"
+        )
+    return np.diag(mat) if is_numpy else mat.diag()
+
+
+def interpolant(arr: arr_type) -> arr_type:
+    return arr * arr * arr * (arr * (arr * 6.0 - 15.0) + 10.0)
+
+
+def perlin_noise_2d(
+    shape: Tuple[int, int],
+    periods: Tuple[int, int],
+    should_tile: Tuple[bool, bool] = (False, False),
+    interpolant_fn: Callable[[np.ndarray], np.ndarray] = interpolant,
+) -> np.ndarray:
+    delta = periods[0] / shape[0], periods[1] / shape[1]
+    d = (shape[0] // periods[0], shape[1] // periods[1])
+    grid = np.mgrid[: periods[0] : delta[0], : periods[1] : delta[1]] % 1  # type: ignore
+    grid = grid.transpose(1, 2, 0)
+    # gradients
+    angles = 2 * np.pi * np.random.rand(periods[0] + 1, periods[1] + 1)
+    gradients = np.dstack((np.cos(angles), np.sin(angles)))
+    if should_tile[0]:
+        gradients[-1, :] = gradients[0, :]
+    if should_tile[1]:
+        gradients[:, -1] = gradients[:, 0]
+    gradients = gradients.repeat(d[0], 0).repeat(d[1], 1)
+    g00 = gradients[: -d[0], : -d[1]]
+    g10 = gradients[d[0] :, : -d[1]]
+    g01 = gradients[: -d[0], d[1] :]
+    g11 = gradients[d[0] :, d[1] :]
+    # ramps
+    n00 = np.sum(np.dstack((grid[:, :, 0], grid[:, :, 1])) * g00, 2)
+    n10 = np.sum(np.dstack((grid[:, :, 0] - 1, grid[:, :, 1])) * g10, 2)
+    n01 = np.sum(np.dstack((grid[:, :, 0], grid[:, :, 1] - 1)) * g01, 2)
+    n11 = np.sum(np.dstack((grid[:, :, 0] - 1, grid[:, :, 1] - 1)) * g11, 2)
+    # interpolation
+    arr = interpolant_fn(grid)
+    n0 = n00 * (1 - arr[:, :, 0]) + arr[:, :, 0] * n10
+    n1 = n01 * (1 - arr[:, :, 0]) + arr[:, :, 0] * n11
+    return np.sqrt(2) * ((1 - arr[:, :, 1]) * n0 + arr[:, :, 1] * n1)
+
+
+def fractal_noise_2d(
+    shape: Tuple[int, int],
+    periods: Tuple[int, int],
+    octaves: int = 1,
+    persistence: float = 0.5,
+    lacunarity: int = 2,
+    should_tile: Tuple[bool, bool] = (False, False),
+    interpolant_fn: Callable[[np.ndarray], np.ndarray] = interpolant,
+) -> np.ndarray:
+    noise = np.zeros(shape)
+    frequency = 1
+    amplitude = 1.0
+    for _ in range(octaves):
+        noise += amplitude * perlin_noise_2d(
+            shape,
+            (frequency * periods[0], frequency * periods[1]),
+            should_tile,
+            interpolant_fn,
+        )
+        frequency *= lacunarity
+        amplitude *= persistence
+    return noise
+
+
+def contrast_noise(arr: arr_type) -> arr_type:
+    arr = 0.9998 * arr + 0.0001
+    arr = arr / (1.0 - arr)
+    arr = arr**-2
+    arr = 1.0 / (1.0 + arr)
+    return arr
+
+
+def get_one_hot(feature: Union[list, np.ndarray], dim: int) -> np.ndarray:
+    """
+    Get one-hot representation.
+
+    Parameters
+    ----------
+    feature : array-like, source data of one-hot representation.
+    dim : int, dimension of the one-hot representation.
+
+    Returns
+    -------
+    one_hot : np.ndarray, one-hot representation of `feature`
+
+    """
+
+    one_hot = np.zeros([len(feature), dim], np.int64)
+    one_hot[range(len(one_hot)), np.asarray(feature, np.int64).ravel()] = 1
+    return one_hot
+
+
+def get_indices_from_another(base: np.ndarray, segment: np.ndarray) -> np.ndarray:
+    """
+    Get `segment` elements' indices in `base`.
+
+    Warnings
+    ----------
+    All elements in segment should appear in base to ensure validity.
+
+    Parameters
+    ----------
+    base : np.ndarray, base array.
+    segment : np.ndarray, segment array.
+
+    Returns
+    -------
+    indices : np.ndarray, positions where elements in `segment` appear in `base`
+
+    Examples
+    -------
+    >>> import numpy as np
+    >>> base, segment = np.arange(100), np.random.permutation(100)[:10]
+    >>> assert np.allclose(get_indices_from_another(base, segment), segment)
+
+    """
+    base_sorted_args = np.argsort(base)
+    positions = np.searchsorted(base[base_sorted_args], segment)
+    return base_sorted_args[positions]
+
+
+class UniqueIndices(NamedTuple):
+    """
+    unique           : np.ndarray, unique values of the given array (`arr`).
+    unique_cnt       : np.ndarray, counts of each unique value.
+    sorting_indices  : np.ndarray, indices which can (stably) sort the given
+                                   array by its value.
+    split_arr        : np.ndarray, array which can split the `sorting_indices`
+                                   to make sure that. Each portion of the split
+                                   indices belong & only belong to one of the
+                                   unique values.
+    """
+
+    unique: np.ndarray
+    unique_cnt: np.ndarray
+    sorting_indices: np.ndarray
+    split_arr: np.ndarray
+
+    @property
+    def split_indices(self):
+        return np.split(self.sorting_indices, self.split_arr)
+
+
+def get_unique_indices(arr: np.ndarray) -> UniqueIndices:
+    """
+    Get indices for unique values of an array.
+
+    Parameters
+    ----------
+    arr : np.ndarray, target array which we wish to find indices of each unique value.
+
+    Returns
+    -------
+    UniqueIndices
+
+    Examples
+    -------
+    >>> import numpy as np
+    >>> arr = np.array([1, 2, 3, 2, 4, 1, 0, 1], np.int64)
+    >>> # UniqueIndices(
+    >>> #   unique          = array([0, 1, 2, 3, 4], dtype=int64),
+    >>> #   unique_cnt      = array([1, 3, 2, 1, 1], dtype=int64),
+    >>> #   sorting_indices = array([6, 0, 5, 7, 1, 3, 2, 4], dtype=int64),
+    >>> #   split_arr       = array([1, 4, 6, 7], dtype=int64))
+    >>> #   split_indices   = [array([6], dtype=int64), array([0, 5, 7], dtype=int64),
+    >>> #                      array([1, 3], dtype=int64), array([2], dtype=int64),
+    >>> #                      array([4], dtype=int64)]
+    >>> print(get_unique_indices(arr))
+
+    """
+    unique, unique_inv, unique_cnt = np.unique(
+        arr,
+        return_inverse=True,
+        return_counts=True,
+    )
+    sorting_indices, split_arr = (
+        np.argsort(unique_inv, kind="mergesort"),
+        np.cumsum(unique_cnt)[:-1],
+    )
+    return UniqueIndices(unique, unique_cnt, sorting_indices, split_arr)
+
+
+def get_counter_from_arr(arr: np.ndarray) -> Counter:
+    """
+    Get `Counter` of an array.
+
+    Parameters
+    ----------
+    arr : np.ndarray, target array which we wish to get `Counter` from.
+
+    Returns
+    -------
+    Counter
+
+    Examples
+    -------
+    >>> import numpy as np
+    >>> arr = np.array([1, 2, 3, 2, 4, 1, 0, 1], np.int64)
+    >>> # Counter({1: 3, 2: 2, 0: 1, 3: 1, 4: 1})
+    >>> print(get_counter_from_arr(arr))
+
+    """
+    if isinstance(arr, np.ndarray):
+        arr = dict(zip(*np.unique(arr, return_counts=True)))
+    return Counter(arr)
+
+
+def allclose(*arrays: np.ndarray, **kwargs) -> bool:
+    """
+    Perform `np.allclose` to `arrays` one by one.
+
+    Parameters
+    ----------
+    arrays : np.ndarray, target arrays.
+    **kwargs : keyword arguments which will be passed into `np.allclose`.
+
+    Returns
+    -------
+    allclose : bool
+
+    """
+    for i, arr in enumerate(arrays[:-1]):
+        if not np.allclose(arr, arrays[i + 1], **kwargs):
+            return False
+    return True
+
+
+class StrideArray:
+    def __init__(
+        self,
+        arr: np.ndarray,
+        *,
+        copy: bool = False,
+        writable: Optional[bool] = None,
+    ):
+        self.arr = arr
+        self.shape = arr.shape
+        self.num_dim = len(self.shape)
+        self.strides = arr.strides
+        self.copy = copy
+        if writable is None:
+            writable = copy
+        self.writable = writable
+
+    def __str__(self) -> str:
+        return self.arr.__str__()
+
+    def __repr__(self) -> str:
+        return self.arr.__repr__()
+
+    def _construct(
+        self,
+        shapes: Tuple[int, ...],
+        strides: Tuple[int, ...],
+    ) -> np.ndarray:
+        arr = self.arr.copy() if self.copy else self.arr
+        return as_strided(
+            arr,
+            shape=shapes,
+            strides=strides,
+            writeable=self.writable,
+        )
+
+    @staticmethod
+    def _get_output_dim(in_dim: int, window: int, stride: int) -> int:
+        return (in_dim - window) // stride + 1
+
+    def roll(self, window: int, *, stride: int = 1, axis: int = -1) -> np.ndarray:
+        while axis < 0:
+            axis += self.num_dim
+        target_dim = self.shape[axis]
+        rolled_dim = self._get_output_dim(target_dim, window, stride)
+        if rolled_dim <= 0:
+            msg = f"window ({window}) is too large for target dimension ({target_dim})"
+            raise ValueError(msg)
+        # shapes
+        rolled_shapes = tuple(self.shape[:axis]) + (rolled_dim, window)
+        if axis < self.num_dim - 1:
+            rolled_shapes = rolled_shapes + self.shape[axis + 1 :]
+        # strides
+        previous_strides = tuple(self.strides[:axis])
+        target_stride = (self.strides[axis] * stride,)
+        latter_strides = tuple(self.strides[axis:])
+        rolled_strides = previous_strides + target_stride + latter_strides
+        # construct
+        return self._construct(rolled_shapes, rolled_strides)
+
+    def patch(
+        self,
+        patch_w: int,
+        patch_h: Optional[int] = None,
+        *,
+        h_stride: int = 1,
+        w_stride: int = 1,
+        h_axis: int = -2,
+    ) -> np.ndarray:
+        if self.num_dim < 2:
+            raise ValueError("`patch` requires input with at least 2d")
+        while h_axis < 0:
+            h_axis += self.num_dim
+        w_axis = h_axis + 1
+        if patch_h is None:
+            patch_h = patch_w
+        h_shape, w_shape = self.shape[h_axis], self.shape[w_axis]
+        if h_shape < patch_h:
+            msg = f"patch_h ({patch_h}) is too large for target dimension ({h_shape})"
+            raise ValueError(msg)
+        if w_shape < patch_w:
+            msg = f"patch_w ({patch_w}) is too large for target dimension ({w_shape})"
+            raise ValueError(msg)
+        # shapes
+        patched_h_dim = self._get_output_dim(h_shape, patch_h, h_stride)
+        patched_w_dim = self._get_output_dim(w_shape, patch_w, w_stride)
+        patched_dim = (patched_h_dim, patched_w_dim)
+        patched_dim = patched_dim + (patch_h, patch_w)
+        patched_shapes = tuple(self.shape[:h_axis]) + patched_dim
+        if w_axis < self.num_dim - 1:
+            patched_shapes = patched_shapes + self.shape[w_axis + 1 :]
+        # strides
+        arr_h_stride, arr_w_stride = self.strides[h_axis], self.strides[w_axis]
+        previous_strides = tuple(self.strides[:h_axis])
+        target_stride = (arr_h_stride * h_stride, arr_w_stride * w_stride)
+        target_stride = target_stride + (arr_h_stride, arr_w_stride)
+        latter_strides = tuple(self.strides[w_axis + 1 :])
+        patched_strides = previous_strides + target_stride + latter_strides
+        # construct
+        return self._construct(patched_shapes, patched_strides)
+
+    def repeat(self, k: int, axis: int = -1) -> np.ndarray:
+        while axis < 0:
+            axis += self.num_dim
+        target_dim = self.shape[axis]
+        if target_dim != 1:
+            raise ValueError("`repeat` can only be applied on axis with dim == 1")
+        # shapes
+        repeated_shapes = tuple(self.shape[:axis]) + (k,)
+        if axis < self.num_dim - 1:
+            repeated_shapes = repeated_shapes + self.shape[axis + 1 :]
+        # strides
+        previous_strides = tuple(self.strides[:axis])
+        target_stride = (0,)
+        latter_strides = tuple(self.strides[axis + 1 :])
+        repeated_strides = previous_strides + target_stride + latter_strides
+        # construct
+        return self._construct(repeated_shapes, repeated_strides)
+
+
+class SharedArray:
+    def __init__(
+        self,
+        dtype: Union[type, np.dtype],
+        shape: Union[List[int], Tuple[int, ...]],
+        data: Optional[np.ndarray] = None,
+    ):
+        name = random_hash()
+        d_size = np.dtype(dtype).itemsize * np.prod(shape)
+        self._shm = SharedMemory(create=True, size=d_size, name=name)
+        self.value = np.ndarray(shape=shape, dtype=dtype, buffer=self._shm.buf)
+        if data is not None:
+            self.value[:] = data[:]
+
+    def destroy(self) -> None:
+        self._shm.close()
+        self._shm.unlink()
+
+    @classmethod
+    def from_data(cls, data: np.ndarray) -> "SharedArray":
+        return cls(data.dtype, data.shape, data)
+
+
+def get_label_predictions(logits: np.ndarray, threshold: float) -> np.ndarray:
+    # binary classification
+    if logits.shape[-1] == 2:
+        logits = logits[..., [1]] - logits[..., [0]]
+    if logits.shape[-1] == 1:
+        logit_threshold = math.log(threshold / (1.0 - threshold))
+        return (logits > logit_threshold).astype(int)
+    return logits.argmax(1)[..., None]
+
+
+def get_full_logits(logits: np.ndarray) -> np.ndarray:
+    # binary classification
+    if logits.shape[-1] == 1:
+        logits = np.concatenate([-logits, logits], axis=-1)
+    return logits
+
+
+def make_grid(arr: arr_type, n_row: Optional[int] = None) -> torch.Tensor:
+    if isinstance(arr, np.ndarray):
+        arr = to_torch(arr)
+    if n_row is None:
+        n_row = math.ceil(math.sqrt(len(arr)))
+    return torchvision.utils.make_grid(arr, n_row)
```

### Comparing `carefree-toolkit-0.3.6.3/cftool/cv.py` & `carefree-toolkit-0.3.6.4/cftool/cv.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,260 +1,260 @@
-import math
-
-import numpy as np
-
-from io import BytesIO
-from abc import abstractmethod
-from numpy import ndarray
-from typing import Any
-from typing import Dict
-from typing import Type
-from typing import Tuple
-from typing import Union
-from typing import Optional
-from typing import NamedTuple
-
-from .misc import safe_execute
-from .misc import shallow_copy_dict
-from .misc import WithRegister
-from .array import torch
-from .array import to_torch
-from .types import arr_type
-from .types import torchvision
-
-try:
-    from PIL import Image
-
-    TImage = Image.Image
-except:
-    Image = None
-    TImage = None
-try:
-    import cv2
-except:
-    cv2 = None
-
-
-padding_modes: Dict[str, Type["Padding"]] = {}
-
-
-class ReadImageResponse(NamedTuple):
-    image: np.ndarray
-    alpha: Optional[np.ndarray]
-    original: TImage
-    original_size: Tuple[int, int]
-
-
-def to_rgb(image: TImage, color: Tuple[int, int, int] = (255, 255, 255)) -> TImage:
-    if image.mode == "CMYK":
-        return image.convert("RGB")
-    split = image.split()
-    if len(split) < 4:
-        return image.convert("RGB")
-    if Image is None:
-        raise ValueError("`pillow` is needed for `to_rgb`")
-    background = Image.new("RGB", image.size, color)
-    background.paste(image, mask=split[3])
-    return background
-
-
-def to_uint8(normalized_img: arr_type) -> arr_type:
-    if isinstance(normalized_img, ndarray):
-        return (np.clip(normalized_img * 255.0, 0.0, 255.0)).astype(np.uint8)
-    return torch.clamp(normalized_img * 255.0, 0.0, 255.0).to(torch.uint8)
-
-
-def np_to_bytes(img_arr: ndarray) -> bytes:
-    if Image is None:
-        raise ValueError("`pillow` is needed for `np_to_bytes`")
-    if img_arr.dtype != np.uint8:
-        img_arr = to_uint8(img_arr)
-    bytes_io = BytesIO()
-    Image.fromarray(img_arr).save(bytes_io, format="PNG")
-    return bytes_io.getvalue()
-
-
-def restrict_wh(w: int, h: int, max_wh: int) -> Tuple[int, int]:
-    max_original_wh = max(w, h)
-    if max_original_wh <= max_wh:
-        return w, h
-    wh_ratio = w / h
-    if wh_ratio >= 1:
-        return max_wh, round(max_wh / wh_ratio)
-    return round(max_wh * wh_ratio), max_wh
-
-
-def get_suitable_size(n: int, anchor: int) -> int:
-    if n <= anchor:
-        return anchor
-    mod = n % anchor
-    return n - mod + int(mod > 0.5 * anchor) * anchor
-
-
-def read_image(
-    image: Union[str, TImage],
-    max_wh: Optional[int],
-    *,
-    anchor: Optional[int],
-    to_gray: bool = False,
-    to_mask: bool = False,
-    resample: Any = Image.LANCZOS,
-    normalize: bool = True,
-    padding_mode: Optional[str] = None,
-    padding_kwargs: Optional[Dict[str, Any]] = None,
-    to_torch_fmt: bool = True,
-) -> ReadImageResponse:
-    if Image is None:
-        raise ValueError("`pillow` is needed for `read_image`")
-    if isinstance(image, str):
-        image = Image.open(image)
-    alpha = None
-    original = image
-    if image.mode == "RGBA":
-        alpha = image.split()[3]
-    if not to_mask and not to_gray:
-        if alpha is None or padding_mode is None:
-            image = to_rgb(image)
-        else:
-            padding = Padding.make(padding_mode, {})
-            padding_kw = shallow_copy_dict(padding_kwargs or {})
-            padding_kw.update(dict(image=image, alpha=alpha))
-            image = safe_execute(padding.pad, padding_kw)
-    else:
-        if to_mask and to_gray:
-            raise ValueError("`to_mask` & `to_gray` should not be True simultaneously")
-        if to_mask and image.mode == "RGBA":
-            image = alpha
-        else:
-            image = image.convert("L")
-    original_w, original_h = image.size
-    if max_wh is None:
-        w, h = original_w, original_h
-    else:
-        w, h = restrict_wh(original_w, original_h, max_wh)
-    if anchor is not None:
-        w, h = map(get_suitable_size, (w, h), (anchor, anchor))
-    image = image.resize((w, h), resample=resample)
-    image = np.array(image)
-    if normalize:
-        image = image.astype(np.float32) / 255.0
-    if alpha is not None:
-        alpha = np.array(alpha)[None, None]
-        if normalize:
-            alpha = alpha.astype(np.float32) / 255.0
-    if to_torch_fmt:
-        if to_mask or to_gray:
-            image = image[None, None]
-        else:
-            image = image[None].transpose(0, 3, 1, 2)
-    return ReadImageResponse(image, alpha, original, (original_w, original_h))
-
-
-def save_images(arr: arr_type, path: str, n_row: Optional[int] = None) -> None:
-    if isinstance(arr, np.ndarray):
-        arr = to_torch(arr)
-    if n_row is None:
-        n_row = math.ceil(math.sqrt(len(arr)))
-    torchvision.utils.save_image(arr, path, normalize=True, nrow=n_row)
-
-
-class ImageProcessor:
-    @staticmethod
-    def _calculate_cdf(histogram: ndarray) -> ndarray:
-        cdf = histogram.cumsum()
-        normalized_cdf = cdf / float(cdf.max())
-        return normalized_cdf
-
-    @staticmethod
-    def _calculate_lookup(source_cdf: ndarray, reference_cdf: ndarray) -> ndarray:
-        lookup_table = np.zeros(256, np.uint8)
-        lookup_val = 0
-        for source_index, source_val in enumerate(source_cdf):
-            for reference_index, reference_val in enumerate(reference_cdf):
-                if reference_val >= source_val:
-                    lookup_val = reference_index
-                    break
-            lookup_table[source_index] = lookup_val
-        return lookup_table
-
-    # accept uint8 inputs
-    @classmethod
-    def match_histograms(
-        cls,
-        source: ndarray,
-        reference: ndarray,
-        mask: Optional[ndarray] = None,
-        *,
-        strength: float = 1.0,
-    ) -> ndarray:
-        if cv2 is None:
-            raise ValueError("`cv2` is needed for `match_histograms`")
-        if strength <= 0.0:
-            return source
-        rev_mask = None if mask is None else ~mask
-        transformed_channels = []
-        for channel in range(source.shape[-1]):
-            source_channel = source[..., channel]
-            reference_channel = reference[..., channel]
-            if mask is None:
-                src_ch = source_channel
-                ref_ch = reference_channel
-            else:
-                src_ch = source_channel[mask]
-                ref_ch = reference_channel[mask]
-            source_hist, _ = np.histogram(src_ch, 256, [0, 256])
-            reference_hist, _ = np.histogram(ref_ch, 256, [0, 256])
-            source_cdf = cls._calculate_cdf(source_hist)
-            reference_cdf = cls._calculate_cdf(reference_hist)
-            lookup = cls._calculate_lookup(source_cdf, reference_cdf)
-            if 0.0 < strength < 1.0:
-                for i, value in enumerate(lookup):
-                    lookup[i] = round(value * strength + i * (1.0 - strength))
-            transformed = cv2.LUT(source_channel, lookup)
-            if rev_mask is not None:
-                transformed[rev_mask] = reference_channel[rev_mask]
-            transformed_channels.append(transformed)
-        return np.stack(transformed_channels, axis=2)
-
-
-class Padding(WithRegister):
-    d = padding_modes
-
-    @abstractmethod
-    def pad(self, image: Image.Image, alpha: Image.Image, **kwargs: Any) -> Image.Image:
-        pass
-
-
-@Padding.register("cv2_ns")
-class CV2NS(Padding):
-    def pad(
-        self,
-        image: Image.Image,
-        alpha: Image.Image,
-        *,
-        radius: int = 5,
-        **kwargs: Any,
-    ) -> Image.Image:
-        if cv2 is None:
-            raise ValueError("`cv2` is needed for `CV2NS`")
-        img_arr = np.array(image.convert("RGB"))[..., ::-1]
-        mask_arr = np.array(alpha)
-        rs = cv2.inpaint(img_arr, 255 - mask_arr, radius, cv2.INPAINT_NS)
-        return Image.fromarray(rs[..., ::-1])
-
-
-@Padding.register("cv2_telea")
-class CV2Telea(Padding):
-    def pad(
-        self,
-        image: Image.Image,
-        alpha: Image.Image,
-        *,
-        radius: int = 5,
-        **kwargs: Any,
-    ) -> Image.Image:
-        if cv2 is None:
-            raise ValueError("`cv2` is needed for `CV2Telea`")
-        img_arr = np.array(image.convert("RGB"))[..., ::-1]
-        mask_arr = np.array(alpha)
-        rs = cv2.inpaint(img_arr, 255 - mask_arr, radius, cv2.INPAINT_TELEA)
-        return Image.fromarray(rs[..., ::-1])
+import math
+
+import numpy as np
+
+from io import BytesIO
+from abc import abstractmethod
+from numpy import ndarray
+from typing import Any
+from typing import Dict
+from typing import Type
+from typing import Tuple
+from typing import Union
+from typing import Optional
+from typing import NamedTuple
+
+from .misc import safe_execute
+from .misc import shallow_copy_dict
+from .misc import WithRegister
+from .array import torch
+from .array import to_torch
+from .types import arr_type
+from .types import torchvision
+
+try:
+    from PIL import Image
+
+    TImage = Image.Image
+except:
+    Image = None
+    TImage = None
+try:
+    import cv2
+except:
+    cv2 = None
+
+
+padding_modes: Dict[str, Type["Padding"]] = {}
+
+
+class ReadImageResponse(NamedTuple):
+    image: np.ndarray
+    alpha: Optional[np.ndarray]
+    original: TImage
+    original_size: Tuple[int, int]
+
+
+def to_rgb(image: TImage, color: Tuple[int, int, int] = (255, 255, 255)) -> TImage:
+    if image.mode == "CMYK":
+        return image.convert("RGB")
+    split = image.split()
+    if len(split) < 4:
+        return image.convert("RGB")
+    if Image is None:
+        raise ValueError("`pillow` is needed for `to_rgb`")
+    background = Image.new("RGB", image.size, color)
+    background.paste(image, mask=split[3])
+    return background
+
+
+def to_uint8(normalized_img: arr_type) -> arr_type:
+    if isinstance(normalized_img, ndarray):
+        return (np.clip(normalized_img * 255.0, 0.0, 255.0)).astype(np.uint8)
+    return torch.clamp(normalized_img * 255.0, 0.0, 255.0).to(torch.uint8)
+
+
+def np_to_bytes(img_arr: ndarray) -> bytes:
+    if Image is None:
+        raise ValueError("`pillow` is needed for `np_to_bytes`")
+    if img_arr.dtype != np.uint8:
+        img_arr = to_uint8(img_arr)
+    bytes_io = BytesIO()
+    Image.fromarray(img_arr).save(bytes_io, format="PNG")
+    return bytes_io.getvalue()
+
+
+def restrict_wh(w: int, h: int, max_wh: int) -> Tuple[int, int]:
+    max_original_wh = max(w, h)
+    if max_original_wh <= max_wh:
+        return w, h
+    wh_ratio = w / h
+    if wh_ratio >= 1:
+        return max_wh, round(max_wh / wh_ratio)
+    return round(max_wh * wh_ratio), max_wh
+
+
+def get_suitable_size(n: int, anchor: int) -> int:
+    if n <= anchor:
+        return anchor
+    mod = n % anchor
+    return n - mod + int(mod > 0.5 * anchor) * anchor
+
+
+def read_image(
+    image: Union[str, TImage],
+    max_wh: Optional[int],
+    *,
+    anchor: Optional[int],
+    to_gray: bool = False,
+    to_mask: bool = False,
+    resample: Any = Image.LANCZOS,
+    normalize: bool = True,
+    padding_mode: Optional[str] = None,
+    padding_kwargs: Optional[Dict[str, Any]] = None,
+    to_torch_fmt: bool = True,
+) -> ReadImageResponse:
+    if Image is None:
+        raise ValueError("`pillow` is needed for `read_image`")
+    if isinstance(image, str):
+        image = Image.open(image)
+    alpha = None
+    original = image
+    if image.mode == "RGBA":
+        alpha = image.split()[3]
+    if not to_mask and not to_gray:
+        if alpha is None or padding_mode is None:
+            image = to_rgb(image)
+        else:
+            padding = Padding.make(padding_mode, {})
+            padding_kw = shallow_copy_dict(padding_kwargs or {})
+            padding_kw.update(dict(image=image, alpha=alpha))
+            image = safe_execute(padding.pad, padding_kw)
+    else:
+        if to_mask and to_gray:
+            raise ValueError("`to_mask` & `to_gray` should not be True simultaneously")
+        if to_mask and image.mode == "RGBA":
+            image = alpha
+        else:
+            image = image.convert("L")
+    original_w, original_h = image.size
+    if max_wh is None:
+        w, h = original_w, original_h
+    else:
+        w, h = restrict_wh(original_w, original_h, max_wh)
+    if anchor is not None:
+        w, h = map(get_suitable_size, (w, h), (anchor, anchor))
+    image = image.resize((w, h), resample=resample)
+    image = np.array(image)
+    if normalize:
+        image = image.astype(np.float32) / 255.0
+    if alpha is not None:
+        alpha = np.array(alpha)[None, None]
+        if normalize:
+            alpha = alpha.astype(np.float32) / 255.0
+    if to_torch_fmt:
+        if to_mask or to_gray:
+            image = image[None, None]
+        else:
+            image = image[None].transpose(0, 3, 1, 2)
+    return ReadImageResponse(image, alpha, original, (original_w, original_h))
+
+
+def save_images(arr: arr_type, path: str, n_row: Optional[int] = None) -> None:
+    if isinstance(arr, np.ndarray):
+        arr = to_torch(arr)
+    if n_row is None:
+        n_row = math.ceil(math.sqrt(len(arr)))
+    torchvision.utils.save_image(arr, path, normalize=True, nrow=n_row)
+
+
+class ImageProcessor:
+    @staticmethod
+    def _calculate_cdf(histogram: ndarray) -> ndarray:
+        cdf = histogram.cumsum()
+        normalized_cdf = cdf / float(cdf.max())
+        return normalized_cdf
+
+    @staticmethod
+    def _calculate_lookup(source_cdf: ndarray, reference_cdf: ndarray) -> ndarray:
+        lookup_table = np.zeros(256, np.uint8)
+        lookup_val = 0
+        for source_index, source_val in enumerate(source_cdf):
+            for reference_index, reference_val in enumerate(reference_cdf):
+                if reference_val >= source_val:
+                    lookup_val = reference_index
+                    break
+            lookup_table[source_index] = lookup_val
+        return lookup_table
+
+    # accept uint8 inputs
+    @classmethod
+    def match_histograms(
+        cls,
+        source: ndarray,
+        reference: ndarray,
+        mask: Optional[ndarray] = None,
+        *,
+        strength: float = 1.0,
+    ) -> ndarray:
+        if cv2 is None:
+            raise ValueError("`cv2` is needed for `match_histograms`")
+        if strength <= 0.0:
+            return source
+        rev_mask = None if mask is None else ~mask
+        transformed_channels = []
+        for channel in range(source.shape[-1]):
+            source_channel = source[..., channel]
+            reference_channel = reference[..., channel]
+            if mask is None:
+                src_ch = source_channel
+                ref_ch = reference_channel
+            else:
+                src_ch = source_channel[mask]
+                ref_ch = reference_channel[mask]
+            source_hist, _ = np.histogram(src_ch, 256, [0, 256])
+            reference_hist, _ = np.histogram(ref_ch, 256, [0, 256])
+            source_cdf = cls._calculate_cdf(source_hist)
+            reference_cdf = cls._calculate_cdf(reference_hist)
+            lookup = cls._calculate_lookup(source_cdf, reference_cdf)
+            if 0.0 < strength < 1.0:
+                for i, value in enumerate(lookup):
+                    lookup[i] = round(value * strength + i * (1.0 - strength))
+            transformed = cv2.LUT(source_channel, lookup)
+            if rev_mask is not None:
+                transformed[rev_mask] = reference_channel[rev_mask]
+            transformed_channels.append(transformed)
+        return np.stack(transformed_channels, axis=2)
+
+
+class Padding(WithRegister):
+    d = padding_modes
+
+    @abstractmethod
+    def pad(self, image: Image.Image, alpha: Image.Image, **kwargs: Any) -> Image.Image:
+        pass
+
+
+@Padding.register("cv2_ns")
+class CV2NS(Padding):
+    def pad(
+        self,
+        image: Image.Image,
+        alpha: Image.Image,
+        *,
+        radius: int = 5,
+        **kwargs: Any,
+    ) -> Image.Image:
+        if cv2 is None:
+            raise ValueError("`cv2` is needed for `CV2NS`")
+        img_arr = np.array(image.convert("RGB"))[..., ::-1]
+        mask_arr = np.array(alpha)
+        rs = cv2.inpaint(img_arr, 255 - mask_arr, radius, cv2.INPAINT_NS)
+        return Image.fromarray(rs[..., ::-1])
+
+
+@Padding.register("cv2_telea")
+class CV2Telea(Padding):
+    def pad(
+        self,
+        image: Image.Image,
+        alpha: Image.Image,
+        *,
+        radius: int = 5,
+        **kwargs: Any,
+    ) -> Image.Image:
+        if cv2 is None:
+            raise ValueError("`cv2` is needed for `CV2Telea`")
+        img_arr = np.array(image.convert("RGB"))[..., ::-1]
+        mask_arr = np.array(alpha)
+        rs = cv2.inpaint(img_arr, 255 - mask_arr, radius, cv2.INPAINT_TELEA)
+        return Image.fromarray(rs[..., ::-1])
```

### Comparing `carefree-toolkit-0.3.6.3/cftool/data_structures.py` & `carefree-toolkit-0.3.6.4/cftool/data_structures.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,511 +1,524 @@
-import io
-import gc
-import time
-
-from typing import Any
-from typing import Set
-from typing import Dict
-from typing import List
-from typing import Type
-from typing import Tuple
-from typing import Union
-from typing import Generic
-from typing import TypeVar
-from typing import Callable
-from typing import Iterator
-from typing import Optional
-from typing import NamedTuple
-from pydantic import Field
-from pydantic import BaseModel
-
-from .misc import print_info
-from .misc import sort_dict_by_value
-from .constants import TIME_FORMAT
-
-try:
-    import networkx as nx
-except:
-    nx = None
-try:
-    import matplotlib.pyplot as plt
-    import matplotlib.patches as mpatches
-except:
-    plt = None
-    mpatches = None
-try:
-    from PIL import Image
-
-    TImage = Image.Image
-except:
-    Image = None
-    TImage = None
-
-
-TItemData = TypeVar("TItemData")
-TTypes = TypeVar("TTypes")
-TItem = TypeVar("TItem")
-
-
-class Item(Generic[TItemData]):
-    def __init__(self, key: str, data: TItemData) -> None:
-        self.key = key
-        self.data = data
-
-
-class Bundle(Generic[TItemData]):
-    def __init__(self, *, no_mapping: bool = False) -> None:
-        """
-        * use mapping is fast at the cost of doubled memory.
-        * for the `queue` use case, mapping is not needed because all operations
-        focus on the first item.
-
-        Details
-        -------
-        * no_mapping = False
-            * get    : O(1)
-            * push   : O(1)
-            * remove : O(1) (if not found) / O(n)
-        * no_mapping = True
-            * get    : O(n)
-            * push   : O(1)
-            * remove : O(n)
-        * `queue` (both cases, so use no_mapping = False to save memory)
-            * get    : O(1)
-            * push   : O(1)
-            * remove : O(1)
-        """
-
-        self._items: List[Item[TItemData]] = []
-        self._mapping: Optional[Dict[str, Item[TItemData]]] = None if no_mapping else {}
-
-    def __len__(self) -> int:
-        return len(self._items)
-
-    def __iter__(self) -> Iterator[Item[TItemData]]:
-        return iter(self._items)
-
-    @property
-    def first(self) -> Optional[Item[TItemData]]:
-        if self.is_empty:
-            return None
-        return self._items[0]
-
-    @property
-    def last(self) -> Optional[Item[TItemData]]:
-        if self.is_empty:
-            return None
-        return self._items[-1]
-
-    @property
-    def is_empty(self) -> bool:
-        return not self._items
-
-    def get(self, key: str) -> Optional[Item[TItemData]]:
-        if self._mapping is not None:
-            return self._mapping.get(key)
-        for item in self._items:
-            if key == item.key:
-                return item
-        return None
-
-    def get_index(self, index: int) -> Item[TItemData]:
-        return self._items[index]
-
-    def push(self, item: Item[TItemData]) -> None:
-        if self.get(item.key) is not None:
-            raise ValueError(f"item '{item.key}' already exists")
-        self._items.append(item)
-        if self._mapping is not None:
-            self._mapping[item.key] = item
-
-    def remove(self, key: str) -> Optional[Item[TItemData]]:
-        if self._mapping is None:
-            for i, item in enumerate(self._items):
-                if key == item.key:
-                    self._items.pop(i)
-                    return item
-            return None
-        item = self._mapping.pop(key, None)  # type: ignore
-        if item is not None:
-            for i, _item in enumerate(self._items):
-                if key == _item.key:
-                    self._items.pop(i)
-                    break
-        return item
-
-
-class QueuesInQueue(Generic[TItemData]):
-    def __init__(self, *, no_mapping: bool = True) -> None:
-        self._cursor = 0
-        self._queues: Bundle[Bundle[TItemData]] = Bundle(no_mapping=no_mapping)
-
-    def __iter__(self) -> Iterator[Item[Bundle[TItemData]]]:
-        return iter(self._queues)
-
-    @property
-    def is_empty(self) -> bool:
-        return self.num_items == 0
-
-    @property
-    def num_queues(self) -> int:
-        return len(self._queues)
-
-    @property
-    def num_items(self) -> int:
-        return sum(len(q.data) for q in self._queues)
-
-    def get(self, queue_id: str) -> Optional[Item[Bundle[TItemData]]]:
-        return self._queues.get(queue_id)
-
-    def push(self, queue_id: str, item: Item[TItemData]) -> None:
-        queue_item = self._queues.get(queue_id)
-        if queue_item is not None:
-            queue = queue_item.data
-        else:
-            queue = Bundle()
-            self._queues.push(Item(queue_id, queue))
-        queue.push(item)
-
-    def next(self) -> Tuple[Optional[str], Optional[Item[TItemData]]]:
-        if self._queues.is_empty:
-            return None, None
-        self._cursor %= len(self._queues)
-        queue = self._queues.get_index(self._cursor)
-        item = queue.data.first
-        if item is None:
-            self._queues.remove(queue.key)
-            return self.next()
-        self._cursor += 1
-        return queue.key, item
-
-    def remove(self, queue_id: str, item_key: str) -> None:
-        queue_item = self._queues.get(queue_id)
-        if queue_item is None:
-            return
-        queue_item.data.remove(item_key)
-        if queue_item.data.is_empty:
-            self._queues.remove(queue_id)
-
-    def get_pending(self, item_key: str) -> Optional[List[Item[TItemData]]]:
-        if self._queues.is_empty:
-            return None
-        layer = 0
-        searched = False
-        pending: List[Item[TItemData]] = []
-        finished_searching = [False] * len(self._queues)
-
-        init = (self._cursor + len(self._queues) - 1) % len(self._queues)
-        cursor = init
-        while not all(finished_searching):
-            if not finished_searching[cursor]:
-                queue = self._queues.get_index(cursor)
-                if layer >= len(queue.data):
-                    finished_searching[cursor] = True
-                else:
-                    item = queue.data.get_index(layer)
-                    if item.key == item_key:
-                        searched = True
-                        break
-                    pending.append(item)
-            cursor = (cursor + 1) % len(self._queues)
-            if cursor == init:
-                layer += 1
-
-        return pending if searched else None
-
-
-class Types(Generic[TTypes]):
-    def __init__(self) -> None:
-        self._types: Dict[str, Type[TTypes]] = {}
-
-    def __iter__(self) -> Iterator[str]:
-        return iter(self._types)
-
-    def __setitem__(self, key: str, value: Type[TTypes]) -> None:
-        self._types[key] = value
-
-    def make(self, key: str, *args: Any, **kwargs: Any) -> Optional[TTypes]:
-        t = self._types.get(key)
-        return None if t is None else t(*args, **kwargs)
-
-    def items(self) -> Iterator[Tuple[str, Type[TTypes]]]:
-        return self._types.items()  # type: ignore
-
-    def values(self) -> Iterator[Type[TTypes]]:
-        return self._types.values()  # type: ignore
-
-
-class ILoadableItem(Generic[TItem]):
-    _item: Optional[TItem]
-
-    def __init__(
-        self,
-        init_fn: Callable[[], TItem],
-        *,
-        init: bool = False,
-        force_keep: bool = False,
-    ):
-        self.init_fn = init_fn
-        self.load_time = time.time()
-        self.force_keep = force_keep
-        self._item = init_fn() if init or force_keep else None
-
-    def load(self, **kwargs: Any) -> TItem:
-        self.load_time = time.time()
-        if self._item is None:
-            self._item = self.init_fn()
-        return self._item
-
-    def unload(self) -> None:
-        self._item = None
-        gc.collect()
-
-
-class ILoadablePool(Generic[TItem]):
-    pool: Dict[str, ILoadableItem]
-    activated: Dict[str, ILoadableItem]
-
-    # set `limit` to negative values to indicate 'no limit'
-    def __init__(self, limit: int = -1):
-        self.pool = {}
-        self.activated = {}
-        self.limit = limit
-        if limit == 0:
-            raise ValueError(
-                "limit should either be negative "
-                "(which indicates 'no limit') or be positive"
-            )
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.pool
-
-    @property
-    def num_activated(self) -> int:
-        return len([v for v in self.activated.values() if not v.force_keep])
-
-    def register(self, key: str, init_fn: Callable[[bool], ILoadableItem]) -> None:
-        if key in self.pool:
-            raise ValueError(f"key '{key}' already exists")
-        init = self.limit < 0 or self.num_activated < self.limit
-        loadable_item = init_fn(init)
-        self.pool[key] = loadable_item
-        if init or loadable_item.force_keep:
-            self.activated[key] = loadable_item
-
-    def get(self, key: str, **kwargs: Any) -> TItem:
-        loadable_item = self.pool.get(key)
-        if loadable_item is None:
-            raise ValueError(f"key '{key}' does not exist")
-        item = loadable_item.load(**kwargs)
-        if key in self.activated:
-            return item
-        load_times = {
-            key: item.load_time
-            for key, item in self.activated.items()
-            if not item.force_keep
-        }
-        print("> activated", self.activated)
-        print("> load_times", load_times)
-        earliest_key = list(sort_dict_by_value(load_times).keys())[0]
-        self.activated.pop(earliest_key).unload()
-        self.activated[key] = loadable_item
-        time_format = "-".join(TIME_FORMAT.split("-")[:-1])
-        print_info(
-            f"'{earliest_key}' is unloaded to make room for '{key}' "
-            f"(last updated: {time.strftime(time_format, time.localtime(loadable_item.load_time))})"
-        )
-        return item
-
-
-class InjectionPack(BaseModel):
-    index: int
-    field: str
-
-
-class WorkNode(BaseModel):
-    key: str = Field(
-        ...,
-        description="Key of the node, should be identical within the same workflow",
-    )
-    endpoint: str = Field(..., description="Algorithm endpoint of the node")
-    injections: Dict[str, Union[InjectionPack, List[InjectionPack]]] = Field(
-        ...,
-        description=(
-            "Injection map, maps 'key' from other `WorkNode` (A) to 'index' of A's results  & "
-            "'field' of the algorithm's field. In runtime, we'll collect "
-            "the (list of) results from the depedencies (other `WorkNode`) and "
-            "inject the specific result (based on 'index') to the algorithm's field.\n"
-            "> If external caches is provided, the 'key' could be the key of the external cache.\n"
-            "> Hierarchy injection is also supported, you just need to set 'field' to:\n"
-            ">> `a.b.c` to inject the result to data['a']['b']['c']\n"
-            ">> `a.0.b` to inject the first result to data['a'][0]['b']\n"
-        ),
-    )
-    data: Dict[str, Any] = Field(..., description="Algorithm's data")
-
-    def to_item(self) -> Item["WorkNode"]:
-        return Item(self.key, self)
-
-
-class ToposortResult(NamedTuple):
-    in_edges: Dict[str, Set[str]]
-    hierarchy: List[List[Item[WorkNode]]]
-    edge_labels: Dict[Tuple[str, str], str]
-
-
-class Workflow(Bundle[WorkNode]):
-    def push(self, node: WorkNode) -> None:
-        return super().push(node.to_item())
-
-    def toposort(self) -> ToposortResult:
-        in_edges = {item.key: set() for item in self}
-        out_degrees = {item.key: 0 for item in self}
-        edge_labels: Dict[Tuple[str, str], str] = {}
-        for item in self:
-            for dep, packs in item.data.injections.items():
-                in_edges[dep].add(item.key)
-                out_degrees[item.key] += 1
-                if not isinstance(packs, list):
-                    packs = [packs]
-                for pack in packs:
-                    label_key = (item.key, dep)
-                    existing_label = edge_labels.get(label_key)
-                    if existing_label is None:
-                        edge_labels[label_key] = pack.field
-                    else:
-                        edge_labels[label_key] = f"{existing_label}, {pack.field}"
-
-        ready = [k for k, v in out_degrees.items() if v == 0]
-        result = []
-        while ready:
-            layer = ready.copy()
-            result.append(layer)
-            ready.clear()
-            for dep in layer:
-                for node in in_edges[dep]:
-                    out_degrees[node] -= 1
-                    if out_degrees[node] == 0:
-                        ready.append(node)
-
-        if len(self) != sum(map(len, result)):
-            raise ValueError("cyclic dependency detected")
-
-        hierarchy = [list(map(self.get, layer)) for layer in result]
-        return ToposortResult(in_edges, hierarchy, edge_labels)
-
-    def get_dependency_path(self, target: str) -> ToposortResult:
-        def dfs(key: str) -> None:
-            if key in reachable:
-                return
-            reachable.add(key)
-            for dep_key in self.get(key).data.injections:
-                dfs(dep_key)
-
-        reachable = set()
-        dfs(target)
-        in_edges, raw_hierarchy, edge_labels = self.toposort()
-        hierarchy = []
-        for raw_layer in raw_hierarchy:
-            layer = []
-            for item in raw_layer:
-                if item.key in reachable:
-                    layer.append(item)
-            if layer:
-                hierarchy.append(layer)
-        return ToposortResult(in_edges, hierarchy, edge_labels)
-
-    def to_json(self) -> List[Dict[str, Any]]:
-        return [node.data.dict() for node in self]
-
-    @classmethod
-    def from_json(cls, data: List[Dict[str, Any]]) -> "Workflow":
-        workflow = cls()
-        for json in data:
-            workflow.push(WorkNode(**json))
-        return workflow
-
-    def render(
-        self,
-        *,
-        target: Optional[str] = None,
-        fig_w_ratio: int = 4,
-        fig_h_ratio: int = 3,
-        dpi: int = 200,
-        node_size: int = 2000,
-        node_shape: str = "s",
-        node_color: str = "lightblue",
-        layout: str = "multipartite_layout",
-    ) -> TImage:
-        if nx is None:
-            raise ValueError("networkx is required for `render`")
-        if plt is None or mpatches is None:
-            raise ValueError("matplotlib is required for `render`")
-        if Image is None:
-            raise ValueError("PIL is required for `render`")
-        # setup graph
-        G = nx.DiGraph()
-        if target is None:
-            target = self.last.key
-        in_edges, hierarchy, edge_labels = self.get_dependency_path(target)
-        # setup plt
-        fig_w = max(fig_w_ratio * len(hierarchy), 8)
-        fig_h = fig_h_ratio * max(map(len, hierarchy))
-        plt.figure(figsize=(fig_w, fig_h), dpi=dpi)
-        box = plt.gca().get_position()
-        plt.gca().set_position([box.x0, box.y0, box.width * 0.8, box.height])
-        # map key to indices
-        key2idx = {}
-        for layer in hierarchy:
-            for node in layer:
-                key2idx[node.key] = len(key2idx)
-        # add nodes
-        for i, layer in enumerate(hierarchy):
-            for node in layer:
-                G.add_node(key2idx[node.key], subset=f"layer_{i}")
-        # add edges
-        for dep, links in in_edges.items():
-            for link in links:
-                if dep not in key2idx or link not in key2idx:
-                    continue
-                label = edge_labels[(link, dep)]
-                G.add_edge(key2idx[dep], key2idx[link], label=label)
-        # calculate positions
-        layout_fn = getattr(nx, layout, None)
-        if layout_fn is None:
-            raise ValueError(f"unknown layout: {layout}")
-        pos = layout_fn(G)
-        # draw the nodes
-        nodes_styles = dict(
-            node_size=node_size,
-            node_shape=node_shape,
-            node_color=node_color,
-        )
-        nx.draw_networkx_nodes(G, pos, **nodes_styles)
-        node_labels_styles = dict(
-            font_size=18,
-        )
-        nx.draw_networkx_labels(G, pos, **node_labels_styles)
-        # draw the edges
-        nx_edge_labels = nx.get_edge_attributes(G, "label")
-        nx.draw_networkx_edges(
-            G,
-            pos,
-            arrows=True,
-            arrowstyle="-|>",
-            arrowsize=16,
-            node_size=nodes_styles["node_size"],
-            node_shape=nodes_styles["node_shape"],
-        )
-        nx.draw_networkx_edge_labels(G, pos, edge_labels=nx_edge_labels)
-        # draw captions
-        patches = [
-            mpatches.Patch(color=node_color, label=f"{idx}: {key}")
-            for key, idx in key2idx.items()
-        ]
-        plt.legend(handles=patches, bbox_to_anchor=(1, 0.5), loc="center left")
-        # render
-        plt.axis("off")
-        buf = io.BytesIO()
-        plt.savefig(buf, format="png")
-        buf.seek(0)
-        return Image.open(buf)
+import io
+import gc
+import time
+
+from typing import Any
+from typing import Set
+from typing import Dict
+from typing import List
+from typing import Type
+from typing import Tuple
+from typing import Union
+from typing import Generic
+from typing import TypeVar
+from typing import Callable
+from typing import Iterator
+from typing import Optional
+from typing import NamedTuple
+from pydantic import Field
+from pydantic import BaseModel
+
+from .misc import print_info
+from .misc import sort_dict_by_value
+from .constants import TIME_FORMAT
+
+try:
+    import networkx as nx
+except:
+    nx = None
+try:
+    import matplotlib.pyplot as plt
+    import matplotlib.patches as mpatches
+except:
+    plt = None
+    mpatches = None
+try:
+    from PIL import Image
+
+    TImage = Image.Image
+except:
+    Image = None
+    TImage = None
+
+
+TItemData = TypeVar("TItemData")
+TTypes = TypeVar("TTypes")
+TItem = TypeVar("TItem")
+
+
+class Item(Generic[TItemData]):
+    def __init__(self, key: str, data: TItemData) -> None:
+        self.key = key
+        self.data = data
+
+
+class Bundle(Generic[TItemData]):
+    def __init__(self, *, no_mapping: bool = False) -> None:
+        """
+        * use mapping is fast at the cost of doubled memory.
+        * for the `queue` use case, mapping is not needed because all operations
+        focus on the first item.
+
+        Details
+        -------
+        * no_mapping = False
+            * get    : O(1)
+            * push   : O(1)
+            * remove : O(1) (if not found) / O(n)
+        * no_mapping = True
+            * get    : O(n)
+            * push   : O(1)
+            * remove : O(n)
+        * `queue` (both cases, so use no_mapping = False to save memory)
+            * get    : O(1)
+            * push   : O(1)
+            * remove : O(1)
+        """
+
+        self._items: List[Item[TItemData]] = []
+        self._mapping: Optional[Dict[str, Item[TItemData]]] = None if no_mapping else {}
+
+    def __len__(self) -> int:
+        return len(self._items)
+
+    def __iter__(self) -> Iterator[Item[TItemData]]:
+        return iter(self._items)
+
+    @property
+    def first(self) -> Optional[Item[TItemData]]:
+        if self.is_empty:
+            return None
+        return self._items[0]
+
+    @property
+    def last(self) -> Optional[Item[TItemData]]:
+        if self.is_empty:
+            return None
+        return self._items[-1]
+
+    @property
+    def is_empty(self) -> bool:
+        return not self._items
+
+    def get(self, key: str) -> Optional[Item[TItemData]]:
+        if self._mapping is not None:
+            return self._mapping.get(key)
+        for item in self._items:
+            if key == item.key:
+                return item
+        return None
+
+    def get_index(self, index: int) -> Item[TItemData]:
+        return self._items[index]
+
+    def push(self, item: Item[TItemData]) -> None:
+        if self.get(item.key) is not None:
+            raise ValueError(f"item '{item.key}' already exists")
+        self._items.append(item)
+        if self._mapping is not None:
+            self._mapping[item.key] = item
+
+    def remove(self, key: str) -> Optional[Item[TItemData]]:
+        if self._mapping is None:
+            for i, item in enumerate(self._items):
+                if key == item.key:
+                    self._items.pop(i)
+                    return item
+            return None
+        item = self._mapping.pop(key, None)  # type: ignore
+        if item is not None:
+            for i, _item in enumerate(self._items):
+                if key == _item.key:
+                    self._items.pop(i)
+                    break
+        return item
+
+
+class QueuesInQueue(Generic[TItemData]):
+    def __init__(self, *, no_mapping: bool = True) -> None:
+        self._cursor = 0
+        self._queues: Bundle[Bundle[TItemData]] = Bundle(no_mapping=no_mapping)
+
+    def __iter__(self) -> Iterator[Item[Bundle[TItemData]]]:
+        return iter(self._queues)
+
+    @property
+    def is_empty(self) -> bool:
+        return self.num_items == 0
+
+    @property
+    def num_queues(self) -> int:
+        return len(self._queues)
+
+    @property
+    def num_items(self) -> int:
+        return sum(len(q.data) for q in self._queues)
+
+    def get(self, queue_id: str) -> Optional[Item[Bundle[TItemData]]]:
+        return self._queues.get(queue_id)
+
+    def push(self, queue_id: str, item: Item[TItemData]) -> None:
+        queue_item = self._queues.get(queue_id)
+        if queue_item is not None:
+            queue = queue_item.data
+        else:
+            queue = Bundle()
+            self._queues.push(Item(queue_id, queue))
+        queue.push(item)
+
+    def next(self) -> Tuple[Optional[str], Optional[Item[TItemData]]]:
+        if self._queues.is_empty:
+            return None, None
+        self._cursor %= len(self._queues)
+        queue = self._queues.get_index(self._cursor)
+        item = queue.data.first
+        if item is None:
+            self._queues.remove(queue.key)
+            return self.next()
+        self._cursor += 1
+        return queue.key, item
+
+    def remove(self, queue_id: str, item_key: str) -> None:
+        queue_item = self._queues.get(queue_id)
+        if queue_item is None:
+            return
+        queue_item.data.remove(item_key)
+        if queue_item.data.is_empty:
+            self._queues.remove(queue_id)
+
+    def get_pending(self, item_key: str) -> Optional[List[Item[TItemData]]]:
+        if self._queues.is_empty:
+            return None
+        layer = 0
+        searched = False
+        pending: List[Item[TItemData]] = []
+        finished_searching = [False] * len(self._queues)
+
+        init = (self._cursor + len(self._queues) - 1) % len(self._queues)
+        cursor = init
+        while not all(finished_searching):
+            if not finished_searching[cursor]:
+                queue = self._queues.get_index(cursor)
+                if layer >= len(queue.data):
+                    finished_searching[cursor] = True
+                else:
+                    item = queue.data.get_index(layer)
+                    if item.key == item_key:
+                        searched = True
+                        break
+                    pending.append(item)
+            cursor = (cursor + 1) % len(self._queues)
+            if cursor == init:
+                layer += 1
+
+        return pending if searched else None
+
+
+class Types(Generic[TTypes]):
+    def __init__(self) -> None:
+        self._types: Dict[str, Type[TTypes]] = {}
+
+    def __iter__(self) -> Iterator[str]:
+        return iter(self._types)
+
+    def __setitem__(self, key: str, value: Type[TTypes]) -> None:
+        self._types[key] = value
+
+    def make(self, key: str, *args: Any, **kwargs: Any) -> Optional[TTypes]:
+        t = self._types.get(key)
+        return None if t is None else t(*args, **kwargs)
+
+    def items(self) -> Iterator[Tuple[str, Type[TTypes]]]:
+        return self._types.items()  # type: ignore
+
+    def values(self) -> Iterator[Type[TTypes]]:
+        return self._types.values()  # type: ignore
+
+
+class ILoadableItem(Generic[TItem]):
+    _item: Optional[TItem]
+
+    def __init__(
+        self,
+        init_fn: Callable[[], TItem],
+        *,
+        init: bool = False,
+        force_keep: bool = False,
+    ):
+        self.init_fn = init_fn
+        self.load_time = time.time()
+        self.force_keep = force_keep
+        self._item = init_fn() if init or force_keep else None
+
+    def load(self, **kwargs: Any) -> TItem:
+        self.load_time = time.time()
+        if self._item is None:
+            self._item = self.init_fn()
+        return self._item
+
+    def unload(self) -> None:
+        self._item = None
+        gc.collect()
+
+
+class ILoadablePool(Generic[TItem]):
+    pool: Dict[str, ILoadableItem]
+    activated: Dict[str, ILoadableItem]
+
+    # set `limit` to negative values to indicate 'no limit'
+    def __init__(self, limit: int = -1):
+        self.pool = {}
+        self.activated = {}
+        self.limit = limit
+        if limit == 0:
+            raise ValueError(
+                "limit should either be negative "
+                "(which indicates 'no limit') or be positive"
+            )
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.pool
+
+    @property
+    def num_activated(self) -> int:
+        return len([v for v in self.activated.values() if not v.force_keep])
+
+    def register(self, key: str, init_fn: Callable[[bool], ILoadableItem]) -> None:
+        if key in self.pool:
+            raise ValueError(f"key '{key}' already exists")
+        init = self.limit < 0 or self.num_activated < self.limit
+        loadable_item = init_fn(init)
+        self.pool[key] = loadable_item
+        if init or loadable_item.force_keep:
+            self.activated[key] = loadable_item
+
+    def get(self, key: str, **kwargs: Any) -> TItem:
+        loadable_item = self.pool.get(key)
+        if loadable_item is None:
+            raise ValueError(f"key '{key}' does not exist")
+        item = loadable_item.load(**kwargs)
+        if key in self.activated:
+            return item
+        load_times = {
+            key: item.load_time
+            for key, item in self.activated.items()
+            if not item.force_keep
+        }
+        print("> activated", self.activated)
+        print("> load_times", load_times)
+        earliest_key = list(sort_dict_by_value(load_times).keys())[0]
+        self.activated.pop(earliest_key).unload()
+        self.activated[key] = loadable_item
+        time_format = "-".join(TIME_FORMAT.split("-")[:-1])
+        print_info(
+            f"'{earliest_key}' is unloaded to make room for '{key}' "
+            f"(last updated: {time.strftime(time_format, time.localtime(loadable_item.load_time))})"
+        )
+        return item
+
+
+class InjectionPack(BaseModel):
+    index: int
+    field: str
+
+
+class WorkNode(BaseModel):
+    key: str = Field(
+        ...,
+        description="Key of the node, should be identical within the same workflow",
+    )
+    endpoint: str = Field(..., description="Algorithm endpoint of the node")
+    injections: Dict[str, Union[InjectionPack, List[InjectionPack]]] = Field(
+        ...,
+        description=(
+            "Injection map, maps 'key' from other `WorkNode` (A) to 'index' of A's results  & "
+            "'field' of the algorithm's field. In runtime, we'll collect "
+            "the (list of) results from the depedencies (other `WorkNode`) and "
+            "inject the specific result (based on 'index') to the algorithm's field.\n"
+            "> If external caches is provided, the 'key' could be the key of the external cache.\n"
+            "> Hierarchy injection is also supported, you just need to set 'field' to:\n"
+            ">> `a.b.c` to inject the result to data['a']['b']['c']\n"
+            ">> `a.0.b` to inject the first result to data['a'][0]['b']\n"
+        ),
+    )
+    data: Dict[str, Any] = Field(..., description="Algorithm's data")
+
+    def to_item(self) -> Item["WorkNode"]:
+        return Item(self.key, self)
+
+
+class ToposortResult(NamedTuple):
+    in_edges: Dict[str, Set[str]]
+    hierarchy: List[List[Item[WorkNode]]]
+    edge_labels: Dict[Tuple[str, str], str]
+
+
+class Workflow(Bundle[WorkNode]):
+    def copy(self) -> "Workflow":
+        return Workflow.from_json(self.to_json())
+
+    def push(self, node: WorkNode) -> None:
+        return super().push(node.to_item())
+
+    def toposort(self) -> ToposortResult:
+        in_edges = {item.key: set() for item in self}
+        out_degrees = {item.key: 0 for item in self}
+        edge_labels: Dict[Tuple[str, str], str] = {}
+        for item in self:
+            for dep, packs in item.data.injections.items():
+                in_edges[dep].add(item.key)
+                out_degrees[item.key] += 1
+                if not isinstance(packs, list):
+                    packs = [packs]
+                for pack in packs:
+                    label_key = (item.key, dep)
+                    existing_label = edge_labels.get(label_key)
+                    if existing_label is None:
+                        edge_labels[label_key] = pack.field
+                    else:
+                        edge_labels[label_key] = f"{existing_label}, {pack.field}"
+
+        ready = [k for k, v in out_degrees.items() if v == 0]
+        result = []
+        while ready:
+            layer = ready.copy()
+            result.append(layer)
+            ready.clear()
+            for dep in layer:
+                for node in in_edges[dep]:
+                    out_degrees[node] -= 1
+                    if out_degrees[node] == 0:
+                        ready.append(node)
+
+        if len(self) != sum(map(len, result)):
+            raise ValueError("cyclic dependency detected")
+
+        hierarchy = [list(map(self.get, layer)) for layer in result]
+        return ToposortResult(in_edges, hierarchy, edge_labels)
+
+    def get_dependency_path(self, target: str) -> ToposortResult:
+        def dfs(key: str) -> None:
+            if key in reachable:
+                return
+            reachable.add(key)
+            for dep_key in self.get(key).data.injections:
+                dfs(dep_key)
+
+        reachable = set()
+        dfs(target)
+        in_edges, raw_hierarchy, edge_labels = self.toposort()
+        hierarchy = []
+        for raw_layer in raw_hierarchy:
+            layer = []
+            for item in raw_layer:
+                if item.key in reachable:
+                    layer.append(item)
+            if layer:
+                hierarchy.append(layer)
+        return ToposortResult(in_edges, hierarchy, edge_labels)
+
+    def to_json(self) -> List[Dict[str, Any]]:
+        return [node.data.dict() for node in self]
+
+    @classmethod
+    def from_json(cls, data: List[Dict[str, Any]]) -> "Workflow":
+        workflow = cls()
+        for json in data:
+            workflow.push(WorkNode(**json))
+        return workflow
+
+    def inject_caches(self, caches: Dict[str, Any]) -> "Workflow":
+        for k in caches:
+            self.push(WorkNode(key=k, endpoint="", injections={}, data={}))
+        return self
+
+    def render(
+        self,
+        *,
+        target: Optional[str] = None,
+        caches: Optional[Dict[str, Any]] = None,
+        fig_w_ratio: int = 4,
+        fig_h_ratio: int = 3,
+        dpi: int = 200,
+        node_size: int = 2000,
+        node_shape: str = "s",
+        node_color: str = "lightblue",
+        layout: str = "multipartite_layout",
+    ) -> TImage:
+        if nx is None:
+            raise ValueError("networkx is required for `render`")
+        if plt is None or mpatches is None:
+            raise ValueError("matplotlib is required for `render`")
+        if Image is None:
+            raise ValueError("PIL is required for `render`")
+        # setup workflow
+        workflow = self.copy()
+        if caches is not None:
+            workflow.inject_caches(caches)
+        # setup graph
+        G = nx.DiGraph()
+        if target is None:
+            target = self.last.key
+        in_edges, hierarchy, edge_labels = workflow.get_dependency_path(target)
+        # setup plt
+        fig_w = max(fig_w_ratio * len(hierarchy), 8)
+        fig_h = fig_h_ratio * max(map(len, hierarchy))
+        plt.figure(figsize=(fig_w, fig_h), dpi=dpi)
+        box = plt.gca().get_position()
+        plt.gca().set_position([box.x0, box.y0, box.width * 0.8, box.height])
+        # map key to indices
+        key2idx = {}
+        for layer in hierarchy:
+            for node in layer:
+                key2idx[node.key] = len(key2idx)
+        # add nodes
+        for i, layer in enumerate(hierarchy):
+            for node in layer:
+                G.add_node(key2idx[node.key], subset=f"layer_{i}")
+        # add edges
+        for dep, links in in_edges.items():
+            for link in links:
+                if dep not in key2idx or link not in key2idx:
+                    continue
+                label = edge_labels[(link, dep)]
+                G.add_edge(key2idx[dep], key2idx[link], label=label)
+        # calculate positions
+        layout_fn = getattr(nx, layout, None)
+        if layout_fn is None:
+            raise ValueError(f"unknown layout: {layout}")
+        pos = layout_fn(G)
+        # draw the nodes
+        nodes_styles = dict(
+            node_size=node_size,
+            node_shape=node_shape,
+            node_color=node_color,
+        )
+        nx.draw_networkx_nodes(G, pos, **nodes_styles)
+        node_labels_styles = dict(
+            font_size=18,
+        )
+        nx.draw_networkx_labels(G, pos, **node_labels_styles)
+        # draw the edges
+        nx_edge_labels = nx.get_edge_attributes(G, "label")
+        nx.draw_networkx_edges(
+            G,
+            pos,
+            arrows=True,
+            arrowstyle="-|>",
+            arrowsize=16,
+            node_size=nodes_styles["node_size"],
+            node_shape=nodes_styles["node_shape"],
+        )
+        nx.draw_networkx_edge_labels(G, pos, edge_labels=nx_edge_labels)
+        # draw captions
+        patches = [
+            mpatches.Patch(color=node_color, label=f"{idx}: {key}")
+            for key, idx in key2idx.items()
+        ]
+        plt.legend(handles=patches, bbox_to_anchor=(1, 0.5), loc="center left")
+        # render
+        plt.axis("off")
+        buf = io.BytesIO()
+        plt.savefig(buf, format="png")
+        buf.seek(0)
+        return Image.open(buf)
```

### Comparing `carefree-toolkit-0.3.6.3/cftool/dist/core.py` & `carefree-toolkit-0.3.6.4/cftool/dist/core.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,542 +1,542 @@
-import os
-import dill
-import time
-import pprint
-import random
-import signal
-import inspect
-import logging
-import platform
-
-from tqdm import tqdm
-from typing import Any
-from typing import Dict
-from typing import List
-from typing import Tuple
-from typing import Union
-from typing import Optional
-from typing import Callable
-from pathos.pools import ProcessPool
-from multiprocessing import Process
-from multiprocessing.managers import SyncManager
-
-from ..misc import timestamp
-from ..misc import grouped_into
-from ..misc import print_warning
-from ..misc import LoggingMixin
-from ..misc import PureLoggingMixin
-from ..manage import PCManager
-from ..manage import GPUManager
-from ..manage import ResourceManager
-
-
-LINUX = platform.system() == "Linux"
-dill._dill._reverse_typemap["ClassType"] = type
-
-
-class Parallel(PureLoggingMixin):
-    """
-    Util class which can help running tasks in parallel.
-
-    Warnings
-    ----------
-        On platforms other than Linux, functions are dramatically reduced because
-        only Linux system well supports pickling. In this occasion, `Parallel`
-        will simply leverage `pathos` to do the jobs.
-
-    Parameters
-    ----------
-    num_jobs : int, number of jobs run in parallel.
-    sleep : float, idle duration of new jobs.
-    use_tqdm: bool, whether show progress bar (with tqdm) or not.
-    use_cuda: bool, whether tasks need CUDA or not.
-    name : str, summary name of these tasks.
-    meta_name : str, name of the meta information.
-    logging_folder : str, where the logging will be placed.
-    task_names : List[str], names of each task.
-    resource_config : Dict[str, Any], config used in `ResourceManager`.
-
-    Examples
-    ----------
-    >>> def add_one(x):
-    >>>     import time
-    >>>     time.sleep(1)
-    >>>     return x + 1
-    >>>
-    >>> print(Parallel(10)(add_one, list(range(10))).parallel_results)
-
-    """
-
-    class _ParallelError(Exception):
-        pass
-
-    def __init__(
-        self,
-        num_jobs: int,
-        *,
-        sleep: float = 1.0,
-        use_tqdm: bool = True,
-        use_cuda: bool = False,
-        name: Optional[str] = None,
-        meta_name: Optional[str] = None,
-        logging_folder: Optional[str] = None,
-        task_names: Optional[List[str]] = None,
-        tqdm_config: Optional[Dict[str, Any]] = None,
-        resource_config: Optional[Dict[str, Any]] = None,
-        warn_num_jobs: bool = True,
-    ):
-        self._rs = None
-        self._use_tqdm, self._use_cuda = use_tqdm, use_cuda
-        self._num_jobs, self._sleep = num_jobs, sleep
-        if tqdm_config is None:
-            tqdm_config = {}
-        if resource_config is None:
-            resource_config = {}
-        if logging_folder is None:
-            logging_folder = os.path.join(os.getcwd(), "_parallel_", "logs")
-        self._tqdm_config = tqdm_config
-        self._resource_config = resource_config
-        self._name, self._meta_name = name, meta_name
-        self._logging_folder, self._task_names = logging_folder, task_names
-        self._refresh_patience = resource_config.setdefault("refresh_patience", 10)
-        self._init_logger(self.meta_log_name)
-        self._warn_num_jobs = warn_num_jobs
-
-    def __call__(self, f: Callable, *args_list: Any) -> "Parallel":
-        # if f returns a dict with 'terminate' key, Parallel can be terminated at
-        # early stage by setting 'terminate' key to True
-        n_tasks = len(args_list[0])
-        n_jobs = min(self._num_jobs, n_tasks)
-        if self._task_names is None:
-            self._task_names = [None] * n_tasks
-        if not LINUX or n_jobs <= 1:
-            if LINUX and self._warn_num_jobs:
-                print_warning(
-                    "Detected Linux system but "
-                    f"n_jobs={n_jobs}, functions will be dramatically reduced.\n"
-                    "* It is recommended to set n_jobs to a larger value"
-                )
-            results = []
-            task_names = list(map(self._get_task_name, range(n_tasks)))
-            if n_jobs <= 1:
-                iterator = (f(*args) for args in zip(*args_list))
-            else:
-                p = ProcessPool(ncpus=n_jobs)
-                iterator = p.imap(f, *args_list)
-            if self._use_tqdm:
-                iterator = tqdm(iterator, total=n_tasks, **self._tqdm_config)
-            for result in iterator:
-                results.append(result)
-            self._rs = dict(zip(task_names, results))
-            return self
-        self._func, self._args_list = f, args_list
-        self._cursor, self._all_task_indices = 0, list(range(n_jobs, n_tasks))
-        self._log_meta_msg("initializing sync manager")
-        self._sync_manager = SyncManager()
-        self._sync_manager.start(lambda: signal.signal(signal.SIGINT, signal.SIG_IGN))
-        meta = {"n_jobs": n_jobs, "n_tasks": n_tasks, "terminated": False}
-        self._rs = self._sync_manager.dict(
-            {
-                "__meta__": meta,
-                "__exceptions__": {},
-            }
-        )
-        self._overwritten_task_info = {}
-        self._pid2task_idx = None
-        self._log_meta_msg("initializing resource manager")
-        self._resource_manager = ResourceManager(
-            self._resource_config, self._get_task_name, self._refresh_patience
-        )
-        self._log_meta_msg("registering PC manager")
-        pc_manager = PCManager()
-        ram_methods = {
-            "get_pid_usage_dict": None,
-            "get_pid_usage": pc_manager.get_pid_ram_usage,
-            "get_available_dict": lambda: {"total": pc_manager.get_available_ram()},
-        }
-        self._resource_manager.register("RAM", ram_methods)
-        gpu_config = self._resource_config.setdefault("gpu_config", {})
-        default_cuda_list = None if self._use_cuda else []
-        available_cuda_list = gpu_config.setdefault(
-            "available_cuda_list", default_cuda_list
-        )
-        if available_cuda_list is None or available_cuda_list:
-            self._log_meta_msg("registering GPU manager")
-            if available_cuda_list is not None:
-                available_cuda_list = list(map(int, available_cuda_list))
-            gpu_manager = GPUManager(available_cuda_list)
-            gpu_methods = {
-                "get_pid_usage": None,
-                "get_pid_usage_dict": gpu_manager.get_pid_usages,
-                "get_available_dict": gpu_manager.get_gpu_frees,
-            }
-            self._resource_manager.register("GPU", gpu_methods)
-        self._resource_manager.register_logging(self._init_logger, self)
-        self._log_meta_msg("initializing with refreshing")
-        self._refresh(skip_check_finished=True)
-        self._working_processes = None
-        if not self._use_tqdm:
-            self._tqdm_bar = None
-        else:
-            self._tqdm_bar = tqdm(list(range(n_tasks)), **self._tqdm_config)
-        try:
-            self._log_meta_msg("initializing processes")
-            init_task_indices = list(range(n_jobs))
-            init_processes = [
-                self._get_process(i, start=False) for i in init_task_indices
-            ]
-            if self.terminated:
-                self._user_terminate()
-            init_failed_slots, init_failed_task_indices = [], []
-            for i, (task_idx, process) in enumerate(
-                zip(init_task_indices, init_processes)
-            ):
-                if process is None:
-                    init_failed_slots.append(i)
-                    init_failed_task_indices.append(task_idx)
-                    task_name = self._get_task_name(task_idx)
-                    self._log_with_meta(
-                        task_name,
-                        "initialization failed, it may due to lack of resources",
-                        msg_level=logging.WARNING,
-                    )
-            if init_failed_slots:
-                for slot in init_failed_slots:
-                    init_task_indices[slot] = None
-                    init_processes[slot] = [None] * 4
-                self._all_task_indices = (
-                    init_failed_task_indices + self._all_task_indices
-                )
-            self._working_task_indices = init_task_indices
-            self._working_processes, task_info = map(list, zip(*init_processes))
-            self._log_meta_msg("starting all initial processes")
-            tuple(
-                map(
-                    lambda p_: None if p_ is None else p_.start(),
-                    self._working_processes,
-                )
-            )
-            tuple(
-                map(
-                    self._record_process,
-                    self._working_task_indices,
-                    self._working_processes,
-                    task_info,
-                )
-            )
-            self._resource_manager.initialize_running_usages()
-            self._log_meta_msg("entering parallel main loop")
-            while True:
-                self._log_meta_msg("waiting for finished slot")
-                self._wait_and_handle_finish(wait_until_finish=True)
-                if not self._add_new_processes():
-                    break
-        except KeyboardInterrupt:
-            self.exception(self.meta_log_name, f"keyboard interrupted")
-            exceptions = self.exceptions
-            exceptions["base"] = self._ParallelError("Keyboard Interrupted")
-            self._rs["__exceptions__"] = exceptions
-        except Exception as err:
-            self.exception(self.meta_log_name, f"exception occurred, {err}")
-            exceptions = self.exceptions
-            exceptions["base"] = err
-            self._rs["__exceptions__"] = exceptions
-        finally:
-            self._log_meta_msg("joining processes left behind")
-            if self._working_processes is not None:
-                for process in self._working_processes:
-                    if process is None:
-                        continue
-                    process.join()
-            if self._tqdm_bar is not None:
-                self._tqdm_bar.close()
-            self._log_meta_msg("casting parallel results to Python dict")
-            self._rs = dict(self._rs)
-            self._log_meta_msg("shutting down sync manager")
-            self._sync_manager.shutdown()
-            self.log_block_msg(
-                self.meta_log_name,
-                "parallel results",
-                pprint.pformat(self._rs, compact=True),
-            )
-        return self
-
-    def grouped(self, f: Callable, *args_list: Any) -> "Parallel":
-        num_jobs = min(len(args_list[0]), self._num_jobs)
-        grouped_args_list = [grouped_into(args, num_jobs) for args in args_list]
-
-        def _grouped_f(i: int, *args_list_: Tuple[Any], cuda: Any = None) -> List[Any]:
-            results: List[Any] = []
-            kwargs = {} if not self._use_cuda else {"cuda": cuda}
-            for args in tqdm(
-                zip(*args_list_),
-                total=len(args_list_[0]),
-                position=i + 1,
-                leave=False,
-            ):
-                results.append(f(*args, **kwargs))
-            return results
-
-        return self(_grouped_f, list(range(num_jobs)), *grouped_args_list)
-
-    @property
-    def meta(self) -> Dict[str, Any]:
-        return self._rs["__meta__"]
-
-    @property
-    def exceptions(self) -> Dict[str, Any]:
-        return self._rs["__exceptions__"]
-
-    @property
-    def terminated(self) -> bool:
-        return self.meta["terminated"]
-
-    @property
-    def parallel_results(self) -> Dict[str, Any]:
-        return self._rs
-
-    @property
-    def ordered_results(self) -> List[Any]:
-        return [None if key is None else self._rs[key] for key in self._task_names]
-
-    def __sleep(self, skip_check_finished: bool) -> None:
-        time.sleep(self._sleep + random.random())
-        self._refresh(skip_check_finished=skip_check_finished)
-
-    def __wait(self, wait_until_finished: bool) -> List[int]:
-        try:
-            while True:
-                task_names = ", ".join(
-                    map(
-                        self._get_task_name,
-                        filter(bool, self._working_task_indices),
-                    )
-                )
-                self._log_meta_msg(
-                    f"waiting for slots (working tasks : {task_names})",
-                    msg_level=logging.DEBUG,
-                )
-                finished_slots = []
-                for i, (task_idx, process) in enumerate(
-                    zip(self._working_task_indices, self._working_processes)
-                ):
-                    if process is None:
-                        self._log_meta_msg(f"pending on slot {i}")
-                        finished_slots.append(i)
-                        continue
-                    task_name = self._get_task_name(task_idx)
-                    if not process.is_alive():
-                        msg = f"in slot {i} is found finished"
-                        self._log_with_meta(task_name, msg)
-                        finished_slots.append(i)
-                if not wait_until_finished or finished_slots:
-                    return finished_slots
-                self.__sleep(skip_check_finished=True)
-        except KeyboardInterrupt:
-            self._set_terminate(scope="wait")
-            raise self._ParallelError("Keyboard Interrupted")
-
-    def _init_logger(self, task_name: str) -> None:
-        logging_folder = os.path.join(self._logging_folder, task_name)
-        os.makedirs(logging_folder, exist_ok=True)
-        logging_path = os.path.join(logging_folder, f"{timestamp()}.log")
-        self._setup_logger(task_name, logging_path)
-
-    def _refresh(self, skip_check_finished: bool) -> None:
-        if self._pid2task_idx is None:
-            self._pid2task_idx = self._resource_manager.pid2task_idx
-        if not self._resource_manager.inference_usages_initialized:
-            self._resource_manager.initialize_inference_usages()
-        if not self._resource_manager.checkpoint_initialized:
-            return
-        self._resource_manager.log_pid_usages_and_inference_frees()
-        self._resource_manager.check()
-        if not skip_check_finished:
-            self._wait_and_handle_finish(wait_until_finish=False)
-
-    def _wait_and_handle_finish(self, wait_until_finish: bool) -> None:
-        finished_slots = self.__wait(wait_until_finish)
-        if not finished_slots:
-            return
-        if self.terminated:
-            self._user_terminate()
-        finished_bundle = [[], []]
-        for finished_slot in finished_slots[::-1]:
-            if self._tqdm_bar is not None:
-                self._tqdm_bar.update()
-            tuple(
-                map(
-                    list.append,
-                    finished_bundle,
-                    map(
-                        list.pop,
-                        [self._working_task_indices, self._working_processes],
-                        [finished_slot] * 2,
-                    ),
-                )
-            )
-        for task_idx, process in zip(*finished_bundle):
-            task_name = self._resource_manager.handle_finish(task_idx, process)
-            if task_name is None:
-                continue
-            self.del_logger(task_name)
-
-    def _add_new_processes(self) -> bool:
-        n_working = len(self._working_processes)
-        n_new_jobs = self._num_jobs - n_working
-        n_res = len(self._all_task_indices) - self._cursor
-        if n_res > 0:
-            n_new_jobs = min(n_new_jobs, n_res)
-            for _ in range(n_new_jobs):
-                new_task_idx = self._all_task_indices[self._cursor]
-                self._working_processes.append(self._get_process(new_task_idx))
-                self._working_task_indices.append(new_task_idx)
-                self._cursor += 1
-            return True
-        return n_working > 0
-
-    def _user_terminate(self) -> None:
-        self._log_meta_msg(
-            "`_user_terminate` method hit, joining processes",
-            logging.ERROR,
-        )
-        for process in self._working_processes:
-            if process is None:
-                continue
-            process.join()
-        self._log_meta_msg(
-            "processes joined, raising self._ParallelError",
-            logging.ERROR,
-        )
-        recorded_exceptions = self.exceptions
-        if not recorded_exceptions:
-            raise self._ParallelError("Parallel terminated by user action")
-        else:
-            raise self._ParallelError("Parallel terminated by unexpected errors")
-
-    def _set_terminate(self, **kwargs) -> None:
-        meta = self.meta
-        meta["terminated"] = True
-        self._rs["__meta__"] = meta
-        if not kwargs:
-            suffix = ""
-        else:
-            suffix = f" ({' ; '.join(f'{k}: {v}' for k, v in kwargs.items())})"
-        self._log_meta_msg(f"`_set_terminate` method hit{suffix}", logging.ERROR)
-
-    def _get_task_name(self, task_idx: int) -> Optional[str]:
-        if task_idx is None:
-            return
-        if self._task_names[task_idx] is None:
-            self._task_names[task_idx] = f"task_{task_idx}"
-        task_name = f"{self._task_names[task_idx]}{self.name_suffix}"
-        self._init_logger(task_name)
-        return task_name
-
-    def _f_wrapper(self, task_idx: int, cuda: int = None) -> Callable:
-        task_name = self._get_task_name(task_idx)
-        logger = self._loggers_[task_name]
-
-        def log_method(msg, msg_level=logging.INFO, frame=None):
-            if frame is None:
-                frame = inspect.currentframe().f_back
-            self.log_msg(logger, msg, msg_level, frame)
-            return logger
-
-        def _inner(*args):
-            if self.terminated:
-                return
-            try:
-                log_method("task started", logging.DEBUG)
-                kwargs = {}
-                f_wants_cuda = f_wants_log_method = False
-                f_signature = inspect.signature(self._func)
-                for name, param in f_signature.parameters.items():
-                    if param.kind is inspect.Parameter.VAR_KEYWORD:
-                        f_wants_cuda = f_wants_log_method = True
-                        break
-                    if name == "cuda":
-                        f_wants_cuda = True
-                        continue
-                    if name == "log_method":
-                        f_wants_log_method = True
-                        continue
-                if not f_wants_cuda:
-                    if self._use_cuda:
-                        log_method(
-                            "task function doesn't want cuda but cuda is used",
-                            logging.WARNING,
-                        )
-                else:
-                    log_method("task function wants cuda")
-                    kwargs["cuda"] = cuda
-                if not f_wants_log_method:
-                    msg = "task function doesn't want log_method"
-                    log_method(msg, logging.WARNING)
-                else:
-                    log_method("task function wants log_method")
-                    kwargs["log_method"] = log_method
-                self._rs[task_name] = rs = self._func(*args, **kwargs)
-                terminate = isinstance(rs, dict) and rs.get("terminate", False)
-                if not terminate:
-                    log_method("task finished", logging.DEBUG)
-            except KeyboardInterrupt:
-                log_method("key board interrupted", logging.ERROR)
-                return
-            except Exception as err:
-                logger.exception(
-                    f"exception occurred, {err}",
-                    extra={"func_prefix": LoggingMixin._get_func_prefix(None)},
-                )
-                terminate = True
-                exceptions = self.exceptions
-                self._rs[task_name] = rs = err
-                exceptions[task_name] = rs
-                self._rs["__exceptions__"] = exceptions
-            if terminate:
-                self._set_terminate(scope="f_wrapper", task=task_name)
-                log_method("task terminated", logging.ERROR)
-
-        return _inner
-
-    def _get_process(
-        self,
-        task_idx: int,
-        start: bool = True,
-    ) -> Optional[Union[Tuple[Process, Dict[str, Any]], Process]]:
-        rs = self._resource_manager.get_process(
-            task_idx,
-            lambda: self.__sleep(skip_check_finished=False),
-            start,
-        )
-        task_name = rs["__task_name__"]
-        if not rs["__create_process__"]:
-            return
-        if not self._use_cuda or "GPU" not in rs:
-            args = (task_idx,)
-        else:
-            args = (task_idx, rs["GPU"]["tgt_resource_id"])
-        target = self._f_wrapper(*args)
-        process = Process(
-            target=target, args=tuple(args[task_idx] for args in self._args_list)
-        )
-        self._log_with_meta(task_name, "process created")
-        if start:
-            process.start()
-            self._log_with_meta(task_name, "process started")
-            self._record_process(task_idx, process, rs)
-            return process
-        return process, rs
-
-    def _record_process(
-        self,
-        task_idx: int,
-        process: Optional[Process],
-        rs: Dict[str, Any],
-    ) -> None:
-        if process is None:
-            return
-        self._resource_manager.record_process(task_idx, process, rs)
-
-
-__all__ = ["Parallel"]
+import os
+import dill
+import time
+import pprint
+import random
+import signal
+import inspect
+import logging
+import platform
+
+from tqdm import tqdm
+from typing import Any
+from typing import Dict
+from typing import List
+from typing import Tuple
+from typing import Union
+from typing import Optional
+from typing import Callable
+from pathos.pools import ProcessPool
+from multiprocessing import Process
+from multiprocessing.managers import SyncManager
+
+from ..misc import timestamp
+from ..misc import grouped_into
+from ..misc import print_warning
+from ..misc import LoggingMixin
+from ..misc import PureLoggingMixin
+from ..manage import PCManager
+from ..manage import GPUManager
+from ..manage import ResourceManager
+
+
+LINUX = platform.system() == "Linux"
+dill._dill._reverse_typemap["ClassType"] = type
+
+
+class Parallel(PureLoggingMixin):
+    """
+    Util class which can help running tasks in parallel.
+
+    Warnings
+    ----------
+        On platforms other than Linux, functions are dramatically reduced because
+        only Linux system well supports pickling. In this occasion, `Parallel`
+        will simply leverage `pathos` to do the jobs.
+
+    Parameters
+    ----------
+    num_jobs : int, number of jobs run in parallel.
+    sleep : float, idle duration of new jobs.
+    use_tqdm: bool, whether show progress bar (with tqdm) or not.
+    use_cuda: bool, whether tasks need CUDA or not.
+    name : str, summary name of these tasks.
+    meta_name : str, name of the meta information.
+    logging_folder : str, where the logging will be placed.
+    task_names : List[str], names of each task.
+    resource_config : Dict[str, Any], config used in `ResourceManager`.
+
+    Examples
+    ----------
+    >>> def add_one(x):
+    >>>     import time
+    >>>     time.sleep(1)
+    >>>     return x + 1
+    >>>
+    >>> print(Parallel(10)(add_one, list(range(10))).parallel_results)
+
+    """
+
+    class _ParallelError(Exception):
+        pass
+
+    def __init__(
+        self,
+        num_jobs: int,
+        *,
+        sleep: float = 1.0,
+        use_tqdm: bool = True,
+        use_cuda: bool = False,
+        name: Optional[str] = None,
+        meta_name: Optional[str] = None,
+        logging_folder: Optional[str] = None,
+        task_names: Optional[List[str]] = None,
+        tqdm_config: Optional[Dict[str, Any]] = None,
+        resource_config: Optional[Dict[str, Any]] = None,
+        warn_num_jobs: bool = True,
+    ):
+        self._rs = None
+        self._use_tqdm, self._use_cuda = use_tqdm, use_cuda
+        self._num_jobs, self._sleep = num_jobs, sleep
+        if tqdm_config is None:
+            tqdm_config = {}
+        if resource_config is None:
+            resource_config = {}
+        if logging_folder is None:
+            logging_folder = os.path.join(os.getcwd(), "_parallel_", "logs")
+        self._tqdm_config = tqdm_config
+        self._resource_config = resource_config
+        self._name, self._meta_name = name, meta_name
+        self._logging_folder, self._task_names = logging_folder, task_names
+        self._refresh_patience = resource_config.setdefault("refresh_patience", 10)
+        self._init_logger(self.meta_log_name)
+        self._warn_num_jobs = warn_num_jobs
+
+    def __call__(self, f: Callable, *args_list: Any) -> "Parallel":
+        # if f returns a dict with 'terminate' key, Parallel can be terminated at
+        # early stage by setting 'terminate' key to True
+        n_tasks = len(args_list[0])
+        n_jobs = min(self._num_jobs, n_tasks)
+        if self._task_names is None:
+            self._task_names = [None] * n_tasks
+        if not LINUX or n_jobs <= 1:
+            if LINUX and self._warn_num_jobs:
+                print_warning(
+                    "Detected Linux system but "
+                    f"n_jobs={n_jobs}, functions will be dramatically reduced.\n"
+                    "* It is recommended to set n_jobs to a larger value"
+                )
+            results = []
+            task_names = list(map(self._get_task_name, range(n_tasks)))
+            if n_jobs <= 1:
+                iterator = (f(*args) for args in zip(*args_list))
+            else:
+                p = ProcessPool(ncpus=n_jobs)
+                iterator = p.imap(f, *args_list)
+            if self._use_tqdm:
+                iterator = tqdm(iterator, total=n_tasks, **self._tqdm_config)
+            for result in iterator:
+                results.append(result)
+            self._rs = dict(zip(task_names, results))
+            return self
+        self._func, self._args_list = f, args_list
+        self._cursor, self._all_task_indices = 0, list(range(n_jobs, n_tasks))
+        self._log_meta_msg("initializing sync manager")
+        self._sync_manager = SyncManager()
+        self._sync_manager.start(lambda: signal.signal(signal.SIGINT, signal.SIG_IGN))
+        meta = {"n_jobs": n_jobs, "n_tasks": n_tasks, "terminated": False}
+        self._rs = self._sync_manager.dict(
+            {
+                "__meta__": meta,
+                "__exceptions__": {},
+            }
+        )
+        self._overwritten_task_info = {}
+        self._pid2task_idx = None
+        self._log_meta_msg("initializing resource manager")
+        self._resource_manager = ResourceManager(
+            self._resource_config, self._get_task_name, self._refresh_patience
+        )
+        self._log_meta_msg("registering PC manager")
+        pc_manager = PCManager()
+        ram_methods = {
+            "get_pid_usage_dict": None,
+            "get_pid_usage": pc_manager.get_pid_ram_usage,
+            "get_available_dict": lambda: {"total": pc_manager.get_available_ram()},
+        }
+        self._resource_manager.register("RAM", ram_methods)
+        gpu_config = self._resource_config.setdefault("gpu_config", {})
+        default_cuda_list = None if self._use_cuda else []
+        available_cuda_list = gpu_config.setdefault(
+            "available_cuda_list", default_cuda_list
+        )
+        if available_cuda_list is None or available_cuda_list:
+            self._log_meta_msg("registering GPU manager")
+            if available_cuda_list is not None:
+                available_cuda_list = list(map(int, available_cuda_list))
+            gpu_manager = GPUManager(available_cuda_list)
+            gpu_methods = {
+                "get_pid_usage": None,
+                "get_pid_usage_dict": gpu_manager.get_pid_usages,
+                "get_available_dict": gpu_manager.get_gpu_frees,
+            }
+            self._resource_manager.register("GPU", gpu_methods)
+        self._resource_manager.register_logging(self._init_logger, self)
+        self._log_meta_msg("initializing with refreshing")
+        self._refresh(skip_check_finished=True)
+        self._working_processes = None
+        if not self._use_tqdm:
+            self._tqdm_bar = None
+        else:
+            self._tqdm_bar = tqdm(list(range(n_tasks)), **self._tqdm_config)
+        try:
+            self._log_meta_msg("initializing processes")
+            init_task_indices = list(range(n_jobs))
+            init_processes = [
+                self._get_process(i, start=False) for i in init_task_indices
+            ]
+            if self.terminated:
+                self._user_terminate()
+            init_failed_slots, init_failed_task_indices = [], []
+            for i, (task_idx, process) in enumerate(
+                zip(init_task_indices, init_processes)
+            ):
+                if process is None:
+                    init_failed_slots.append(i)
+                    init_failed_task_indices.append(task_idx)
+                    task_name = self._get_task_name(task_idx)
+                    self._log_with_meta(
+                        task_name,
+                        "initialization failed, it may due to lack of resources",
+                        msg_level=logging.WARNING,
+                    )
+            if init_failed_slots:
+                for slot in init_failed_slots:
+                    init_task_indices[slot] = None
+                    init_processes[slot] = [None] * 4
+                self._all_task_indices = (
+                    init_failed_task_indices + self._all_task_indices
+                )
+            self._working_task_indices = init_task_indices
+            self._working_processes, task_info = map(list, zip(*init_processes))
+            self._log_meta_msg("starting all initial processes")
+            tuple(
+                map(
+                    lambda p_: None if p_ is None else p_.start(),
+                    self._working_processes,
+                )
+            )
+            tuple(
+                map(
+                    self._record_process,
+                    self._working_task_indices,
+                    self._working_processes,
+                    task_info,
+                )
+            )
+            self._resource_manager.initialize_running_usages()
+            self._log_meta_msg("entering parallel main loop")
+            while True:
+                self._log_meta_msg("waiting for finished slot")
+                self._wait_and_handle_finish(wait_until_finish=True)
+                if not self._add_new_processes():
+                    break
+        except KeyboardInterrupt:
+            self.exception(self.meta_log_name, f"keyboard interrupted")
+            exceptions = self.exceptions
+            exceptions["base"] = self._ParallelError("Keyboard Interrupted")
+            self._rs["__exceptions__"] = exceptions
+        except Exception as err:
+            self.exception(self.meta_log_name, f"exception occurred, {err}")
+            exceptions = self.exceptions
+            exceptions["base"] = err
+            self._rs["__exceptions__"] = exceptions
+        finally:
+            self._log_meta_msg("joining processes left behind")
+            if self._working_processes is not None:
+                for process in self._working_processes:
+                    if process is None:
+                        continue
+                    process.join()
+            if self._tqdm_bar is not None:
+                self._tqdm_bar.close()
+            self._log_meta_msg("casting parallel results to Python dict")
+            self._rs = dict(self._rs)
+            self._log_meta_msg("shutting down sync manager")
+            self._sync_manager.shutdown()
+            self.log_block_msg(
+                self.meta_log_name,
+                "parallel results",
+                pprint.pformat(self._rs, compact=True),
+            )
+        return self
+
+    def grouped(self, f: Callable, *args_list: Any) -> "Parallel":
+        num_jobs = min(len(args_list[0]), self._num_jobs)
+        grouped_args_list = [grouped_into(args, num_jobs) for args in args_list]
+
+        def _grouped_f(i: int, *args_list_: Tuple[Any], cuda: Any = None) -> List[Any]:
+            results: List[Any] = []
+            kwargs = {} if not self._use_cuda else {"cuda": cuda}
+            for args in tqdm(
+                zip(*args_list_),
+                total=len(args_list_[0]),
+                position=i + 1,
+                leave=False,
+            ):
+                results.append(f(*args, **kwargs))
+            return results
+
+        return self(_grouped_f, list(range(num_jobs)), *grouped_args_list)
+
+    @property
+    def meta(self) -> Dict[str, Any]:
+        return self._rs["__meta__"]
+
+    @property
+    def exceptions(self) -> Dict[str, Any]:
+        return self._rs["__exceptions__"]
+
+    @property
+    def terminated(self) -> bool:
+        return self.meta["terminated"]
+
+    @property
+    def parallel_results(self) -> Dict[str, Any]:
+        return self._rs
+
+    @property
+    def ordered_results(self) -> List[Any]:
+        return [None if key is None else self._rs[key] for key in self._task_names]
+
+    def __sleep(self, skip_check_finished: bool) -> None:
+        time.sleep(self._sleep + random.random())
+        self._refresh(skip_check_finished=skip_check_finished)
+
+    def __wait(self, wait_until_finished: bool) -> List[int]:
+        try:
+            while True:
+                task_names = ", ".join(
+                    map(
+                        self._get_task_name,
+                        filter(bool, self._working_task_indices),
+                    )
+                )
+                self._log_meta_msg(
+                    f"waiting for slots (working tasks : {task_names})",
+                    msg_level=logging.DEBUG,
+                )
+                finished_slots = []
+                for i, (task_idx, process) in enumerate(
+                    zip(self._working_task_indices, self._working_processes)
+                ):
+                    if process is None:
+                        self._log_meta_msg(f"pending on slot {i}")
+                        finished_slots.append(i)
+                        continue
+                    task_name = self._get_task_name(task_idx)
+                    if not process.is_alive():
+                        msg = f"in slot {i} is found finished"
+                        self._log_with_meta(task_name, msg)
+                        finished_slots.append(i)
+                if not wait_until_finished or finished_slots:
+                    return finished_slots
+                self.__sleep(skip_check_finished=True)
+        except KeyboardInterrupt:
+            self._set_terminate(scope="wait")
+            raise self._ParallelError("Keyboard Interrupted")
+
+    def _init_logger(self, task_name: str) -> None:
+        logging_folder = os.path.join(self._logging_folder, task_name)
+        os.makedirs(logging_folder, exist_ok=True)
+        logging_path = os.path.join(logging_folder, f"{timestamp()}.log")
+        self._setup_logger(task_name, logging_path)
+
+    def _refresh(self, skip_check_finished: bool) -> None:
+        if self._pid2task_idx is None:
+            self._pid2task_idx = self._resource_manager.pid2task_idx
+        if not self._resource_manager.inference_usages_initialized:
+            self._resource_manager.initialize_inference_usages()
+        if not self._resource_manager.checkpoint_initialized:
+            return
+        self._resource_manager.log_pid_usages_and_inference_frees()
+        self._resource_manager.check()
+        if not skip_check_finished:
+            self._wait_and_handle_finish(wait_until_finish=False)
+
+    def _wait_and_handle_finish(self, wait_until_finish: bool) -> None:
+        finished_slots = self.__wait(wait_until_finish)
+        if not finished_slots:
+            return
+        if self.terminated:
+            self._user_terminate()
+        finished_bundle = [[], []]
+        for finished_slot in finished_slots[::-1]:
+            if self._tqdm_bar is not None:
+                self._tqdm_bar.update()
+            tuple(
+                map(
+                    list.append,
+                    finished_bundle,
+                    map(
+                        list.pop,
+                        [self._working_task_indices, self._working_processes],
+                        [finished_slot] * 2,
+                    ),
+                )
+            )
+        for task_idx, process in zip(*finished_bundle):
+            task_name = self._resource_manager.handle_finish(task_idx, process)
+            if task_name is None:
+                continue
+            self.del_logger(task_name)
+
+    def _add_new_processes(self) -> bool:
+        n_working = len(self._working_processes)
+        n_new_jobs = self._num_jobs - n_working
+        n_res = len(self._all_task_indices) - self._cursor
+        if n_res > 0:
+            n_new_jobs = min(n_new_jobs, n_res)
+            for _ in range(n_new_jobs):
+                new_task_idx = self._all_task_indices[self._cursor]
+                self._working_processes.append(self._get_process(new_task_idx))
+                self._working_task_indices.append(new_task_idx)
+                self._cursor += 1
+            return True
+        return n_working > 0
+
+    def _user_terminate(self) -> None:
+        self._log_meta_msg(
+            "`_user_terminate` method hit, joining processes",
+            logging.ERROR,
+        )
+        for process in self._working_processes:
+            if process is None:
+                continue
+            process.join()
+        self._log_meta_msg(
+            "processes joined, raising self._ParallelError",
+            logging.ERROR,
+        )
+        recorded_exceptions = self.exceptions
+        if not recorded_exceptions:
+            raise self._ParallelError("Parallel terminated by user action")
+        else:
+            raise self._ParallelError("Parallel terminated by unexpected errors")
+
+    def _set_terminate(self, **kwargs) -> None:
+        meta = self.meta
+        meta["terminated"] = True
+        self._rs["__meta__"] = meta
+        if not kwargs:
+            suffix = ""
+        else:
+            suffix = f" ({' ; '.join(f'{k}: {v}' for k, v in kwargs.items())})"
+        self._log_meta_msg(f"`_set_terminate` method hit{suffix}", logging.ERROR)
+
+    def _get_task_name(self, task_idx: int) -> Optional[str]:
+        if task_idx is None:
+            return
+        if self._task_names[task_idx] is None:
+            self._task_names[task_idx] = f"task_{task_idx}"
+        task_name = f"{self._task_names[task_idx]}{self.name_suffix}"
+        self._init_logger(task_name)
+        return task_name
+
+    def _f_wrapper(self, task_idx: int, cuda: int = None) -> Callable:
+        task_name = self._get_task_name(task_idx)
+        logger = self._loggers_[task_name]
+
+        def log_method(msg, msg_level=logging.INFO, frame=None):
+            if frame is None:
+                frame = inspect.currentframe().f_back
+            self.log_msg(logger, msg, msg_level, frame)
+            return logger
+
+        def _inner(*args):
+            if self.terminated:
+                return
+            try:
+                log_method("task started", logging.DEBUG)
+                kwargs = {}
+                f_wants_cuda = f_wants_log_method = False
+                f_signature = inspect.signature(self._func)
+                for name, param in f_signature.parameters.items():
+                    if param.kind is inspect.Parameter.VAR_KEYWORD:
+                        f_wants_cuda = f_wants_log_method = True
+                        break
+                    if name == "cuda":
+                        f_wants_cuda = True
+                        continue
+                    if name == "log_method":
+                        f_wants_log_method = True
+                        continue
+                if not f_wants_cuda:
+                    if self._use_cuda:
+                        log_method(
+                            "task function doesn't want cuda but cuda is used",
+                            logging.WARNING,
+                        )
+                else:
+                    log_method("task function wants cuda")
+                    kwargs["cuda"] = cuda
+                if not f_wants_log_method:
+                    msg = "task function doesn't want log_method"
+                    log_method(msg, logging.WARNING)
+                else:
+                    log_method("task function wants log_method")
+                    kwargs["log_method"] = log_method
+                self._rs[task_name] = rs = self._func(*args, **kwargs)
+                terminate = isinstance(rs, dict) and rs.get("terminate", False)
+                if not terminate:
+                    log_method("task finished", logging.DEBUG)
+            except KeyboardInterrupt:
+                log_method("key board interrupted", logging.ERROR)
+                return
+            except Exception as err:
+                logger.exception(
+                    f"exception occurred, {err}",
+                    extra={"func_prefix": LoggingMixin._get_func_prefix(None)},
+                )
+                terminate = True
+                exceptions = self.exceptions
+                self._rs[task_name] = rs = err
+                exceptions[task_name] = rs
+                self._rs["__exceptions__"] = exceptions
+            if terminate:
+                self._set_terminate(scope="f_wrapper", task=task_name)
+                log_method("task terminated", logging.ERROR)
+
+        return _inner
+
+    def _get_process(
+        self,
+        task_idx: int,
+        start: bool = True,
+    ) -> Optional[Union[Tuple[Process, Dict[str, Any]], Process]]:
+        rs = self._resource_manager.get_process(
+            task_idx,
+            lambda: self.__sleep(skip_check_finished=False),
+            start,
+        )
+        task_name = rs["__task_name__"]
+        if not rs["__create_process__"]:
+            return
+        if not self._use_cuda or "GPU" not in rs:
+            args = (task_idx,)
+        else:
+            args = (task_idx, rs["GPU"]["tgt_resource_id"])
+        target = self._f_wrapper(*args)
+        process = Process(
+            target=target, args=tuple(args[task_idx] for args in self._args_list)
+        )
+        self._log_with_meta(task_name, "process created")
+        if start:
+            process.start()
+            self._log_with_meta(task_name, "process started")
+            self._record_process(task_idx, process, rs)
+            return process
+        return process, rs
+
+    def _record_process(
+        self,
+        task_idx: int,
+        process: Optional[Process],
+        rs: Dict[str, Any],
+    ) -> None:
+        if process is None:
+            return
+        self._resource_manager.record_process(task_idx, process, rs)
+
+
+__all__ = ["Parallel"]
```

### Comparing `carefree-toolkit-0.3.6.3/cftool/geometry.py` & `carefree-toolkit-0.3.6.4/cftool/geometry.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,376 +1,376 @@
-import math
-
-import numpy as np
-
-from enum import Enum
-from typing import List
-from typing import Tuple
-from typing import Union
-from typing import TypeVar
-from typing import Optional
-from pydantic import BaseModel
-from dataclasses import dataclass
-
-
-class PivotType(str, Enum):
-    LT = "lt"
-    TOP = "top"
-    RT = "rt"
-    LEFT = "left"
-    CENTER = "center"
-    RIGHT = "right"
-    LB = "lb"
-    BOTTOM = "bottom"
-    RB = "rb"
-
-
-# 从左上角开始，「顺时针排布」的八个角点，加上最后的中心点
-outer_pivots: List[PivotType] = [
-    PivotType.LT,
-    PivotType.TOP,
-    PivotType.RT,
-    PivotType.RIGHT,
-    PivotType.RB,
-    PivotType.BOTTOM,
-    PivotType.LB,
-    PivotType.LEFT,
-]
-all_pivots: List[PivotType] = outer_pivots + [PivotType.CENTER]
-# 从左上角开始，「顺时针排布」的四个角点
-corner_pivots: List[PivotType] = [
-    PivotType.LT,
-    PivotType.RT,
-    PivotType.RB,
-    PivotType.LB,
-]
-edge_pivots: List[PivotType] = [
-    PivotType.TOP,
-    PivotType.RIGHT,
-    PivotType.BOTTOM,
-    PivotType.LEFT,
-]
-mid_pivots: List[PivotType] = edge_pivots + [PivotType.CENTER]
-
-
-def is_close(a: float, b: float, *, atol: float = 1.0e-6, rtol: float = 1.0e-4) -> bool:
-    diff = abs(a - b)
-    a = max(a, 1.0e-8)
-    b = max(b, 1.0e-8)
-    if diff >= atol or abs(diff / a) >= rtol or abs(diff / b) >= rtol:
-        return False
-    return True
-
-
-@dataclass
-class Point:
-    x: float
-    y: float
-
-    @property
-    def tuple(self) -> Tuple[float, float]:
-        return self.x, self.y
-
-    def __rmatmul__(self, other: "Matrix2D") -> "Point":
-        x, y = self.x, self.y
-        a, b, c, d, e, f = other.tuple
-        return Point(x=a * x + c * y + e, y=b * x + d * y + f)
-
-    def inside(self, box: "Matrix2D") -> bool:
-        x, y = (box.inverse @ self).tuple
-        return 0 <= x <= 1 and 0 <= y <= 1
-
-    @classmethod
-    def origin(cls) -> "Point":
-        return cls(x=0.0, y=0.0)
-
-
-@dataclass
-class Line:
-    start: Point
-    end: Point
-
-    def intersect(self, other: "Line", extendable: bool = False) -> Optional[Point]:
-        x1, y1 = self.start.tuple
-        x2, y2 = self.end.tuple
-        x3, y3 = other.start.tuple
-        x4, y4 = other.end.tuple
-        x13 = x1 - x3
-        x21 = x2 - x1
-        x43 = x4 - x3
-        y13 = y1 - y3
-        y21 = y2 - y1
-        y43 = y4 - y3
-        denom = y43 * x21 - x43 * y21
-        if is_close(denom, 0):
-            return None
-        uA = (x43 * y13 - y43 * x13) / denom
-        uB = (x21 * y13 - y21 * x13) / denom
-        if extendable or (0 <= uA <= 1 and 0 <= uB <= 1):
-            return Point(x1 + uA * (x2 - x1), y1 + uA * (y2 - y1))
-        return None
-
-    def distance_to(self, target_line: "Line") -> float:
-        x1, y1 = self.start.tuple
-        x2, y2 = self.end.tuple
-        x4, y4 = target_line.end.tuple
-        dy = y1 - y2 or 10e-10
-        k = (x1 - x2) / dy
-        d = (k * (y2 - y4) + x4 - x2) / math.sqrt(1 + k**2)
-        return d
-
-
-class Matrix2DProperties(BaseModel):
-    x: float
-    y: float
-    w: float
-    h: float
-    theta: float
-    skew_x: float
-    skew_y: float
-
-
-TMatMul = TypeVar("TMatMul", bound=Union[Point, "Matrix2D"])
-
-
-class Matrix2D(BaseModel):
-    a: float
-    b: float
-    c: float
-    d: float
-    e: float
-    f: float
-
-    def __matmul__(self, other: TMatMul) -> TMatMul:
-        if isinstance(other, Point):
-            return other.__rmatmul__(self)
-        if isinstance(other, Matrix2D):
-            a1, b1, c1, d1, e1, f1 = self.tuple
-            a2, b2, c2, d2, e2, f2 = other.tuple
-            return Matrix2D(
-                a=a1 * a2 + c1 * b2,
-                b=b1 * a2 + d1 * b2,
-                c=a1 * c2 + c1 * d2,
-                d=b1 * c2 + d1 * d2,
-                e=a1 * e2 + c1 * f2 + e1,
-                f=b1 * e2 + d1 * f2 + f1,
-            )
-        msg = f"unsupported operand type(s) for @: 'Matrix2D' and '{type(other)}'"
-        raise TypeError(msg)
-
-    @property
-    def tuple(self) -> Tuple[float, float, float, float, float, float]:
-        return self.a, self.b, self.c, self.d, self.e, self.f
-
-    @property
-    def x(self) -> float:
-        return self.e
-
-    @property
-    def y(self) -> float:
-        return self.f
-
-    @property
-    def position(self) -> Point:
-        return Point(self.e, self.f)
-
-    @property
-    def w(self) -> float:
-        return math.sqrt(self.a**2 + self.b**2)
-
-    @property
-    def h(self) -> float:
-        return (self.a * self.d - self.b * self.c) / max(self.w, 1.0e-12)
-
-    @property
-    def wh(self) -> Tuple[float, float]:
-        w = self.w
-        h = (self.a * self.d - self.b * self.c) / max(w, 1.0e-12)
-        return w, h
-
-    @property
-    def area(self) -> float:
-        w, h = self.wh
-        return w * abs(h)
-
-    @property
-    def theta(self) -> float:
-        return -math.atan2(self.b, self.a)
-
-    @property
-    def matrix(self) -> np.ndarray:
-        return np.array([[self.a, self.c, self.e], [self.b, self.d, self.f]])
-
-    @property
-    def inverse(self) -> "Matrix2D":
-        a, b, c, d, e, f = self.tuple
-        ad = a * d
-        bc = b * c
-        return Matrix2D(
-            a=d / (ad - bc),
-            b=b / (bc - ad),
-            c=c / (bc - ad),
-            d=a / (ad - bc),
-            e=(d * e - c * f) / (bc - ad),
-            f=(b * e - a * f) / (ad - bc),
-        )
-
-    @property
-    def lt(self) -> Point:
-        return Point(self.e, self.f)
-
-    @property
-    def top(self) -> Point:
-        return Point(0.5 * self.a + self.e, 0.5 * self.b + self.f)
-
-    @property
-    def rt(self) -> Point:
-        return Point(self.a + self.e, self.b + self.f)
-
-    @property
-    def right(self) -> Point:
-        return self @ Point(1.0, 0.5)
-
-    @property
-    def rb(self) -> Point:
-        return self @ Point(1.0, 1.0)
-
-    @property
-    def bottom(self) -> Point:
-        return self @ Point(0.5, 1.0)
-
-    @property
-    def lb(self) -> Point:
-        return Point(self.c + self.e, self.d + self.f)
-
-    @property
-    def left(self) -> Point:
-        return Point(0.5 * self.c + self.e, 0.5 * self.d + self.f)
-
-    @property
-    def center(self) -> Point:
-        return self @ Point(0.5, 0.5)
-
-    def pivot(self, pivot: PivotType) -> Point:
-        return getattr(self, pivot.value)
-
-    # lt -> rt -> rb -> lb
-    @property
-    def corner_points(self) -> List[Point]:
-        return [self.pivot(pivot) for pivot in corner_pivots]
-
-    # top -> right -> bottom -> left -> center
-    @property
-    def mid_points(self) -> List[Point]:
-        return [self.pivot(pivot) for pivot in mid_pivots]
-
-    # lt -> top -> rt -> right -> rb -> bottom -> lb -> left -> center
-    @property
-    def all_points(self) -> List[Point]:
-        return [self.pivot(pivot) for pivot in all_pivots]
-
-    # top -> right -> bottom -> left
-    @property
-    def edges(self) -> List[Line]:
-        corners = self.corner_points
-        return [Line(corner, corners[(i + 1) % 4]) for i, corner in enumerate(corners)]
-
-    def decompose(self) -> Matrix2DProperties:
-        w, h = self.wh
-        a, b, c, d, e, f = self.tuple
-        return Matrix2DProperties(
-            x=e,
-            y=f,
-            w=w,
-            h=h,
-            theta=self.theta,
-            skew_x=math.atan2(a * c + b * d, w**2),
-            skew_y=0.0,
-        )
-
-    @classmethod
-    def skew_matrix(
-        cls,
-        skew_x: float,
-        skew_y: float,
-        center: Optional[Point] = None,
-    ) -> "Matrix2D":
-        center = center or Point.origin()
-        tx = math.tan(skew_x)
-        ty = math.tan(skew_y)
-        return cls(a=1, b=ty, c=tx, d=1, e=-tx * center.y, f=-ty * center.x)
-
-    @classmethod
-    def scale_matrix(
-        cls,
-        w: float,
-        h: float,
-        center: Optional[Point] = None,
-    ) -> "Matrix2D":
-        center = center or Point.origin()
-        return cls(a=w, b=0, c=0, d=h, e=center.x * (1 - w), f=center.y * (1 - h))
-
-    @classmethod
-    def rotation_matrix(
-        cls,
-        theta: float,
-        center: Optional[Point] = None,
-    ) -> "Matrix2D":
-        center = center or Point.origin()
-        sin = math.sin(theta)
-        cos = math.cos(theta)
-        return cls(
-            a=cos,
-            b=-sin,
-            c=sin,
-            d=cos,
-            e=(1.0 - cos) * center.x - center.y * sin,
-            f=(1.0 - cos) * center.y + center.x * sin,
-        )
-
-    @classmethod
-    def move_matrix(cls, x: float, y: float) -> "Matrix2D":
-        return cls(a=1, b=0, c=0, d=1, e=x, f=y)
-
-    @classmethod
-    def from_properties(cls, properties: Matrix2DProperties) -> "Matrix2D":
-        return (
-            cls.move_matrix(properties.x, properties.y)
-            @ cls.rotation_matrix(properties.theta)
-            @ cls.scale_matrix(properties.w, properties.h)
-            @ cls.skew_matrix(properties.skew_x, properties.skew_y)
-        )
-
-
-class HitTest:
-    @staticmethod
-    def line_line(a: Line, b: Line) -> bool:
-        return a.intersect(b) is not None
-
-    @staticmethod
-    def line_box(a: Line, b: Matrix2D) -> bool:
-        edges = b.edges
-        for edge in edges:
-            if HitTest.line_line(a, edge):
-                return True
-        return False
-
-    @staticmethod
-    def box_box(a: Matrix2D, b: Matrix2D) -> bool:
-        b_edges = b.edges
-        for b_edge in b_edges:
-            if HitTest.line_box(b_edge, a):
-                return True
-        if a.position.inside(b):
-            return True
-        if b.position.inside(a):
-            return True
-        return False
-
-
-__all__ = [
-    "PivotType",
-    "Point",
-    "Line",
-    "Matrix2D",
-    "HitTest",
-]
+import math
+
+import numpy as np
+
+from enum import Enum
+from typing import List
+from typing import Tuple
+from typing import Union
+from typing import TypeVar
+from typing import Optional
+from pydantic import BaseModel
+from dataclasses import dataclass
+
+
+class PivotType(str, Enum):
+    LT = "lt"
+    TOP = "top"
+    RT = "rt"
+    LEFT = "left"
+    CENTER = "center"
+    RIGHT = "right"
+    LB = "lb"
+    BOTTOM = "bottom"
+    RB = "rb"
+
+
+# 从左上角开始，「顺时针排布」的八个角点，加上最后的中心点
+outer_pivots: List[PivotType] = [
+    PivotType.LT,
+    PivotType.TOP,
+    PivotType.RT,
+    PivotType.RIGHT,
+    PivotType.RB,
+    PivotType.BOTTOM,
+    PivotType.LB,
+    PivotType.LEFT,
+]
+all_pivots: List[PivotType] = outer_pivots + [PivotType.CENTER]
+# 从左上角开始，「顺时针排布」的四个角点
+corner_pivots: List[PivotType] = [
+    PivotType.LT,
+    PivotType.RT,
+    PivotType.RB,
+    PivotType.LB,
+]
+edge_pivots: List[PivotType] = [
+    PivotType.TOP,
+    PivotType.RIGHT,
+    PivotType.BOTTOM,
+    PivotType.LEFT,
+]
+mid_pivots: List[PivotType] = edge_pivots + [PivotType.CENTER]
+
+
+def is_close(a: float, b: float, *, atol: float = 1.0e-6, rtol: float = 1.0e-4) -> bool:
+    diff = abs(a - b)
+    a = max(a, 1.0e-8)
+    b = max(b, 1.0e-8)
+    if diff >= atol or abs(diff / a) >= rtol or abs(diff / b) >= rtol:
+        return False
+    return True
+
+
+@dataclass
+class Point:
+    x: float
+    y: float
+
+    @property
+    def tuple(self) -> Tuple[float, float]:
+        return self.x, self.y
+
+    def __rmatmul__(self, other: "Matrix2D") -> "Point":
+        x, y = self.x, self.y
+        a, b, c, d, e, f = other.tuple
+        return Point(x=a * x + c * y + e, y=b * x + d * y + f)
+
+    def inside(self, box: "Matrix2D") -> bool:
+        x, y = (box.inverse @ self).tuple
+        return 0 <= x <= 1 and 0 <= y <= 1
+
+    @classmethod
+    def origin(cls) -> "Point":
+        return cls(x=0.0, y=0.0)
+
+
+@dataclass
+class Line:
+    start: Point
+    end: Point
+
+    def intersect(self, other: "Line", extendable: bool = False) -> Optional[Point]:
+        x1, y1 = self.start.tuple
+        x2, y2 = self.end.tuple
+        x3, y3 = other.start.tuple
+        x4, y4 = other.end.tuple
+        x13 = x1 - x3
+        x21 = x2 - x1
+        x43 = x4 - x3
+        y13 = y1 - y3
+        y21 = y2 - y1
+        y43 = y4 - y3
+        denom = y43 * x21 - x43 * y21
+        if is_close(denom, 0):
+            return None
+        uA = (x43 * y13 - y43 * x13) / denom
+        uB = (x21 * y13 - y21 * x13) / denom
+        if extendable or (0 <= uA <= 1 and 0 <= uB <= 1):
+            return Point(x1 + uA * (x2 - x1), y1 + uA * (y2 - y1))
+        return None
+
+    def distance_to(self, target_line: "Line") -> float:
+        x1, y1 = self.start.tuple
+        x2, y2 = self.end.tuple
+        x4, y4 = target_line.end.tuple
+        dy = y1 - y2 or 10e-10
+        k = (x1 - x2) / dy
+        d = (k * (y2 - y4) + x4 - x2) / math.sqrt(1 + k**2)
+        return d
+
+
+class Matrix2DProperties(BaseModel):
+    x: float
+    y: float
+    w: float
+    h: float
+    theta: float
+    skew_x: float
+    skew_y: float
+
+
+TMatMul = TypeVar("TMatMul", bound=Union[Point, "Matrix2D"])
+
+
+class Matrix2D(BaseModel):
+    a: float
+    b: float
+    c: float
+    d: float
+    e: float
+    f: float
+
+    def __matmul__(self, other: TMatMul) -> TMatMul:
+        if isinstance(other, Point):
+            return other.__rmatmul__(self)
+        if isinstance(other, Matrix2D):
+            a1, b1, c1, d1, e1, f1 = self.tuple
+            a2, b2, c2, d2, e2, f2 = other.tuple
+            return Matrix2D(
+                a=a1 * a2 + c1 * b2,
+                b=b1 * a2 + d1 * b2,
+                c=a1 * c2 + c1 * d2,
+                d=b1 * c2 + d1 * d2,
+                e=a1 * e2 + c1 * f2 + e1,
+                f=b1 * e2 + d1 * f2 + f1,
+            )
+        msg = f"unsupported operand type(s) for @: 'Matrix2D' and '{type(other)}'"
+        raise TypeError(msg)
+
+    @property
+    def tuple(self) -> Tuple[float, float, float, float, float, float]:
+        return self.a, self.b, self.c, self.d, self.e, self.f
+
+    @property
+    def x(self) -> float:
+        return self.e
+
+    @property
+    def y(self) -> float:
+        return self.f
+
+    @property
+    def position(self) -> Point:
+        return Point(self.e, self.f)
+
+    @property
+    def w(self) -> float:
+        return math.sqrt(self.a**2 + self.b**2)
+
+    @property
+    def h(self) -> float:
+        return (self.a * self.d - self.b * self.c) / max(self.w, 1.0e-12)
+
+    @property
+    def wh(self) -> Tuple[float, float]:
+        w = self.w
+        h = (self.a * self.d - self.b * self.c) / max(w, 1.0e-12)
+        return w, h
+
+    @property
+    def area(self) -> float:
+        w, h = self.wh
+        return w * abs(h)
+
+    @property
+    def theta(self) -> float:
+        return -math.atan2(self.b, self.a)
+
+    @property
+    def matrix(self) -> np.ndarray:
+        return np.array([[self.a, self.c, self.e], [self.b, self.d, self.f]])
+
+    @property
+    def inverse(self) -> "Matrix2D":
+        a, b, c, d, e, f = self.tuple
+        ad = a * d
+        bc = b * c
+        return Matrix2D(
+            a=d / (ad - bc),
+            b=b / (bc - ad),
+            c=c / (bc - ad),
+            d=a / (ad - bc),
+            e=(d * e - c * f) / (bc - ad),
+            f=(b * e - a * f) / (ad - bc),
+        )
+
+    @property
+    def lt(self) -> Point:
+        return Point(self.e, self.f)
+
+    @property
+    def top(self) -> Point:
+        return Point(0.5 * self.a + self.e, 0.5 * self.b + self.f)
+
+    @property
+    def rt(self) -> Point:
+        return Point(self.a + self.e, self.b + self.f)
+
+    @property
+    def right(self) -> Point:
+        return self @ Point(1.0, 0.5)
+
+    @property
+    def rb(self) -> Point:
+        return self @ Point(1.0, 1.0)
+
+    @property
+    def bottom(self) -> Point:
+        return self @ Point(0.5, 1.0)
+
+    @property
+    def lb(self) -> Point:
+        return Point(self.c + self.e, self.d + self.f)
+
+    @property
+    def left(self) -> Point:
+        return Point(0.5 * self.c + self.e, 0.5 * self.d + self.f)
+
+    @property
+    def center(self) -> Point:
+        return self @ Point(0.5, 0.5)
+
+    def pivot(self, pivot: PivotType) -> Point:
+        return getattr(self, pivot.value)
+
+    # lt -> rt -> rb -> lb
+    @property
+    def corner_points(self) -> List[Point]:
+        return [self.pivot(pivot) for pivot in corner_pivots]
+
+    # top -> right -> bottom -> left -> center
+    @property
+    def mid_points(self) -> List[Point]:
+        return [self.pivot(pivot) for pivot in mid_pivots]
+
+    # lt -> top -> rt -> right -> rb -> bottom -> lb -> left -> center
+    @property
+    def all_points(self) -> List[Point]:
+        return [self.pivot(pivot) for pivot in all_pivots]
+
+    # top -> right -> bottom -> left
+    @property
+    def edges(self) -> List[Line]:
+        corners = self.corner_points
+        return [Line(corner, corners[(i + 1) % 4]) for i, corner in enumerate(corners)]
+
+    def decompose(self) -> Matrix2DProperties:
+        w, h = self.wh
+        a, b, c, d, e, f = self.tuple
+        return Matrix2DProperties(
+            x=e,
+            y=f,
+            w=w,
+            h=h,
+            theta=self.theta,
+            skew_x=math.atan2(a * c + b * d, w**2),
+            skew_y=0.0,
+        )
+
+    @classmethod
+    def skew_matrix(
+        cls,
+        skew_x: float,
+        skew_y: float,
+        center: Optional[Point] = None,
+    ) -> "Matrix2D":
+        center = center or Point.origin()
+        tx = math.tan(skew_x)
+        ty = math.tan(skew_y)
+        return cls(a=1, b=ty, c=tx, d=1, e=-tx * center.y, f=-ty * center.x)
+
+    @classmethod
+    def scale_matrix(
+        cls,
+        w: float,
+        h: float,
+        center: Optional[Point] = None,
+    ) -> "Matrix2D":
+        center = center or Point.origin()
+        return cls(a=w, b=0, c=0, d=h, e=center.x * (1 - w), f=center.y * (1 - h))
+
+    @classmethod
+    def rotation_matrix(
+        cls,
+        theta: float,
+        center: Optional[Point] = None,
+    ) -> "Matrix2D":
+        center = center or Point.origin()
+        sin = math.sin(theta)
+        cos = math.cos(theta)
+        return cls(
+            a=cos,
+            b=-sin,
+            c=sin,
+            d=cos,
+            e=(1.0 - cos) * center.x - center.y * sin,
+            f=(1.0 - cos) * center.y + center.x * sin,
+        )
+
+    @classmethod
+    def move_matrix(cls, x: float, y: float) -> "Matrix2D":
+        return cls(a=1, b=0, c=0, d=1, e=x, f=y)
+
+    @classmethod
+    def from_properties(cls, properties: Matrix2DProperties) -> "Matrix2D":
+        return (
+            cls.move_matrix(properties.x, properties.y)
+            @ cls.rotation_matrix(properties.theta)
+            @ cls.scale_matrix(properties.w, properties.h)
+            @ cls.skew_matrix(properties.skew_x, properties.skew_y)
+        )
+
+
+class HitTest:
+    @staticmethod
+    def line_line(a: Line, b: Line) -> bool:
+        return a.intersect(b) is not None
+
+    @staticmethod
+    def line_box(a: Line, b: Matrix2D) -> bool:
+        edges = b.edges
+        for edge in edges:
+            if HitTest.line_line(a, edge):
+                return True
+        return False
+
+    @staticmethod
+    def box_box(a: Matrix2D, b: Matrix2D) -> bool:
+        b_edges = b.edges
+        for b_edge in b_edges:
+            if HitTest.line_box(b_edge, a):
+                return True
+        if a.position.inside(b):
+            return True
+        if b.position.inside(a):
+            return True
+        return False
+
+
+__all__ = [
+    "PivotType",
+    "Point",
+    "Line",
+    "Matrix2D",
+    "HitTest",
+]
```

### Comparing `carefree-toolkit-0.3.6.3/cftool/manage.py` & `carefree-toolkit-0.3.6.4/cftool/manage.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,609 +1,609 @@
-import psutil
-import logging
-import subprocess
-
-from typing import Any
-from typing import Dict
-from typing import List
-from typing import Tuple
-from typing import Union
-from typing import Callable
-from typing import Optional
-from collections import defaultdict
-
-from .misc import PureLoggingMixin
-
-
-class PCManager:
-    """Util class which can check PC status (unit: MB)."""
-
-    @staticmethod
-    def get_available_ram() -> float:
-        return psutil.virtual_memory().available / 1024**2
-
-    @staticmethod
-    def get_pid_ram_usage(pid: int) -> float:
-        try:
-            process = psutil.Process(pid)
-        except psutil.NoSuchProcess:
-            return 0.0
-        return process.memory_info().rss / 1024**2
-
-
-class GPUManager:
-    """
-    Util class which can check CUDA usages.
-
-    Parameters
-    ----------
-    available_cuda_list : {None, list}, indicates CUDAs which are available.
-    * If None, then all CUDAs will be available.
-    reuse : bool, indicates whether one CUDA could be used multiple times.
-    * If `available_cuda_list` is None, then `reuse` will have no effect.
-
-    Examples
-    --------
-    >>> available_cuda_list = list(range(8))  # indicates that CUDA-0, ..., CUDA-7 is available
-    >>> cuda = GPUManager(available_cuda_list).choose()  # `cuda` will be the CUDA id with most memory
-
-    """
-
-    def __init__(
-        self,
-        available_cuda_list: Optional[List[Union[str, int]]] = None,
-        *,
-        reuse: bool = True,
-    ):
-        self._reuse = reuse
-        if available_cuda_list is None:
-            self._available_cuda = None
-        else:
-            self._available_cuda = set(map(int, available_cuda_list))
-
-    @staticmethod
-    def _query_gpu() -> List[Dict[str, int]]:
-        q_args = ["index", "gpu_name", "memory.free", "memory.total"]
-        cmd = f"nvidia-smi --query-gpu={','.join(q_args)} --format=csv,noheader"
-        results = subprocess.Popen(
-            cmd,
-            shell=True,
-            stdout=subprocess.PIPE,
-            close_fds=True,
-        ).communicate()[0]
-        results = list(filter(bool, results.decode("utf-8").strip().split("\n")))
-
-        def _parse(line):
-            numeric_args = ["memory.free", "memory.total"]
-            power_manage_enable = lambda v: ("Not Support" not in v)
-            to_numeric = lambda v: float(
-                v.upper().strip().replace("MIB", "").replace("W", "")
-            )
-            process = lambda k, v: (
-                (int(to_numeric(v)) if power_manage_enable(v) else 1)
-                if k in numeric_args
-                else v.strip()
-            )
-            rs = {k: process(k, v) for k, v in zip(q_args, line.strip().split(","))}
-            rs["index"] = int(rs["index"])
-            return rs
-
-        return list(map(_parse, results))
-
-    @staticmethod
-    def _query_pid() -> List[Tuple[int, int]]:
-        cmd = "nvidia-smi --query-compute-apps=pid,used_memory --format=csv,noheader"
-        results = subprocess.Popen(
-            cmd,
-            shell=True,
-            stdout=subprocess.PIPE,
-            close_fds=True,
-        ).communicate()[0]
-        results = list(filter(bool, results.decode("utf-8").strip().split("\n")))
-        pid_list = []
-        for line in results:
-            key, value = map(int, line.replace("MiB", "").strip().split(", "))
-            pid_list.append((key, value))
-        return pid_list
-
-    @staticmethod
-    def _sort_by_memory(
-        gpus: List[Dict[str, int]],
-        by_size: bool = False,
-    ) -> List[Dict[str, int]]:
-        if by_size:
-            return sorted(gpus, key=lambda d: d["memory.free"], reverse=True)
-        return sorted(
-            gpus,
-            key=lambda d: float(d["memory.free"]) / d["memory.total"],
-            reverse=True,
-        )
-
-    def _gpu_filter(self, gpu: Dict[str, int]):
-        return self._available_cuda is None or gpu["index"] in self._available_cuda
-
-    def choose(self) -> int:
-        if isinstance(self._available_cuda, set) and not self._available_cuda:
-            raise ValueError("No more CUDAs are available")
-        chosen_gpu = int(
-            next(
-                filter(
-                    self._gpu_filter,
-                    self._sort_by_memory(self._query_gpu(), True),
-                )
-            )["index"]
-        )
-        if not self._reuse and self._available_cuda is not None:
-            self._available_cuda.remove(chosen_gpu)
-        return chosen_gpu
-
-    def get_gpu_frees(self) -> Dict[int, int]:
-        return {
-            gpu["index"]: gpu["memory.free"]
-            for gpu in filter(self._gpu_filter, self._query_gpu())
-        }
-
-    def get_pid_usages(self) -> Dict[int, int]:
-        usages = defaultdict(int)
-        for key, usage in self._query_pid():
-            usages[key] += usage
-        return usages
-
-
-class ResourceManager:
-    """
-    Util class which can monitor & manage resources.
-    * It utilizes `PCManager` & `GPUManager` defined above.
-    * It is currently used in cftool.dist.core.Parallel only.
-
-    """
-
-    def __init__(
-        self,
-        config: Dict[str, Any],
-        get_task_name: Callable[[int], Optional[str]],
-        refresh_patience: int,
-    ):
-        self._resources, self._info_dict, self._overwritten_task_info = [], {}, {}
-        self._init_logger = self._meta_log_name = None
-        self._log_msg = self._log_block_msg = None
-        self._log_meta_msg = self._log_with_meta = None
-        self.pid2task_idx, self._get_task_name = {}, get_task_name
-        self.config, self._refresh_patience = config, refresh_patience
-
-    def register(self, resource_name: str, methods: Dict[str, Callable]) -> None:
-        self._resources.append(resource_name)
-        resource_config = self.config.setdefault(f"{resource_name.lower()}_config", {})
-        preset_usages = resource_config.setdefault("preset_usages", {})
-        minimum_resource = resource_config.setdefault(
-            "minimum_resource",
-            preset_usages.setdefault("__default__", 1024),
-        )
-        counter_threshold = resource_config.setdefault("counter_threshold", 4)
-        warning_threshold = resource_config.setdefault("warning_threshold", 1024)
-        info = self._info_dict.setdefault(
-            resource_name,
-            {
-                "preset_usages": preset_usages,
-                "minimum_resource": minimum_resource,
-                "counter_threshold": counter_threshold,
-                "warning_threshold": warning_threshold,
-            },
-        )
-        get_pid_usage, get_pid_usage_dict, get_available_dict = map(
-            methods.get,
-            ["get_pid_usage", "get_pid_usage_dict", "get_available_dict"],
-        )
-        if get_pid_usage is None and get_pid_usage_dict is None:
-            raise ValueError(
-                "either get_pid_usage or get_pid_usage_dict "
-                "should be provided in methods"
-            )
-        if get_available_dict is None:
-            raise ValueError("get_available_dict should be provided in methods")
-        info["get_pid_usage"] = get_pid_usage
-        info["get_pid_usage_dict"] = get_pid_usage_dict
-        info["get_available_dict"] = get_available_dict
-        info["inference_frees"], info["checkpoint_pid_usages"] = {}, {}
-        info["running_pid_usages"], info["running_pid_counters"] = {}, {}
-        info["inference_usages_initialized"] = False
-        info["pid2resource_id"] = {}
-
-    def register_logging(
-        self,
-        init_logger: Callable[[str], None],
-        mixin: PureLoggingMixin,
-    ):
-        self._init_logger, self._meta_log_name = init_logger, mixin.meta_log_name
-        self._log_msg, self._log_block_msg = mixin.log_msg, mixin.log_block_msg
-        self._log_meta_msg = mixin._log_meta_msg
-        self._log_with_meta = mixin._log_with_meta
-
-    @property
-    def inference_usages_initialized(self) -> bool:
-        for info in self._info_dict.values():
-            if not info["inference_usages_initialized"]:
-                return False
-        return True
-
-    @property
-    def checkpoint_initialized(self) -> bool:
-        for info in self._info_dict.values():
-            if not info["checkpoint_pid_usages"]:
-                return False
-        return True
-
-    @staticmethod
-    def _get_all_relevant_processes(pid: int) -> List[psutil.Process]:
-        parent = psutil.Process(pid)
-        processes = [parent]
-        for process in parent.children(recursive=True):
-            processes.append(process)
-        return processes
-
-    @staticmethod
-    def _get_pid_usages(info: Dict[str, Any]) -> Dict[str, int]:
-        get_pid_usage_dict = info["get_pid_usage_dict"]
-        if get_pid_usage_dict is not None:
-            return get_pid_usage_dict()
-        pid_usages, get_pid_usage = {}, info["get_pid_usage"]
-        for pid in info["running_pid_usages"].keys():
-            try:
-                processes = ResourceManager._get_all_relevant_processes(pid)
-                pid_usages[pid] = int(
-                    sum(get_pid_usage(process.pid) for process in processes)
-                )
-            except psutil.NoSuchProcess:
-                pid_usages[pid] = 0
-        return pid_usages
-
-    @staticmethod
-    def get_dict_block_msg(d: Dict[str, int]) -> str:
-        keys = sorted(d.keys())
-        values = [d[key] for key in keys]
-        header = " | ".join(map(lambda pid: f"{pid:^12s}", map(str, keys)))
-        body = " | ".join(map(lambda usage: f"{int(usage):^10d}MB", values))
-        len_header = len(header)
-        above = f"{'=' * len_header}\n{header}\n{'-' * len_header}"
-        return f"{above}\n{body}\n{'-' * len_header}"
-
-    def default_usage(self, resource: str) -> int:
-        return int(self._info_dict[resource]["preset_usages"]["__default__"])
-
-    def initialize_running_usages(self) -> None:
-        for info in self._info_dict.values():
-            info["running_pid_usages"] = info["checkpoint_pid_usages"].copy()
-
-    def initialize_inference_usages(self) -> None:
-        for info in self._info_dict.values():
-            info["inference_frees"] = info["get_available_dict"]()
-            info["inference_usages_initialized"] = True
-
-    def log_pid_usages_and_inference_frees(self) -> None:
-        for resource in self._resources:
-            info = self._info_dict[resource]
-            self._log_block_msg(
-                self._meta_log_name,
-                f"current pid {resource} usages",
-                self.get_dict_block_msg(self._get_pid_usages(info)),
-                logging.DEBUG,
-            )
-            self._log_block_msg(
-                self._meta_log_name,
-                f"current inference {resource} frees",
-                self.get_dict_block_msg(info["inference_frees"]),
-                logging.DEBUG,
-            )
-
-    def check(self) -> None:
-        for resource in self._resources:
-            info = self._info_dict[resource]
-            checkpoint_pid_usages, running_pid_usages, running_pid_counters = map(
-                info.get,
-                [
-                    "checkpoint_pid_usages",
-                    "running_pid_usages",
-                    "running_pid_counters",
-                ],
-            )
-            get_pid_usage, get_pid_usage_dict = map(
-                info.get,
-                ["get_pid_usage", "get_pid_usage_dict"],
-            )
-            if get_pid_usage is None:
-                pid_usage_dict = get_pid_usage_dict()
-                get_pid_usage = lambda pid_: pid_usage_dict.get(pid_, 0)
-            for pid, checkpoint_usage in checkpoint_pid_usages.items():
-                task_name = self._get_task_name(self.pid2task_idx[pid])
-                self._log_msg(
-                    task_name,
-                    f"checkpoint {resource} usage : {checkpoint_usage} MB",
-                    logging.DEBUG,
-                )
-                children_pid_usages = {}
-                try:
-                    processes = self._get_all_relevant_processes(pid)
-                except psutil.NoSuchProcess as err:
-                    self._log_with_meta(
-                        task_name,
-                        f"already finished, {err}",
-                        logging.INFO,
-                    )
-                    continue
-                current_usage = get_pid_usage(pid)
-                for process in processes[1:]:
-                    process_usage = get_pid_usage(process.pid)
-                    children_pid_usages[process.pid] = process_usage
-                    current_usage += process_usage
-                if children_pid_usages:
-                    self._log_block_msg(
-                        task_name,
-                        f"children {resource} usages",
-                        self.get_dict_block_msg(children_pid_usages),
-                        logging.DEBUG,
-                    )
-                self._log_msg(
-                    task_name,
-                    f"current {resource} usage : {current_usage} MB",
-                    logging.DEBUG,
-                )
-                if current_usage == 0:
-                    continue
-                running_usage = running_pid_usages[pid]
-                self._log_msg(
-                    task_name,
-                    f"running {resource} usage : {running_usage} MB",
-                    logging.DEBUG,
-                )
-                if running_usage > checkpoint_usage:
-                    running_pid_counters[pid] = self._refresh_patience
-                    self._log_msg(
-                        task_name,
-                        f"increasing {resource} counter directly to "
-                        f"{self._refresh_patience}",
-                        logging.DEBUG,
-                    )
-                elif abs(running_usage - current_usage) <= info["counter_threshold"]:
-                    running_pid_counters[pid] += 1
-                    self._log_msg(
-                        task_name,
-                        f"increasing {resource} counter to "
-                        f"{running_pid_counters[pid]}",
-                        logging.DEBUG,
-                    )
-                else:
-                    running_pid_counters[pid] = 0
-                    msg = f"reset {resource} counter"
-                    self._log_msg(task_name, msg, logging.DEBUG)
-                running_pid_usages[pid] = current_usage
-                if running_pid_counters[pid] >= self._refresh_patience:
-                    d_usage = current_usage - checkpoint_usage
-                    self._log_msg(
-                        task_name,
-                        f"delta {resource} usage : {d_usage} MB",
-                        logging.DEBUG,
-                    )
-                    checkpoint_pid_usages[pid] = current_usage
-                    inference_frees = info["inference_frees"]
-                    actual_frees = info["get_available_dict"]()
-                    inference_frees[info["pid2resource_id"][pid]] -= d_usage
-                    self._log_block_msg(
-                        task_name,
-                        f"inference {resource} frees after updating delta usage",
-                        self.get_dict_block_msg(inference_frees),
-                        logging.DEBUG,
-                    )
-                    self._log_block_msg(
-                        task_name,
-                        f"actual {resource} frees",
-                        self.get_dict_block_msg(actual_frees),
-                        logging.DEBUG,
-                    )
-                    running_pid_counters[pid] = 0
-                    msg = f"reset {resource} counter"
-                    self._log_msg(task_name, msg, logging.DEBUG)
-
-    def get_process(
-        self,
-        task_idx: int,
-        sleep_method: Callable,
-        start: bool,
-    ) -> Dict[str, Any]:
-        task_name = self._get_task_name(task_idx)
-        results: Dict[str, Any] = {
-            "__task_name__": task_name,
-            "__create_process__": True,
-        }
-        for resource in self._resources:
-            info = self._info_dict[resource]
-            local_results = results.setdefault(resource, {})
-            preset_usage = info["preset_usages"].setdefault(
-                task_idx,
-                self.default_usage(resource),
-            )
-            self._log_with_meta(
-                task_name,
-                f"preset {resource} usage : {preset_usage} MB; "
-                f"minimum {resource} memory needed : {info['minimum_resource']} MB",
-            )
-            try:
-                while True:
-                    inference_frees, minimum_resource = map(
-                        info.get,
-                        ["inference_frees", "minimum_resource"],
-                    )
-                    self._log_msg(task_name, f"checking {resource}")
-                    if len(inference_frees) == 1:
-                        tgt_resource_id = next(iter(inference_frees.keys()))
-                        free_memory = inference_frees[tgt_resource_id]
-                    else:
-                        tgt_resource_id, free_memory = sorted(
-                            inference_frees.items(), key=lambda kv: kv[1]
-                        )[-1]
-                    self._log_msg(
-                        task_name,
-                        f"best choice : {resource} {tgt_resource_id} with "
-                        f"{free_memory} MB free memory",
-                        logging.DEBUG,
-                    )
-                    local_results["preset_usage"] = preset_usage
-                    local_results["tgt_resource_id"] = tgt_resource_id
-                    if preset_usage < free_memory - minimum_resource:
-                        self._log_msg(
-                            task_name,
-                            f"acceptable, {resource} checked",
-                            logging.DEBUG,
-                        )
-                        break
-                    if not start:
-                        self._log_msg(
-                            task_name,
-                            "not acceptable, also break out because it's initializing",
-                            logging.DEBUG,
-                        )
-                        results["__create_process__"] = False
-                        break
-                    self._log_msg(task_name, "not acceptable, waiting", logging.DEBUG)
-                    sleep_method()
-                if results["__create_process__"]:
-                    inference_frees[tgt_resource_id] -= preset_usage
-            except KeyboardInterrupt:
-                results["__create_process__"] = False
-                return results
-        return results
-
-    def record_process(
-        self,
-        task_idx: int,
-        process: psutil.Process,
-        rs: Dict[str, Any],
-    ) -> None:
-        pid = process.pid
-        task_name = self._get_task_name(task_idx)
-        rs_task_name = rs["__task_name__"]
-        assert_msg = f"internal error occurred, {task_name} != {rs_task_name}"
-        assert task_name == rs_task_name, assert_msg
-        task_info, overwritten = None, False
-        self.pid2task_idx[pid] = task_idx
-        for resource in self._resources:
-            local_rs = rs[resource]
-            info = self._info_dict[resource]
-            pid2resource_id = info["pid2resource_id"]
-            checkpoint_pid_usages, running_pid_usages, running_pid_counters = map(
-                info.get,
-                [
-                    "checkpoint_pid_usages",
-                    "running_pid_usages",
-                    "running_pid_counters",
-                ],
-            )
-            if pid in pid2resource_id:
-                self._log_with_meta(
-                    task_name,
-                    f"pid ({pid}) collision started for {resource}",
-                    logging.WARNING,
-                )
-                if not overwritten:
-                    overwritten = True
-                    task_info = self._overwritten_task_info.setdefault(task_name, {})
-                    task_info["pid"], task_info["task_idx"] = (
-                        pid,
-                        self.pid2task_idx[pid],
-                    )
-                task_resource_info = task_info.setdefault(f"{resource}_info", {})
-                task_resource_info["ckpt_usage"] = checkpoint_pid_usages[pid]
-                task_resource_info["running_usage"] = running_pid_usages[pid]
-                task_resource_info["resource_id"] = pid2resource_id[pid]
-            running_pid_counters[pid] = 0
-            resource_id = pid2resource_id[pid] = local_rs["tgt_resource_id"]
-            usage = local_rs["preset_usage"]
-            checkpoint_pid_usages[pid] = running_pid_usages[pid] = usage
-            self._log_with_meta(
-                task_name,
-                f"record : using {resource} {resource_id} with {usage} MB "
-                f"memory usage (pid : {pid})",
-            )
-
-    def handle_finish(self, task_idx: int, process: psutil.Process) -> Optional[str]:
-        if process is None:
-            return
-        pid = process.pid
-        task_name = self._get_task_name(task_idx)
-        self._init_logger(task_name)
-        task_info = None
-        if task_name not in self._overwritten_task_info:
-            pid_task_idx = self.pid2task_idx.pop(pid)
-        else:
-            task_info = self._overwritten_task_info.pop(task_name)
-            recorded_pid, pid_task_idx = map(task_info.get, ["pid", "task_idx"])
-            assert_msg = f"internal error occurred ({pid} != {recorded_pid})"
-            assert pid == recorded_pid, assert_msg
-        msg = "task_idx should be identical with pid_task_idx, internal error occurred"
-        assert task_idx == pid_task_idx, msg
-        for resource in self._resources:
-            resource_info = self._info_dict[resource]
-            if task_info is not None:
-                task_resource_info = task_info[f"{resource}_info"]
-                resource_id = task_resource_info["resource_id"]
-                pid_ckpt_usage, pid_running_usage = map(
-                    task_resource_info.get, ["ckpt_usage", "running_usage"]
-                )
-                self._log_with_meta(
-                    task_name,
-                    f"pid ({pid}) collision ended for {resource}",
-                    logging.WARNING,
-                )
-            else:
-                pid_ckpt_usage, pid_running_usage, _ = map(
-                    dict.pop,
-                    [
-                        resource_info["checkpoint_pid_usages"],
-                        resource_info["running_pid_usages"],
-                        resource_info["running_pid_counters"],
-                    ],
-                    [pid] * 3,
-                )
-                resource_id = resource_info["pid2resource_id"].pop(pid)
-            pid_usage = pid_running_usage
-            if pid_running_usage != pid_ckpt_usage:
-                self._log_with_meta(
-                    task_name,
-                    f"running pid {resource} usage ({pid_running_usage}) != "
-                    f"checkpoint pid {resource} usage ({pid_ckpt_usage}), "
-                    f"checkpoint {resource} usage will be used to inference "
-                    f"{resource} free",
-                    logging.WARNING,
-                )
-                pid_usage = pid_ckpt_usage
-            preset_usage = resource_info["preset_usages"][task_idx]
-            if pid_running_usage >= preset_usage + resource_info["warning_threshold"]:
-                self._log_with_meta(
-                    task_name,
-                    f"running pid {resource} usage ({pid_running_usage}) exceeded "
-                    f"preset cuda {resource} usage ({preset_usage}) so much, "
-                    f"it may cause {resource} out of memory",
-                    logging.WARNING,
-                )
-            self._log_with_meta(
-                task_name,
-                f"finished, releasing {pid_ckpt_usage} MB (inference) memory "
-                f"from {resource} {resource_id}",
-            )
-            inference_frees = resource_info["inference_frees"]
-            inference_frees[resource_id] += pid_usage
-            for name in [task_name, self._meta_log_name]:
-                self._log_block_msg(
-                    name,
-                    f"inference {resource} frees after releasing",
-                    self.get_dict_block_msg(inference_frees),
-                    logging.DEBUG,
-                )
-                self._log_block_msg(
-                    name,
-                    f"actual {resource} frees",
-                    self.get_dict_block_msg(resource_info["get_available_dict"]()),
-                    logging.DEBUG,
-                )
-        return task_name
-
-
-__all__ = ["PCManager", "GPUManager", "ResourceManager"]
+import psutil
+import logging
+import subprocess
+
+from typing import Any
+from typing import Dict
+from typing import List
+from typing import Tuple
+from typing import Union
+from typing import Callable
+from typing import Optional
+from collections import defaultdict
+
+from .misc import PureLoggingMixin
+
+
+class PCManager:
+    """Util class which can check PC status (unit: MB)."""
+
+    @staticmethod
+    def get_available_ram() -> float:
+        return psutil.virtual_memory().available / 1024**2
+
+    @staticmethod
+    def get_pid_ram_usage(pid: int) -> float:
+        try:
+            process = psutil.Process(pid)
+        except psutil.NoSuchProcess:
+            return 0.0
+        return process.memory_info().rss / 1024**2
+
+
+class GPUManager:
+    """
+    Util class which can check CUDA usages.
+
+    Parameters
+    ----------
+    available_cuda_list : {None, list}, indicates CUDAs which are available.
+    * If None, then all CUDAs will be available.
+    reuse : bool, indicates whether one CUDA could be used multiple times.
+    * If `available_cuda_list` is None, then `reuse` will have no effect.
+
+    Examples
+    --------
+    >>> available_cuda_list = list(range(8))  # indicates that CUDA-0, ..., CUDA-7 is available
+    >>> cuda = GPUManager(available_cuda_list).choose()  # `cuda` will be the CUDA id with most memory
+
+    """
+
+    def __init__(
+        self,
+        available_cuda_list: Optional[List[Union[str, int]]] = None,
+        *,
+        reuse: bool = True,
+    ):
+        self._reuse = reuse
+        if available_cuda_list is None:
+            self._available_cuda = None
+        else:
+            self._available_cuda = set(map(int, available_cuda_list))
+
+    @staticmethod
+    def _query_gpu() -> List[Dict[str, int]]:
+        q_args = ["index", "gpu_name", "memory.free", "memory.total"]
+        cmd = f"nvidia-smi --query-gpu={','.join(q_args)} --format=csv,noheader"
+        results = subprocess.Popen(
+            cmd,
+            shell=True,
+            stdout=subprocess.PIPE,
+            close_fds=True,
+        ).communicate()[0]
+        results = list(filter(bool, results.decode("utf-8").strip().split("\n")))
+
+        def _parse(line):
+            numeric_args = ["memory.free", "memory.total"]
+            power_manage_enable = lambda v: ("Not Support" not in v)
+            to_numeric = lambda v: float(
+                v.upper().strip().replace("MIB", "").replace("W", "")
+            )
+            process = lambda k, v: (
+                (int(to_numeric(v)) if power_manage_enable(v) else 1)
+                if k in numeric_args
+                else v.strip()
+            )
+            rs = {k: process(k, v) for k, v in zip(q_args, line.strip().split(","))}
+            rs["index"] = int(rs["index"])
+            return rs
+
+        return list(map(_parse, results))
+
+    @staticmethod
+    def _query_pid() -> List[Tuple[int, int]]:
+        cmd = "nvidia-smi --query-compute-apps=pid,used_memory --format=csv,noheader"
+        results = subprocess.Popen(
+            cmd,
+            shell=True,
+            stdout=subprocess.PIPE,
+            close_fds=True,
+        ).communicate()[0]
+        results = list(filter(bool, results.decode("utf-8").strip().split("\n")))
+        pid_list = []
+        for line in results:
+            key, value = map(int, line.replace("MiB", "").strip().split(", "))
+            pid_list.append((key, value))
+        return pid_list
+
+    @staticmethod
+    def _sort_by_memory(
+        gpus: List[Dict[str, int]],
+        by_size: bool = False,
+    ) -> List[Dict[str, int]]:
+        if by_size:
+            return sorted(gpus, key=lambda d: d["memory.free"], reverse=True)
+        return sorted(
+            gpus,
+            key=lambda d: float(d["memory.free"]) / d["memory.total"],
+            reverse=True,
+        )
+
+    def _gpu_filter(self, gpu: Dict[str, int]):
+        return self._available_cuda is None or gpu["index"] in self._available_cuda
+
+    def choose(self) -> int:
+        if isinstance(self._available_cuda, set) and not self._available_cuda:
+            raise ValueError("No more CUDAs are available")
+        chosen_gpu = int(
+            next(
+                filter(
+                    self._gpu_filter,
+                    self._sort_by_memory(self._query_gpu(), True),
+                )
+            )["index"]
+        )
+        if not self._reuse and self._available_cuda is not None:
+            self._available_cuda.remove(chosen_gpu)
+        return chosen_gpu
+
+    def get_gpu_frees(self) -> Dict[int, int]:
+        return {
+            gpu["index"]: gpu["memory.free"]
+            for gpu in filter(self._gpu_filter, self._query_gpu())
+        }
+
+    def get_pid_usages(self) -> Dict[int, int]:
+        usages = defaultdict(int)
+        for key, usage in self._query_pid():
+            usages[key] += usage
+        return usages
+
+
+class ResourceManager:
+    """
+    Util class which can monitor & manage resources.
+    * It utilizes `PCManager` & `GPUManager` defined above.
+    * It is currently used in cftool.dist.core.Parallel only.
+
+    """
+
+    def __init__(
+        self,
+        config: Dict[str, Any],
+        get_task_name: Callable[[int], Optional[str]],
+        refresh_patience: int,
+    ):
+        self._resources, self._info_dict, self._overwritten_task_info = [], {}, {}
+        self._init_logger = self._meta_log_name = None
+        self._log_msg = self._log_block_msg = None
+        self._log_meta_msg = self._log_with_meta = None
+        self.pid2task_idx, self._get_task_name = {}, get_task_name
+        self.config, self._refresh_patience = config, refresh_patience
+
+    def register(self, resource_name: str, methods: Dict[str, Callable]) -> None:
+        self._resources.append(resource_name)
+        resource_config = self.config.setdefault(f"{resource_name.lower()}_config", {})
+        preset_usages = resource_config.setdefault("preset_usages", {})
+        minimum_resource = resource_config.setdefault(
+            "minimum_resource",
+            preset_usages.setdefault("__default__", 1024),
+        )
+        counter_threshold = resource_config.setdefault("counter_threshold", 4)
+        warning_threshold = resource_config.setdefault("warning_threshold", 1024)
+        info = self._info_dict.setdefault(
+            resource_name,
+            {
+                "preset_usages": preset_usages,
+                "minimum_resource": minimum_resource,
+                "counter_threshold": counter_threshold,
+                "warning_threshold": warning_threshold,
+            },
+        )
+        get_pid_usage, get_pid_usage_dict, get_available_dict = map(
+            methods.get,
+            ["get_pid_usage", "get_pid_usage_dict", "get_available_dict"],
+        )
+        if get_pid_usage is None and get_pid_usage_dict is None:
+            raise ValueError(
+                "either get_pid_usage or get_pid_usage_dict "
+                "should be provided in methods"
+            )
+        if get_available_dict is None:
+            raise ValueError("get_available_dict should be provided in methods")
+        info["get_pid_usage"] = get_pid_usage
+        info["get_pid_usage_dict"] = get_pid_usage_dict
+        info["get_available_dict"] = get_available_dict
+        info["inference_frees"], info["checkpoint_pid_usages"] = {}, {}
+        info["running_pid_usages"], info["running_pid_counters"] = {}, {}
+        info["inference_usages_initialized"] = False
+        info["pid2resource_id"] = {}
+
+    def register_logging(
+        self,
+        init_logger: Callable[[str], None],
+        mixin: PureLoggingMixin,
+    ):
+        self._init_logger, self._meta_log_name = init_logger, mixin.meta_log_name
+        self._log_msg, self._log_block_msg = mixin.log_msg, mixin.log_block_msg
+        self._log_meta_msg = mixin._log_meta_msg
+        self._log_with_meta = mixin._log_with_meta
+
+    @property
+    def inference_usages_initialized(self) -> bool:
+        for info in self._info_dict.values():
+            if not info["inference_usages_initialized"]:
+                return False
+        return True
+
+    @property
+    def checkpoint_initialized(self) -> bool:
+        for info in self._info_dict.values():
+            if not info["checkpoint_pid_usages"]:
+                return False
+        return True
+
+    @staticmethod
+    def _get_all_relevant_processes(pid: int) -> List[psutil.Process]:
+        parent = psutil.Process(pid)
+        processes = [parent]
+        for process in parent.children(recursive=True):
+            processes.append(process)
+        return processes
+
+    @staticmethod
+    def _get_pid_usages(info: Dict[str, Any]) -> Dict[str, int]:
+        get_pid_usage_dict = info["get_pid_usage_dict"]
+        if get_pid_usage_dict is not None:
+            return get_pid_usage_dict()
+        pid_usages, get_pid_usage = {}, info["get_pid_usage"]
+        for pid in info["running_pid_usages"].keys():
+            try:
+                processes = ResourceManager._get_all_relevant_processes(pid)
+                pid_usages[pid] = int(
+                    sum(get_pid_usage(process.pid) for process in processes)
+                )
+            except psutil.NoSuchProcess:
+                pid_usages[pid] = 0
+        return pid_usages
+
+    @staticmethod
+    def get_dict_block_msg(d: Dict[str, int]) -> str:
+        keys = sorted(d.keys())
+        values = [d[key] for key in keys]
+        header = " | ".join(map(lambda pid: f"{pid:^12s}", map(str, keys)))
+        body = " | ".join(map(lambda usage: f"{int(usage):^10d}MB", values))
+        len_header = len(header)
+        above = f"{'=' * len_header}\n{header}\n{'-' * len_header}"
+        return f"{above}\n{body}\n{'-' * len_header}"
+
+    def default_usage(self, resource: str) -> int:
+        return int(self._info_dict[resource]["preset_usages"]["__default__"])
+
+    def initialize_running_usages(self) -> None:
+        for info in self._info_dict.values():
+            info["running_pid_usages"] = info["checkpoint_pid_usages"].copy()
+
+    def initialize_inference_usages(self) -> None:
+        for info in self._info_dict.values():
+            info["inference_frees"] = info["get_available_dict"]()
+            info["inference_usages_initialized"] = True
+
+    def log_pid_usages_and_inference_frees(self) -> None:
+        for resource in self._resources:
+            info = self._info_dict[resource]
+            self._log_block_msg(
+                self._meta_log_name,
+                f"current pid {resource} usages",
+                self.get_dict_block_msg(self._get_pid_usages(info)),
+                logging.DEBUG,
+            )
+            self._log_block_msg(
+                self._meta_log_name,
+                f"current inference {resource} frees",
+                self.get_dict_block_msg(info["inference_frees"]),
+                logging.DEBUG,
+            )
+
+    def check(self) -> None:
+        for resource in self._resources:
+            info = self._info_dict[resource]
+            checkpoint_pid_usages, running_pid_usages, running_pid_counters = map(
+                info.get,
+                [
+                    "checkpoint_pid_usages",
+                    "running_pid_usages",
+                    "running_pid_counters",
+                ],
+            )
+            get_pid_usage, get_pid_usage_dict = map(
+                info.get,
+                ["get_pid_usage", "get_pid_usage_dict"],
+            )
+            if get_pid_usage is None:
+                pid_usage_dict = get_pid_usage_dict()
+                get_pid_usage = lambda pid_: pid_usage_dict.get(pid_, 0)
+            for pid, checkpoint_usage in checkpoint_pid_usages.items():
+                task_name = self._get_task_name(self.pid2task_idx[pid])
+                self._log_msg(
+                    task_name,
+                    f"checkpoint {resource} usage : {checkpoint_usage} MB",
+                    logging.DEBUG,
+                )
+                children_pid_usages = {}
+                try:
+                    processes = self._get_all_relevant_processes(pid)
+                except psutil.NoSuchProcess as err:
+                    self._log_with_meta(
+                        task_name,
+                        f"already finished, {err}",
+                        logging.INFO,
+                    )
+                    continue
+                current_usage = get_pid_usage(pid)
+                for process in processes[1:]:
+                    process_usage = get_pid_usage(process.pid)
+                    children_pid_usages[process.pid] = process_usage
+                    current_usage += process_usage
+                if children_pid_usages:
+                    self._log_block_msg(
+                        task_name,
+                        f"children {resource} usages",
+                        self.get_dict_block_msg(children_pid_usages),
+                        logging.DEBUG,
+                    )
+                self._log_msg(
+                    task_name,
+                    f"current {resource} usage : {current_usage} MB",
+                    logging.DEBUG,
+                )
+                if current_usage == 0:
+                    continue
+                running_usage = running_pid_usages[pid]
+                self._log_msg(
+                    task_name,
+                    f"running {resource} usage : {running_usage} MB",
+                    logging.DEBUG,
+                )
+                if running_usage > checkpoint_usage:
+                    running_pid_counters[pid] = self._refresh_patience
+                    self._log_msg(
+                        task_name,
+                        f"increasing {resource} counter directly to "
+                        f"{self._refresh_patience}",
+                        logging.DEBUG,
+                    )
+                elif abs(running_usage - current_usage) <= info["counter_threshold"]:
+                    running_pid_counters[pid] += 1
+                    self._log_msg(
+                        task_name,
+                        f"increasing {resource} counter to "
+                        f"{running_pid_counters[pid]}",
+                        logging.DEBUG,
+                    )
+                else:
+                    running_pid_counters[pid] = 0
+                    msg = f"reset {resource} counter"
+                    self._log_msg(task_name, msg, logging.DEBUG)
+                running_pid_usages[pid] = current_usage
+                if running_pid_counters[pid] >= self._refresh_patience:
+                    d_usage = current_usage - checkpoint_usage
+                    self._log_msg(
+                        task_name,
+                        f"delta {resource} usage : {d_usage} MB",
+                        logging.DEBUG,
+                    )
+                    checkpoint_pid_usages[pid] = current_usage
+                    inference_frees = info["inference_frees"]
+                    actual_frees = info["get_available_dict"]()
+                    inference_frees[info["pid2resource_id"][pid]] -= d_usage
+                    self._log_block_msg(
+                        task_name,
+                        f"inference {resource} frees after updating delta usage",
+                        self.get_dict_block_msg(inference_frees),
+                        logging.DEBUG,
+                    )
+                    self._log_block_msg(
+                        task_name,
+                        f"actual {resource} frees",
+                        self.get_dict_block_msg(actual_frees),
+                        logging.DEBUG,
+                    )
+                    running_pid_counters[pid] = 0
+                    msg = f"reset {resource} counter"
+                    self._log_msg(task_name, msg, logging.DEBUG)
+
+    def get_process(
+        self,
+        task_idx: int,
+        sleep_method: Callable,
+        start: bool,
+    ) -> Dict[str, Any]:
+        task_name = self._get_task_name(task_idx)
+        results: Dict[str, Any] = {
+            "__task_name__": task_name,
+            "__create_process__": True,
+        }
+        for resource in self._resources:
+            info = self._info_dict[resource]
+            local_results = results.setdefault(resource, {})
+            preset_usage = info["preset_usages"].setdefault(
+                task_idx,
+                self.default_usage(resource),
+            )
+            self._log_with_meta(
+                task_name,
+                f"preset {resource} usage : {preset_usage} MB; "
+                f"minimum {resource} memory needed : {info['minimum_resource']} MB",
+            )
+            try:
+                while True:
+                    inference_frees, minimum_resource = map(
+                        info.get,
+                        ["inference_frees", "minimum_resource"],
+                    )
+                    self._log_msg(task_name, f"checking {resource}")
+                    if len(inference_frees) == 1:
+                        tgt_resource_id = next(iter(inference_frees.keys()))
+                        free_memory = inference_frees[tgt_resource_id]
+                    else:
+                        tgt_resource_id, free_memory = sorted(
+                            inference_frees.items(), key=lambda kv: kv[1]
+                        )[-1]
+                    self._log_msg(
+                        task_name,
+                        f"best choice : {resource} {tgt_resource_id} with "
+                        f"{free_memory} MB free memory",
+                        logging.DEBUG,
+                    )
+                    local_results["preset_usage"] = preset_usage
+                    local_results["tgt_resource_id"] = tgt_resource_id
+                    if preset_usage < free_memory - minimum_resource:
+                        self._log_msg(
+                            task_name,
+                            f"acceptable, {resource} checked",
+                            logging.DEBUG,
+                        )
+                        break
+                    if not start:
+                        self._log_msg(
+                            task_name,
+                            "not acceptable, also break out because it's initializing",
+                            logging.DEBUG,
+                        )
+                        results["__create_process__"] = False
+                        break
+                    self._log_msg(task_name, "not acceptable, waiting", logging.DEBUG)
+                    sleep_method()
+                if results["__create_process__"]:
+                    inference_frees[tgt_resource_id] -= preset_usage
+            except KeyboardInterrupt:
+                results["__create_process__"] = False
+                return results
+        return results
+
+    def record_process(
+        self,
+        task_idx: int,
+        process: psutil.Process,
+        rs: Dict[str, Any],
+    ) -> None:
+        pid = process.pid
+        task_name = self._get_task_name(task_idx)
+        rs_task_name = rs["__task_name__"]
+        assert_msg = f"internal error occurred, {task_name} != {rs_task_name}"
+        assert task_name == rs_task_name, assert_msg
+        task_info, overwritten = None, False
+        self.pid2task_idx[pid] = task_idx
+        for resource in self._resources:
+            local_rs = rs[resource]
+            info = self._info_dict[resource]
+            pid2resource_id = info["pid2resource_id"]
+            checkpoint_pid_usages, running_pid_usages, running_pid_counters = map(
+                info.get,
+                [
+                    "checkpoint_pid_usages",
+                    "running_pid_usages",
+                    "running_pid_counters",
+                ],
+            )
+            if pid in pid2resource_id:
+                self._log_with_meta(
+                    task_name,
+                    f"pid ({pid}) collision started for {resource}",
+                    logging.WARNING,
+                )
+                if not overwritten:
+                    overwritten = True
+                    task_info = self._overwritten_task_info.setdefault(task_name, {})
+                    task_info["pid"], task_info["task_idx"] = (
+                        pid,
+                        self.pid2task_idx[pid],
+                    )
+                task_resource_info = task_info.setdefault(f"{resource}_info", {})
+                task_resource_info["ckpt_usage"] = checkpoint_pid_usages[pid]
+                task_resource_info["running_usage"] = running_pid_usages[pid]
+                task_resource_info["resource_id"] = pid2resource_id[pid]
+            running_pid_counters[pid] = 0
+            resource_id = pid2resource_id[pid] = local_rs["tgt_resource_id"]
+            usage = local_rs["preset_usage"]
+            checkpoint_pid_usages[pid] = running_pid_usages[pid] = usage
+            self._log_with_meta(
+                task_name,
+                f"record : using {resource} {resource_id} with {usage} MB "
+                f"memory usage (pid : {pid})",
+            )
+
+    def handle_finish(self, task_idx: int, process: psutil.Process) -> Optional[str]:
+        if process is None:
+            return
+        pid = process.pid
+        task_name = self._get_task_name(task_idx)
+        self._init_logger(task_name)
+        task_info = None
+        if task_name not in self._overwritten_task_info:
+            pid_task_idx = self.pid2task_idx.pop(pid)
+        else:
+            task_info = self._overwritten_task_info.pop(task_name)
+            recorded_pid, pid_task_idx = map(task_info.get, ["pid", "task_idx"])
+            assert_msg = f"internal error occurred ({pid} != {recorded_pid})"
+            assert pid == recorded_pid, assert_msg
+        msg = "task_idx should be identical with pid_task_idx, internal error occurred"
+        assert task_idx == pid_task_idx, msg
+        for resource in self._resources:
+            resource_info = self._info_dict[resource]
+            if task_info is not None:
+                task_resource_info = task_info[f"{resource}_info"]
+                resource_id = task_resource_info["resource_id"]
+                pid_ckpt_usage, pid_running_usage = map(
+                    task_resource_info.get, ["ckpt_usage", "running_usage"]
+                )
+                self._log_with_meta(
+                    task_name,
+                    f"pid ({pid}) collision ended for {resource}",
+                    logging.WARNING,
+                )
+            else:
+                pid_ckpt_usage, pid_running_usage, _ = map(
+                    dict.pop,
+                    [
+                        resource_info["checkpoint_pid_usages"],
+                        resource_info["running_pid_usages"],
+                        resource_info["running_pid_counters"],
+                    ],
+                    [pid] * 3,
+                )
+                resource_id = resource_info["pid2resource_id"].pop(pid)
+            pid_usage = pid_running_usage
+            if pid_running_usage != pid_ckpt_usage:
+                self._log_with_meta(
+                    task_name,
+                    f"running pid {resource} usage ({pid_running_usage}) != "
+                    f"checkpoint pid {resource} usage ({pid_ckpt_usage}), "
+                    f"checkpoint {resource} usage will be used to inference "
+                    f"{resource} free",
+                    logging.WARNING,
+                )
+                pid_usage = pid_ckpt_usage
+            preset_usage = resource_info["preset_usages"][task_idx]
+            if pid_running_usage >= preset_usage + resource_info["warning_threshold"]:
+                self._log_with_meta(
+                    task_name,
+                    f"running pid {resource} usage ({pid_running_usage}) exceeded "
+                    f"preset cuda {resource} usage ({preset_usage}) so much, "
+                    f"it may cause {resource} out of memory",
+                    logging.WARNING,
+                )
+            self._log_with_meta(
+                task_name,
+                f"finished, releasing {pid_ckpt_usage} MB (inference) memory "
+                f"from {resource} {resource_id}",
+            )
+            inference_frees = resource_info["inference_frees"]
+            inference_frees[resource_id] += pid_usage
+            for name in [task_name, self._meta_log_name]:
+                self._log_block_msg(
+                    name,
+                    f"inference {resource} frees after releasing",
+                    self.get_dict_block_msg(inference_frees),
+                    logging.DEBUG,
+                )
+                self._log_block_msg(
+                    name,
+                    f"actual {resource} frees",
+                    self.get_dict_block_msg(resource_info["get_available_dict"]()),
+                    logging.DEBUG,
+                )
+        return task_name
+
+
+__all__ = ["PCManager", "GPUManager", "ResourceManager"]
```

### Comparing `carefree-toolkit-0.3.6.3/cftool/misc.py` & `carefree-toolkit-0.3.6.4/cftool/misc.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,2554 +1,2554 @@
-import os
-import sys
-import dill
-import json
-import math
-import time
-import errno
-import random
-import shutil
-import decimal
-import inspect
-import logging
-import hashlib
-import zipfile
-import operator
-import threading
-import unicodedata
-
-import numpy as np
-
-from abc import abstractmethod
-from abc import ABC
-from abc import ABCMeta
-from tqdm import tqdm
-from typing import Any
-from typing import Set
-from typing import Dict
-from typing import List
-from typing import Type
-from typing import Union
-from typing import Generic
-from typing import TypeVar
-from typing import Callable
-from typing import Iterable
-from typing import Optional
-from typing import Protocol
-from typing import NamedTuple
-from argparse import Namespace
-from datetime import datetime
-from datetime import timedelta
-from functools import reduce
-from functools import partial
-from itertools import product
-from collections import OrderedDict
-from dataclasses import asdict
-from dataclasses import fields
-from dataclasses import dataclass
-from dataclasses import Field
-
-from .types import configs_type
-from .types import np_dict_type
-from .types import general_config_type
-from .constants import TIME_FORMAT
-
-
-dill._dill._reverse_typemap["ClassType"] = type
-
-
-# util functions
-
-
-TFnResponse = TypeVar("TFnResponse")
-
-
-class Fn(Protocol):
-    def __call__(self, *args: Any, **kwargs: Any) -> TFnResponse:
-        pass
-
-
-def walk(
-    root: str,
-    hierarchy_callback: Callable[[List[str], str], None],
-    filter_extensions: Optional[Set[str]] = None,
-) -> None:
-    walked = list(os.walk(root))
-    for folder, _, files in tqdm(walked, desc="folders", position=0, mininterval=1):
-        for file in tqdm(files, desc="files", position=1, leave=False, mininterval=1):
-            if filter_extensions is not None:
-                if not any(file.endswith(ext) for ext in filter_extensions):
-                    continue
-            hierarchy = folder.split(os.path.sep) + [file]
-            hierarchy_callback(hierarchy, os.path.join(folder, file))
-
-
-def parse_config(config: general_config_type) -> Dict[str, Any]:
-    if config is None:
-        return {}
-    if isinstance(config, str):
-        with open(config, "r") as f:
-            return json.load(f)
-    return shallow_copy_dict(config)
-
-
-def check_requires(fn: Any, name: str, strict: bool = True) -> bool:
-    if isinstance(fn, type):
-        fn = fn.__init__  # type: ignore
-    signature = inspect.signature(fn)
-    for k, param in signature.parameters.items():
-        if not strict and param.kind is inspect.Parameter.VAR_KEYWORD:
-            return True
-        if k == name:
-            if param.kind is inspect.Parameter.VAR_POSITIONAL:
-                return False
-            return True
-    return False
-
-
-def get_requirements(fn: Any) -> List[str]:
-    if isinstance(fn, type):
-        fn = fn.__init__  # type: ignore
-    requirements = []
-    signature = inspect.signature(fn)
-    for k, param in signature.parameters.items():
-        if param.kind is inspect.Parameter.VAR_KEYWORD:
-            continue
-        if param.kind is inspect.Parameter.VAR_POSITIONAL:
-            continue
-        if param.default is not inspect.Parameter.empty:
-            continue
-        requirements.append(k)
-    return requirements
-
-
-def filter_kw(
-    fn: Callable,
-    kwargs: Dict[str, Any],
-    *,
-    strict: bool = False,
-) -> Dict[str, Any]:
-    kw = {}
-    for k, v in kwargs.items():
-        if check_requires(fn, k, strict):
-            kw[k] = v
-    return kw
-
-
-def safe_execute(fn: Fn, kw: Dict[str, Any], *, strict: bool = False) -> TFnResponse:
-    return fn(**filter_kw(fn, kw, strict=strict))
-
-
-def get_num_positional_args(fn: Callable) -> Union[int, float]:
-    signature = inspect.signature(fn)
-    counter = 0
-    for param in signature.parameters.values():
-        if param.kind is inspect.Parameter.VAR_POSITIONAL:
-            return math.inf
-        if param.kind is inspect.Parameter.POSITIONAL_ONLY:
-            counter += 1
-        elif param.kind is inspect.Parameter.POSITIONAL_OR_KEYWORD:
-            counter += 1
-    return counter
-
-
-def prepare_workspace_from(
-    workspace: str,
-    *,
-    timeout: timedelta = timedelta(30),
-    make: bool = True,
-) -> str:
-    current_time = datetime.now()
-    if os.path.isdir(workspace):
-        for stuff in os.listdir(workspace):
-            if not os.path.isdir(os.path.join(workspace, stuff)):
-                continue
-            try:
-                stuff_time = datetime.strptime(stuff, TIME_FORMAT)
-                stuff_delta = current_time - stuff_time
-                if stuff_delta > timeout:
-                    msg = f"{stuff} will be removed (already {stuff_delta} ago)"
-                    print_warning(msg)
-                    shutil.rmtree(os.path.join(workspace, stuff))
-            except:
-                pass
-    workspace = os.path.join(workspace, current_time.strftime(TIME_FORMAT))
-    if make:
-        os.makedirs(workspace)
-    return workspace
-
-
-def get_latest_workspace(root: str) -> Optional[str]:
-    if not os.path.isdir(root):
-        return None
-    all_workspaces = []
-    for stuff in os.listdir(root):
-        if not os.path.isdir(os.path.join(root, stuff)):
-            continue
-        try:
-            datetime.strptime(stuff, TIME_FORMAT)
-            all_workspaces.append(stuff)
-        except:
-            pass
-    if not all_workspaces:
-        return None
-    return os.path.join(root, sorted(all_workspaces)[-1])
-
-
-def sort_dict_by_value(d: Dict[Any, Any], *, reverse: bool = False) -> OrderedDict:
-    sorted_items = sorted([(v, k) for k, v in d.items()], reverse=reverse)
-    return OrderedDict({item[1]: item[0] for item in sorted_items})
-
-
-def parse_args(args: Any) -> Namespace:
-    return Namespace(**{k: None if not v else v for k, v in args.__dict__.items()})
-
-
-def get_arguments(
-    *,
-    num_back: int = 0,
-    pop_class_attributes: bool = True,
-) -> Dict[str, Any]:
-    frame = inspect.currentframe().f_back  # type: ignore
-    for _ in range(num_back):
-        frame = frame.f_back
-    if frame is None:
-        raise ValueError("`get_arguments` should be called inside a frame")
-    arguments = inspect.getargvalues(frame)[-1]
-    if pop_class_attributes:
-        arguments.pop("self", None)
-        arguments.pop("__class__", None)
-    return arguments
-
-
-def _rmtree(folder: str, patience: float = 10.0) -> None:
-    if not os.path.isdir(folder):
-        return None
-    t = time.time()
-    while True:
-        try:
-            if time.time() - t >= patience:
-                print()
-                print_warning(f"failed to rmtree: {folder}")
-                break
-            shutil.rmtree(folder)
-            break
-        except:
-            print("", end=".", flush=True)
-            time.sleep(1)
-
-
-def timestamp(simplify: bool = False, ensure_different: bool = False) -> str:
-    """
-    Return current timestamp.
-
-    Parameters
-    ----------
-    simplify : bool. If True, format will be simplified to 'year-month-day'.
-    ensure_different : bool. If True, format will include millisecond.
-
-    Returns
-    -------
-    timestamp : str
-
-    """
-
-    now = datetime.now()
-    if simplify:
-        return now.strftime("%Y-%m-%d")
-    if ensure_different:
-        return now.strftime("%Y-%m-%d_%H-%M-%S-%f")
-    return now.strftime("%Y-%m-%d_%H-%M-%S")
-
-
-def prod(iterable: Iterable) -> float:
-    """Return cumulative production of an iterable."""
-
-    return float(reduce(operator.mul, iterable, 1))
-
-
-def hash_code(code: str) -> str:
-    """Return hash code for a string."""
-
-    code = code.encode()
-    return hashlib.md5(code).hexdigest()
-
-
-def hash_dict(d: Dict[str, Any]) -> str:
-    """Return a consistent hash code for an arbitrary dict."""
-
-    def _hash(_d: Dict[str, Any]) -> str:
-        sorted_keys = sorted(_d)
-        hashes = []
-        for k in sorted_keys:
-            v = _d[k]
-            if isinstance(v, dict):
-                hashes.append(_hash(v))
-            elif isinstance(v, set):
-                hashes.append(hash_code(str(sorted(v))))
-            else:
-                hashes.append(hash_code(str(v)))
-        return hash_code("".join(hashes))
-
-    return _hash(d)
-
-
-def random_hash() -> str:
-    return hash_code(str(random.random()))
-
-
-def prefix_dict(d: Dict[str, Any], prefix: str):
-    """Prefix every key in dict `d` with `prefix`."""
-
-    return {f"{prefix}_{k}": v for k, v in d.items()}
-
-
-def shallow_copy_dict(d: dict) -> dict:
-    d = d.copy()
-    for k, v in d.items():
-        if isinstance(v, dict):
-            d[k] = shallow_copy_dict(v)
-    return d
-
-
-def update_dict(src_dict: dict, tgt_dict: dict) -> dict:
-    """
-    Update tgt_dict with src_dict.
-    * Notice that changes will happen only on keys which src_dict holds.
-
-    Parameters
-    ----------
-    src_dict : dict
-    tgt_dict : dict
-
-    Returns
-    -------
-    tgt_dict : dict
-
-    """
-
-    for k, v in src_dict.items():
-        tgt_v = tgt_dict.get(k)
-        if tgt_v is None:
-            tgt_dict[k] = v
-        elif not isinstance(v, dict):
-            tgt_dict[k] = v
-        else:
-            update_dict(v, tgt_v)
-    return tgt_dict
-
-
-def fix_float_to_length(num: float, length: int) -> str:
-    """Change a float number to string format with fixed length."""
-
-    ctx = decimal.Context()
-    ctx.prec = 2 * length
-    d = ctx.create_decimal(repr(num))
-    str_num = format(d, "f").lower()
-    if str_num == "nan":
-        return f"{str_num:^{length}s}"
-    idx = str_num.find(".")
-    if idx == -1:
-        diff = length - len(str_num)
-        if diff <= 0:
-            return str_num
-        if diff == 1:
-            return f"{str_num}."
-        return f"{str_num}.{'0' * (diff - 1)}"
-    length = max(length, idx)
-    return str_num[:length].ljust(length, "0")
-
-
-def truncate_string_to_length(string: str, length: int) -> str:
-    """Truncate a string to make sure its length not exceeding a given length."""
-
-    if len(string) <= length:
-        return string
-    half_length = int(0.5 * length) - 1
-    head = string[:half_length]
-    tail = string[-half_length:]
-    return f"{head}{'.' * (length - 2 * half_length)}{tail}"
-
-
-def grouped(iterable: Iterable, n: int, *, keep_tail: bool = False) -> List[tuple]:
-    """Group an iterable every `n` elements."""
-
-    if not keep_tail:
-        return list(zip(*[iter(iterable)] * n))
-    with batch_manager(iterable, batch_size=n, max_batch_size=n) as manager:
-        return [tuple(batch) for batch in manager]
-
-
-def grouped_into(iterable: Iterable, n: int) -> List[tuple]:
-    """Group an iterable into `n` groups."""
-
-    elements = list(iterable)
-    num_elements = len(elements)
-    num_elem_per_group = int(math.ceil(num_elements / n))
-    results: List[tuple] = []
-    split_idx = num_elements + n - n * num_elem_per_group
-    start = 0
-    for i in range(split_idx):
-        end = start + num_elem_per_group
-        results.append(tuple(elements[start:end]))
-        start = end
-    for i in range(split_idx, n):
-        end = start + num_elem_per_group - 1
-        results.append(tuple(elements[start:end]))
-        start = end
-    return results
-
-
-def is_numeric(s: Any) -> bool:
-    """Check whether `s` is a number."""
-
-    try:
-        s = float(s)
-        return True
-    except (TypeError, ValueError):
-        try:
-            unicodedata.numeric(s)
-            return True
-        except (TypeError, ValueError):
-            return False
-
-
-def register_core(
-    name: str,
-    global_dict: Dict[str, type],
-    *,
-    allow_duplicate: bool = False,
-    before_register: Optional[Callable] = None,
-    after_register: Optional[Callable] = None,
-):
-    def _register(cls):
-        if before_register is not None:
-            before_register(cls)
-        registered = global_dict.get(name)
-        if registered is not None and not allow_duplicate:
-            print_warning(
-                f"'{name}' has already registered "
-                f"in the given global dict ({global_dict})"
-            )
-            return cls
-        global_dict[name] = cls
-        if after_register is not None:
-            after_register(cls)
-        return cls
-
-    return _register
-
-
-def check(constraints: Dict[str, Union[str, List[str]]], *, raise_error: bool = True):
-    def wrapper(fn):
-        def _check_core(k, v):
-            new_v = v
-            constraint_list = constraints.get(k)
-            if constraint_list is not None:
-                if isinstance(constraint_list, str):
-                    constraint_list = [constraint_list]
-                if constraint_list[0] == "choices":
-                    choices = constraint_list[1]
-                    if v not in choices:
-                        raise ValueError(
-                            f"given value ({v}) is not included in "
-                            f"given choices ({choices})"
-                        )
-                else:
-                    for constraint in constraint_list:
-                        check_rs = getattr(SanityChecker, constraint)(v)
-                        if not check_rs["suc"]:
-                            raise ValueError(check_rs["info"])
-                        new_v = check_rs["n"]
-            if v != new_v:
-                if raise_error:
-                    raise ValueError(
-                        f"'{k}' ({v}, {type(v)}) does not satisfy "
-                        f"Constraints({constraint_list})"
-                    )
-                print_warning(f"'{k}' is cast from {v} -> {new_v}")
-            return new_v
-
-        def inner(*args, **kwargs):
-            signature_keys = list(inspect.signature(fn).parameters.keys())
-            new_args = []
-            for arg, signature_key in zip(args, signature_keys[: len(args)]):
-                new_args.append(_check_core(signature_key, arg))
-            new_kwargs = {}
-            for k, v in kwargs.items():
-                new_kwargs[k] = _check_core(k, v)
-            return fn(*new_args, **new_kwargs)
-
-        return inner
-
-    return wrapper
-
-
-def get_err_msg(err: Exception) -> str:
-    return " | ".join(map(repr, sys.exc_info()[:2] + (str(err),)))
-
-
-# util modules
-
-
-TRegister = TypeVar("TRegister", bound="WithRegister", covariant=True)
-TSerializable = TypeVar("TSerializable", bound="ISerializable", covariant=True)
-TSerializableArrays = TypeVar(
-    "TSerializableArrays",
-    bound="ISerializableArrays",
-    covariant=True,
-)
-TSArrays = TypeVar("TSArrays", bound="ISerializableArrays", covariant=True)
-TSDataClass = TypeVar("TSDataClass", bound="ISerializableDataClass", covariant=True)
-TDataClass = TypeVar("TDataClass", bound="DataClassBase")
-
-
-@dataclass
-class DataClassBase(ABC):
-    @property
-    def fields(self) -> List[Field]:
-        return fields(self)
-
-    @property
-    def field_names(self) -> List[str]:
-        return [f.name for f in self.fields]
-
-    @property
-    def attributes(self) -> List[Any]:
-        return [getattr(self, name) for name in self.field_names]
-
-    def asdict(self) -> Dict[str, Any]:
-        return asdict(self)
-
-    def copy(self: TDataClass) -> TDataClass:
-        return type(self)(**shallow_copy_dict(asdict(self)))
-
-    def update_with(self: TDataClass, other: TDataClass) -> TDataClass:
-        d = update_dict(other.asdict(), self.asdict())
-        return self.__class__(**d)
-
-
-class WithRegister(Generic[TRegister]):
-    d: Dict[str, Type[TRegister]]
-    __identifier__: str
-
-    @classmethod
-    def get(cls: Type[TRegister], name: str) -> Type[TRegister]:
-        return cls.d[name]
-
-    @classmethod
-    def has(cls, name: str) -> bool:
-        return name in cls.d
-
-    @classmethod
-    def make(
-        cls: Type[TRegister],
-        name: str,
-        config: Dict[str, Any],
-        *,
-        ensure_safe: bool = False,
-    ) -> TRegister:
-        base = cls.get(name)
-        if not ensure_safe:
-            return base(**config)  # type: ignore
-        return safe_execute(base, config)
-
-    @classmethod
-    def make_multiple(
-        cls: Type[TRegister],
-        names: Union[str, List[str]],
-        configs: configs_type = None,
-        *,
-        ensure_safe: bool = False,
-    ) -> List[TRegister]:
-        if configs is None:
-            configs = {}
-        if isinstance(names, str):
-            assert isinstance(configs, dict)
-            return cls.make(names, configs, ensure_safe=ensure_safe)  # type: ignore
-        if not isinstance(configs, list):
-            configs = [configs.get(name, {}) for name in names]
-        return [
-            cls.make(name, shallow_copy_dict(config), ensure_safe=ensure_safe)
-            for name, config in zip(names, configs)
-        ]
-
-    @classmethod
-    def register(
-        cls,
-        name: str,
-        *,
-        allow_duplicate: bool = False,
-    ) -> Callable:
-        def before(cls_: Type) -> None:
-            cls_.__identifier__ = name
-
-        return register_core(
-            name,
-            cls.d,
-            allow_duplicate=allow_duplicate,
-            before_register=before,
-        )
-
-    @classmethod
-    def remove(cls, name: str) -> Callable:
-        return cls.d.pop(name)
-
-    @classmethod
-    def check_subclass(cls, name: str) -> bool:
-        return issubclass(cls.d[name], cls)
-
-
-@dataclass
-class JsonPack(DataClassBase):
-    type: str
-    info: Dict[str, Any]
-
-
-class ISerializable(WithRegister, Generic[TSerializable], metaclass=ABCMeta):
-    # abstract
-
-    @abstractmethod
-    def to_info(self) -> Dict[str, Any]:
-        pass
-
-    @abstractmethod
-    def from_info(self, info: Dict[str, Any]) -> None:
-        pass
-
-    # optional callbacks
-
-    def after_load(self) -> None:
-        pass
-
-    # api
-
-    def to_pack(self) -> JsonPack:
-        return JsonPack(self.__identifier__, self.to_info())
-
-    @classmethod
-    def from_pack(cls: Type[TSerializable], pack: Dict[str, Any]) -> TSerializable:
-        obj: ISerializable = cls.make(pack["type"], {})
-        obj.from_info(pack["info"])
-        obj.after_load()
-        return obj
-
-    def to_json(self) -> str:
-        return json.dumps(self.to_pack().asdict())
-
-    @classmethod
-    def from_json(cls: Type[TSerializable], json_string: str) -> TSerializable:
-        return cls.from_pack(json.loads(json_string))
-
-    def copy(self: TSerializable) -> TSerializable:
-        copied = self.__class__()
-        copied.from_info(shallow_copy_dict(self.to_info()))
-        return copied
-
-
-class PureFromInfoMixin:
-    def from_info(self, info: Dict[str, Any]) -> None:
-        for k, v in info.items():
-            setattr(self, k, v)
-
-
-class ISerializableArrays(ISerializable, Generic[TSArrays], metaclass=ABCMeta):
-    @abstractmethod
-    def to_npd(self) -> np_dict_type:
-        pass
-
-    @abstractmethod
-    def from_npd(self, npd: np_dict_type) -> None:
-        pass
-
-    def copy(self: TSerializableArrays) -> TSerializableArrays:
-        copied: TSerializableArrays = super().copy()
-        copied.from_npd(shallow_copy_dict(self.to_npd()))
-        return copied
-
-
-@dataclass
-class ISerializableDataClass(
-    ISerializable,
-    DataClassBase,
-    Generic[TSDataClass],
-    metaclass=ABCMeta,
-):
-    @classmethod
-    @abstractmethod
-    def d(cls) -> Dict[str, Type["ISerializableDataClass"]]:
-        pass
-
-    def to_info(self) -> Dict[str, Any]:
-        return self.asdict()
-
-    def from_info(self, info: Dict[str, Any]) -> None:
-        for k, v in info.items():
-            setattr(self, k, v)
-
-    @classmethod
-    def get(cls: Type[TRegister], name: str) -> Type[TRegister]:
-        return cls.d()[name]
-
-    @classmethod
-    def has(cls, name: str) -> bool:
-        return name in cls.d()
-
-    @classmethod
-    def register(
-        cls,
-        name: str,
-        *,
-        allow_duplicate: bool = False,
-    ) -> Callable:
-        def before(cls_: Type) -> None:
-            cls_.__identifier__ = name
-
-        return register_core(
-            name,
-            cls.d(),
-            allow_duplicate=allow_duplicate,
-            before_register=before,
-        )
-
-    @classmethod
-    def remove(cls, name: str) -> Callable:
-        return cls.d().pop(name)
-
-    @classmethod
-    def check_subclass(cls, name: str) -> bool:
-        return issubclass(cls.d()[name], cls)
-
-
-class Serializer:
-    id_file: str = "id.txt"
-    info_file: str = "info.json"
-    npd_folder: str = "npd"
-
-    @classmethod
-    def save_info(
-        cls,
-        folder: str,
-        *,
-        info: Optional[Dict[str, Any]] = None,
-        serializable: Optional[ISerializable] = None,
-    ) -> None:
-        os.makedirs(folder, exist_ok=True)
-        if info is None and serializable is None:
-            raise ValueError("either `info` or `serializable` should be provided")
-        if info is None:
-            info = serializable.to_info()
-        with open(os.path.join(folder, cls.info_file), "w") as f:
-            json.dump(info, f)
-
-    @classmethod
-    def load_info(cls, folder: str) -> Dict[str, Any]:
-        return cls.try_load_info(folder, strict=True)
-
-    @classmethod
-    def try_load_info(
-        cls,
-        folder: str,
-        *,
-        strict: bool = False,
-    ) -> Optional[Dict[str, Any]]:
-        info_path = os.path.join(folder, cls.info_file)
-        if not os.path.isfile(info_path):
-            if not strict:
-                return
-            raise ValueError(f"'{info_path}' does not exist")
-        with open(info_path, "r") as f:
-            info = json.load(f)
-        return info
-
-    @classmethod
-    def save_npd(
-        cls,
-        folder: str,
-        *,
-        npd: Optional[np_dict_type] = None,
-        serializable: Optional[ISerializableArrays] = None,
-    ) -> None:
-        os.makedirs(folder, exist_ok=True)
-        if npd is None and serializable is None:
-            raise ValueError("either `npd` or `serializable` should be provided")
-        if npd is None:
-            npd = serializable.to_npd()
-        npd_folder = os.path.join(folder, cls.npd_folder)
-        os.makedirs(npd_folder, exist_ok=True)
-        for k, v in npd.items():
-            np.save(os.path.join(npd_folder, f"{k}.npy"), v)
-
-    @classmethod
-    def load_npd(cls, folder: str) -> np_dict_type:
-        os.makedirs(folder, exist_ok=True)
-        npd_folder = os.path.join(folder, cls.npd_folder)
-        if not os.path.isdir(npd_folder):
-            raise ValueError(f"'{npd_folder}' does not exist")
-        npd = {}
-        for file in os.listdir(npd_folder):
-            key = os.path.splitext(file)[0]
-            npd[key] = np.load(os.path.join(npd_folder, file))
-        return npd
-
-    @classmethod
-    def save(
-        cls,
-        folder: str,
-        serializable: ISerializable,
-        *,
-        save_npd: bool = True,
-    ) -> None:
-        cls.save_info(folder, serializable=serializable)
-        if save_npd and isinstance(serializable, ISerializableArrays):
-            cls.save_npd(folder, serializable=serializable)
-        with open(os.path.join(folder, cls.id_file), "w") as f:
-            f.write(serializable.__identifier__)
-
-    @classmethod
-    def load(
-        cls,
-        folder: str,
-        base: Type[TSerializable],
-        *,
-        swap_id: Optional[str] = None,
-        swap_info: Optional[Dict[str, Any]] = None,
-        load_npd: bool = True,
-    ) -> TSerializable:
-        serializable = cls.load_empty(folder, base, swap_id=swap_id)
-        serializable.from_info(swap_info or cls.load_info(folder))
-        if load_npd and isinstance(serializable, ISerializableArrays):
-            serializable.from_npd(cls.load_npd(folder))
-        return serializable
-
-    @classmethod
-    def load_empty(
-        cls,
-        folder: str,
-        base: Type[TSerializable],
-        *,
-        swap_id: Optional[str] = None,
-    ) -> TSerializable:
-        if swap_id is not None:
-            s_type = swap_id
-        else:
-            id_path = os.path.join(folder, cls.id_file)
-            if not os.path.isfile(id_path):
-                raise ValueError(f"cannot find '{id_path}'")
-            with open(id_path, "r") as f:
-                s_type = f.read().strip()
-        return base.make(s_type, {})
-
-
-class IWithRequirements:
-    @classmethod
-    def requirements(cls) -> List[str]:
-        requirements = get_requirements(cls)
-        requirements.remove("self")
-        return requirements
-
-
-class SanityChecker:
-    @staticmethod
-    def int(n):
-        rs = {"suc": True}
-        try:
-            rs["n"] = int(n)
-            return rs
-        except Exception as e:
-            rs["suc"], rs["info"] = False, e
-            return rs
-
-    @staticmethod
-    def odd(n):
-        rs = {"suc": True}
-        try:
-            n = rs["n"] = int(n)
-            if n % 2 == 1:
-                return rs
-            rs["suc"], rs["info"] = False, "input is not an odd number"
-            return rs
-        except Exception as e:
-            rs["suc"], rs["info"] = False, e
-            return rs
-
-    @staticmethod
-    def float(n):
-        rs = {"suc": True}
-        try:
-            rs["n"] = float(n)
-            return rs
-        except Exception as e:
-            rs["suc"], rs["info"] = False, e
-            return rs
-
-
-class Incrementer:
-    """
-    Util class which can calculate running mean & running std efficiently.
-
-    Parameters
-    ----------
-    window_size : {int, None}, window size of running statistics.
-    * If None, then all history records will be used for calculation.
-
-    Examples
-    ----------
-    >>> incrementer = Incrementer(window_size=5)
-    >>> for i in range(10):
-    >>>     incrementer.update(i)
-    >>>     if i >= 4:
-    >>>         print(incrementer.mean)  # will print 2.0, 3.0, ..., 6.0, 7.0
-
-    """
-
-    def __init__(self, window_size: int = None):
-        if window_size is not None:
-            if not isinstance(window_size, int):
-                msg = f"window size should be integer, {type(window_size)} found"
-                raise ValueError(msg)
-            if window_size < 2:
-                msg = f"window size should be greater than 2, {window_size} found"
-                raise ValueError(msg)
-        self._window_size = window_size
-        self._n_record = self._previous = None
-        self._running_sum = self._running_square_sum = None
-
-    @property
-    def mean(self):
-        return self._running_sum / self._n_record
-
-    @property
-    def std(self):
-        return math.sqrt(
-            max(
-                0.0,
-                self._running_square_sum / self._n_record - self.mean**2,
-            )
-        )
-
-    @property
-    def n_record(self):
-        return self._n_record
-
-    def update(self, new_value):
-        if self._n_record is None:
-            self._n_record = 1
-            self._running_sum = new_value
-            self._running_square_sum = new_value**2
-        else:
-            self._n_record += 1
-            self._running_sum += new_value
-            self._running_square_sum += new_value**2
-        if self._window_size is not None:
-            if self._previous is None:
-                self._previous = [new_value]
-            else:
-                self._previous.append(new_value)
-            if self._n_record == self._window_size + 1:
-                self._n_record -= 1
-                previous = self._previous.pop(0)
-                self._running_sum -= previous
-                self._running_square_sum -= previous**2
-
-
-class _Formatter(logging.Formatter):
-    """Formatter for logging, which supports millisecond."""
-
-    converter = datetime.fromtimestamp
-
-    def formatTime(self, record, datefmt=None):
-        ct = self.converter(record.created)
-        if datefmt:
-            s = ct.strftime(datefmt)
-        else:
-            t = ct.strftime("%Y-%m-%d %H:%M:%S")
-            s = "%s.%03d" % (t, record.msecs)
-        return s
-
-    def formatMessage(self, record: logging.LogRecord) -> str:
-        record.__dict__.setdefault("func_prefix", "Unknown")
-        return super().formatMessage(record)
-
-
-class LoggingMixin:
-    """
-    Mixin class to provide logging methods for base class.
-
-    Attributes
-    ----------
-    _triggered_ : bool
-    * If not `_triggered_`, log file will not be created.
-
-    _verbose_level_ : int
-    * Preset verbose level of the whole logging process.
-
-    Methods
-    ----------
-    log_msg(self, body, prefix="", verbose_level=1)
-        Log something either through console or to a file.
-        * body : str
-            Main logging message.
-        * prefix : str
-            Prefix added to `body` when logging message goes through console.
-        * verbose_level : int
-            If `self._verbose_level_` >= verbose_level, then logging message
-            will go through console.
-
-    log_block_msg(self, body, prefix="", title="", verbose_level=1)
-        Almost the same as `log_msg`, except adding `title` on top of `body`.
-
-    """
-
-    _triggered_ = False
-    _initialized_ = False
-    _logging_path_ = None
-    _logger_ = _verbose_level_ = None
-    _date_format_string_ = "%Y-%m-%d %H:%M:%S.%f"
-    _formatter_ = _Formatter(
-        "[ {asctime:s} ] [ {levelname:^8s} ] {func_prefix:s} {message:s}",
-        _date_format_string_,
-        style="{",
-    )
-    _timing_dict_, _time_cache_dict_ = {}, {}
-
-    info_prefix = ">  [ info ] "
-    warning_prefix = "> [warning] "
-    error_prefix = "> [ error ] "
-
-    @property
-    def logging_path(self):
-        if self._logging_path_ is None:
-            folder = os.path.join(os.getcwd(), "_logging", type(self).__name__)
-            os.makedirs(folder, exist_ok=True)
-            self._logging_path_ = self.generate_logging_path(folder)
-        return self._logging_path_
-
-    @property
-    def console_handler(self):
-        if self._logger_ is None:
-            return
-        for handler in self._logger_.handlers:
-            if isinstance(handler, logging.StreamHandler):
-                return handler
-
-    @staticmethod
-    def _get_func_prefix(frame=None, return_prefix=True):
-        if frame is None:
-            frame = inspect.currentframe().f_back.f_back
-        if not return_prefix:
-            return frame
-        frame_info = inspect.getframeinfo(frame)
-        file_name = truncate_string_to_length(os.path.basename(frame_info.filename), 16)
-        func_name = truncate_string_to_length(frame_info.function, 24)
-        func_prefix = (
-            f"[ {func_name:^24s} ] [ {file_name:>16s}:{frame_info.lineno:<4d} ]"
-        )
-        return func_prefix
-
-    @staticmethod
-    def _release_handlers(logger):
-        for handler in logger.handlers[:]:
-            handler.close()
-            logger.removeHandler(handler)
-
-    @staticmethod
-    def generate_logging_path(folder: str) -> str:
-        return os.path.join(folder, f"{timestamp()}.log")
-
-    def _init_logging(self, verbose_level: Optional[int] = 2, trigger: bool = True):
-        wants_trigger = trigger and not LoggingMixin._triggered_
-        if LoggingMixin._initialized_ and not wants_trigger:
-            return self
-        LoggingMixin._initialized_ = True
-        logger_name = getattr(self, "_logger_name_", "root")
-        logger = LoggingMixin._logger_ = logging.getLogger(logger_name)
-        LoggingMixin._verbose_level_ = verbose_level
-        if not trigger:
-            return self
-        LoggingMixin._triggered_ = True
-        config = getattr(self, "config", {})
-        self._logging_path_ = config.get("_logging_path_")
-        if self._logging_path_ is None:
-            self._logging_path_ = config["_logging_path_"] = self.logging_path
-        os.makedirs(os.path.dirname(self.logging_path), exist_ok=True)
-        file_handler = logging.FileHandler(self.logging_path, encoding="utf-8")
-        file_handler.setFormatter(self._formatter_)
-        file_handler.setLevel(logging.DEBUG)
-        console = logging.StreamHandler()
-        console.setLevel(logging.INFO)
-        console.setFormatter(_Formatter("{custom_prefix:s}{message:s}", style="{"))
-        logger.setLevel(logging.DEBUG)
-        self._release_handlers(logger)
-        logger.addHandler(console)
-        logger.addHandler(file_handler)
-        self.log_block_msg(sys.version, title="system version", verbose_level=None)
-        return self
-
-    def log_msg(
-        self,
-        body: str,
-        prefix: str = "",
-        verbose_level: Optional[int] = 1,
-        msg_level: int = logging.INFO,
-        frame=None,
-    ):
-        preset_verbose_level = getattr(self, "_verbose_level", None)
-        if preset_verbose_level is not None:
-            self._verbose_level_ = preset_verbose_level
-        elif self._verbose_level_ is None:
-            self._verbose_level_ = 0
-        console_handler = self.console_handler
-        if verbose_level is None or self._verbose_level_ < verbose_level:
-            do_print, console_level = False, msg_level + 10
-        else:
-            do_print, console_level = not LoggingMixin._triggered_, msg_level
-        if console_handler is not None:
-            console_handler.setLevel(console_level)
-        if do_print:
-            print(prefix + body)
-        elif LoggingMixin._triggered_:
-            func_prefix = self._get_func_prefix(frame)
-            self._logger_.log(
-                msg_level,
-                body,
-                extra={"func_prefix": func_prefix, "custom_prefix": prefix},
-            )
-        if console_handler is not None:
-            console_handler.setLevel(logging.INFO)
-
-    def log_block_msg(
-        self,
-        body: str,
-        prefix: str = "",
-        title: str = "",
-        verbose_level: Optional[int] = 1,
-        msg_level: int = logging.INFO,
-        frame=None,
-    ):
-        frame = self._get_func_prefix(frame, False)
-        self.log_msg(f"{title}\n{body}\n", prefix, verbose_level, msg_level, frame)
-
-    def exception(self, body, frame=None):
-        self._logger_.exception(
-            body,
-            extra={
-                "custom_prefix": self.error_prefix,
-                "func_prefix": LoggingMixin._get_func_prefix(frame),
-            },
-        )
-
-    @staticmethod
-    def log_with_external_method(body, prefix, log_method, *args, **kwargs):
-        if log_method is None:
-            print(prefix + body)
-        else:
-            kwargs["frame"] = LoggingMixin._get_func_prefix(
-                kwargs.pop("frame", None),
-                False,
-            )
-            log_method(body, prefix, *args, **kwargs)
-
-    @staticmethod
-    def merge_logs_by_time(*log_files, tgt_file):
-        tgt_folder = os.path.dirname(tgt_file)
-        date_str_len = (
-            len(datetime.today().strftime(LoggingMixin._date_format_string_)) + 4
-        )
-        with lock_manager(tgt_folder, [tgt_file], clear_stuffs_after_exc=False):
-            msg_dict, msg_block, last_searched = {}, [], None
-            for log_file in log_files:
-                with open(log_file, "r") as f:
-                    for line in f:
-                        date_str = line[:date_str_len]
-                        if date_str[:2] == "[ " and date_str[-2:] == " ]":
-                            searched_time = datetime.strptime(
-                                date_str[2:-2],
-                                LoggingMixin._date_format_string_,
-                            )
-                        else:
-                            msg_block.append(line)
-                            continue
-                        if last_searched is not None:
-                            msg_block_ = "".join(msg_block)
-                            msg_dict.setdefault(last_searched, []).append(msg_block_)
-                        last_searched = searched_time
-                        msg_block = [line]
-                    if msg_block:
-                        msg_dict.setdefault(last_searched, []).append(
-                            "".join(msg_block)
-                        )
-            with open(tgt_file, "w") as f:
-                f.write("".join(["".join(msg_dict[key]) for key in sorted(msg_dict)]))
-
-    @classmethod
-    def reset_logging(cls) -> None:
-        cls._triggered_ = False
-        cls._initialized_ = False
-        cls._logging_path_ = None
-        if cls._logger_ is not None:
-            cls._release_handlers(cls._logger_)
-        cls._logger_ = cls._verbose_level_ = None
-        cls._timing_dict_, cls._time_cache_dict_ = {}, {}
-
-    @classmethod
-    def start_timer(cls, name):
-        if name in cls._time_cache_dict_:
-            print_warning(
-                f"'{name}' was already in time cache dict, "
-                "this may cause by calling `start_timer` repeatedly"
-            )
-            return
-        cls._time_cache_dict_[name] = time.time()
-
-    @classmethod
-    def end_timer(cls, name):
-        start_time = cls._time_cache_dict_.pop(name, None)
-        if start_time is None:
-            print_warning(
-                f"'{name}' was not found in time cache dict, "
-                "this may cause by not calling `start_timer` method"
-            )
-            return
-        incrementer = cls._timing_dict_.setdefault(name, Incrementer())
-        incrementer.update(time.time() - start_time)
-
-    def log_timing(self):
-        timing_str_list = ["=" * 138]
-        for name in sorted(self._timing_dict_.keys()):
-            incrementer = self._timing_dict_[name]
-            timing_str_list.append(
-                f"|   {name:<82s}   | "
-                f"{fix_float_to_length(incrementer.mean, 10)} ± "
-                f"{fix_float_to_length(incrementer.std, 10)} | "
-                f"{incrementer.n_record:>12d} hits   |"
-            )
-            timing_str_list.append("-" * 138)
-        self.log_block_msg(
-            "\n".join(timing_str_list),
-            title="timing",
-            verbose_level=None,
-            msg_level=logging.DEBUG,
-        )
-        return self
-
-
-class PureLoggingMixin:
-    """
-    Mixin class to provide (pure) logging method for base class.
-
-    Attributes
-    ----------
-    _loggers_ : dict(int, logging.Logger)
-        Recorded all loggers initialized.
-
-    _formatter_ : _Formatter
-        Formatter for all loggers.
-
-    Methods
-    ----------
-    log_msg(self, name, msg, msg_level=logging.INFO)
-        Log something to a file, with logger initialized by `name`.
-
-    log_block_msg(self, name, title, body, msg_level=logging.INFO)
-        Almost the same as `log_msg`, except adding `title` on top of `body`.
-
-    """
-
-    _name = _meta_name = None
-
-    _formatter_ = LoggingMixin._formatter_
-    _loggers_: Dict[str, logging.Logger] = {}
-    _logger_paths_: Dict[str, str] = {}
-    _timing_dict_ = {}
-
-    @property
-    def meta_suffix(self):
-        return "" if self._meta_name is None else self._meta_name
-
-    @property
-    def name_suffix(self):
-        return "" if self._name is None else f"-{self._name}"
-
-    @property
-    def meta_log_name(self):
-        return f"__meta__{self.meta_suffix}{self.name_suffix}"
-
-    @staticmethod
-    def get_logging_path(logger):
-        logging_path = None
-        for handler in logger.handlers:
-            if isinstance(handler, logging.FileHandler):
-                logging_path = handler.baseFilename
-                break
-        if logging_path is None:
-            raise ValueError(f"No FileHandler was found in given logger '{logger}'")
-        return logging_path
-
-    def _get_logger_info(self, name):
-        logger = name if isinstance(name, logging.Logger) else self._loggers_.get(name)
-        if logger is None:
-            raise ValueError(
-                f"logger for '{name}' is not defined, "
-                "please call `_setup_logger` first"
-            )
-        if isinstance(name, str):
-            logging_path = self._logger_paths_[name]
-        else:
-            logging_path = self.get_logging_path(logger)
-        return logger, os.path.dirname(logging_path), logging_path
-
-    def _setup_logger(self, name, logging_path, level=logging.DEBUG):
-        if name in self._loggers_:
-            return
-        console = logging.StreamHandler()
-        console.setLevel(logging.CRITICAL)
-        console.setFormatter(self._formatter_)
-        file_handler = logging.FileHandler(logging_path)
-        file_handler.setFormatter(self._formatter_)
-        file_handler.setLevel(level)
-        logger = logging.getLogger(name)
-        logger.setLevel(logging.DEBUG)
-        LoggingMixin._release_handlers(logger)
-        logger.addHandler(console)
-        logger.addHandler(file_handler)
-        PureLoggingMixin._loggers_[name] = logger
-        PureLoggingMixin._logger_paths_[name] = logging_path
-        for handler in logging.getLogger().handlers:
-            handler.setLevel(logging.CRITICAL)
-        self.log_block_msg(name, "system version", sys.version)
-
-    def _log_meta_msg(self, msg, msg_level=logging.INFO, frame=None):
-        if frame is None:
-            frame = inspect.currentframe().f_back
-        self.log_msg(self.meta_log_name, msg, msg_level, frame)
-
-    def _log_with_meta(self, task_name, msg, msg_level=logging.INFO, frame=None):
-        if frame is None:
-            frame = inspect.currentframe().f_back
-        self._log_meta_msg(f"{task_name} {msg}", msg_level, frame)
-        self.log_msg(task_name, f"current task {msg}", msg_level, frame)
-
-    def log_msg(self, name, msg, msg_level=logging.INFO, frame=None):
-        logger, logging_folder, logging_path = self._get_logger_info(name)
-        with lock_manager(
-            logging_folder,
-            [logging_path],
-            clear_stuffs_after_exc=False,
-        ):
-            logger.log(
-                msg_level,
-                msg,
-                extra={
-                    "custom_prefix": "",
-                    "func_prefix": LoggingMixin._get_func_prefix(frame),
-                },
-            )
-        return logger
-
-    def log_block_msg(self, name, title, body, msg_level=logging.INFO, frame=None):
-        frame = LoggingMixin._get_func_prefix(frame, False)
-        self.log_msg(name, f"{title}\n{body}\n", msg_level, frame)
-
-    def exception(self, name, msg, frame=None):
-        logger, logging_folder, logging_path = self._get_logger_info(name)
-        with lock_manager(
-            logging_folder,
-            [logging_path],
-            clear_stuffs_after_exc=False,
-        ):
-            logger.exception(
-                msg,
-                extra={
-                    "custom_prefix": LoggingMixin.error_prefix,
-                    "func_prefix": LoggingMixin._get_func_prefix(frame),
-                },
-            )
-
-    def del_logger(self, name):
-        logger = self.log_msg(name, f"clearing up logger information of '{name}'")
-        del self._loggers_[name], self._logger_paths_[name]
-        LoggingMixin._release_handlers(logger)
-        del logger
-
-
-def print_info(msg: str) -> None:
-    print(f"{LoggingMixin.info_prefix}{msg}")
-
-
-def print_warning(msg: str) -> None:
-    print(f"{LoggingMixin.warning_prefix}{msg}")
-
-
-def print_error(msg: str) -> None:
-    print(f"{LoggingMixin.error_prefix}{msg}")
-
-
-class SavingMixin(LoggingMixin):
-    """
-    Mixin class to provide logging & saving method for base class.
-
-    Warnings
-    ----------
-    We require base class to define every property appeared in __init__ (args, kwargs)
-    if we want to utilize `SavingMixin.load_with`
-
-    ```python
-    class Foo:
-        def __init__(self, a, *, b):
-            # these are required
-            self.a = a
-            self.b = b
-            # others could be customized
-            ...
-    ```
-
-    Methods
-    ----------
-    save(self, folder)
-        Save `self` to folder.
-
-    def load(self, folder)
-        Load from folder.
-
-    """
-
-    @property
-    @abstractmethod
-    def data_tuple_base(self) -> Optional[Type[NamedTuple]]:
-        pass
-
-    @property
-    @abstractmethod
-    def data_tuple_attributes(self) -> Optional[List[str]]:
-        pass
-
-    @property
-    def cache_excludes(self):
-        return set()
-
-    @property
-    def lock_verbose(self):
-        verbose_level = getattr(self, "_verbose_level", None)
-        if verbose_level is None:
-            return False
-        return verbose_level >= 5
-
-    def _data_tuple_context(self, *, is_saving: bool):
-        return data_tuple_saving_controller(self, is_saving=is_saving)
-
-    def save(self, folder: str, *, compress: bool = True):
-        with self._data_tuple_context(is_saving=True):
-            Saving.save_instance(self, folder, self.log_msg)
-        if compress:
-            abs_folder = os.path.abspath(folder)
-            base_folder = os.path.dirname(abs_folder)
-            with lock_manager(base_folder, [folder]):
-                Saving.compress(abs_folder, remove_original=True)
-        return self
-
-    def load(self, folder: str, *, compress: bool = True):
-        base_folder = os.path.dirname(os.path.abspath(folder))
-        with lock_manager(base_folder, [folder]):
-            with Saving.compress_loader(
-                folder,
-                compress,
-                remove_extracted=True,
-                logging_mixin=self,
-            ):
-                with self._data_tuple_context(is_saving=False):
-                    Saving.load_instance(self, folder, log_method=self.log_msg)
-        return self
-
-    @staticmethod
-    def load_with(cls: Type, folder: str, *, compress: bool = True) -> Any:
-        # load every thing into a dummy instance
-        dummy = type(cls.__name__, (SavingMixin,), {})()
-        dummy.load(folder, compress=compress)
-        # inject everything into the target instance
-        spec = inspect.getfullargspec(cls.__init__)
-        args = spec.args[1:]
-        kwargs_keys = spec.kwonlyargs
-        arg_values = tuple(getattr(dummy, arg) for arg in args)
-        kwargs = {key: getattr(dummy, key) for key in kwargs_keys}
-        instance = cls(*arg_values, **kwargs)
-        update_dict(dummy.__dict__, instance.__dict__)
-        return instance
-
-
-class Saving(LoggingMixin):
-    """
-    Util class for saving instances.
-
-    Methods
-    ----------
-    save_instance(instance, folder, log_method=None)
-        Save instance to `folder`.
-        * instance : object, instance to save.
-        * folder : str, folder to save to.
-        * log_method : {None, function}, used as `log_method` parameter in
-        `log_with_external_method` method of `LoggingMixin`.
-
-    load_instance(instance, folder, log_method=None)
-        Load instance from `folder`.
-        * instance : object, instance to load, need to be initialized.
-        * folder : str, folder to load from.
-        * log_method : {None, function}, used as `log_method` parameter in
-        `log_with_external_method` method of `LoggingMixin`.
-
-    """
-
-    delim = "^_^"
-    dill_suffix = ".pkl"
-    array_sub_folder = "__arrays"
-
-    @staticmethod
-    def _check_core(elem):
-        if isinstance(elem, dict):
-            if not Saving._check_dict(elem):
-                return False
-        if isinstance(elem, (list, tuple)):
-            if not Saving._check_list_and_tuple(elem):
-                return False
-        if not Saving._check_elem(elem):
-            return False
-        return True
-
-    @staticmethod
-    def _check_elem(elem):
-        if isinstance(elem, (type, np.generic, np.ndarray)):
-            return False
-        if callable(elem):
-            return False
-        try:
-            json.dumps({"": elem})
-            return True
-        except TypeError:
-            return False
-
-    @staticmethod
-    def _check_list_and_tuple(arr: Union[list, tuple]):
-        for elem in arr:
-            if not Saving._check_core(elem):
-                return False
-        return True
-
-    @staticmethod
-    def _check_dict(d: dict):
-        for v in d.values():
-            if not Saving._check_core(v):
-                return False
-        return True
-
-    @staticmethod
-    def save_dict(d: dict, name: str, folder: str) -> str:
-        if Saving._check_dict(d):
-            kwargs = {}
-            suffix, method, mode = ".json", json.dump, "w"
-        else:
-            kwargs = {"recurse": True}
-            suffix, method, mode = Saving.dill_suffix, dill.dump, "wb"
-        file = os.path.join(folder, f"{name}{suffix}")
-        with open(file, mode) as f:
-            method(d, f, **kwargs)
-        return os.path.abspath(file)
-
-    @staticmethod
-    def load_dict(name: str, folder: str = None):
-        if folder is None:
-            folder, name = os.path.split(name)
-        name, suffix = os.path.splitext(name)
-        if not suffix:
-            json_file = os.path.join(folder, f"{name}.json")
-            if os.path.isfile(json_file):
-                with open(json_file, "r") as f:
-                    return json.load(f)
-            dill_file = os.path.join(folder, f"{name}{Saving.dill_suffix}")
-            if os.path.isfile(dill_file):
-                with open(dill_file, "rb") as f:
-                    return dill.load(f)
-        else:
-            assert_msg = f"suffix should be either 'json' or 'pkl', {suffix} found"
-            assert suffix in {".json", ".pkl"}, assert_msg
-            name = f"{name}{suffix}"
-            file = os.path.join(folder, name)
-            if os.path.isfile(file):
-                if suffix == ".json":
-                    mode, load_method = "r", json.load
-                else:
-                    mode, load_method = "rb", dill.load
-                with open(file, mode) as f:
-                    return load_method(f)
-        raise ValueError(f"config '{name}' is not found under '{folder}' folder")
-
-    @staticmethod
-    def deep_copy_dict(d: dict):
-        tmp_folder = os.path.join(os.getcwd(), "___tmp_dict_cache___")
-        if os.path.isdir(tmp_folder):
-            shutil.rmtree(tmp_folder)
-        os.makedirs(tmp_folder)
-        dict_name = "deep_copy"
-        Saving.save_dict(d, dict_name, tmp_folder)
-        loaded_dict = Saving.load_dict(dict_name, tmp_folder)
-        shutil.rmtree(tmp_folder)
-        return loaded_dict
-
-    @staticmethod
-    def get_cache_file(instance):
-        return f"{type(instance).__name__}.pkl"
-
-    @staticmethod
-    def save_instance(instance, folder, log_method=None):
-        instance_str = str(instance)
-        Saving.log_with_external_method(
-            f"saving '{instance_str}' to '{folder}'",
-            Saving.info_prefix,
-            log_method,
-            5,
-        )
-
-        def _record_array(k, v):
-            extension = ".npy" if isinstance(v, np.ndarray) else ".lst"
-            array_attribute_dict[f"{k}{extension}"] = v
-
-        def _check_array(attr_key_, attr_value_, depth=0):
-            if isinstance(attr_value_, dict):
-                for k in list(attr_value_.keys()):
-                    v = attr_value_[k]
-                    extended_k = f"{attr_key_}{delim}{k}"
-                    if isinstance(v, dict):
-                        _check_array(extended_k, v, depth + 1)
-                    elif isinstance(v, array_types):
-                        _record_array(extended_k, v)
-                        attr_value_.pop(k)
-            if isinstance(attr_value_, array_types):
-                _record_array(attr_key_, attr_value_)
-                if depth == 0:
-                    cache_excludes.add(attr_key_)
-
-        main_file = Saving.get_cache_file(instance)
-        instance_dict = shallow_copy_dict(instance.__dict__)
-        verbose, cache_excludes = map(
-            getattr,
-            [instance] * 2,
-            ["lock_verbose", "cache_excludes"],
-            [False, set()],
-        )
-        if os.path.isdir(folder):
-            if verbose:
-                prefix = Saving.warning_prefix
-                msg = f"'{folder}' will be cleaned up when saving '{instance_str}'"
-                Saving.log_with_external_method(
-                    msg, prefix, log_method, msg_level=logging.WARNING
-                )
-            shutil.rmtree(folder)
-        save_path = os.path.join(folder, main_file)
-        array_folder = os.path.join(folder, Saving.array_sub_folder)
-        tuple(
-            map(
-                lambda folder_: os.makedirs(folder_, exist_ok=True),
-                [folder, array_folder],
-            )
-        )
-        sorted_attributes, array_attribute_dict = sorted(instance_dict), {}
-        delim, array_types = Saving.delim, (list, np.ndarray)
-        for attr_key in sorted_attributes:
-            if attr_key in cache_excludes:
-                continue
-            attr_value = instance_dict[attr_key]
-            _check_array(attr_key, attr_value)
-        cache_excludes.add("_verbose_level_")
-        with lock_manager(
-            folder,
-            [os.path.join(folder, main_file)],
-            name=instance_str,
-        ):
-            with open(save_path, "wb") as f:
-                d = {k: v for k, v in instance_dict.items() if k not in cache_excludes}
-                dill.dump(d, f, recurse=True)
-        if array_attribute_dict:
-            sorted_array_files = sorted(array_attribute_dict)
-            sorted_array_files_full_path = list(
-                map(lambda f_: os.path.join(array_folder, f_), sorted_array_files)
-            )
-            with lock_manager(
-                array_folder,
-                sorted_array_files_full_path,
-                name=f"{instance_str} (arrays)",
-            ):
-                for array_file, array_file_full_path in zip(
-                    sorted_array_files, sorted_array_files_full_path
-                ):
-                    array_value = array_attribute_dict[array_file]
-                    if array_file.endswith(".npy"):
-                        np.save(array_file_full_path, array_value)
-                    elif array_file.endswith(".lst"):
-                        with open(array_file_full_path, "wb") as f:
-                            np.save(f, array_value)
-                    else:
-                        raise ValueError(
-                            f"unrecognized file type '{array_file}' occurred"
-                        )
-
-    @staticmethod
-    def load_instance(instance, folder, *, log_method=None, verbose=True):
-        if verbose:
-            Saving.log_with_external_method(
-                f"loading '{instance}' from '{folder}'",
-                Saving.info_prefix,
-                log_method,
-                5,
-            )
-        with open(os.path.join(folder, Saving.get_cache_file(instance)), "rb") as f:
-            instance.__dict__.update(dill.load(f))
-        delim = Saving.delim
-        array_folder = os.path.join(folder, Saving.array_sub_folder)
-        for array_file in os.listdir(array_folder):
-            attr_name, attr_ext = os.path.splitext(array_file)
-            if attr_ext == ".npy":
-                load_method = partial(np.load, allow_pickle=True)
-            elif attr_ext == ".lst":
-
-                def load_method(path):
-                    return np.load(path, allow_pickle=True).tolist()
-
-            else:
-                raise ValueError(f"unrecognized file type '{array_file}' occurred")
-            array_value = load_method(os.path.join(array_folder, array_file))
-            attr_hierarchy = attr_name.split(delim)
-            if len(attr_hierarchy) == 1:
-                instance.__dict__[attr_name] = array_value
-            else:
-                hierarchy_dict = instance.__dict__
-                for attr in attr_hierarchy[:-1]:
-                    hierarchy_dict = hierarchy_dict.setdefault(attr, {})
-                hierarchy_dict[attr_hierarchy[-1]] = array_value
-
-    @staticmethod
-    def prepare_folder(instance, folder):
-        if os.path.isdir(folder):
-            instance.log_msg(
-                f"'{folder}' already exists, it will be cleared up to save our model",
-                instance.warning_prefix,
-                msg_level=logging.WARNING,
-            )
-            shutil.rmtree(folder)
-        os.makedirs(folder)
-
-    @staticmethod
-    def compress(abs_folder, remove_original=True):
-        shutil.make_archive(abs_folder, "zip", abs_folder)
-        if remove_original:
-            shutil.rmtree(abs_folder)
-
-    @staticmethod
-    def compress_loader(
-        folder: str,
-        is_compress: bool,
-        *,
-        remove_extracted: bool = True,
-        logging_mixin: Optional[LoggingMixin] = None,
-    ):
-        class _manager(context_error_handler):
-            def __enter__(self):
-                if is_compress:
-                    if os.path.isdir(folder):
-                        msg = (
-                            f"'{folder}' already exists, "
-                            "it will be cleared up to load our model"
-                        )
-                        if logging_mixin is None:
-                            print(msg)
-                        else:
-                            logging_mixin.log_msg(
-                                msg,
-                                logging_mixin.warning_prefix,
-                                msg_level=logging.WARNING,
-                            )
-                        shutil.rmtree(folder)
-                    with zipfile.ZipFile(f"{folder}.zip", "r") as zip_ref:
-                        zip_ref.extractall(folder)
-
-            def _normal_exit(self, exc_type, exc_val, exc_tb):
-                if is_compress and remove_extracted:
-                    shutil.rmtree(folder)
-
-        return _manager()
-
-
-candidate_type = List[Any]
-candidates_type = Union[List[candidate_type], Dict[str, candidate_type]]
-
-
-class Grid:
-    """
-    Util class provides permutation of simple, flattened candidates.
-    * For permutation of complex, nested param dicts, please refers to
-      `ParamGenerator` in `cftool.param_utils.core`.
-
-    Parameters
-    ----------
-    candidates : candidates_type, cadidates we want to create grid from.
-
-    Examples
-    ----------
-    >>> from cftool.misc import Grid
-    >>>
-    >>> grid = Grid({"a": [1, 2, 3], "b": [1, 2, 3]})
-    >>> for param in grid:
-    >>>     print(param)
-    >>> # output : {'a': 1, 'b': 1}, {'a': 1, 'b': 2}, {'a': 1, 'b': 3}
-    >>> #          {'a': 2, 'b': 1}, ..., {'a': 3, 'b': 3}
-
-    """
-
-    def __init__(self, candidates: candidates_type):
-        self.candidates = candidates
-        self._is_list = isinstance(candidates, list)
-
-    @staticmethod
-    def _yield_lists(lists):
-        yield from map(list, product(*lists))
-
-    def __iter__(self):
-        if self._is_list:
-            yield from self._yield_lists(self.candidates)
-        else:
-            items = sorted(self.candidates.items())
-            if not items:
-                yield {}
-            else:
-                keys, values = zip(*items)
-                for v in map(list, product(*values)):
-                    yield dict(zip(keys, v))
-
-
-nested_type = Dict[str, Union[Any, Dict[str, "nested_type"]]]
-all_nested_type = Dict[str, Union[List[Any], Dict[str, "all_nested_type"]]]
-union_nested_type = Union[nested_type, all_nested_type]
-flattened_type = Dict[str, Any]
-all_flattened_type = Dict[str, List[Any]]
-union_flattened_type = Union[flattened_type, all_flattened_type]
-
-
-def _offset_fn(value) -> int:
-    if not isinstance(value, (list, tuple)):
-        return 1
-    return len(value)
-
-
-class Nested:
-    def __init__(
-        self,
-        nested: union_nested_type,
-        *,
-        offset_fn: Callable[[Any], int] = _offset_fn,
-        delim: str = "^_^",
-    ):
-        self.nested = nested
-        self.offset_fn, self.delim = offset_fn, delim
-        self._flattened = self._sorted_flattened_keys = None
-        self._sorted_flattened_offsets = None
-
-    def apply(self, fn: Callable[[Any], Any]) -> "Nested":
-        def _apply(src, tgt):
-            for k, v in src.items():
-                if isinstance(v, dict):
-                    next_tgt = tgt.setdefault(k, {})
-                    _apply(v, next_tgt)
-                else:
-                    tgt[k] = fn(v)
-            return tgt
-
-        return Nested(_apply(self.nested, {}))
-
-    @property
-    def flattened(self) -> union_flattened_type:
-        if self._flattened is None:
-            self._flattened = self.flatten_nested(self.nested)
-        return self._flattened
-
-    @property
-    def sorted_flattened_keys(self) -> List[str]:
-        if self._sorted_flattened_keys is None:
-            self._sorted_flattened_keys = sorted(self.flattened)
-        return self._sorted_flattened_keys
-
-    @property
-    def sorted_flattened_offsets(self) -> List[int]:
-        if self._sorted_flattened_offsets is None:
-            offsets = []
-            for key in self.sorted_flattened_keys:
-                value = self.get_value_from(key)
-                offsets.append(self.offset_fn(value))
-            self._sorted_flattened_offsets = offsets
-        return self._sorted_flattened_offsets
-
-    def get_value_from(self, flattened_key: str) -> Any:
-        value = self.nested
-        for sub_key in flattened_key.split(self.delim):
-            value = value[sub_key]
-        return value
-
-    def flatten_nested(self, nested: nested_type) -> nested_type:
-        flattened = []
-
-        def _flatten(d, pre_key: Union[None, str]):
-            for name, value in d.items():
-                if pre_key is None:
-                    next_pre_key = name
-                else:
-                    next_pre_key = f"{pre_key}{self.delim}{name}"
-                if isinstance(value, dict):
-                    _flatten(value, next_pre_key)
-                else:
-                    flattened.append((next_pre_key, value))
-            return flattened
-
-        return dict(_flatten(nested, None))
-
-    def nest_flattened(self, flattened: flattened_type) -> nested_type:
-        sorted_pairs = sorted(
-            map(lambda k, v: (k.split(self.delim), v), *zip(*flattened.items())),
-            key=len,
-        )
-        nested = {}
-        for key_list, value in sorted_pairs:
-            if len(key_list) == 1:
-                nested[key_list[0]] = value
-            else:
-                parent = nested.setdefault(key_list[0], {})
-                for key in key_list[1:-1]:
-                    parent = parent.setdefault(key, {})
-                parent[key_list[-1]] = value
-        return nested
-
-    def flattened2array(self, flattened: flattened_type) -> np.ndarray:
-        value_list = []
-        for key in self.sorted_flattened_keys:
-            value = flattened[key]
-            value = list(value) if isinstance(value, (list, tuple)) else [value]
-            value_list.extend(value)
-        return np.array(value_list, np.float32)
-
-    def array2flattened(self, array: np.ndarray) -> flattened_type:
-        cursor = 0
-        flattened = {}
-        for key, offset in zip(
-            self.sorted_flattened_keys,
-            self.sorted_flattened_offsets,
-        ):
-            end = cursor + offset
-            if offset == 1:
-                value = array[cursor]
-            else:
-                value = array[cursor:end].tolist()
-                if isinstance(value, tuple):
-                    value = tuple(value)
-            flattened[key] = value
-            cursor = end
-        return flattened
-
-
-class Sampler:
-    """
-    Util class which can help sampling indices from probabilities.
-
-    Parameters
-    ----------
-    method : str, sampling method.
-    * Currently only 'multinomial' is supported.
-    probabilities : np.ndarray, probabilities we'll use.
-
-    Examples
-    ----------
-    >>> import numpy as np
-    >>> arr = [[0.1, 0.2, 0.3, 0.4], [0.4, 0.3, 0.2, 0.1]]
-    >>> probabilities = np.array(arr, np.float32)
-    >>> sampler = Sampler("multinomial", probabilities)
-    >>> print(sampler.sample(10))
-
-    """
-
-    def __init__(self, method: str, probabilities: np.ndarray):
-        self.method = method
-        self.p = probabilities
-        self._p_shape = list(self.p.shape)
-        if self.is_flat:
-            self._p_block = self.p
-        else:
-            self._p_block = self.p.reshape([-1, self._p_shape[-1]])
-
-    def __str__(self):
-        return f"Sampler({self.method})"
-
-    __repr__ = __str__
-
-    @property
-    def is_flat(self):
-        return len(self._p_shape) == 1
-
-    def _reshape(self, n: int, samples: np.ndarray) -> np.ndarray:
-        return samples.reshape([n] + self._p_shape[:-1]).astype(np.int64)
-
-    def sample(self, n: int) -> np.ndarray:
-        return getattr(self, self.method)(n)
-
-    @staticmethod
-    def _multinomial_flat(n: int, p: np.ndarray) -> np.ndarray:
-        samples = np.random.multinomial(n, p)
-        return np.repeat(np.arange(len(p)), samples)
-
-    def multinomial(self, n: int) -> np.ndarray:
-        if self.is_flat:
-            sampled_indices = self._multinomial_flat(n, self.p)
-        else:
-            stacks = [self._multinomial_flat(n, p) for p in self._p_block]
-            sampled_indices = np.vstack(stacks).T
-        return self._reshape(n, sampled_indices)
-
-
-class DownloadProgressBar(tqdm):
-    def update_to(
-        self,
-        b: int = 1,
-        bsize: int = 1,
-        tsize: Optional[int] = None,
-    ) -> None:
-        if tsize is not None:
-            self.total = tsize
-        self.update(b * bsize - self.n)
-
-
-class OPTBase(ABC):
-    def __init__(self):
-        self._opt = self.defaults
-        self.update_from_env()
-
-    @property
-    @abstractmethod
-    def env_key(self) -> str:
-        pass
-
-    @property
-    @abstractmethod
-    def defaults(self) -> Dict[str, Any]:
-        pass
-
-    def __getattr__(self, __name: str) -> Any:
-        return self._opt[__name]
-
-    def update_from_env(self) -> None:
-        env_opt_json = os.environ.get(self.env_key)
-        if env_opt_json is not None:
-            self._opt.update(json.loads(env_opt_json))
-
-    def opt_context(self, increment: Dict[str, Any]) -> Any:
-        class _:
-            def __init__(self) -> None:
-                self._increment = increment
-                self._backup = shallow_copy_dict(instance._opt)
-
-            def __enter__(self) -> None:
-                instance._opt.update(self._increment)
-
-            def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
-                instance._opt.update(self._backup)
-
-        instance = self
-        return _()
-
-    def opt_env_context(self, increment: Dict[str, Any]) -> Any:
-        class _:
-            def __init__(self) -> None:
-                self._increment = increment
-                self._backup = os.environ.get(instance.env_key)
-
-            def __enter__(self) -> None:
-                os.environ[instance.env_key] = json.dumps(self._increment)
-
-            def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
-                if self._backup is None:
-                    del os.environ[instance.env_key]
-                else:
-                    os.environ[instance.env_key] = self._backup
-
-        instance = self
-        return _()
-
-
-# contexts
-
-
-class context_error_handler:
-    """Util class which provides exception handling when using context manager."""
-
-    @property
-    def exception_suffix(self):
-        return ""
-
-    def _normal_exit(self, exc_type, exc_val, exc_tb):
-        pass
-
-    def _exception_exit(self, exc_type, exc_val, exc_tb):
-        pass
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        if not exc_type:
-            self._normal_exit(exc_type, exc_val, exc_tb)
-        else:
-            self._exception_exit(exc_type, exc_val, exc_tb)
-
-
-class timeit(context_error_handler):
-    """
-    Timing context manager.
-
-    Examples
-    --------
-    >>> with timeit("something"):
-    >>>     # do something here
-    >>> # will print ">  [ info ] timing for    something     : x.xxxx"
-
-    """
-
-    def __init__(self, msg, precision=6):
-        self._msg = msg
-        self._p = precision
-
-    def __enter__(self):
-        self._t = time.time()
-
-    def _normal_exit(self, exc_type, exc_val, exc_tb):
-        prefix = LoggingMixin.info_prefix
-        print(
-            f"{prefix}timing for {self._msg:^16s} : "
-            f"{time.time() - self._t:{self._p}.{self._p-2}f}"
-        )
-
-
-class _lock_file_refresher(threading.Thread):
-    def __init__(self, lock_file, delay=1, refresh=0.01):
-        super().__init__()
-        self.__stop_event = threading.Event()
-        self._lock_file, self._delay, self._refresh = lock_file, delay, refresh
-        with open(lock_file, "r") as f:
-            self._lock_file_contents = f.read()
-
-    def run(self) -> None:
-        counter = 0
-        while True:
-            counter += 1
-            time.sleep(self._refresh)
-            if counter * self._refresh >= self._delay:
-                counter = 0
-                with open(self._lock_file, "w") as f:
-                    prefix = "\n\n"
-                    add_line = f"{prefix}refreshed at {timestamp()}"
-                    f.write(self._lock_file_contents + add_line)
-            if self.__stop_event.is_set():
-                break
-
-    def stop(self):
-        self.__stop_event.set()
-
-
-class lock_manager(context_error_handler, LoggingMixin):
-    """
-    Util class to make simultaneously-write process safe with some
-    hacked (ugly) tricks.
-
-    Examples
-    --------
-    >>> import dill
-    >>> workspace = "_cache"
-    >>> target_write_files_full_path = [
-    >>>     os.path.join(workspace, "file1.pkl"),
-    >>>     os.path.join(workspace, "file2.pkl")
-    >>> ]
-    >>> with lock_manager(workspace, target_write_files_full_path):
-    >>>     for write_file_full_path in target_write_files_full_path:
-    >>>         with open(write_file_full_path, "wb") as wf:
-    >>>             dill.dump(..., wf)
-
-    """
-
-    delay = 0.01
-    __lock__ = "__lock__"
-
-    def __init__(
-        self,
-        workspace,
-        stuffs,
-        verbose_level=None,
-        set_lock=True,
-        clear_stuffs_after_exc=True,
-        name=None,
-        wait=1000,
-    ):
-        self._workspace = workspace
-        self._verbose_level = verbose_level
-        self._name, self._wait = name, wait
-        os.makedirs(workspace, exist_ok=True)
-        self._stuffs, self._set_lock = stuffs, set_lock
-        self._clear_stuffs = clear_stuffs_after_exc
-        self._is_locked = False
-
-    def __enter__(self):
-        frame = inspect.currentframe().f_back
-        self.log_msg(
-            f"waiting for lock at {self.lock_file}",
-            self.info_prefix,
-            5,
-            logging.DEBUG,
-            frame,
-        )
-        enter_time = file_modify = None
-        while True:
-            try:
-                fd = os.open(self.lock_file, os.O_CREAT | os.O_EXCL | os.O_RDWR)
-                self.log_msg(
-                    "lock acquired",
-                    self.info_prefix,
-                    5,
-                    logging.DEBUG,
-                    frame,
-                )
-                if not self._set_lock:
-                    self.log_msg(
-                        "releasing lock since set_lock=False",
-                        self.info_prefix,
-                        5,
-                        logging.DEBUG,
-                        frame,
-                    )
-                    os.unlink(self.lock_file)
-                    self.__refresher = None
-                else:
-                    self.log_msg(
-                        "writing info to lock file",
-                        self.info_prefix,
-                        5,
-                        logging.DEBUG,
-                        frame,
-                    )
-                    with os.fdopen(fd, "a") as f:
-                        f.write(
-                            f"name      : {self._name}\n"
-                            f"timestamp : {timestamp()}\n"
-                            f"workspace : {self._workspace}\n"
-                            f"stuffs    :\n{self.cache_stuffs_str}"
-                        )
-                    self.__refresher = _lock_file_refresher(self.lock_file)
-                    self.__refresher.start()
-                break
-            except OSError as e:
-                if e.errno != errno.EEXIST:
-                    raise
-                try:
-                    if file_modify is None:
-                        enter_time = time.time()
-                        file_modify = os.path.getmtime(self.lock_file)
-                    else:
-                        new_file_modify = os.path.getmtime(self.lock_file)
-                        if new_file_modify != file_modify:
-                            enter_time = time.time()
-                            file_modify = new_file_modify
-                        else:
-                            wait_time = time.time() - enter_time
-                            if wait_time >= self._wait:
-                                raise ValueError(
-                                    f"'{self.lock_file}' has been waited "
-                                    f"for too long ({wait_time})"
-                                )
-                    time.sleep(random.random() * self.delay + self.delay)
-                except ValueError:
-                    msg = f"lock_manager was blocked by dead lock ({self.lock_file})"
-                    self.exception(msg)
-                    raise
-                except FileNotFoundError:
-                    pass
-        self.log_block_msg(
-            self.cache_stuffs_str,
-            title="start processing following stuffs:",
-            verbose_level=5,
-            msg_level=logging.DEBUG,
-            frame=frame,
-        )
-        self._is_locked = True
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        if self.__refresher is not None:
-            self.__refresher.stop()
-            self.__refresher.join()
-        if self._set_lock:
-            super().__exit__(exc_type, exc_val, exc_tb)
-
-    def _normal_exit(self, exc_type, exc_val, exc_tb, frame=None):
-        if self._set_lock:
-            os.unlink(self.lock_file)
-        if frame is None:
-            frame = inspect.currentframe().f_back.f_back.f_back
-        self.log_msg("lock released", self.info_prefix, 5, logging.DEBUG, frame)
-
-    def _exception_exit(self, exc_type, exc_val, exc_tb):
-        frame = inspect.currentframe().f_back.f_back.f_back
-        if self._clear_stuffs:
-            for stuff in self._stuffs:
-                if os.path.isfile(stuff):
-                    self.log_msg(
-                        f"clearing cached file: {stuff}",
-                        ">> ",
-                        5,
-                        logging.ERROR,
-                        frame,
-                    )
-                    os.remove(stuff)
-                elif os.path.isdir(stuff):
-                    self.log_msg(
-                        f"clearing cached directory: {stuff}",
-                        ">> ",
-                        5,
-                        logging.ERROR,
-                        frame,
-                    )
-                    shutil.rmtree(stuff)
-        self._normal_exit(exc_type, exc_val, exc_tb, frame)
-
-    @property
-    def locked(self):
-        return self._is_locked
-
-    @property
-    def available(self):
-        return not os.path.isfile(self.lock_file)
-
-    @property
-    def cache_stuffs_str(self):
-        return "\n".join([f">> {stuff}" for stuff in self._stuffs])
-
-    @property
-    def exception_suffix(self):
-        return f", clearing caches for safety{self.logging_suffix}"
-
-    @property
-    def lock_file(self):
-        return os.path.join(self._workspace, self.__lock__)
-
-    @property
-    def logging_suffix(self):
-        return "" if self._name is None else f" - {self._name}"
-
-
-class batch_manager(context_error_handler):
-    """
-    Process data in batch.
-
-    Parameters
-    ----------
-    inputs : tuple(np.ndarray), auxiliary array inputs.
-    n_elem : {int, float}, indicates how many elements will be processed in a batch.
-    batch_size : int, indicates the batch_size; if None, batch_size will be
-                      calculated by `n_elem`.
-
-    Examples
-    --------
-    >>> with batch_manager(np.arange(5), np.arange(1, 6), batch_size=2) as manager:
-    >>>     for arr, tensor in manager:
-    >>>         print(arr, tensor)
-    >>>         # Will print:
-    >>>         #   [0 1], [1 2]
-    >>>         #   [2 3], [3 4]
-    >>>         #   [4]  , [5]
-
-    """
-
-    def __init__(
-        self,
-        *inputs,
-        n_elem: int = 1e6,
-        batch_size: Optional[int] = None,
-        max_batch_size: int = 1024,
-    ):
-        if not inputs:
-            raise ValueError("inputs should be provided in general_batch_manager")
-        input_lengths = list(map(len, inputs))
-        self._n, self._inputs = input_lengths[0], inputs
-        assert_msg = "inputs should be of same length"
-        assert all(length == self._n for length in input_lengths), assert_msg
-        if batch_size is not None:
-            self._batch_size = batch_size
-        else:
-            n_elem = int(n_elem)
-            self._batch_size = int(
-                n_elem / sum(map(lambda arr: prod(arr.shape[1:]), inputs))
-            )
-        self._batch_size = min(max_batch_size, min(self._n, self._batch_size))
-        self._n_epoch = int(self._n / self._batch_size)
-        self._n_epoch += int(self._n_epoch * self._batch_size < self._n)
-
-    def __enter__(self):
-        return self
-
-    def __iter__(self):
-        self._start, self._end = 0, self._batch_size
-        return self
-
-    def __next__(self):
-        if self._start >= self._n:
-            raise StopIteration
-        batched_data = tuple(
-            map(
-                lambda arr: arr[self._start : self._end],
-                self._inputs,
-            )
-        )
-        self._start, self._end = self._end, self._end + self._batch_size
-        if len(batched_data) == 1:
-            return batched_data[0]
-        return batched_data
-
-    def __len__(self):
-        return self._n_epoch
-
-
-class timing_context(context_error_handler):
-    """
-    Wrap codes in any base class of `LoggingMixin` with this timing context to timeit.
-
-    Parameters
-    ----------
-    logging_mixin : LoggingMixin, arbitrary base classes of LoggingMixin.
-    name : str, explain what the wrapped codes are doing.
-    enable : bool, whether enable this `timing_context`.
-
-    Examples
-    --------
-    >>> import time
-    >>> import random
-    >>> instance = type(
-    >>>    "test", (LoggingMixin,),
-    >>>    {"config": {}, "_verbose_level": 2}
-    >>> )()._init_logging(2, True)
-    >>> for _ in range(50):
-    >>>     with timing_context(instance, "random sleep"):
-    >>>         time.sleep(random.random() * 0.1)
-    >>> instance.log_timing()
-
-    """
-
-    def __init__(self, logging_mixin: LoggingMixin, name: str, *, enable: bool = True):
-        self._cls, self._name = logging_mixin, name
-        self._enable = enable
-
-    @property
-    def timer_name(self):
-        return f"[{type(self._cls).__name__:^24s}] {self._name}"
-
-    def __enter__(self):
-        if self._enable:
-            self._cls.start_timer(self.timer_name)
-
-    def _normal_exit(self, exc_type, exc_val, exc_tb):
-        if self._enable:
-            self._cls.end_timer(self.timer_name)
-
-
-class data_tuple_saving_controller(context_error_handler):
-    """
-    Help saving DataTuple of SavingMixin.
-
-    Parameters
-    ----------
-    instance : SavingMixin, instance whose DataTuples are to be saved / loaded.
-    is_saving : bool, whether it is a saving context or not.
-    """
-
-    __prefix__ = "_Data_Tuple__"
-
-    def __init__(self, instance: SavingMixin, *, is_saving: bool):
-        self._instance = instance
-        self._is_saving = is_saving
-        self._data_tuple_base = instance.data_tuple_base
-        self._data_tuple_attributes = instance.data_tuple_attributes
-        if self.trigger and is_saving:
-            self._data_tuples: List[NamedTuple] = [
-                instance.__dict__.pop(attr) for attr in self._data_tuple_attributes
-            ]
-
-    def __enter__(self):
-        if self.trigger and self._is_saving:
-            self.__tmp_attr_list = []
-            for attr, data_tuple in zip(
-                self._data_tuple_attributes,
-                self._data_tuples,
-            ):
-                local_attr_list = self._get_attr(attr, data_tuple)
-                for local_attr, data in zip(local_attr_list, data_tuple):
-                    setattr(self._instance, local_attr, data)
-                self.__tmp_attr_list += local_attr_list
-
-    @property
-    def trigger(self):
-        return (
-            self._data_tuple_base is not None
-            and self._data_tuple_attributes is not None
-        )
-
-    def _normal_exit(self, exc_type, exc_val, exc_tb):
-        if self.trigger:
-            if self._is_saving:
-                for attr, data_tuple in zip(
-                    self._data_tuple_attributes,
-                    self._data_tuples,
-                ):
-                    setattr(self._instance, attr, self._data_tuple_base(*data_tuple))
-                for attr in self.__tmp_attr_list:
-                    self._instance.__dict__.pop(attr)
-                del self._data_tuples
-            else:
-                attr_pool_map = self._get_attr()
-                for core_attr, attr_dict in attr_pool_map.items():
-                    local_attr_values = []
-                    for idx in range(len(attr_dict)):
-                        local_attr = attr_dict[idx]
-                        local_attr_values.append(
-                            self._instance.__dict__.pop(local_attr)
-                        )
-                    setattr(
-                        self._instance,
-                        core_attr,
-                        self._data_tuple_base(*local_attr_values),
-                    )
-
-    def _get_attr(
-        self,
-        attr: Optional[str] = None,
-        data_tuple: Optional[NamedTuple] = None,
-    ) -> Optional[Union[List[str], Dict[str, Dict[int, str]]]]:
-        prefix = self.__prefix__
-        if self._is_saving:
-            if data_tuple is None:
-                raise ValueError("data tuple should be provided in saving context")
-            assert isinstance(attr, str), "attr should be string in saving context"
-            return [f"{prefix}{attr}_{i}" for i in range(len(data_tuple))]
-        attr_pool = list(
-            filter(
-                lambda attr_: attr_.startswith(prefix),
-                self._instance.__dict__.keys(),
-            )
-        )
-        attr_pool_split = [attr_[len(prefix) :].split("_") for attr_ in attr_pool]
-        attr_pool_map = {}
-        for attr, attr_split in zip(attr_pool, attr_pool_split):
-            core_attr, idx = "_".join(attr_split[:-1]), int(attr_split[-1])
-            local_map = attr_pool_map.setdefault(core_attr, {})
-            local_map[idx] = attr
-        loaded_attr_list = sorted(attr_pool_map)
-        preset_attr_list = sorted(self._data_tuple_attributes)
-        assert_msg = (
-            f"loaded attributes ({loaded_attr_list}) "
-            f"are not identical with preset attributes ({preset_attr_list})"
-        )
-        assert loaded_attr_list == preset_attr_list, assert_msg
-        return attr_pool_map
+import os
+import sys
+import dill
+import json
+import math
+import time
+import errno
+import random
+import shutil
+import decimal
+import inspect
+import logging
+import hashlib
+import zipfile
+import operator
+import threading
+import unicodedata
+
+import numpy as np
+
+from abc import abstractmethod
+from abc import ABC
+from abc import ABCMeta
+from tqdm import tqdm
+from typing import Any
+from typing import Set
+from typing import Dict
+from typing import List
+from typing import Type
+from typing import Union
+from typing import Generic
+from typing import TypeVar
+from typing import Callable
+from typing import Iterable
+from typing import Optional
+from typing import Protocol
+from typing import NamedTuple
+from argparse import Namespace
+from datetime import datetime
+from datetime import timedelta
+from functools import reduce
+from functools import partial
+from itertools import product
+from collections import OrderedDict
+from dataclasses import asdict
+from dataclasses import fields
+from dataclasses import dataclass
+from dataclasses import Field
+
+from .types import configs_type
+from .types import np_dict_type
+from .types import general_config_type
+from .constants import TIME_FORMAT
+
+
+dill._dill._reverse_typemap["ClassType"] = type
+
+
+# util functions
+
+
+TFnResponse = TypeVar("TFnResponse")
+
+
+class Fn(Protocol):
+    def __call__(self, *args: Any, **kwargs: Any) -> TFnResponse:
+        pass
+
+
+def walk(
+    root: str,
+    hierarchy_callback: Callable[[List[str], str], None],
+    filter_extensions: Optional[Set[str]] = None,
+) -> None:
+    walked = list(os.walk(root))
+    for folder, _, files in tqdm(walked, desc="folders", position=0, mininterval=1):
+        for file in tqdm(files, desc="files", position=1, leave=False, mininterval=1):
+            if filter_extensions is not None:
+                if not any(file.endswith(ext) for ext in filter_extensions):
+                    continue
+            hierarchy = folder.split(os.path.sep) + [file]
+            hierarchy_callback(hierarchy, os.path.join(folder, file))
+
+
+def parse_config(config: general_config_type) -> Dict[str, Any]:
+    if config is None:
+        return {}
+    if isinstance(config, str):
+        with open(config, "r") as f:
+            return json.load(f)
+    return shallow_copy_dict(config)
+
+
+def check_requires(fn: Any, name: str, strict: bool = True) -> bool:
+    if isinstance(fn, type):
+        fn = fn.__init__  # type: ignore
+    signature = inspect.signature(fn)
+    for k, param in signature.parameters.items():
+        if not strict and param.kind is inspect.Parameter.VAR_KEYWORD:
+            return True
+        if k == name:
+            if param.kind is inspect.Parameter.VAR_POSITIONAL:
+                return False
+            return True
+    return False
+
+
+def get_requirements(fn: Any) -> List[str]:
+    if isinstance(fn, type):
+        fn = fn.__init__  # type: ignore
+    requirements = []
+    signature = inspect.signature(fn)
+    for k, param in signature.parameters.items():
+        if param.kind is inspect.Parameter.VAR_KEYWORD:
+            continue
+        if param.kind is inspect.Parameter.VAR_POSITIONAL:
+            continue
+        if param.default is not inspect.Parameter.empty:
+            continue
+        requirements.append(k)
+    return requirements
+
+
+def filter_kw(
+    fn: Callable,
+    kwargs: Dict[str, Any],
+    *,
+    strict: bool = False,
+) -> Dict[str, Any]:
+    kw = {}
+    for k, v in kwargs.items():
+        if check_requires(fn, k, strict):
+            kw[k] = v
+    return kw
+
+
+def safe_execute(fn: Fn, kw: Dict[str, Any], *, strict: bool = False) -> TFnResponse:
+    return fn(**filter_kw(fn, kw, strict=strict))
+
+
+def get_num_positional_args(fn: Callable) -> Union[int, float]:
+    signature = inspect.signature(fn)
+    counter = 0
+    for param in signature.parameters.values():
+        if param.kind is inspect.Parameter.VAR_POSITIONAL:
+            return math.inf
+        if param.kind is inspect.Parameter.POSITIONAL_ONLY:
+            counter += 1
+        elif param.kind is inspect.Parameter.POSITIONAL_OR_KEYWORD:
+            counter += 1
+    return counter
+
+
+def prepare_workspace_from(
+    workspace: str,
+    *,
+    timeout: timedelta = timedelta(30),
+    make: bool = True,
+) -> str:
+    current_time = datetime.now()
+    if os.path.isdir(workspace):
+        for stuff in os.listdir(workspace):
+            if not os.path.isdir(os.path.join(workspace, stuff)):
+                continue
+            try:
+                stuff_time = datetime.strptime(stuff, TIME_FORMAT)
+                stuff_delta = current_time - stuff_time
+                if stuff_delta > timeout:
+                    msg = f"{stuff} will be removed (already {stuff_delta} ago)"
+                    print_warning(msg)
+                    shutil.rmtree(os.path.join(workspace, stuff))
+            except:
+                pass
+    workspace = os.path.join(workspace, current_time.strftime(TIME_FORMAT))
+    if make:
+        os.makedirs(workspace)
+    return workspace
+
+
+def get_latest_workspace(root: str) -> Optional[str]:
+    if not os.path.isdir(root):
+        return None
+    all_workspaces = []
+    for stuff in os.listdir(root):
+        if not os.path.isdir(os.path.join(root, stuff)):
+            continue
+        try:
+            datetime.strptime(stuff, TIME_FORMAT)
+            all_workspaces.append(stuff)
+        except:
+            pass
+    if not all_workspaces:
+        return None
+    return os.path.join(root, sorted(all_workspaces)[-1])
+
+
+def sort_dict_by_value(d: Dict[Any, Any], *, reverse: bool = False) -> OrderedDict:
+    sorted_items = sorted([(v, k) for k, v in d.items()], reverse=reverse)
+    return OrderedDict({item[1]: item[0] for item in sorted_items})
+
+
+def parse_args(args: Any) -> Namespace:
+    return Namespace(**{k: None if not v else v for k, v in args.__dict__.items()})
+
+
+def get_arguments(
+    *,
+    num_back: int = 0,
+    pop_class_attributes: bool = True,
+) -> Dict[str, Any]:
+    frame = inspect.currentframe().f_back  # type: ignore
+    for _ in range(num_back):
+        frame = frame.f_back
+    if frame is None:
+        raise ValueError("`get_arguments` should be called inside a frame")
+    arguments = inspect.getargvalues(frame)[-1]
+    if pop_class_attributes:
+        arguments.pop("self", None)
+        arguments.pop("__class__", None)
+    return arguments
+
+
+def _rmtree(folder: str, patience: float = 10.0) -> None:
+    if not os.path.isdir(folder):
+        return None
+    t = time.time()
+    while True:
+        try:
+            if time.time() - t >= patience:
+                print()
+                print_warning(f"failed to rmtree: {folder}")
+                break
+            shutil.rmtree(folder)
+            break
+        except:
+            print("", end=".", flush=True)
+            time.sleep(1)
+
+
+def timestamp(simplify: bool = False, ensure_different: bool = False) -> str:
+    """
+    Return current timestamp.
+
+    Parameters
+    ----------
+    simplify : bool. If True, format will be simplified to 'year-month-day'.
+    ensure_different : bool. If True, format will include millisecond.
+
+    Returns
+    -------
+    timestamp : str
+
+    """
+
+    now = datetime.now()
+    if simplify:
+        return now.strftime("%Y-%m-%d")
+    if ensure_different:
+        return now.strftime("%Y-%m-%d_%H-%M-%S-%f")
+    return now.strftime("%Y-%m-%d_%H-%M-%S")
+
+
+def prod(iterable: Iterable) -> float:
+    """Return cumulative production of an iterable."""
+
+    return float(reduce(operator.mul, iterable, 1))
+
+
+def hash_code(code: str) -> str:
+    """Return hash code for a string."""
+
+    code = code.encode()
+    return hashlib.md5(code).hexdigest()
+
+
+def hash_dict(d: Dict[str, Any]) -> str:
+    """Return a consistent hash code for an arbitrary dict."""
+
+    def _hash(_d: Dict[str, Any]) -> str:
+        sorted_keys = sorted(_d)
+        hashes = []
+        for k in sorted_keys:
+            v = _d[k]
+            if isinstance(v, dict):
+                hashes.append(_hash(v))
+            elif isinstance(v, set):
+                hashes.append(hash_code(str(sorted(v))))
+            else:
+                hashes.append(hash_code(str(v)))
+        return hash_code("".join(hashes))
+
+    return _hash(d)
+
+
+def random_hash() -> str:
+    return hash_code(str(random.random()))
+
+
+def prefix_dict(d: Dict[str, Any], prefix: str):
+    """Prefix every key in dict `d` with `prefix`."""
+
+    return {f"{prefix}_{k}": v for k, v in d.items()}
+
+
+def shallow_copy_dict(d: dict) -> dict:
+    d = d.copy()
+    for k, v in d.items():
+        if isinstance(v, dict):
+            d[k] = shallow_copy_dict(v)
+    return d
+
+
+def update_dict(src_dict: dict, tgt_dict: dict) -> dict:
+    """
+    Update tgt_dict with src_dict.
+    * Notice that changes will happen only on keys which src_dict holds.
+
+    Parameters
+    ----------
+    src_dict : dict
+    tgt_dict : dict
+
+    Returns
+    -------
+    tgt_dict : dict
+
+    """
+
+    for k, v in src_dict.items():
+        tgt_v = tgt_dict.get(k)
+        if tgt_v is None:
+            tgt_dict[k] = v
+        elif not isinstance(v, dict):
+            tgt_dict[k] = v
+        else:
+            update_dict(v, tgt_v)
+    return tgt_dict
+
+
+def fix_float_to_length(num: float, length: int) -> str:
+    """Change a float number to string format with fixed length."""
+
+    ctx = decimal.Context()
+    ctx.prec = 2 * length
+    d = ctx.create_decimal(repr(num))
+    str_num = format(d, "f").lower()
+    if str_num == "nan":
+        return f"{str_num:^{length}s}"
+    idx = str_num.find(".")
+    if idx == -1:
+        diff = length - len(str_num)
+        if diff <= 0:
+            return str_num
+        if diff == 1:
+            return f"{str_num}."
+        return f"{str_num}.{'0' * (diff - 1)}"
+    length = max(length, idx)
+    return str_num[:length].ljust(length, "0")
+
+
+def truncate_string_to_length(string: str, length: int) -> str:
+    """Truncate a string to make sure its length not exceeding a given length."""
+
+    if len(string) <= length:
+        return string
+    half_length = int(0.5 * length) - 1
+    head = string[:half_length]
+    tail = string[-half_length:]
+    return f"{head}{'.' * (length - 2 * half_length)}{tail}"
+
+
+def grouped(iterable: Iterable, n: int, *, keep_tail: bool = False) -> List[tuple]:
+    """Group an iterable every `n` elements."""
+
+    if not keep_tail:
+        return list(zip(*[iter(iterable)] * n))
+    with batch_manager(iterable, batch_size=n, max_batch_size=n) as manager:
+        return [tuple(batch) for batch in manager]
+
+
+def grouped_into(iterable: Iterable, n: int) -> List[tuple]:
+    """Group an iterable into `n` groups."""
+
+    elements = list(iterable)
+    num_elements = len(elements)
+    num_elem_per_group = int(math.ceil(num_elements / n))
+    results: List[tuple] = []
+    split_idx = num_elements + n - n * num_elem_per_group
+    start = 0
+    for i in range(split_idx):
+        end = start + num_elem_per_group
+        results.append(tuple(elements[start:end]))
+        start = end
+    for i in range(split_idx, n):
+        end = start + num_elem_per_group - 1
+        results.append(tuple(elements[start:end]))
+        start = end
+    return results
+
+
+def is_numeric(s: Any) -> bool:
+    """Check whether `s` is a number."""
+
+    try:
+        s = float(s)
+        return True
+    except (TypeError, ValueError):
+        try:
+            unicodedata.numeric(s)
+            return True
+        except (TypeError, ValueError):
+            return False
+
+
+def register_core(
+    name: str,
+    global_dict: Dict[str, type],
+    *,
+    allow_duplicate: bool = False,
+    before_register: Optional[Callable] = None,
+    after_register: Optional[Callable] = None,
+):
+    def _register(cls):
+        if before_register is not None:
+            before_register(cls)
+        registered = global_dict.get(name)
+        if registered is not None and not allow_duplicate:
+            print_warning(
+                f"'{name}' has already registered "
+                f"in the given global dict ({global_dict})"
+            )
+            return cls
+        global_dict[name] = cls
+        if after_register is not None:
+            after_register(cls)
+        return cls
+
+    return _register
+
+
+def check(constraints: Dict[str, Union[str, List[str]]], *, raise_error: bool = True):
+    def wrapper(fn):
+        def _check_core(k, v):
+            new_v = v
+            constraint_list = constraints.get(k)
+            if constraint_list is not None:
+                if isinstance(constraint_list, str):
+                    constraint_list = [constraint_list]
+                if constraint_list[0] == "choices":
+                    choices = constraint_list[1]
+                    if v not in choices:
+                        raise ValueError(
+                            f"given value ({v}) is not included in "
+                            f"given choices ({choices})"
+                        )
+                else:
+                    for constraint in constraint_list:
+                        check_rs = getattr(SanityChecker, constraint)(v)
+                        if not check_rs["suc"]:
+                            raise ValueError(check_rs["info"])
+                        new_v = check_rs["n"]
+            if v != new_v:
+                if raise_error:
+                    raise ValueError(
+                        f"'{k}' ({v}, {type(v)}) does not satisfy "
+                        f"Constraints({constraint_list})"
+                    )
+                print_warning(f"'{k}' is cast from {v} -> {new_v}")
+            return new_v
+
+        def inner(*args, **kwargs):
+            signature_keys = list(inspect.signature(fn).parameters.keys())
+            new_args = []
+            for arg, signature_key in zip(args, signature_keys[: len(args)]):
+                new_args.append(_check_core(signature_key, arg))
+            new_kwargs = {}
+            for k, v in kwargs.items():
+                new_kwargs[k] = _check_core(k, v)
+            return fn(*new_args, **new_kwargs)
+
+        return inner
+
+    return wrapper
+
+
+def get_err_msg(err: Exception) -> str:
+    return " | ".join(map(repr, sys.exc_info()[:2] + (str(err),)))
+
+
+# util modules
+
+
+TRegister = TypeVar("TRegister", bound="WithRegister", covariant=True)
+TSerializable = TypeVar("TSerializable", bound="ISerializable", covariant=True)
+TSerializableArrays = TypeVar(
+    "TSerializableArrays",
+    bound="ISerializableArrays",
+    covariant=True,
+)
+TSArrays = TypeVar("TSArrays", bound="ISerializableArrays", covariant=True)
+TSDataClass = TypeVar("TSDataClass", bound="ISerializableDataClass", covariant=True)
+TDataClass = TypeVar("TDataClass", bound="DataClassBase")
+
+
+@dataclass
+class DataClassBase(ABC):
+    @property
+    def fields(self) -> List[Field]:
+        return fields(self)
+
+    @property
+    def field_names(self) -> List[str]:
+        return [f.name for f in self.fields]
+
+    @property
+    def attributes(self) -> List[Any]:
+        return [getattr(self, name) for name in self.field_names]
+
+    def asdict(self) -> Dict[str, Any]:
+        return asdict(self)
+
+    def copy(self: TDataClass) -> TDataClass:
+        return type(self)(**shallow_copy_dict(asdict(self)))
+
+    def update_with(self: TDataClass, other: TDataClass) -> TDataClass:
+        d = update_dict(other.asdict(), self.asdict())
+        return self.__class__(**d)
+
+
+class WithRegister(Generic[TRegister]):
+    d: Dict[str, Type[TRegister]]
+    __identifier__: str
+
+    @classmethod
+    def get(cls: Type[TRegister], name: str) -> Type[TRegister]:
+        return cls.d[name]
+
+    @classmethod
+    def has(cls, name: str) -> bool:
+        return name in cls.d
+
+    @classmethod
+    def make(
+        cls: Type[TRegister],
+        name: str,
+        config: Dict[str, Any],
+        *,
+        ensure_safe: bool = False,
+    ) -> TRegister:
+        base = cls.get(name)
+        if not ensure_safe:
+            return base(**config)  # type: ignore
+        return safe_execute(base, config)
+
+    @classmethod
+    def make_multiple(
+        cls: Type[TRegister],
+        names: Union[str, List[str]],
+        configs: configs_type = None,
+        *,
+        ensure_safe: bool = False,
+    ) -> List[TRegister]:
+        if configs is None:
+            configs = {}
+        if isinstance(names, str):
+            assert isinstance(configs, dict)
+            return cls.make(names, configs, ensure_safe=ensure_safe)  # type: ignore
+        if not isinstance(configs, list):
+            configs = [configs.get(name, {}) for name in names]
+        return [
+            cls.make(name, shallow_copy_dict(config), ensure_safe=ensure_safe)
+            for name, config in zip(names, configs)
+        ]
+
+    @classmethod
+    def register(
+        cls,
+        name: str,
+        *,
+        allow_duplicate: bool = False,
+    ) -> Callable:
+        def before(cls_: Type) -> None:
+            cls_.__identifier__ = name
+
+        return register_core(
+            name,
+            cls.d,
+            allow_duplicate=allow_duplicate,
+            before_register=before,
+        )
+
+    @classmethod
+    def remove(cls, name: str) -> Callable:
+        return cls.d.pop(name)
+
+    @classmethod
+    def check_subclass(cls, name: str) -> bool:
+        return issubclass(cls.d[name], cls)
+
+
+@dataclass
+class JsonPack(DataClassBase):
+    type: str
+    info: Dict[str, Any]
+
+
+class ISerializable(WithRegister, Generic[TSerializable], metaclass=ABCMeta):
+    # abstract
+
+    @abstractmethod
+    def to_info(self) -> Dict[str, Any]:
+        pass
+
+    @abstractmethod
+    def from_info(self, info: Dict[str, Any]) -> None:
+        pass
+
+    # optional callbacks
+
+    def after_load(self) -> None:
+        pass
+
+    # api
+
+    def to_pack(self) -> JsonPack:
+        return JsonPack(self.__identifier__, self.to_info())
+
+    @classmethod
+    def from_pack(cls: Type[TSerializable], pack: Dict[str, Any]) -> TSerializable:
+        obj: ISerializable = cls.make(pack["type"], {})
+        obj.from_info(pack["info"])
+        obj.after_load()
+        return obj
+
+    def to_json(self) -> str:
+        return json.dumps(self.to_pack().asdict())
+
+    @classmethod
+    def from_json(cls: Type[TSerializable], json_string: str) -> TSerializable:
+        return cls.from_pack(json.loads(json_string))
+
+    def copy(self: TSerializable) -> TSerializable:
+        copied = self.__class__()
+        copied.from_info(shallow_copy_dict(self.to_info()))
+        return copied
+
+
+class PureFromInfoMixin:
+    def from_info(self, info: Dict[str, Any]) -> None:
+        for k, v in info.items():
+            setattr(self, k, v)
+
+
+class ISerializableArrays(ISerializable, Generic[TSArrays], metaclass=ABCMeta):
+    @abstractmethod
+    def to_npd(self) -> np_dict_type:
+        pass
+
+    @abstractmethod
+    def from_npd(self, npd: np_dict_type) -> None:
+        pass
+
+    def copy(self: TSerializableArrays) -> TSerializableArrays:
+        copied: TSerializableArrays = super().copy()
+        copied.from_npd(shallow_copy_dict(self.to_npd()))
+        return copied
+
+
+@dataclass
+class ISerializableDataClass(
+    ISerializable,
+    DataClassBase,
+    Generic[TSDataClass],
+    metaclass=ABCMeta,
+):
+    @classmethod
+    @abstractmethod
+    def d(cls) -> Dict[str, Type["ISerializableDataClass"]]:
+        pass
+
+    def to_info(self) -> Dict[str, Any]:
+        return self.asdict()
+
+    def from_info(self, info: Dict[str, Any]) -> None:
+        for k, v in info.items():
+            setattr(self, k, v)
+
+    @classmethod
+    def get(cls: Type[TRegister], name: str) -> Type[TRegister]:
+        return cls.d()[name]
+
+    @classmethod
+    def has(cls, name: str) -> bool:
+        return name in cls.d()
+
+    @classmethod
+    def register(
+        cls,
+        name: str,
+        *,
+        allow_duplicate: bool = False,
+    ) -> Callable:
+        def before(cls_: Type) -> None:
+            cls_.__identifier__ = name
+
+        return register_core(
+            name,
+            cls.d(),
+            allow_duplicate=allow_duplicate,
+            before_register=before,
+        )
+
+    @classmethod
+    def remove(cls, name: str) -> Callable:
+        return cls.d().pop(name)
+
+    @classmethod
+    def check_subclass(cls, name: str) -> bool:
+        return issubclass(cls.d()[name], cls)
+
+
+class Serializer:
+    id_file: str = "id.txt"
+    info_file: str = "info.json"
+    npd_folder: str = "npd"
+
+    @classmethod
+    def save_info(
+        cls,
+        folder: str,
+        *,
+        info: Optional[Dict[str, Any]] = None,
+        serializable: Optional[ISerializable] = None,
+    ) -> None:
+        os.makedirs(folder, exist_ok=True)
+        if info is None and serializable is None:
+            raise ValueError("either `info` or `serializable` should be provided")
+        if info is None:
+            info = serializable.to_info()
+        with open(os.path.join(folder, cls.info_file), "w") as f:
+            json.dump(info, f)
+
+    @classmethod
+    def load_info(cls, folder: str) -> Dict[str, Any]:
+        return cls.try_load_info(folder, strict=True)
+
+    @classmethod
+    def try_load_info(
+        cls,
+        folder: str,
+        *,
+        strict: bool = False,
+    ) -> Optional[Dict[str, Any]]:
+        info_path = os.path.join(folder, cls.info_file)
+        if not os.path.isfile(info_path):
+            if not strict:
+                return
+            raise ValueError(f"'{info_path}' does not exist")
+        with open(info_path, "r") as f:
+            info = json.load(f)
+        return info
+
+    @classmethod
+    def save_npd(
+        cls,
+        folder: str,
+        *,
+        npd: Optional[np_dict_type] = None,
+        serializable: Optional[ISerializableArrays] = None,
+    ) -> None:
+        os.makedirs(folder, exist_ok=True)
+        if npd is None and serializable is None:
+            raise ValueError("either `npd` or `serializable` should be provided")
+        if npd is None:
+            npd = serializable.to_npd()
+        npd_folder = os.path.join(folder, cls.npd_folder)
+        os.makedirs(npd_folder, exist_ok=True)
+        for k, v in npd.items():
+            np.save(os.path.join(npd_folder, f"{k}.npy"), v)
+
+    @classmethod
+    def load_npd(cls, folder: str) -> np_dict_type:
+        os.makedirs(folder, exist_ok=True)
+        npd_folder = os.path.join(folder, cls.npd_folder)
+        if not os.path.isdir(npd_folder):
+            raise ValueError(f"'{npd_folder}' does not exist")
+        npd = {}
+        for file in os.listdir(npd_folder):
+            key = os.path.splitext(file)[0]
+            npd[key] = np.load(os.path.join(npd_folder, file))
+        return npd
+
+    @classmethod
+    def save(
+        cls,
+        folder: str,
+        serializable: ISerializable,
+        *,
+        save_npd: bool = True,
+    ) -> None:
+        cls.save_info(folder, serializable=serializable)
+        if save_npd and isinstance(serializable, ISerializableArrays):
+            cls.save_npd(folder, serializable=serializable)
+        with open(os.path.join(folder, cls.id_file), "w") as f:
+            f.write(serializable.__identifier__)
+
+    @classmethod
+    def load(
+        cls,
+        folder: str,
+        base: Type[TSerializable],
+        *,
+        swap_id: Optional[str] = None,
+        swap_info: Optional[Dict[str, Any]] = None,
+        load_npd: bool = True,
+    ) -> TSerializable:
+        serializable = cls.load_empty(folder, base, swap_id=swap_id)
+        serializable.from_info(swap_info or cls.load_info(folder))
+        if load_npd and isinstance(serializable, ISerializableArrays):
+            serializable.from_npd(cls.load_npd(folder))
+        return serializable
+
+    @classmethod
+    def load_empty(
+        cls,
+        folder: str,
+        base: Type[TSerializable],
+        *,
+        swap_id: Optional[str] = None,
+    ) -> TSerializable:
+        if swap_id is not None:
+            s_type = swap_id
+        else:
+            id_path = os.path.join(folder, cls.id_file)
+            if not os.path.isfile(id_path):
+                raise ValueError(f"cannot find '{id_path}'")
+            with open(id_path, "r") as f:
+                s_type = f.read().strip()
+        return base.make(s_type, {})
+
+
+class IWithRequirements:
+    @classmethod
+    def requirements(cls) -> List[str]:
+        requirements = get_requirements(cls)
+        requirements.remove("self")
+        return requirements
+
+
+class SanityChecker:
+    @staticmethod
+    def int(n):
+        rs = {"suc": True}
+        try:
+            rs["n"] = int(n)
+            return rs
+        except Exception as e:
+            rs["suc"], rs["info"] = False, e
+            return rs
+
+    @staticmethod
+    def odd(n):
+        rs = {"suc": True}
+        try:
+            n = rs["n"] = int(n)
+            if n % 2 == 1:
+                return rs
+            rs["suc"], rs["info"] = False, "input is not an odd number"
+            return rs
+        except Exception as e:
+            rs["suc"], rs["info"] = False, e
+            return rs
+
+    @staticmethod
+    def float(n):
+        rs = {"suc": True}
+        try:
+            rs["n"] = float(n)
+            return rs
+        except Exception as e:
+            rs["suc"], rs["info"] = False, e
+            return rs
+
+
+class Incrementer:
+    """
+    Util class which can calculate running mean & running std efficiently.
+
+    Parameters
+    ----------
+    window_size : {int, None}, window size of running statistics.
+    * If None, then all history records will be used for calculation.
+
+    Examples
+    ----------
+    >>> incrementer = Incrementer(window_size=5)
+    >>> for i in range(10):
+    >>>     incrementer.update(i)
+    >>>     if i >= 4:
+    >>>         print(incrementer.mean)  # will print 2.0, 3.0, ..., 6.0, 7.0
+
+    """
+
+    def __init__(self, window_size: int = None):
+        if window_size is not None:
+            if not isinstance(window_size, int):
+                msg = f"window size should be integer, {type(window_size)} found"
+                raise ValueError(msg)
+            if window_size < 2:
+                msg = f"window size should be greater than 2, {window_size} found"
+                raise ValueError(msg)
+        self._window_size = window_size
+        self._n_record = self._previous = None
+        self._running_sum = self._running_square_sum = None
+
+    @property
+    def mean(self):
+        return self._running_sum / self._n_record
+
+    @property
+    def std(self):
+        return math.sqrt(
+            max(
+                0.0,
+                self._running_square_sum / self._n_record - self.mean**2,
+            )
+        )
+
+    @property
+    def n_record(self):
+        return self._n_record
+
+    def update(self, new_value):
+        if self._n_record is None:
+            self._n_record = 1
+            self._running_sum = new_value
+            self._running_square_sum = new_value**2
+        else:
+            self._n_record += 1
+            self._running_sum += new_value
+            self._running_square_sum += new_value**2
+        if self._window_size is not None:
+            if self._previous is None:
+                self._previous = [new_value]
+            else:
+                self._previous.append(new_value)
+            if self._n_record == self._window_size + 1:
+                self._n_record -= 1
+                previous = self._previous.pop(0)
+                self._running_sum -= previous
+                self._running_square_sum -= previous**2
+
+
+class _Formatter(logging.Formatter):
+    """Formatter for logging, which supports millisecond."""
+
+    converter = datetime.fromtimestamp
+
+    def formatTime(self, record, datefmt=None):
+        ct = self.converter(record.created)
+        if datefmt:
+            s = ct.strftime(datefmt)
+        else:
+            t = ct.strftime("%Y-%m-%d %H:%M:%S")
+            s = "%s.%03d" % (t, record.msecs)
+        return s
+
+    def formatMessage(self, record: logging.LogRecord) -> str:
+        record.__dict__.setdefault("func_prefix", "Unknown")
+        return super().formatMessage(record)
+
+
+class LoggingMixin:
+    """
+    Mixin class to provide logging methods for base class.
+
+    Attributes
+    ----------
+    _triggered_ : bool
+    * If not `_triggered_`, log file will not be created.
+
+    _verbose_level_ : int
+    * Preset verbose level of the whole logging process.
+
+    Methods
+    ----------
+    log_msg(self, body, prefix="", verbose_level=1)
+        Log something either through console or to a file.
+        * body : str
+            Main logging message.
+        * prefix : str
+            Prefix added to `body` when logging message goes through console.
+        * verbose_level : int
+            If `self._verbose_level_` >= verbose_level, then logging message
+            will go through console.
+
+    log_block_msg(self, body, prefix="", title="", verbose_level=1)
+        Almost the same as `log_msg`, except adding `title` on top of `body`.
+
+    """
+
+    _triggered_ = False
+    _initialized_ = False
+    _logging_path_ = None
+    _logger_ = _verbose_level_ = None
+    _date_format_string_ = "%Y-%m-%d %H:%M:%S.%f"
+    _formatter_ = _Formatter(
+        "[ {asctime:s} ] [ {levelname:^8s} ] {func_prefix:s} {message:s}",
+        _date_format_string_,
+        style="{",
+    )
+    _timing_dict_, _time_cache_dict_ = {}, {}
+
+    info_prefix = ">  [ info ] "
+    warning_prefix = "> [warning] "
+    error_prefix = "> [ error ] "
+
+    @property
+    def logging_path(self):
+        if self._logging_path_ is None:
+            folder = os.path.join(os.getcwd(), "_logging", type(self).__name__)
+            os.makedirs(folder, exist_ok=True)
+            self._logging_path_ = self.generate_logging_path(folder)
+        return self._logging_path_
+
+    @property
+    def console_handler(self):
+        if self._logger_ is None:
+            return
+        for handler in self._logger_.handlers:
+            if isinstance(handler, logging.StreamHandler):
+                return handler
+
+    @staticmethod
+    def _get_func_prefix(frame=None, return_prefix=True):
+        if frame is None:
+            frame = inspect.currentframe().f_back.f_back
+        if not return_prefix:
+            return frame
+        frame_info = inspect.getframeinfo(frame)
+        file_name = truncate_string_to_length(os.path.basename(frame_info.filename), 16)
+        func_name = truncate_string_to_length(frame_info.function, 24)
+        func_prefix = (
+            f"[ {func_name:^24s} ] [ {file_name:>16s}:{frame_info.lineno:<4d} ]"
+        )
+        return func_prefix
+
+    @staticmethod
+    def _release_handlers(logger):
+        for handler in logger.handlers[:]:
+            handler.close()
+            logger.removeHandler(handler)
+
+    @staticmethod
+    def generate_logging_path(folder: str) -> str:
+        return os.path.join(folder, f"{timestamp()}.log")
+
+    def _init_logging(self, verbose_level: Optional[int] = 2, trigger: bool = True):
+        wants_trigger = trigger and not LoggingMixin._triggered_
+        if LoggingMixin._initialized_ and not wants_trigger:
+            return self
+        LoggingMixin._initialized_ = True
+        logger_name = getattr(self, "_logger_name_", "root")
+        logger = LoggingMixin._logger_ = logging.getLogger(logger_name)
+        LoggingMixin._verbose_level_ = verbose_level
+        if not trigger:
+            return self
+        LoggingMixin._triggered_ = True
+        config = getattr(self, "config", {})
+        self._logging_path_ = config.get("_logging_path_")
+        if self._logging_path_ is None:
+            self._logging_path_ = config["_logging_path_"] = self.logging_path
+        os.makedirs(os.path.dirname(self.logging_path), exist_ok=True)
+        file_handler = logging.FileHandler(self.logging_path, encoding="utf-8")
+        file_handler.setFormatter(self._formatter_)
+        file_handler.setLevel(logging.DEBUG)
+        console = logging.StreamHandler()
+        console.setLevel(logging.INFO)
+        console.setFormatter(_Formatter("{custom_prefix:s}{message:s}", style="{"))
+        logger.setLevel(logging.DEBUG)
+        self._release_handlers(logger)
+        logger.addHandler(console)
+        logger.addHandler(file_handler)
+        self.log_block_msg(sys.version, title="system version", verbose_level=None)
+        return self
+
+    def log_msg(
+        self,
+        body: str,
+        prefix: str = "",
+        verbose_level: Optional[int] = 1,
+        msg_level: int = logging.INFO,
+        frame=None,
+    ):
+        preset_verbose_level = getattr(self, "_verbose_level", None)
+        if preset_verbose_level is not None:
+            self._verbose_level_ = preset_verbose_level
+        elif self._verbose_level_ is None:
+            self._verbose_level_ = 0
+        console_handler = self.console_handler
+        if verbose_level is None or self._verbose_level_ < verbose_level:
+            do_print, console_level = False, msg_level + 10
+        else:
+            do_print, console_level = not LoggingMixin._triggered_, msg_level
+        if console_handler is not None:
+            console_handler.setLevel(console_level)
+        if do_print:
+            print(prefix + body)
+        elif LoggingMixin._triggered_:
+            func_prefix = self._get_func_prefix(frame)
+            self._logger_.log(
+                msg_level,
+                body,
+                extra={"func_prefix": func_prefix, "custom_prefix": prefix},
+            )
+        if console_handler is not None:
+            console_handler.setLevel(logging.INFO)
+
+    def log_block_msg(
+        self,
+        body: str,
+        prefix: str = "",
+        title: str = "",
+        verbose_level: Optional[int] = 1,
+        msg_level: int = logging.INFO,
+        frame=None,
+    ):
+        frame = self._get_func_prefix(frame, False)
+        self.log_msg(f"{title}\n{body}\n", prefix, verbose_level, msg_level, frame)
+
+    def exception(self, body, frame=None):
+        self._logger_.exception(
+            body,
+            extra={
+                "custom_prefix": self.error_prefix,
+                "func_prefix": LoggingMixin._get_func_prefix(frame),
+            },
+        )
+
+    @staticmethod
+    def log_with_external_method(body, prefix, log_method, *args, **kwargs):
+        if log_method is None:
+            print(prefix + body)
+        else:
+            kwargs["frame"] = LoggingMixin._get_func_prefix(
+                kwargs.pop("frame", None),
+                False,
+            )
+            log_method(body, prefix, *args, **kwargs)
+
+    @staticmethod
+    def merge_logs_by_time(*log_files, tgt_file):
+        tgt_folder = os.path.dirname(tgt_file)
+        date_str_len = (
+            len(datetime.today().strftime(LoggingMixin._date_format_string_)) + 4
+        )
+        with lock_manager(tgt_folder, [tgt_file], clear_stuffs_after_exc=False):
+            msg_dict, msg_block, last_searched = {}, [], None
+            for log_file in log_files:
+                with open(log_file, "r") as f:
+                    for line in f:
+                        date_str = line[:date_str_len]
+                        if date_str[:2] == "[ " and date_str[-2:] == " ]":
+                            searched_time = datetime.strptime(
+                                date_str[2:-2],
+                                LoggingMixin._date_format_string_,
+                            )
+                        else:
+                            msg_block.append(line)
+                            continue
+                        if last_searched is not None:
+                            msg_block_ = "".join(msg_block)
+                            msg_dict.setdefault(last_searched, []).append(msg_block_)
+                        last_searched = searched_time
+                        msg_block = [line]
+                    if msg_block:
+                        msg_dict.setdefault(last_searched, []).append(
+                            "".join(msg_block)
+                        )
+            with open(tgt_file, "w") as f:
+                f.write("".join(["".join(msg_dict[key]) for key in sorted(msg_dict)]))
+
+    @classmethod
+    def reset_logging(cls) -> None:
+        cls._triggered_ = False
+        cls._initialized_ = False
+        cls._logging_path_ = None
+        if cls._logger_ is not None:
+            cls._release_handlers(cls._logger_)
+        cls._logger_ = cls._verbose_level_ = None
+        cls._timing_dict_, cls._time_cache_dict_ = {}, {}
+
+    @classmethod
+    def start_timer(cls, name):
+        if name in cls._time_cache_dict_:
+            print_warning(
+                f"'{name}' was already in time cache dict, "
+                "this may cause by calling `start_timer` repeatedly"
+            )
+            return
+        cls._time_cache_dict_[name] = time.time()
+
+    @classmethod
+    def end_timer(cls, name):
+        start_time = cls._time_cache_dict_.pop(name, None)
+        if start_time is None:
+            print_warning(
+                f"'{name}' was not found in time cache dict, "
+                "this may cause by not calling `start_timer` method"
+            )
+            return
+        incrementer = cls._timing_dict_.setdefault(name, Incrementer())
+        incrementer.update(time.time() - start_time)
+
+    def log_timing(self):
+        timing_str_list = ["=" * 138]
+        for name in sorted(self._timing_dict_.keys()):
+            incrementer = self._timing_dict_[name]
+            timing_str_list.append(
+                f"|   {name:<82s}   | "
+                f"{fix_float_to_length(incrementer.mean, 10)} ± "
+                f"{fix_float_to_length(incrementer.std, 10)} | "
+                f"{incrementer.n_record:>12d} hits   |"
+            )
+            timing_str_list.append("-" * 138)
+        self.log_block_msg(
+            "\n".join(timing_str_list),
+            title="timing",
+            verbose_level=None,
+            msg_level=logging.DEBUG,
+        )
+        return self
+
+
+class PureLoggingMixin:
+    """
+    Mixin class to provide (pure) logging method for base class.
+
+    Attributes
+    ----------
+    _loggers_ : dict(int, logging.Logger)
+        Recorded all loggers initialized.
+
+    _formatter_ : _Formatter
+        Formatter for all loggers.
+
+    Methods
+    ----------
+    log_msg(self, name, msg, msg_level=logging.INFO)
+        Log something to a file, with logger initialized by `name`.
+
+    log_block_msg(self, name, title, body, msg_level=logging.INFO)
+        Almost the same as `log_msg`, except adding `title` on top of `body`.
+
+    """
+
+    _name = _meta_name = None
+
+    _formatter_ = LoggingMixin._formatter_
+    _loggers_: Dict[str, logging.Logger] = {}
+    _logger_paths_: Dict[str, str] = {}
+    _timing_dict_ = {}
+
+    @property
+    def meta_suffix(self):
+        return "" if self._meta_name is None else self._meta_name
+
+    @property
+    def name_suffix(self):
+        return "" if self._name is None else f"-{self._name}"
+
+    @property
+    def meta_log_name(self):
+        return f"__meta__{self.meta_suffix}{self.name_suffix}"
+
+    @staticmethod
+    def get_logging_path(logger):
+        logging_path = None
+        for handler in logger.handlers:
+            if isinstance(handler, logging.FileHandler):
+                logging_path = handler.baseFilename
+                break
+        if logging_path is None:
+            raise ValueError(f"No FileHandler was found in given logger '{logger}'")
+        return logging_path
+
+    def _get_logger_info(self, name):
+        logger = name if isinstance(name, logging.Logger) else self._loggers_.get(name)
+        if logger is None:
+            raise ValueError(
+                f"logger for '{name}' is not defined, "
+                "please call `_setup_logger` first"
+            )
+        if isinstance(name, str):
+            logging_path = self._logger_paths_[name]
+        else:
+            logging_path = self.get_logging_path(logger)
+        return logger, os.path.dirname(logging_path), logging_path
+
+    def _setup_logger(self, name, logging_path, level=logging.DEBUG):
+        if name in self._loggers_:
+            return
+        console = logging.StreamHandler()
+        console.setLevel(logging.CRITICAL)
+        console.setFormatter(self._formatter_)
+        file_handler = logging.FileHandler(logging_path)
+        file_handler.setFormatter(self._formatter_)
+        file_handler.setLevel(level)
+        logger = logging.getLogger(name)
+        logger.setLevel(logging.DEBUG)
+        LoggingMixin._release_handlers(logger)
+        logger.addHandler(console)
+        logger.addHandler(file_handler)
+        PureLoggingMixin._loggers_[name] = logger
+        PureLoggingMixin._logger_paths_[name] = logging_path
+        for handler in logging.getLogger().handlers:
+            handler.setLevel(logging.CRITICAL)
+        self.log_block_msg(name, "system version", sys.version)
+
+    def _log_meta_msg(self, msg, msg_level=logging.INFO, frame=None):
+        if frame is None:
+            frame = inspect.currentframe().f_back
+        self.log_msg(self.meta_log_name, msg, msg_level, frame)
+
+    def _log_with_meta(self, task_name, msg, msg_level=logging.INFO, frame=None):
+        if frame is None:
+            frame = inspect.currentframe().f_back
+        self._log_meta_msg(f"{task_name} {msg}", msg_level, frame)
+        self.log_msg(task_name, f"current task {msg}", msg_level, frame)
+
+    def log_msg(self, name, msg, msg_level=logging.INFO, frame=None):
+        logger, logging_folder, logging_path = self._get_logger_info(name)
+        with lock_manager(
+            logging_folder,
+            [logging_path],
+            clear_stuffs_after_exc=False,
+        ):
+            logger.log(
+                msg_level,
+                msg,
+                extra={
+                    "custom_prefix": "",
+                    "func_prefix": LoggingMixin._get_func_prefix(frame),
+                },
+            )
+        return logger
+
+    def log_block_msg(self, name, title, body, msg_level=logging.INFO, frame=None):
+        frame = LoggingMixin._get_func_prefix(frame, False)
+        self.log_msg(name, f"{title}\n{body}\n", msg_level, frame)
+
+    def exception(self, name, msg, frame=None):
+        logger, logging_folder, logging_path = self._get_logger_info(name)
+        with lock_manager(
+            logging_folder,
+            [logging_path],
+            clear_stuffs_after_exc=False,
+        ):
+            logger.exception(
+                msg,
+                extra={
+                    "custom_prefix": LoggingMixin.error_prefix,
+                    "func_prefix": LoggingMixin._get_func_prefix(frame),
+                },
+            )
+
+    def del_logger(self, name):
+        logger = self.log_msg(name, f"clearing up logger information of '{name}'")
+        del self._loggers_[name], self._logger_paths_[name]
+        LoggingMixin._release_handlers(logger)
+        del logger
+
+
+def print_info(msg: str) -> None:
+    print(f"{LoggingMixin.info_prefix}{msg}")
+
+
+def print_warning(msg: str) -> None:
+    print(f"{LoggingMixin.warning_prefix}{msg}")
+
+
+def print_error(msg: str) -> None:
+    print(f"{LoggingMixin.error_prefix}{msg}")
+
+
+class SavingMixin(LoggingMixin):
+    """
+    Mixin class to provide logging & saving method for base class.
+
+    Warnings
+    ----------
+    We require base class to define every property appeared in __init__ (args, kwargs)
+    if we want to utilize `SavingMixin.load_with`
+
+    ```python
+    class Foo:
+        def __init__(self, a, *, b):
+            # these are required
+            self.a = a
+            self.b = b
+            # others could be customized
+            ...
+    ```
+
+    Methods
+    ----------
+    save(self, folder)
+        Save `self` to folder.
+
+    def load(self, folder)
+        Load from folder.
+
+    """
+
+    @property
+    @abstractmethod
+    def data_tuple_base(self) -> Optional[Type[NamedTuple]]:
+        pass
+
+    @property
+    @abstractmethod
+    def data_tuple_attributes(self) -> Optional[List[str]]:
+        pass
+
+    @property
+    def cache_excludes(self):
+        return set()
+
+    @property
+    def lock_verbose(self):
+        verbose_level = getattr(self, "_verbose_level", None)
+        if verbose_level is None:
+            return False
+        return verbose_level >= 5
+
+    def _data_tuple_context(self, *, is_saving: bool):
+        return data_tuple_saving_controller(self, is_saving=is_saving)
+
+    def save(self, folder: str, *, compress: bool = True):
+        with self._data_tuple_context(is_saving=True):
+            Saving.save_instance(self, folder, self.log_msg)
+        if compress:
+            abs_folder = os.path.abspath(folder)
+            base_folder = os.path.dirname(abs_folder)
+            with lock_manager(base_folder, [folder]):
+                Saving.compress(abs_folder, remove_original=True)
+        return self
+
+    def load(self, folder: str, *, compress: bool = True):
+        base_folder = os.path.dirname(os.path.abspath(folder))
+        with lock_manager(base_folder, [folder]):
+            with Saving.compress_loader(
+                folder,
+                compress,
+                remove_extracted=True,
+                logging_mixin=self,
+            ):
+                with self._data_tuple_context(is_saving=False):
+                    Saving.load_instance(self, folder, log_method=self.log_msg)
+        return self
+
+    @staticmethod
+    def load_with(cls: Type, folder: str, *, compress: bool = True) -> Any:
+        # load every thing into a dummy instance
+        dummy = type(cls.__name__, (SavingMixin,), {})()
+        dummy.load(folder, compress=compress)
+        # inject everything into the target instance
+        spec = inspect.getfullargspec(cls.__init__)
+        args = spec.args[1:]
+        kwargs_keys = spec.kwonlyargs
+        arg_values = tuple(getattr(dummy, arg) for arg in args)
+        kwargs = {key: getattr(dummy, key) for key in kwargs_keys}
+        instance = cls(*arg_values, **kwargs)
+        update_dict(dummy.__dict__, instance.__dict__)
+        return instance
+
+
+class Saving(LoggingMixin):
+    """
+    Util class for saving instances.
+
+    Methods
+    ----------
+    save_instance(instance, folder, log_method=None)
+        Save instance to `folder`.
+        * instance : object, instance to save.
+        * folder : str, folder to save to.
+        * log_method : {None, function}, used as `log_method` parameter in
+        `log_with_external_method` method of `LoggingMixin`.
+
+    load_instance(instance, folder, log_method=None)
+        Load instance from `folder`.
+        * instance : object, instance to load, need to be initialized.
+        * folder : str, folder to load from.
+        * log_method : {None, function}, used as `log_method` parameter in
+        `log_with_external_method` method of `LoggingMixin`.
+
+    """
+
+    delim = "^_^"
+    dill_suffix = ".pkl"
+    array_sub_folder = "__arrays"
+
+    @staticmethod
+    def _check_core(elem):
+        if isinstance(elem, dict):
+            if not Saving._check_dict(elem):
+                return False
+        if isinstance(elem, (list, tuple)):
+            if not Saving._check_list_and_tuple(elem):
+                return False
+        if not Saving._check_elem(elem):
+            return False
+        return True
+
+    @staticmethod
+    def _check_elem(elem):
+        if isinstance(elem, (type, np.generic, np.ndarray)):
+            return False
+        if callable(elem):
+            return False
+        try:
+            json.dumps({"": elem})
+            return True
+        except TypeError:
+            return False
+
+    @staticmethod
+    def _check_list_and_tuple(arr: Union[list, tuple]):
+        for elem in arr:
+            if not Saving._check_core(elem):
+                return False
+        return True
+
+    @staticmethod
+    def _check_dict(d: dict):
+        for v in d.values():
+            if not Saving._check_core(v):
+                return False
+        return True
+
+    @staticmethod
+    def save_dict(d: dict, name: str, folder: str) -> str:
+        if Saving._check_dict(d):
+            kwargs = {}
+            suffix, method, mode = ".json", json.dump, "w"
+        else:
+            kwargs = {"recurse": True}
+            suffix, method, mode = Saving.dill_suffix, dill.dump, "wb"
+        file = os.path.join(folder, f"{name}{suffix}")
+        with open(file, mode) as f:
+            method(d, f, **kwargs)
+        return os.path.abspath(file)
+
+    @staticmethod
+    def load_dict(name: str, folder: str = None):
+        if folder is None:
+            folder, name = os.path.split(name)
+        name, suffix = os.path.splitext(name)
+        if not suffix:
+            json_file = os.path.join(folder, f"{name}.json")
+            if os.path.isfile(json_file):
+                with open(json_file, "r") as f:
+                    return json.load(f)
+            dill_file = os.path.join(folder, f"{name}{Saving.dill_suffix}")
+            if os.path.isfile(dill_file):
+                with open(dill_file, "rb") as f:
+                    return dill.load(f)
+        else:
+            assert_msg = f"suffix should be either 'json' or 'pkl', {suffix} found"
+            assert suffix in {".json", ".pkl"}, assert_msg
+            name = f"{name}{suffix}"
+            file = os.path.join(folder, name)
+            if os.path.isfile(file):
+                if suffix == ".json":
+                    mode, load_method = "r", json.load
+                else:
+                    mode, load_method = "rb", dill.load
+                with open(file, mode) as f:
+                    return load_method(f)
+        raise ValueError(f"config '{name}' is not found under '{folder}' folder")
+
+    @staticmethod
+    def deep_copy_dict(d: dict):
+        tmp_folder = os.path.join(os.getcwd(), "___tmp_dict_cache___")
+        if os.path.isdir(tmp_folder):
+            shutil.rmtree(tmp_folder)
+        os.makedirs(tmp_folder)
+        dict_name = "deep_copy"
+        Saving.save_dict(d, dict_name, tmp_folder)
+        loaded_dict = Saving.load_dict(dict_name, tmp_folder)
+        shutil.rmtree(tmp_folder)
+        return loaded_dict
+
+    @staticmethod
+    def get_cache_file(instance):
+        return f"{type(instance).__name__}.pkl"
+
+    @staticmethod
+    def save_instance(instance, folder, log_method=None):
+        instance_str = str(instance)
+        Saving.log_with_external_method(
+            f"saving '{instance_str}' to '{folder}'",
+            Saving.info_prefix,
+            log_method,
+            5,
+        )
+
+        def _record_array(k, v):
+            extension = ".npy" if isinstance(v, np.ndarray) else ".lst"
+            array_attribute_dict[f"{k}{extension}"] = v
+
+        def _check_array(attr_key_, attr_value_, depth=0):
+            if isinstance(attr_value_, dict):
+                for k in list(attr_value_.keys()):
+                    v = attr_value_[k]
+                    extended_k = f"{attr_key_}{delim}{k}"
+                    if isinstance(v, dict):
+                        _check_array(extended_k, v, depth + 1)
+                    elif isinstance(v, array_types):
+                        _record_array(extended_k, v)
+                        attr_value_.pop(k)
+            if isinstance(attr_value_, array_types):
+                _record_array(attr_key_, attr_value_)
+                if depth == 0:
+                    cache_excludes.add(attr_key_)
+
+        main_file = Saving.get_cache_file(instance)
+        instance_dict = shallow_copy_dict(instance.__dict__)
+        verbose, cache_excludes = map(
+            getattr,
+            [instance] * 2,
+            ["lock_verbose", "cache_excludes"],
+            [False, set()],
+        )
+        if os.path.isdir(folder):
+            if verbose:
+                prefix = Saving.warning_prefix
+                msg = f"'{folder}' will be cleaned up when saving '{instance_str}'"
+                Saving.log_with_external_method(
+                    msg, prefix, log_method, msg_level=logging.WARNING
+                )
+            shutil.rmtree(folder)
+        save_path = os.path.join(folder, main_file)
+        array_folder = os.path.join(folder, Saving.array_sub_folder)
+        tuple(
+            map(
+                lambda folder_: os.makedirs(folder_, exist_ok=True),
+                [folder, array_folder],
+            )
+        )
+        sorted_attributes, array_attribute_dict = sorted(instance_dict), {}
+        delim, array_types = Saving.delim, (list, np.ndarray)
+        for attr_key in sorted_attributes:
+            if attr_key in cache_excludes:
+                continue
+            attr_value = instance_dict[attr_key]
+            _check_array(attr_key, attr_value)
+        cache_excludes.add("_verbose_level_")
+        with lock_manager(
+            folder,
+            [os.path.join(folder, main_file)],
+            name=instance_str,
+        ):
+            with open(save_path, "wb") as f:
+                d = {k: v for k, v in instance_dict.items() if k not in cache_excludes}
+                dill.dump(d, f, recurse=True)
+        if array_attribute_dict:
+            sorted_array_files = sorted(array_attribute_dict)
+            sorted_array_files_full_path = list(
+                map(lambda f_: os.path.join(array_folder, f_), sorted_array_files)
+            )
+            with lock_manager(
+                array_folder,
+                sorted_array_files_full_path,
+                name=f"{instance_str} (arrays)",
+            ):
+                for array_file, array_file_full_path in zip(
+                    sorted_array_files, sorted_array_files_full_path
+                ):
+                    array_value = array_attribute_dict[array_file]
+                    if array_file.endswith(".npy"):
+                        np.save(array_file_full_path, array_value)
+                    elif array_file.endswith(".lst"):
+                        with open(array_file_full_path, "wb") as f:
+                            np.save(f, array_value)
+                    else:
+                        raise ValueError(
+                            f"unrecognized file type '{array_file}' occurred"
+                        )
+
+    @staticmethod
+    def load_instance(instance, folder, *, log_method=None, verbose=True):
+        if verbose:
+            Saving.log_with_external_method(
+                f"loading '{instance}' from '{folder}'",
+                Saving.info_prefix,
+                log_method,
+                5,
+            )
+        with open(os.path.join(folder, Saving.get_cache_file(instance)), "rb") as f:
+            instance.__dict__.update(dill.load(f))
+        delim = Saving.delim
+        array_folder = os.path.join(folder, Saving.array_sub_folder)
+        for array_file in os.listdir(array_folder):
+            attr_name, attr_ext = os.path.splitext(array_file)
+            if attr_ext == ".npy":
+                load_method = partial(np.load, allow_pickle=True)
+            elif attr_ext == ".lst":
+
+                def load_method(path):
+                    return np.load(path, allow_pickle=True).tolist()
+
+            else:
+                raise ValueError(f"unrecognized file type '{array_file}' occurred")
+            array_value = load_method(os.path.join(array_folder, array_file))
+            attr_hierarchy = attr_name.split(delim)
+            if len(attr_hierarchy) == 1:
+                instance.__dict__[attr_name] = array_value
+            else:
+                hierarchy_dict = instance.__dict__
+                for attr in attr_hierarchy[:-1]:
+                    hierarchy_dict = hierarchy_dict.setdefault(attr, {})
+                hierarchy_dict[attr_hierarchy[-1]] = array_value
+
+    @staticmethod
+    def prepare_folder(instance, folder):
+        if os.path.isdir(folder):
+            instance.log_msg(
+                f"'{folder}' already exists, it will be cleared up to save our model",
+                instance.warning_prefix,
+                msg_level=logging.WARNING,
+            )
+            shutil.rmtree(folder)
+        os.makedirs(folder)
+
+    @staticmethod
+    def compress(abs_folder, remove_original=True):
+        shutil.make_archive(abs_folder, "zip", abs_folder)
+        if remove_original:
+            shutil.rmtree(abs_folder)
+
+    @staticmethod
+    def compress_loader(
+        folder: str,
+        is_compress: bool,
+        *,
+        remove_extracted: bool = True,
+        logging_mixin: Optional[LoggingMixin] = None,
+    ):
+        class _manager(context_error_handler):
+            def __enter__(self):
+                if is_compress:
+                    if os.path.isdir(folder):
+                        msg = (
+                            f"'{folder}' already exists, "
+                            "it will be cleared up to load our model"
+                        )
+                        if logging_mixin is None:
+                            print(msg)
+                        else:
+                            logging_mixin.log_msg(
+                                msg,
+                                logging_mixin.warning_prefix,
+                                msg_level=logging.WARNING,
+                            )
+                        shutil.rmtree(folder)
+                    with zipfile.ZipFile(f"{folder}.zip", "r") as zip_ref:
+                        zip_ref.extractall(folder)
+
+            def _normal_exit(self, exc_type, exc_val, exc_tb):
+                if is_compress and remove_extracted:
+                    shutil.rmtree(folder)
+
+        return _manager()
+
+
+candidate_type = List[Any]
+candidates_type = Union[List[candidate_type], Dict[str, candidate_type]]
+
+
+class Grid:
+    """
+    Util class provides permutation of simple, flattened candidates.
+    * For permutation of complex, nested param dicts, please refers to
+      `ParamGenerator` in `cftool.param_utils.core`.
+
+    Parameters
+    ----------
+    candidates : candidates_type, cadidates we want to create grid from.
+
+    Examples
+    ----------
+    >>> from cftool.misc import Grid
+    >>>
+    >>> grid = Grid({"a": [1, 2, 3], "b": [1, 2, 3]})
+    >>> for param in grid:
+    >>>     print(param)
+    >>> # output : {'a': 1, 'b': 1}, {'a': 1, 'b': 2}, {'a': 1, 'b': 3}
+    >>> #          {'a': 2, 'b': 1}, ..., {'a': 3, 'b': 3}
+
+    """
+
+    def __init__(self, candidates: candidates_type):
+        self.candidates = candidates
+        self._is_list = isinstance(candidates, list)
+
+    @staticmethod
+    def _yield_lists(lists):
+        yield from map(list, product(*lists))
+
+    def __iter__(self):
+        if self._is_list:
+            yield from self._yield_lists(self.candidates)
+        else:
+            items = sorted(self.candidates.items())
+            if not items:
+                yield {}
+            else:
+                keys, values = zip(*items)
+                for v in map(list, product(*values)):
+                    yield dict(zip(keys, v))
+
+
+nested_type = Dict[str, Union[Any, Dict[str, "nested_type"]]]
+all_nested_type = Dict[str, Union[List[Any], Dict[str, "all_nested_type"]]]
+union_nested_type = Union[nested_type, all_nested_type]
+flattened_type = Dict[str, Any]
+all_flattened_type = Dict[str, List[Any]]
+union_flattened_type = Union[flattened_type, all_flattened_type]
+
+
+def _offset_fn(value) -> int:
+    if not isinstance(value, (list, tuple)):
+        return 1
+    return len(value)
+
+
+class Nested:
+    def __init__(
+        self,
+        nested: union_nested_type,
+        *,
+        offset_fn: Callable[[Any], int] = _offset_fn,
+        delim: str = "^_^",
+    ):
+        self.nested = nested
+        self.offset_fn, self.delim = offset_fn, delim
+        self._flattened = self._sorted_flattened_keys = None
+        self._sorted_flattened_offsets = None
+
+    def apply(self, fn: Callable[[Any], Any]) -> "Nested":
+        def _apply(src, tgt):
+            for k, v in src.items():
+                if isinstance(v, dict):
+                    next_tgt = tgt.setdefault(k, {})
+                    _apply(v, next_tgt)
+                else:
+                    tgt[k] = fn(v)
+            return tgt
+
+        return Nested(_apply(self.nested, {}))
+
+    @property
+    def flattened(self) -> union_flattened_type:
+        if self._flattened is None:
+            self._flattened = self.flatten_nested(self.nested)
+        return self._flattened
+
+    @property
+    def sorted_flattened_keys(self) -> List[str]:
+        if self._sorted_flattened_keys is None:
+            self._sorted_flattened_keys = sorted(self.flattened)
+        return self._sorted_flattened_keys
+
+    @property
+    def sorted_flattened_offsets(self) -> List[int]:
+        if self._sorted_flattened_offsets is None:
+            offsets = []
+            for key in self.sorted_flattened_keys:
+                value = self.get_value_from(key)
+                offsets.append(self.offset_fn(value))
+            self._sorted_flattened_offsets = offsets
+        return self._sorted_flattened_offsets
+
+    def get_value_from(self, flattened_key: str) -> Any:
+        value = self.nested
+        for sub_key in flattened_key.split(self.delim):
+            value = value[sub_key]
+        return value
+
+    def flatten_nested(self, nested: nested_type) -> nested_type:
+        flattened = []
+
+        def _flatten(d, pre_key: Union[None, str]):
+            for name, value in d.items():
+                if pre_key is None:
+                    next_pre_key = name
+                else:
+                    next_pre_key = f"{pre_key}{self.delim}{name}"
+                if isinstance(value, dict):
+                    _flatten(value, next_pre_key)
+                else:
+                    flattened.append((next_pre_key, value))
+            return flattened
+
+        return dict(_flatten(nested, None))
+
+    def nest_flattened(self, flattened: flattened_type) -> nested_type:
+        sorted_pairs = sorted(
+            map(lambda k, v: (k.split(self.delim), v), *zip(*flattened.items())),
+            key=len,
+        )
+        nested = {}
+        for key_list, value in sorted_pairs:
+            if len(key_list) == 1:
+                nested[key_list[0]] = value
+            else:
+                parent = nested.setdefault(key_list[0], {})
+                for key in key_list[1:-1]:
+                    parent = parent.setdefault(key, {})
+                parent[key_list[-1]] = value
+        return nested
+
+    def flattened2array(self, flattened: flattened_type) -> np.ndarray:
+        value_list = []
+        for key in self.sorted_flattened_keys:
+            value = flattened[key]
+            value = list(value) if isinstance(value, (list, tuple)) else [value]
+            value_list.extend(value)
+        return np.array(value_list, np.float32)
+
+    def array2flattened(self, array: np.ndarray) -> flattened_type:
+        cursor = 0
+        flattened = {}
+        for key, offset in zip(
+            self.sorted_flattened_keys,
+            self.sorted_flattened_offsets,
+        ):
+            end = cursor + offset
+            if offset == 1:
+                value = array[cursor]
+            else:
+                value = array[cursor:end].tolist()
+                if isinstance(value, tuple):
+                    value = tuple(value)
+            flattened[key] = value
+            cursor = end
+        return flattened
+
+
+class Sampler:
+    """
+    Util class which can help sampling indices from probabilities.
+
+    Parameters
+    ----------
+    method : str, sampling method.
+    * Currently only 'multinomial' is supported.
+    probabilities : np.ndarray, probabilities we'll use.
+
+    Examples
+    ----------
+    >>> import numpy as np
+    >>> arr = [[0.1, 0.2, 0.3, 0.4], [0.4, 0.3, 0.2, 0.1]]
+    >>> probabilities = np.array(arr, np.float32)
+    >>> sampler = Sampler("multinomial", probabilities)
+    >>> print(sampler.sample(10))
+
+    """
+
+    def __init__(self, method: str, probabilities: np.ndarray):
+        self.method = method
+        self.p = probabilities
+        self._p_shape = list(self.p.shape)
+        if self.is_flat:
+            self._p_block = self.p
+        else:
+            self._p_block = self.p.reshape([-1, self._p_shape[-1]])
+
+    def __str__(self):
+        return f"Sampler({self.method})"
+
+    __repr__ = __str__
+
+    @property
+    def is_flat(self):
+        return len(self._p_shape) == 1
+
+    def _reshape(self, n: int, samples: np.ndarray) -> np.ndarray:
+        return samples.reshape([n] + self._p_shape[:-1]).astype(np.int64)
+
+    def sample(self, n: int) -> np.ndarray:
+        return getattr(self, self.method)(n)
+
+    @staticmethod
+    def _multinomial_flat(n: int, p: np.ndarray) -> np.ndarray:
+        samples = np.random.multinomial(n, p)
+        return np.repeat(np.arange(len(p)), samples)
+
+    def multinomial(self, n: int) -> np.ndarray:
+        if self.is_flat:
+            sampled_indices = self._multinomial_flat(n, self.p)
+        else:
+            stacks = [self._multinomial_flat(n, p) for p in self._p_block]
+            sampled_indices = np.vstack(stacks).T
+        return self._reshape(n, sampled_indices)
+
+
+class DownloadProgressBar(tqdm):
+    def update_to(
+        self,
+        b: int = 1,
+        bsize: int = 1,
+        tsize: Optional[int] = None,
+    ) -> None:
+        if tsize is not None:
+            self.total = tsize
+        self.update(b * bsize - self.n)
+
+
+class OPTBase(ABC):
+    def __init__(self):
+        self._opt = self.defaults
+        self.update_from_env()
+
+    @property
+    @abstractmethod
+    def env_key(self) -> str:
+        pass
+
+    @property
+    @abstractmethod
+    def defaults(self) -> Dict[str, Any]:
+        pass
+
+    def __getattr__(self, __name: str) -> Any:
+        return self._opt[__name]
+
+    def update_from_env(self) -> None:
+        env_opt_json = os.environ.get(self.env_key)
+        if env_opt_json is not None:
+            self._opt.update(json.loads(env_opt_json))
+
+    def opt_context(self, increment: Dict[str, Any]) -> Any:
+        class _:
+            def __init__(self) -> None:
+                self._increment = increment
+                self._backup = shallow_copy_dict(instance._opt)
+
+            def __enter__(self) -> None:
+                instance._opt.update(self._increment)
+
+            def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
+                instance._opt.update(self._backup)
+
+        instance = self
+        return _()
+
+    def opt_env_context(self, increment: Dict[str, Any]) -> Any:
+        class _:
+            def __init__(self) -> None:
+                self._increment = increment
+                self._backup = os.environ.get(instance.env_key)
+
+            def __enter__(self) -> None:
+                os.environ[instance.env_key] = json.dumps(self._increment)
+
+            def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
+                if self._backup is None:
+                    del os.environ[instance.env_key]
+                else:
+                    os.environ[instance.env_key] = self._backup
+
+        instance = self
+        return _()
+
+
+# contexts
+
+
+class context_error_handler:
+    """Util class which provides exception handling when using context manager."""
+
+    @property
+    def exception_suffix(self):
+        return ""
+
+    def _normal_exit(self, exc_type, exc_val, exc_tb):
+        pass
+
+    def _exception_exit(self, exc_type, exc_val, exc_tb):
+        pass
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if not exc_type:
+            self._normal_exit(exc_type, exc_val, exc_tb)
+        else:
+            self._exception_exit(exc_type, exc_val, exc_tb)
+
+
+class timeit(context_error_handler):
+    """
+    Timing context manager.
+
+    Examples
+    --------
+    >>> with timeit("something"):
+    >>>     # do something here
+    >>> # will print ">  [ info ] timing for    something     : x.xxxx"
+
+    """
+
+    def __init__(self, msg, precision=6):
+        self._msg = msg
+        self._p = precision
+
+    def __enter__(self):
+        self._t = time.time()
+
+    def _normal_exit(self, exc_type, exc_val, exc_tb):
+        prefix = LoggingMixin.info_prefix
+        print(
+            f"{prefix}timing for {self._msg:^16s} : "
+            f"{time.time() - self._t:{self._p}.{self._p-2}f}"
+        )
+
+
+class _lock_file_refresher(threading.Thread):
+    def __init__(self, lock_file, delay=1, refresh=0.01):
+        super().__init__()
+        self.__stop_event = threading.Event()
+        self._lock_file, self._delay, self._refresh = lock_file, delay, refresh
+        with open(lock_file, "r") as f:
+            self._lock_file_contents = f.read()
+
+    def run(self) -> None:
+        counter = 0
+        while True:
+            counter += 1
+            time.sleep(self._refresh)
+            if counter * self._refresh >= self._delay:
+                counter = 0
+                with open(self._lock_file, "w") as f:
+                    prefix = "\n\n"
+                    add_line = f"{prefix}refreshed at {timestamp()}"
+                    f.write(self._lock_file_contents + add_line)
+            if self.__stop_event.is_set():
+                break
+
+    def stop(self):
+        self.__stop_event.set()
+
+
+class lock_manager(context_error_handler, LoggingMixin):
+    """
+    Util class to make simultaneously-write process safe with some
+    hacked (ugly) tricks.
+
+    Examples
+    --------
+    >>> import dill
+    >>> workspace = "_cache"
+    >>> target_write_files_full_path = [
+    >>>     os.path.join(workspace, "file1.pkl"),
+    >>>     os.path.join(workspace, "file2.pkl")
+    >>> ]
+    >>> with lock_manager(workspace, target_write_files_full_path):
+    >>>     for write_file_full_path in target_write_files_full_path:
+    >>>         with open(write_file_full_path, "wb") as wf:
+    >>>             dill.dump(..., wf)
+
+    """
+
+    delay = 0.01
+    __lock__ = "__lock__"
+
+    def __init__(
+        self,
+        workspace,
+        stuffs,
+        verbose_level=None,
+        set_lock=True,
+        clear_stuffs_after_exc=True,
+        name=None,
+        wait=1000,
+    ):
+        self._workspace = workspace
+        self._verbose_level = verbose_level
+        self._name, self._wait = name, wait
+        os.makedirs(workspace, exist_ok=True)
+        self._stuffs, self._set_lock = stuffs, set_lock
+        self._clear_stuffs = clear_stuffs_after_exc
+        self._is_locked = False
+
+    def __enter__(self):
+        frame = inspect.currentframe().f_back
+        self.log_msg(
+            f"waiting for lock at {self.lock_file}",
+            self.info_prefix,
+            5,
+            logging.DEBUG,
+            frame,
+        )
+        enter_time = file_modify = None
+        while True:
+            try:
+                fd = os.open(self.lock_file, os.O_CREAT | os.O_EXCL | os.O_RDWR)
+                self.log_msg(
+                    "lock acquired",
+                    self.info_prefix,
+                    5,
+                    logging.DEBUG,
+                    frame,
+                )
+                if not self._set_lock:
+                    self.log_msg(
+                        "releasing lock since set_lock=False",
+                        self.info_prefix,
+                        5,
+                        logging.DEBUG,
+                        frame,
+                    )
+                    os.unlink(self.lock_file)
+                    self.__refresher = None
+                else:
+                    self.log_msg(
+                        "writing info to lock file",
+                        self.info_prefix,
+                        5,
+                        logging.DEBUG,
+                        frame,
+                    )
+                    with os.fdopen(fd, "a") as f:
+                        f.write(
+                            f"name      : {self._name}\n"
+                            f"timestamp : {timestamp()}\n"
+                            f"workspace : {self._workspace}\n"
+                            f"stuffs    :\n{self.cache_stuffs_str}"
+                        )
+                    self.__refresher = _lock_file_refresher(self.lock_file)
+                    self.__refresher.start()
+                break
+            except OSError as e:
+                if e.errno != errno.EEXIST:
+                    raise
+                try:
+                    if file_modify is None:
+                        enter_time = time.time()
+                        file_modify = os.path.getmtime(self.lock_file)
+                    else:
+                        new_file_modify = os.path.getmtime(self.lock_file)
+                        if new_file_modify != file_modify:
+                            enter_time = time.time()
+                            file_modify = new_file_modify
+                        else:
+                            wait_time = time.time() - enter_time
+                            if wait_time >= self._wait:
+                                raise ValueError(
+                                    f"'{self.lock_file}' has been waited "
+                                    f"for too long ({wait_time})"
+                                )
+                    time.sleep(random.random() * self.delay + self.delay)
+                except ValueError:
+                    msg = f"lock_manager was blocked by dead lock ({self.lock_file})"
+                    self.exception(msg)
+                    raise
+                except FileNotFoundError:
+                    pass
+        self.log_block_msg(
+            self.cache_stuffs_str,
+            title="start processing following stuffs:",
+            verbose_level=5,
+            msg_level=logging.DEBUG,
+            frame=frame,
+        )
+        self._is_locked = True
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if self.__refresher is not None:
+            self.__refresher.stop()
+            self.__refresher.join()
+        if self._set_lock:
+            super().__exit__(exc_type, exc_val, exc_tb)
+
+    def _normal_exit(self, exc_type, exc_val, exc_tb, frame=None):
+        if self._set_lock:
+            os.unlink(self.lock_file)
+        if frame is None:
+            frame = inspect.currentframe().f_back.f_back.f_back
+        self.log_msg("lock released", self.info_prefix, 5, logging.DEBUG, frame)
+
+    def _exception_exit(self, exc_type, exc_val, exc_tb):
+        frame = inspect.currentframe().f_back.f_back.f_back
+        if self._clear_stuffs:
+            for stuff in self._stuffs:
+                if os.path.isfile(stuff):
+                    self.log_msg(
+                        f"clearing cached file: {stuff}",
+                        ">> ",
+                        5,
+                        logging.ERROR,
+                        frame,
+                    )
+                    os.remove(stuff)
+                elif os.path.isdir(stuff):
+                    self.log_msg(
+                        f"clearing cached directory: {stuff}",
+                        ">> ",
+                        5,
+                        logging.ERROR,
+                        frame,
+                    )
+                    shutil.rmtree(stuff)
+        self._normal_exit(exc_type, exc_val, exc_tb, frame)
+
+    @property
+    def locked(self):
+        return self._is_locked
+
+    @property
+    def available(self):
+        return not os.path.isfile(self.lock_file)
+
+    @property
+    def cache_stuffs_str(self):
+        return "\n".join([f">> {stuff}" for stuff in self._stuffs])
+
+    @property
+    def exception_suffix(self):
+        return f", clearing caches for safety{self.logging_suffix}"
+
+    @property
+    def lock_file(self):
+        return os.path.join(self._workspace, self.__lock__)
+
+    @property
+    def logging_suffix(self):
+        return "" if self._name is None else f" - {self._name}"
+
+
+class batch_manager(context_error_handler):
+    """
+    Process data in batch.
+
+    Parameters
+    ----------
+    inputs : tuple(np.ndarray), auxiliary array inputs.
+    n_elem : {int, float}, indicates how many elements will be processed in a batch.
+    batch_size : int, indicates the batch_size; if None, batch_size will be
+                      calculated by `n_elem`.
+
+    Examples
+    --------
+    >>> with batch_manager(np.arange(5), np.arange(1, 6), batch_size=2) as manager:
+    >>>     for arr, tensor in manager:
+    >>>         print(arr, tensor)
+    >>>         # Will print:
+    >>>         #   [0 1], [1 2]
+    >>>         #   [2 3], [3 4]
+    >>>         #   [4]  , [5]
+
+    """
+
+    def __init__(
+        self,
+        *inputs,
+        n_elem: int = 1e6,
+        batch_size: Optional[int] = None,
+        max_batch_size: int = 1024,
+    ):
+        if not inputs:
+            raise ValueError("inputs should be provided in general_batch_manager")
+        input_lengths = list(map(len, inputs))
+        self._n, self._inputs = input_lengths[0], inputs
+        assert_msg = "inputs should be of same length"
+        assert all(length == self._n for length in input_lengths), assert_msg
+        if batch_size is not None:
+            self._batch_size = batch_size
+        else:
+            n_elem = int(n_elem)
+            self._batch_size = int(
+                n_elem / sum(map(lambda arr: prod(arr.shape[1:]), inputs))
+            )
+        self._batch_size = min(max_batch_size, min(self._n, self._batch_size))
+        self._n_epoch = int(self._n / self._batch_size)
+        self._n_epoch += int(self._n_epoch * self._batch_size < self._n)
+
+    def __enter__(self):
+        return self
+
+    def __iter__(self):
+        self._start, self._end = 0, self._batch_size
+        return self
+
+    def __next__(self):
+        if self._start >= self._n:
+            raise StopIteration
+        batched_data = tuple(
+            map(
+                lambda arr: arr[self._start : self._end],
+                self._inputs,
+            )
+        )
+        self._start, self._end = self._end, self._end + self._batch_size
+        if len(batched_data) == 1:
+            return batched_data[0]
+        return batched_data
+
+    def __len__(self):
+        return self._n_epoch
+
+
+class timing_context(context_error_handler):
+    """
+    Wrap codes in any base class of `LoggingMixin` with this timing context to timeit.
+
+    Parameters
+    ----------
+    logging_mixin : LoggingMixin, arbitrary base classes of LoggingMixin.
+    name : str, explain what the wrapped codes are doing.
+    enable : bool, whether enable this `timing_context`.
+
+    Examples
+    --------
+    >>> import time
+    >>> import random
+    >>> instance = type(
+    >>>    "test", (LoggingMixin,),
+    >>>    {"config": {}, "_verbose_level": 2}
+    >>> )()._init_logging(2, True)
+    >>> for _ in range(50):
+    >>>     with timing_context(instance, "random sleep"):
+    >>>         time.sleep(random.random() * 0.1)
+    >>> instance.log_timing()
+
+    """
+
+    def __init__(self, logging_mixin: LoggingMixin, name: str, *, enable: bool = True):
+        self._cls, self._name = logging_mixin, name
+        self._enable = enable
+
+    @property
+    def timer_name(self):
+        return f"[{type(self._cls).__name__:^24s}] {self._name}"
+
+    def __enter__(self):
+        if self._enable:
+            self._cls.start_timer(self.timer_name)
+
+    def _normal_exit(self, exc_type, exc_val, exc_tb):
+        if self._enable:
+            self._cls.end_timer(self.timer_name)
+
+
+class data_tuple_saving_controller(context_error_handler):
+    """
+    Help saving DataTuple of SavingMixin.
+
+    Parameters
+    ----------
+    instance : SavingMixin, instance whose DataTuples are to be saved / loaded.
+    is_saving : bool, whether it is a saving context or not.
+    """
+
+    __prefix__ = "_Data_Tuple__"
+
+    def __init__(self, instance: SavingMixin, *, is_saving: bool):
+        self._instance = instance
+        self._is_saving = is_saving
+        self._data_tuple_base = instance.data_tuple_base
+        self._data_tuple_attributes = instance.data_tuple_attributes
+        if self.trigger and is_saving:
+            self._data_tuples: List[NamedTuple] = [
+                instance.__dict__.pop(attr) for attr in self._data_tuple_attributes
+            ]
+
+    def __enter__(self):
+        if self.trigger and self._is_saving:
+            self.__tmp_attr_list = []
+            for attr, data_tuple in zip(
+                self._data_tuple_attributes,
+                self._data_tuples,
+            ):
+                local_attr_list = self._get_attr(attr, data_tuple)
+                for local_attr, data in zip(local_attr_list, data_tuple):
+                    setattr(self._instance, local_attr, data)
+                self.__tmp_attr_list += local_attr_list
+
+    @property
+    def trigger(self):
+        return (
+            self._data_tuple_base is not None
+            and self._data_tuple_attributes is not None
+        )
+
+    def _normal_exit(self, exc_type, exc_val, exc_tb):
+        if self.trigger:
+            if self._is_saving:
+                for attr, data_tuple in zip(
+                    self._data_tuple_attributes,
+                    self._data_tuples,
+                ):
+                    setattr(self._instance, attr, self._data_tuple_base(*data_tuple))
+                for attr in self.__tmp_attr_list:
+                    self._instance.__dict__.pop(attr)
+                del self._data_tuples
+            else:
+                attr_pool_map = self._get_attr()
+                for core_attr, attr_dict in attr_pool_map.items():
+                    local_attr_values = []
+                    for idx in range(len(attr_dict)):
+                        local_attr = attr_dict[idx]
+                        local_attr_values.append(
+                            self._instance.__dict__.pop(local_attr)
+                        )
+                    setattr(
+                        self._instance,
+                        core_attr,
+                        self._data_tuple_base(*local_attr_values),
+                    )
+
+    def _get_attr(
+        self,
+        attr: Optional[str] = None,
+        data_tuple: Optional[NamedTuple] = None,
+    ) -> Optional[Union[List[str], Dict[str, Dict[int, str]]]]:
+        prefix = self.__prefix__
+        if self._is_saving:
+            if data_tuple is None:
+                raise ValueError("data tuple should be provided in saving context")
+            assert isinstance(attr, str), "attr should be string in saving context"
+            return [f"{prefix}{attr}_{i}" for i in range(len(data_tuple))]
+        attr_pool = list(
+            filter(
+                lambda attr_: attr_.startswith(prefix),
+                self._instance.__dict__.keys(),
+            )
+        )
+        attr_pool_split = [attr_[len(prefix) :].split("_") for attr_ in attr_pool]
+        attr_pool_map = {}
+        for attr, attr_split in zip(attr_pool, attr_pool_split):
+            core_attr, idx = "_".join(attr_split[:-1]), int(attr_split[-1])
+            local_map = attr_pool_map.setdefault(core_attr, {})
+            local_map[idx] = attr
+        loaded_attr_list = sorted(attr_pool_map)
+        preset_attr_list = sorted(self._data_tuple_attributes)
+        assert_msg = (
+            f"loaded attributes ({loaded_attr_list}) "
+            f"are not identical with preset attributes ({preset_attr_list})"
+        )
+        assert loaded_attr_list == preset_attr_list, assert_msg
+        return attr_pool_map
```

### Comparing `carefree-toolkit-0.3.6.3/cftool/pipeline.py` & `carefree-toolkit-0.3.6.4/cftool/pipeline.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-import os
-import shutil
-
-from abc import abstractmethod
-from abc import ABCMeta
-from typing import Any
-from typing import Dict
-from typing import List
-from typing import Type
-from typing import Union
-from typing import TypeVar
-from typing import Optional
-from typing import ContextManager
-from zipfile import ZipFile
-from tempfile import mkdtemp
-
-from .misc import WithRegister
-from .misc import ISerializable
-from .misc import ISerializableDataClass
-
-
-TBlock = TypeVar("TBlock", bound="IBlock")
-TConfig = TypeVar("TConfig", bound="ISerializableDataClass")
-TPipeline = TypeVar("TPipeline", bound="IPipeline")
-
-pipelines: Dict[str, Type["IPipeline"]] = {}
-pipeline_blocks: Dict[str, Type["IBlock"]] = {}
-
-
-def get_req_choices(req: TBlock) -> List[str]:
-    return [r.strip() for r in req.__identifier__.split("|")]
-
-
-def check_requirement(block: "IBlock", previous: Dict[str, "IBlock"]) -> None:
-    for req in block.requirements:
-        choices = get_req_choices(req)
-        if all(c != "none" and c not in previous for c in choices):
-            raise ValueError(
-                f"'{block.__identifier__}' requires '{req}', "
-                "but none is provided in the previous blocks"
-            )
-
-
-def get_workspace(folder: str, *, force_new: bool = False) -> ContextManager:
-    class _:
-        tmp_folder: Optional[str]
-
-        def __init__(self) -> None:
-            self.tmp_folder = None
-
-        def __enter__(self) -> str:
-            if os.path.isdir(folder):
-                if not force_new:
-                    return folder
-                self.tmp_folder = mkdtemp()
-                shutil.copytree(folder, self.tmp_folder, dirs_exist_ok=True)
-                return self.tmp_folder
-            path = f"{folder}.zip"
-            if not os.path.isfile(path):
-                raise ValueError(f"neither '{folder}' nor '{path}' exists")
-            self.tmp_folder = mkdtemp()
-            with ZipFile(path, "r") as ref:
-                ref.extractall(self.tmp_folder)
-            return self.tmp_folder
-
-        def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
-            if self.tmp_folder is not None:
-                shutil.rmtree(self.tmp_folder)
-
-    return _()
-
-
-class IBlock(WithRegister["IBlock"], metaclass=ABCMeta):
-    d = pipeline_blocks
-
-    """
-    This property should be injected by the `IPipeline`.
-    > In runtime (i.e. executing the `run` method), this property will represent ALL `IBlock`s used in the `IPipeline`.
-    """
-    previous: Dict[str, TBlock]
-
-    @abstractmethod
-    def build(self, config: TConfig) -> None:
-        """This method can modify the `config` inplace, which will affect the following blocks"""
-
-    @property
-    def requirements(self) -> List[Type[TBlock]]:
-        return []
-
-    def try_get_previous(self, block: Union[str, Type[TBlock]]) -> Optional[TBlock]:
-        if not isinstance(block, str):
-            block = block.__identifier__
-        return self.previous.get(block)
-
-    def get_previous(self, block: Union[str, Type[TBlock]]) -> TBlock:
-        b = self.try_get_previous(block)
-        if b is None:
-            raise ValueError(f"cannot find '{block}' in `previous`")
-        return b
-
-
-class IPipeline(ISerializable["IPipeline"], metaclass=ABCMeta):
-    d = pipelines
-
-    config: TConfig
-    blocks: List[TBlock]
-
-    def __init__(self) -> None:
-        self.blocks = []
-
-    # abstract
-
-    @classmethod
-    @abstractmethod
-    def init(cls: Type[TPipeline], config: TConfig) -> TPipeline:
-        pass
-
-    @property
-    @abstractmethod
-    def config_base(self) -> Type[TConfig]:
-        pass
-
-    @property
-    @abstractmethod
-    def block_base(self) -> Type[TBlock]:
-        pass
-
-    # inheritance
-
-    def to_info(self) -> Dict[str, Any]:
-        using_serializable_blocks = self.using_serializable_blocks
-        return dict(
-            blocks=[
-                b.to_pack().asdict() if using_serializable_blocks else b.__identifier__
-                for b in self.blocks
-            ],
-            config=self.config.to_pack().asdict(),
-        )
-
-    def from_info(self, info: Dict[str, Any]) -> None:
-        self.config = self.config_base.from_pack(info["config"])
-        block_base = self.block_base
-        using_serializable_blocks = self.using_serializable_blocks
-        blocks: List[block_base] = []
-        for block in info["blocks"]:
-            blocks.append(
-                block_base.from_pack(block)
-                if using_serializable_blocks
-                else block_base.make(block, {})
-            )
-        self.build(*blocks)
-
-    # optional callbacks
-
-    def before_block_build(self, block: TBlock) -> None:
-        pass
-
-    def after_block_build(self, block: TBlock) -> None:
-        pass
-
-    # api
-
-    @property
-    def using_serializable_blocks(self) -> bool:
-        return issubclass(self.block_base, ISerializable)
-
-    @property
-    def block_mappings(self) -> Dict[str, TBlock]:
-        return {b.__identifier__: b for b in self.blocks}
-
-    def try_get_block(self, block: Union[str, Type[TBlock]]) -> Optional[TBlock]:
-        if not isinstance(block, str):
-            block = block.__identifier__
-        return self.block_mappings.get(block)
-
-    def get_block(self, block: Union[str, Type[TBlock]]) -> TBlock:
-        b = self.try_get_block(block)
-        if b is None:
-            raise ValueError(f"cannot find '{block}' in `previous`")
-        return b
-
-    def remove(self, *block_names: str) -> None:
-        pop_indices = []
-        for i, block in enumerate(self.blocks):
-            if block.__identifier__ in block_names:
-                pop_indices.append(i)
-        for i in pop_indices[::-1]:
-            self.blocks.pop(i)
-
-    def build(self, *blocks: TBlock) -> None:
-        previous: Dict[str, TBlock] = self.block_mappings
-        for block in blocks:
-            check_requirement(block, previous)
-            block.previous = previous
-            self.before_block_build(block)
-            block.build(self.config)
-            self.after_block_build(block)
-            previous[block.__identifier__] = block
-            self.blocks.append(block)
-
-
-__all__ = [
-    "IBlock",
-    "IPipeline",
-    "TPipeline",
-    "get_workspace",
-    "get_req_choices",
-]
+import os
+import shutil
+
+from abc import abstractmethod
+from abc import ABCMeta
+from typing import Any
+from typing import Dict
+from typing import List
+from typing import Type
+from typing import Union
+from typing import TypeVar
+from typing import Optional
+from typing import ContextManager
+from zipfile import ZipFile
+from tempfile import mkdtemp
+
+from .misc import WithRegister
+from .misc import ISerializable
+from .misc import ISerializableDataClass
+
+
+TBlock = TypeVar("TBlock", bound="IBlock")
+TConfig = TypeVar("TConfig", bound="ISerializableDataClass")
+TPipeline = TypeVar("TPipeline", bound="IPipeline")
+
+pipelines: Dict[str, Type["IPipeline"]] = {}
+pipeline_blocks: Dict[str, Type["IBlock"]] = {}
+
+
+def get_req_choices(req: TBlock) -> List[str]:
+    return [r.strip() for r in req.__identifier__.split("|")]
+
+
+def check_requirement(block: "IBlock", previous: Dict[str, "IBlock"]) -> None:
+    for req in block.requirements:
+        choices = get_req_choices(req)
+        if all(c != "none" and c not in previous for c in choices):
+            raise ValueError(
+                f"'{block.__identifier__}' requires '{req}', "
+                "but none is provided in the previous blocks"
+            )
+
+
+def get_workspace(folder: str, *, force_new: bool = False) -> ContextManager:
+    class _:
+        tmp_folder: Optional[str]
+
+        def __init__(self) -> None:
+            self.tmp_folder = None
+
+        def __enter__(self) -> str:
+            if os.path.isdir(folder):
+                if not force_new:
+                    return folder
+                self.tmp_folder = mkdtemp()
+                shutil.copytree(folder, self.tmp_folder, dirs_exist_ok=True)
+                return self.tmp_folder
+            path = f"{folder}.zip"
+            if not os.path.isfile(path):
+                raise ValueError(f"neither '{folder}' nor '{path}' exists")
+            self.tmp_folder = mkdtemp()
+            with ZipFile(path, "r") as ref:
+                ref.extractall(self.tmp_folder)
+            return self.tmp_folder
+
+        def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
+            if self.tmp_folder is not None:
+                shutil.rmtree(self.tmp_folder)
+
+    return _()
+
+
+class IBlock(WithRegister["IBlock"], metaclass=ABCMeta):
+    d = pipeline_blocks
+
+    """
+    This property should be injected by the `IPipeline`.
+    > In runtime (i.e. executing the `run` method), this property will represent ALL `IBlock`s used in the `IPipeline`.
+    """
+    previous: Dict[str, TBlock]
+
+    @abstractmethod
+    def build(self, config: TConfig) -> None:
+        """This method can modify the `config` inplace, which will affect the following blocks"""
+
+    @property
+    def requirements(self) -> List[Type[TBlock]]:
+        return []
+
+    def try_get_previous(self, block: Union[str, Type[TBlock]]) -> Optional[TBlock]:
+        if not isinstance(block, str):
+            block = block.__identifier__
+        return self.previous.get(block)
+
+    def get_previous(self, block: Union[str, Type[TBlock]]) -> TBlock:
+        b = self.try_get_previous(block)
+        if b is None:
+            raise ValueError(f"cannot find '{block}' in `previous`")
+        return b
+
+
+class IPipeline(ISerializable["IPipeline"], metaclass=ABCMeta):
+    d = pipelines
+
+    config: TConfig
+    blocks: List[TBlock]
+
+    def __init__(self) -> None:
+        self.blocks = []
+
+    # abstract
+
+    @classmethod
+    @abstractmethod
+    def init(cls: Type[TPipeline], config: TConfig) -> TPipeline:
+        pass
+
+    @property
+    @abstractmethod
+    def config_base(self) -> Type[TConfig]:
+        pass
+
+    @property
+    @abstractmethod
+    def block_base(self) -> Type[TBlock]:
+        pass
+
+    # inheritance
+
+    def to_info(self) -> Dict[str, Any]:
+        using_serializable_blocks = self.using_serializable_blocks
+        return dict(
+            blocks=[
+                b.to_pack().asdict() if using_serializable_blocks else b.__identifier__
+                for b in self.blocks
+            ],
+            config=self.config.to_pack().asdict(),
+        )
+
+    def from_info(self, info: Dict[str, Any]) -> None:
+        self.config = self.config_base.from_pack(info["config"])
+        block_base = self.block_base
+        using_serializable_blocks = self.using_serializable_blocks
+        blocks: List[block_base] = []
+        for block in info["blocks"]:
+            blocks.append(
+                block_base.from_pack(block)
+                if using_serializable_blocks
+                else block_base.make(block, {})
+            )
+        self.build(*blocks)
+
+    # optional callbacks
+
+    def before_block_build(self, block: TBlock) -> None:
+        pass
+
+    def after_block_build(self, block: TBlock) -> None:
+        pass
+
+    # api
+
+    @property
+    def using_serializable_blocks(self) -> bool:
+        return issubclass(self.block_base, ISerializable)
+
+    @property
+    def block_mappings(self) -> Dict[str, TBlock]:
+        return {b.__identifier__: b for b in self.blocks}
+
+    def try_get_block(self, block: Union[str, Type[TBlock]]) -> Optional[TBlock]:
+        if not isinstance(block, str):
+            block = block.__identifier__
+        return self.block_mappings.get(block)
+
+    def get_block(self, block: Union[str, Type[TBlock]]) -> TBlock:
+        b = self.try_get_block(block)
+        if b is None:
+            raise ValueError(f"cannot find '{block}' in `previous`")
+        return b
+
+    def remove(self, *block_names: str) -> None:
+        pop_indices = []
+        for i, block in enumerate(self.blocks):
+            if block.__identifier__ in block_names:
+                pop_indices.append(i)
+        for i in pop_indices[::-1]:
+            self.blocks.pop(i)
+
+    def build(self, *blocks: TBlock) -> None:
+        previous: Dict[str, TBlock] = self.block_mappings
+        for block in blocks:
+            check_requirement(block, previous)
+            block.previous = previous
+            self.before_block_build(block)
+            block.build(self.config)
+            self.after_block_build(block)
+            previous[block.__identifier__] = block
+            self.blocks.append(block)
+
+
+__all__ = [
+    "IBlock",
+    "IPipeline",
+    "TPipeline",
+    "get_workspace",
+    "get_req_choices",
+]
```

### Comparing `carefree-toolkit-0.3.6.3/cftool/types.py` & `carefree-toolkit-0.3.6.4/cftool/types.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import numpy as np
-
-from typing import Any
-from typing import Dict
-from typing import List
-from typing import Union
-from typing import Callable
-from typing import Optional
-from typing import NamedTuple
-
-try:
-    import torch
-    import torchvision
-    import torch.nn.functional as F
-except:
-
-    class _torch(NamedTuple):
-        device: Any
-        Tensor: Any
-        from_numpy: Callable
-
-    class _torchvision_utils(NamedTuple):
-        make_grid: Callable
-        save_image: Callable
-
-    class _torchvision(NamedTuple):
-        utils: _torchvision_utils
-
-    torch = _torch(None, None, lambda: None)
-    torchvision = _torchvision_utils(lambda: None, lambda: None)
-    F = None
-
-
-general_config_type = Optional[Union[str, Dict[str, Any]]]
-configs_type = Optional[Union[List[Dict[str, Any]], Dict[str, Any]]]
-
-arr_type = Union[np.ndarray, torch.Tensor]
-np_dict_type = Dict[str, Union[np.ndarray, Any]]
-tensor_dict_type = Dict[str, Union[torch.Tensor, Any]]
+import numpy as np
+
+from typing import Any
+from typing import Dict
+from typing import List
+from typing import Union
+from typing import Callable
+from typing import Optional
+from typing import NamedTuple
+
+try:
+    import torch
+    import torchvision
+    import torch.nn.functional as F
+except:
+
+    class _torch(NamedTuple):
+        device: Any
+        Tensor: Any
+        from_numpy: Callable
+
+    class _torchvision_utils(NamedTuple):
+        make_grid: Callable
+        save_image: Callable
+
+    class _torchvision(NamedTuple):
+        utils: _torchvision_utils
+
+    torch = _torch(None, None, lambda: None)
+    torchvision = _torchvision_utils(lambda: None, lambda: None)
+    F = None
+
+
+general_config_type = Optional[Union[str, Dict[str, Any]]]
+configs_type = Optional[Union[List[Dict[str, Any]], Dict[str, Any]]]
+
+arr_type = Union[np.ndarray, torch.Tensor]
+np_dict_type = Dict[str, Union[np.ndarray, Any]]
+tensor_dict_type = Dict[str, Union[torch.Tensor, Any]]
```

### Comparing `carefree-toolkit-0.3.6.3/setup.py` & `carefree-toolkit-0.3.6.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from setuptools import setup
-from setuptools import find_packages
-
-
-VERSION = "0.3.6.3"
-
-DESCRIPTION = "Some commonly used functions and modules"
-with open("README.md") as f:
-    LONG_DESCRIPTION = f.read()
-
-INSTALL_REQUIRES = [
-    "dill",
-    "tqdm",
-    "future",
-    "psutil",
-    "pathos",
-    "pydantic",
-    "numpy>=1.22.3",
-]
-
-setup(
-    name="carefree-toolkit",
-    version=VERSION,
-    packages=find_packages(exclude=("tests",)),
-    install_requires=INSTALL_REQUIRES,
-    author="carefree0910",
-    author_email="syameimaru.saki@gmail.com",
-    url="https://github.com/carefree0910/carefree-toolkit",
-    download_url=f"https://github.com/carefree0910/carefree-toolkit/archive/v{VERSION}.tar.gz",
-    description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
-    long_description_content_type="text/markdown",
-    keywords="python numpy data-science",
-)
+from setuptools import setup
+from setuptools import find_packages
+
+
+VERSION = "0.3.6.4"
+
+DESCRIPTION = "Some commonly used functions and modules"
+with open("README.md") as f:
+    LONG_DESCRIPTION = f.read()
+
+INSTALL_REQUIRES = [
+    "dill",
+    "tqdm",
+    "future",
+    "psutil",
+    "pathos",
+    "pydantic",
+    "numpy>=1.22.3",
+]
+
+setup(
+    name="carefree-toolkit",
+    version=VERSION,
+    packages=find_packages(exclude=("tests",)),
+    install_requires=INSTALL_REQUIRES,
+    author="carefree0910",
+    author_email="syameimaru.saki@gmail.com",
+    url="https://github.com/carefree0910/carefree-toolkit",
+    download_url=f"https://github.com/carefree0910/carefree-toolkit/archive/v{VERSION}.tar.gz",
+    description=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    long_description_content_type="text/markdown",
+    keywords="python numpy data-science",
+)
```

