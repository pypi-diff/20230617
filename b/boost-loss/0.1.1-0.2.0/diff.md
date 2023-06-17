# Comparing `tmp/boost_loss-0.1.1.tar.gz` & `tmp/boost_loss-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boost_loss-0.1.1.tar", max compression
+gzip compressed data, was "boost_loss-0.2.0.tar", max compression
```

## Comparing `boost_loss-0.1.1.tar` & `boost_loss-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1078 2023-06-16 11:28:07.283080 boost_loss-0.1.1/LICENSE
--rw-r--r--   0        0        0     3968 2023-06-16 11:28:07.283080 boost_loss-0.1.1/README.md
--rw-r--r--   0        0        0     2479 2023-06-16 11:28:08.203142 boost_loss-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      405 2023-06-16 11:28:08.147138 boost_loss-0.1.1/src/boost_loss/__init__.py
--rw-r--r--   0        0        0    15912 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/base.py
--rw-r--r--   0        0        0     1417 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/debug.py
--rw-r--r--   0        0        0        0 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/py.typed
--rw-r--r--   0        0        0      715 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/regression/__init__.py
--rw-r--r--   0        0        0     2354 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/regression/asymmetric.py
--rw-r--r--   0        0        0     9074 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/regression/regression.py
--rw-r--r--   0        0        0    10252 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/regression/sklearn.py
--rw-r--r--   0        0        0     1510 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/resuming.py
--rw-r--r--   0        0        0     7082 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/sklearn.py
--rw-r--r--   0        0        0     6621 2023-06-16 11:28:07.283080 boost_loss-0.1.1/src/boost_loss/torch.py
--rw-r--r--   0        0        0     5335 1970-01-01 00:00:00.000000 boost_loss-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-17 04:36:13.397056 boost_loss-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5315 2023-06-17 04:36:13.397056 boost_loss-0.2.0/README.md
+-rw-r--r--   0        0        0     2479 2023-06-17 04:36:14.213066 boost_loss-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      405 2023-06-17 04:36:14.165066 boost_loss-0.2.0/src/boost_loss/__init__.py
+-rw-r--r--   0        0        0    15912 2023-06-17 04:36:13.397056 boost_loss-0.2.0/src/boost_loss/base.py
+-rw-r--r--   0        0        0     1417 2023-06-17 04:36:13.397056 boost_loss-0.2.0/src/boost_loss/debug.py
+-rw-r--r--   0        0        0        0 2023-06-17 04:36:13.397056 boost_loss-0.2.0/src/boost_loss/py.typed
+-rw-r--r--   0        0        0      715 2023-06-17 04:36:13.397056 boost_loss-0.2.0/src/boost_loss/regression/__init__.py
+-rw-r--r--   0        0        0     2354 2023-06-17 04:36:13.397056 boost_loss-0.2.0/src/boost_loss/regression/asymmetric.py
+-rw-r--r--   0        0        0     9074 2023-06-17 04:36:13.397056 boost_loss-0.2.0/src/boost_loss/regression/regression.py
+-rw-r--r--   0        0        0    10252 2023-06-17 04:36:13.397056 boost_loss-0.2.0/src/boost_loss/regression/sklearn.py
+-rw-r--r--   0        0        0     1510 2023-06-17 04:36:13.397056 boost_loss-0.2.0/src/boost_loss/resuming.py
+-rw-r--r--   0        0        0     8429 2023-06-17 04:36:13.401056 boost_loss-0.2.0/src/boost_loss/sklearn.py
+-rw-r--r--   0        0        0     6621 2023-06-17 04:36:13.401056 boost_loss-0.2.0/src/boost_loss/torch.py
+-rw-r--r--   0        0        0     6682 1970-01-01 00:00:00.000000 boost_loss-0.2.0/PKG-INFO
```

### Comparing `boost_loss-0.1.1/LICENSE` & `boost_loss-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.1/README.md` & `boost_loss-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -174,75 +174,160 @@
 00000ad0: 2320 496e 7374 616c 6c61 7469 6f6e 0a0a  # Installation..
 00000ae0: 496e 7374 616c 6c20 7468 6973 2076 6961  Install this via
 00000af0: 2070 6970 2028 6f72 2079 6f75 7220 6661   pip (or your fa
 00000b00: 766f 7572 6974 6520 7061 636b 6167 6520  vourite package 
 00000b10: 6d61 6e61 6765 7229 3a0a 0a60 6060 7368  manager):..```sh
 00000b20: 656c 6c0a 7069 7020 696e 7374 616c 6c20  ell.pip install 
 00000b30: 626f 6f73 742d 6c6f 7373 0a60 6060 0a0a  boost-loss.```..
-00000b40: 2323 2043 6f6e 7472 6962 7574 6f72 7320  ## Contributors 
-00000b50: e29c a80a 0a54 6861 6e6b 7320 676f 6573  .....Thanks goes
-00000b60: 2074 6f20 7468 6573 6520 776f 6e64 6572   to these wonder
-00000b70: 6675 6c20 7065 6f70 6c65 2028 5b65 6d6f  ful people ([emo
-00000b80: 6a69 206b 6579 5d28 6874 7470 733a 2f2f  ji key](https://
-00000b90: 616c 6c63 6f6e 7472 6962 7574 6f72 732e  allcontributors.
-00000ba0: 6f72 672f 646f 6373 2f65 6e2f 656d 6f6a  org/docs/en/emoj
-00000bb0: 692d 6b65 7929 293a 0a0a 3c21 2d2d 2070  i-key)):..<!-- p
-00000bc0: 7265 7474 6965 722d 6967 6e6f 7265 2d73  rettier-ignore-s
-00000bd0: 7461 7274 202d 2d3e 0a3c 212d 2d20 414c  tart -->.<!-- AL
-00000be0: 4c2d 434f 4e54 5249 4255 544f 5253 2d4c  L-CONTRIBUTORS-L
-00000bf0: 4953 543a 5354 4152 5420 2d20 446f 206e  IST:START - Do n
-00000c00: 6f74 2072 656d 6f76 6520 6f72 206d 6f64  ot remove or mod
-00000c10: 6966 7920 7468 6973 2073 6563 7469 6f6e  ify this section
-00000c20: 202d 2d3e 0a3c 212d 2d20 7072 6574 7469   -->.<!-- pretti
-00000c30: 6572 2d69 676e 6f72 652d 7374 6172 7420  er-ignore-start 
-00000c40: 2d2d 3e0a 3c21 2d2d 206d 6172 6b64 6f77  -->.<!-- markdow
-00000c50: 6e6c 696e 742d 6469 7361 626c 6520 2d2d  nlint-disable --
-00000c60: 3e0a 3c74 6162 6c65 3e0a 2020 3c74 626f  >.<table>.  <tbo
-00000c70: 6479 3e0a 2020 2020 3c74 723e 0a20 2020  dy>.    <tr>.   
-00000c80: 2020 203c 7464 2061 6c69 676e 3d22 6365     <td align="ce
-00000c90: 6e74 6572 2220 7661 6c69 676e 3d22 746f  nter" valign="to
-00000ca0: 7022 2077 6964 7468 3d22 3134 2e32 3825  p" width="14.28%
-00000cb0: 223e 3c61 2068 7265 663d 2268 7474 7073  "><a href="https
-00000cc0: 3a2f 2f67 6974 6875 622e 636f 6d2f 3334  ://github.com/34
-00000cd0: 6a22 3e3c 696d 6720 7372 633d 2268 7474  j"><img src="htt
-00000ce0: 7073 3a2f 2f61 7661 7461 7273 2e67 6974  ps://avatars.git
-00000cf0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000d00: 6f6d 2f75 2f35 3533 3338 3231 353f 763d  om/u/55338215?v=
-00000d10: 343f 733d 3830 2220 7769 6474 683d 2238  4?s=80" width="8
-00000d20: 3070 783b 2220 616c 743d 2233 346a 222f  0px;" alt="34j"/
-00000d30: 3e3c 6272 202f 3e3c 7375 623e 3c62 3e33  ><br /><sub><b>3
-00000d40: 346a 3c2f 623e 3c2f 7375 623e 3c2f 613e  4j</b></sub></a>
-00000d50: 3c62 7220 2f3e 3c61 2068 7265 663d 2268  <br /><a href="h
-00000d60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000d70: 6d2f 3334 6a2f 626f 6f73 742d 6c6f 7373  m/34j/boost-loss
-00000d80: 2f63 6f6d 6d69 7473 3f61 7574 686f 723d  /commits?author=
-00000d90: 3334 6a22 2074 6974 6c65 3d22 436f 6465  34j" title="Code
-00000da0: 223e f09f 92bb 3c2f 613e 203c 6120 6872  ">....</a> <a hr
-00000db0: 6566 3d22 2369 6465 6173 2d33 346a 2220  ef="#ideas-34j" 
-00000dc0: 7469 746c 653d 2249 6465 6173 2c20 506c  title="Ideas, Pl
-00000dd0: 616e 6e69 6e67 2c20 2620 4665 6564 6261  anning, & Feedba
-00000de0: 636b 223e f09f a494 3c2f 613e 203c 6120  ck">....</a> <a 
-00000df0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00000e00: 7468 7562 2e63 6f6d 2f33 346a 2f62 6f6f  thub.com/34j/boo
-00000e10: 7374 2d6c 6f73 732f 636f 6d6d 6974 733f  st-loss/commits?
-00000e20: 6175 7468 6f72 3d33 346a 2220 7469 746c  author=34j" titl
-00000e30: 653d 2244 6f63 756d 656e 7461 7469 6f6e  e="Documentation
-00000e40: 223e f09f 9396 3c2f 613e 3c2f 7464 3e0a  ">....</a></td>.
-00000e50: 2020 2020 3c2f 7472 3e0a 2020 3c2f 7462      </tr>.  </tb
-00000e60: 6f64 793e 0a3c 2f74 6162 6c65 3e0a 0a3c  ody>.</table>..<
-00000e70: 212d 2d20 6d61 726b 646f 776e 6c69 6e74  !-- markdownlint
-00000e80: 2d72 6573 746f 7265 202d 2d3e 0a3c 212d  -restore -->.<!-
-00000e90: 2d20 7072 6574 7469 6572 2d69 676e 6f72  - prettier-ignor
-00000ea0: 652d 656e 6420 2d2d 3e0a 0a3c 212d 2d20  e-end -->..<!-- 
-00000eb0: 414c 4c2d 434f 4e54 5249 4255 544f 5253  ALL-CONTRIBUTORS
-00000ec0: 2d4c 4953 543a 454e 4420 2d2d 3e0a 3c21  -LIST:END -->.<!
-00000ed0: 2d2d 2070 7265 7474 6965 722d 6967 6e6f  -- prettier-igno
-00000ee0: 7265 2d65 6e64 202d 2d3e 0a0a 5468 6973  re-end -->..This
-00000ef0: 2070 726f 6a65 6374 2066 6f6c 6c6f 7773   project follows
-00000f00: 2074 6865 205b 616c 6c2d 636f 6e74 7269   the [all-contri
-00000f10: 6275 746f 7273 5d28 6874 7470 733a 2f2f  butors](https://
-00000f20: 6769 7468 7562 2e63 6f6d 2f61 6c6c 2d63  github.com/all-c
-00000f30: 6f6e 7472 6962 7574 6f72 732f 616c 6c2d  ontributors/all-
-00000f40: 636f 6e74 7269 6275 746f 7273 2920 7370  contributors) sp
-00000f50: 6563 6966 6963 6174 696f 6e2e 2043 6f6e  ecification. Con
-00000f60: 7472 6962 7574 696f 6e73 206f 6620 616e  tributions of an
-00000f70: 7920 6b69 6e64 2077 656c 636f 6d65 210a  y kind welcome!.
+00000b40: 2323 2055 7361 6765 0a0a 2323 2320 4261  ## Usage..### Ba
+00000b50: 7369 6320 5573 6167 650a 0a60 6060 7079  sic Usage..```py
+00000b60: 7468 6f6e 0a69 6d70 6f72 7420 6e75 6d70  thon.import nump
+00000b70: 7920 6173 206e 700a 0a66 726f 6d20 626f  y as np..from bo
+00000b80: 6f73 745f 6c6f 7373 2069 6d70 6f72 7420  ost_loss import 
+00000b90: 4c6f 7373 4261 7365 0a66 726f 6d20 6e75  LossBase.from nu
+00000ba0: 6d70 792e 7479 7069 6e67 2069 6d70 6f72  mpy.typing impor
+00000bb0: 7420 4e44 4172 7261 790a 0a0a 636c 6173  t NDArray...clas
+00000bc0: 7320 4c32 4c6f 7373 284c 6f73 7342 6173  s L2Loss(LossBas
+00000bd0: 6529 3a0a 2020 2020 6465 6620 6c6f 7373  e):.    def loss
+00000be0: 2873 656c 662c 2079 5f74 7275 653a 204e  (self, y_true: N
+00000bf0: 4441 7272 6179 2c20 795f 7072 6564 3a20  DArray, y_pred: 
+00000c00: 4e44 4172 7261 7929 202d 3e20 4e44 4172  NDArray) -> NDAr
+00000c10: 7261 793a 0a20 2020 2020 2020 2072 6574  ray:.        ret
+00000c20: 7572 6e20 2879 5f74 7275 6520 2d20 795f  urn (y_true - y_
+00000c30: 7072 6564 2920 2a2a 2032 202f 2032 0a0a  pred) ** 2 / 2..
+00000c40: 2020 2020 6465 6620 6772 6164 2873 656c      def grad(sel
+00000c50: 662c 2079 5f74 7275 653a 204e 4441 7272  f, y_true: NDArr
+00000c60: 6179 2c20 795f 7072 6564 3a20 4e44 4172  ay, y_pred: NDAr
+00000c70: 7261 7929 202d 3e20 4e44 4172 7261 793a  ray) -> NDArray:
+00000c80: 2023 2064 4c2f 6479 5f70 7265 640a 2020   # dL/dy_pred.  
+00000c90: 2020 2020 2020 7265 7475 726e 202d 2028        return - (
+00000ca0: 795f 7472 7565 202d 2079 5f70 7265 6429  y_true - y_pred)
+00000cb0: 0a0a 2020 2020 6465 6620 6865 7373 2873  ..    def hess(s
+00000cc0: 656c 662c 2079 5f74 7275 653a 204e 4441  elf, y_true: NDA
+00000cd0: 7272 6179 2c20 795f 7072 6564 3a20 4e44  rray, y_pred: ND
+00000ce0: 4172 7261 7929 202d 3e20 4e44 4172 7261  Array) -> NDArra
+00000cf0: 793a 2023 2064 5e32 4c2f 6479 5f70 7265  y: # d^2L/dy_pre
+00000d00: 645e 320a 2020 2020 2020 2020 7265 7475  d^2.        retu
+00000d10: 726e 206e 702e 6f6e 6573 5f6c 696b 6528  rn np.ones_like(
+00000d20: 795f 7472 7565 290a 6060 600a 0a60 6060  y_true).```..```
+00000d30: 7079 7468 6f6e 0a69 6d70 6f72 7420 6c69  python.import li
+00000d40: 6768 7467 626d 2061 7320 6c67 620a 0a66  ghtgbm as lgb..f
+00000d50: 726f 6d20 626f 6f73 745f 6c6f 7373 2069  rom boost_loss i
+00000d60: 6d70 6f72 7420 6170 706c 795f 6375 7374  mport apply_cust
+00000d70: 6f6d 5f6c 6f73 730a 6672 6f6d 2073 6b6c  om_loss.from skl
+00000d80: 6561 726e 2e64 6174 6173 6574 7320 696d  earn.datasets im
+00000d90: 706f 7274 206c 6f61 645f 626f 7374 6f6e  port load_boston
+00000da0: 0a0a 0a58 2c20 7920 3d20 6c6f 6164 5f62  ...X, y = load_b
+00000db0: 6f73 746f 6e28 7265 7475 726e 5f58 5f79  oston(return_X_y
+00000dc0: 3d54 7275 6529 0a61 7070 6c79 5f63 7573  =True).apply_cus
+00000dd0: 746f 6d5f 6c6f 7373 286c 6762 2e4c 4742  tom_loss(lgb.LGB
+00000de0: 4d52 6567 7265 7373 6f72 2829 2c20 4c32  MRegressor(), L2
+00000df0: 4c6f 7373 2829 292e 6669 7428 582c 2079  Loss()).fit(X, y
+00000e00: 290a 6060 600a 0a42 7569 6c74 2d69 6e20  ).```..Built-in 
+00000e10: 6c6f 7373 6573 2061 7265 2061 7661 696c  losses are avail
+00000e20: 6162 6c65 2e20 5b5e 626f 6b62 6f6b 626f  able. [^bokbokbo
+00000e30: 6b5d 0a0a 6060 6070 7974 686f 6e0a 6672  k]..```python.fr
+00000e40: 6f6d 2062 6f6f 7374 5f6c 6f73 732e 7265  om boost_loss.re
+00000e50: 6772 6573 7369 6f6e 2069 6d70 6f72 7420  gression import 
+00000e60: 4c6f 6743 6f73 684c 6f73 730a 6060 600a  LogCoshLoss.```.
+00000e70: 0a23 2323 205b 6074 6f72 6368 2e61 7574  .### [`torch.aut
+00000e80: 6f67 7261 6460 5d28 6874 7470 733a 2f2f  ograd`](https://
+00000e90: 7079 746f 7263 682e 6f72 672f 646f 6373  pytorch.org/docs
+00000ea0: 2f73 7461 626c 652f 6175 746f 6772 6164  /stable/autograd
+00000eb0: 2e68 746d 6c29 204c 6f73 7320 5b5e 6175  .html) Loss [^au
+00000ec0: 746f 6772 6164 5d0a 0a60 6060 7079 7468  tograd]..```pyth
+00000ed0: 6f6e 0a69 6d70 6f72 7420 746f 7263 680a  on.import torch.
+00000ee0: 0a66 726f 6d20 626f 6f73 745f 6c6f 7373  .from boost_loss
+00000ef0: 2e74 6f72 6368 2069 6d70 6f72 7420 546f  .torch import To
+00000f00: 7263 684c 6f73 7342 6173 650a 0a0a 636c  rchLossBase...cl
+00000f10: 6173 7320 4c32 4c6f 7373 546f 7263 6828  ass L2LossTorch(
+00000f20: 546f 7263 684c 6f73 7342 6173 6529 3a0a  TorchLossBase):.
+00000f30: 2020 2020 6465 6620 6c6f 7373 5f74 6f72      def loss_tor
+00000f40: 6368 2873 656c 662c 2079 5f74 7275 653a  ch(self, y_true:
+00000f50: 2074 6f72 6368 2e54 656e 736f 722c 2079   torch.Tensor, y
+00000f60: 5f70 7265 643a 2074 6f72 6368 2e54 656e  _pred: torch.Ten
+00000f70: 736f 7229 202d 3e20 746f 7263 682e 5465  sor) -> torch.Te
+00000f80: 6e73 6f72 3a0a 2020 2020 2020 2020 7265  nsor:.        re
+00000f90: 7475 726e 2028 795f 7472 7565 202d 2079  turn (y_true - y
+00000fa0: 5f70 7265 6429 202a 2a20 3220 2f20 320a  _pred) ** 2 / 2.
+00000fb0: 6060 600a 0a23 2320 436f 6e74 7269 6275  ```..## Contribu
+00000fc0: 746f 7273 20e2 9ca8 0a0a 5468 616e 6b73  tors .....Thanks
+00000fd0: 2067 6f65 7320 746f 2074 6865 7365 2077   goes to these w
+00000fe0: 6f6e 6465 7266 756c 2070 656f 706c 6520  onderful people 
+00000ff0: 285b 656d 6f6a 6920 6b65 795d 2868 7474  ([emoji key](htt
+00001000: 7073 3a2f 2f61 6c6c 636f 6e74 7269 6275  ps://allcontribu
+00001010: 746f 7273 2e6f 7267 2f64 6f63 732f 656e  tors.org/docs/en
+00001020: 2f65 6d6f 6a69 2d6b 6579 2929 3a0a 0a3c  /emoji-key)):..<
+00001030: 212d 2d20 7072 6574 7469 6572 2d69 676e  !-- prettier-ign
+00001040: 6f72 652d 7374 6172 7420 2d2d 3e0a 3c21  ore-start -->.<!
+00001050: 2d2d 2041 4c4c 2d43 4f4e 5452 4942 5554  -- ALL-CONTRIBUT
+00001060: 4f52 532d 4c49 5354 3a53 5441 5254 202d  ORS-LIST:START -
+00001070: 2044 6f20 6e6f 7420 7265 6d6f 7665 206f   Do not remove o
+00001080: 7220 6d6f 6469 6679 2074 6869 7320 7365  r modify this se
+00001090: 6374 696f 6e20 2d2d 3e0a 3c21 2d2d 2070  ction -->.<!-- p
+000010a0: 7265 7474 6965 722d 6967 6e6f 7265 2d73  rettier-ignore-s
+000010b0: 7461 7274 202d 2d3e 0a3c 212d 2d20 6d61  tart -->.<!-- ma
+000010c0: 726b 646f 776e 6c69 6e74 2d64 6973 6162  rkdownlint-disab
+000010d0: 6c65 202d 2d3e 0a3c 7461 626c 653e 0a20  le -->.<table>. 
+000010e0: 203c 7462 6f64 793e 0a20 2020 203c 7472   <tbody>.    <tr
+000010f0: 3e0a 2020 2020 2020 3c74 6420 616c 6967  >.      <td alig
+00001100: 6e3d 2263 656e 7465 7222 2076 616c 6967  n="center" valig
+00001110: 6e3d 2274 6f70 2220 7769 6474 683d 2231  n="top" width="1
+00001120: 342e 3238 2522 3e3c 6120 6872 6566 3d22  4.28%"><a href="
+00001130: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001140: 6f6d 2f33 346a 223e 3c69 6d67 2073 7263  om/34j"><img src
+00001150: 3d22 6874 7470 733a 2f2f 6176 6174 6172  ="https://avatar
+00001160: 732e 6769 7468 7562 7573 6572 636f 6e74  s.githubusercont
+00001170: 656e 742e 636f 6d2f 752f 3535 3333 3832  ent.com/u/553382
+00001180: 3135 3f76 3d34 3f73 3d38 3022 2077 6964  15?v=4?s=80" wid
+00001190: 7468 3d22 3830 7078 3b22 2061 6c74 3d22  th="80px;" alt="
+000011a0: 3334 6a22 2f3e 3c62 7220 2f3e 3c73 7562  34j"/><br /><sub
+000011b0: 3e3c 623e 3334 6a3c 2f62 3e3c 2f73 7562  ><b>34j</b></sub
+000011c0: 3e3c 2f61 3e3c 6272 202f 3e3c 6120 6872  ></a><br /><a hr
+000011d0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000011e0: 7562 2e63 6f6d 2f33 346a 2f62 6f6f 7374  ub.com/34j/boost
+000011f0: 2d6c 6f73 732f 636f 6d6d 6974 733f 6175  -loss/commits?au
+00001200: 7468 6f72 3d33 346a 2220 7469 746c 653d  thor=34j" title=
+00001210: 2243 6f64 6522 3ef0 9f92 bb3c 2f61 3e20  "Code">....</a> 
+00001220: 3c61 2068 7265 663d 2223 6964 6561 732d  <a href="#ideas-
+00001230: 3334 6a22 2074 6974 6c65 3d22 4964 6561  34j" title="Idea
+00001240: 732c 2050 6c61 6e6e 696e 672c 2026 2046  s, Planning, & F
+00001250: 6565 6462 6163 6b22 3ef0 9fa4 943c 2f61  eedback">....</a
+00001260: 3e20 3c61 2068 7265 663d 2268 7474 7073  > <a href="https
+00001270: 3a2f 2f67 6974 6875 622e 636f 6d2f 3334  ://github.com/34
+00001280: 6a2f 626f 6f73 742d 6c6f 7373 2f63 6f6d  j/boost-loss/com
+00001290: 6d69 7473 3f61 7574 686f 723d 3334 6a22  mits?author=34j"
+000012a0: 2074 6974 6c65 3d22 446f 6375 6d65 6e74   title="Document
+000012b0: 6174 696f 6e22 3ef0 9f93 963c 2f61 3e3c  ation">....</a><
+000012c0: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+000012d0: 203c 2f74 626f 6479 3e0a 3c2f 7461 626c   </tbody>.</tabl
+000012e0: 653e 0a0a 3c21 2d2d 206d 6172 6b64 6f77  e>..<!-- markdow
+000012f0: 6e6c 696e 742d 7265 7374 6f72 6520 2d2d  nlint-restore --
+00001300: 3e0a 3c21 2d2d 2070 7265 7474 6965 722d  >.<!-- prettier-
+00001310: 6967 6e6f 7265 2d65 6e64 202d 2d3e 0a0a  ignore-end -->..
+00001320: 3c21 2d2d 2041 4c4c 2d43 4f4e 5452 4942  <!-- ALL-CONTRIB
+00001330: 5554 4f52 532d 4c49 5354 3a45 4e44 202d  UTORS-LIST:END -
+00001340: 2d3e 0a3c 212d 2d20 7072 6574 7469 6572  ->.<!-- prettier
+00001350: 2d69 676e 6f72 652d 656e 6420 2d2d 3e0a  -ignore-end -->.
+00001360: 0a54 6869 7320 7072 6f6a 6563 7420 666f  .This project fo
+00001370: 6c6c 6f77 7320 7468 6520 5b61 6c6c 2d63  llows the [all-c
+00001380: 6f6e 7472 6962 7574 6f72 735d 2868 7474  ontributors](htt
+00001390: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000013a0: 616c 6c2d 636f 6e74 7269 6275 746f 7273  all-contributors
+000013b0: 2f61 6c6c 2d63 6f6e 7472 6962 7574 6f72  /all-contributor
+000013c0: 7329 2073 7065 6369 6669 6361 7469 6f6e  s) specification
+000013d0: 2e20 436f 6e74 7269 6275 7469 6f6e 7320  . Contributions 
+000013e0: 6f66 2061 6e79 206b 696e 6420 7765 6c63  of any kind welc
+000013f0: 6f6d 6521 0a0a 5b5e 626f 6b62 6f6b 626f  ome!..[^bokbokbo
+00001400: 6b5d 3a20 496e 7370 6972 6564 2062 7920  k]: Inspired by 
+00001410: 5b6f 7263 6861 7264 6269 7264 732f 626f  [orchardbirds/bo
+00001420: 6b62 6f6b 626f 6b5d 2868 7474 7073 3a2f  kbokbok](https:/
+00001430: 2f67 6974 6875 622e 636f 6d2f 6f72 6368  /github.com/orch
+00001440: 6172 6462 6972 6473 2f62 6f6b 626f 6b62  ardbirds/bokbokb
+00001450: 6f6b 290a 5b5e 6175 746f 6772 6164 5d3a  ok).[^autograd]:
+00001460: 2049 6e73 7069 7265 6420 6279 205b 546f   Inspired by [To
+00001470: 6d65 7252 6f6e 656e 3334 2f74 7265 6562  merRonen34/treeb
+00001480: 6f6f 7374 5f61 7574 6f67 7261 645d 2868  oost_autograd](h
+00001490: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000014a0: 6d2f 546f 6d65 7252 6f6e 656e 3334 2f74  m/TomerRonen34/t
+000014b0: 7265 6562 6f6f 7374 5f61 7574 6f67 7261  reeboost_autogra
+000014c0: 6429 0a                                  d).
```

### Comparing `boost_loss-0.1.1/pyproject.toml` & `boost_loss-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boost-loss"
-version = "0.1.1"
+version = "0.2.0"
 description = "Utilities for easy use of custom losses in CatBoost, LightGBM, XGBoost"
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/boost-loss"
 documentation = "https://boost-loss.readthedocs.io"
 classifiers = [
```

### Comparing `boost_loss-0.1.1/src/boost_loss/base.py` & `boost_loss-0.2.0/src/boost_loss/base.py`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.1/src/boost_loss/debug.py` & `boost_loss-0.2.0/src/boost_loss/debug.py`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.1/src/boost_loss/regression/__init__.py` & `boost_loss-0.2.0/src/boost_loss/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.1/src/boost_loss/regression/asymmetric.py` & `boost_loss-0.2.0/src/boost_loss/regression/asymmetric.py`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.1/src/boost_loss/regression/regression.py` & `boost_loss-0.2.0/src/boost_loss/regression/regression.py`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.1/src/boost_loss/regression/sklearn.py` & `boost_loss-0.2.0/src/boost_loss/regression/sklearn.py`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.1/src/boost_loss/resuming.py` & `boost_loss-0.2.0/src/boost_loss/resuming.py`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.1/src/boost_loss/sklearn.py` & `boost_loss-0.2.0/src/boost_loss/sklearn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import functools
 import importlib.util
 from typing import Any, Literal, TypeVar, overload
-from unittest.mock import patch
 
 import catboost as cb
 import lightgbm as lgb
 import numpy as np
 import xgboost as xgb
 from sklearn.base import BaseEstimator, clone
 from sklearn.compose import TransformedTargetRegressor
@@ -78,19 +77,19 @@
     if isinstance(estimator, cb.CatBoost):
         estimator.set_params(loss_function=loss, eval_metric=loss)
     if isinstance(estimator, lgb.LGBMModel):
         estimator.set_params(objective=loss)
         estimator_fit = estimator.fit
 
         @functools.wraps(estimator_fit)
-        def fit(self: lgb.LGBMModel, X: Any, y: Any, **fit_params: Any) -> Any:
+        def fit(X: Any, y: Any, **fit_params: Any) -> Any:
             fit_params["eval_metric"] = loss.eval_metric_lgb
-            return estimator_fit(self, X, y, **fit_params)
+            return estimator_fit(X, y, **fit_params)
 
-        patch.object(estimator, "fit", fit)
+        setattr(estimator, "fit", fit)
     if isinstance(estimator, xgb.XGBModel):
         estimator.set_params(objective=loss, eval_metric=loss.eval_metric_xgb_sklearn)
 
     if recursive:
         for key, value in estimator.get_params(deep=True).items():
             if hasattr(value, "fit"):
                 estimator.set_params(
@@ -110,14 +109,16 @@
     from ngboost import NGBoost
     from ngboost.distns import Normal
     from numpy.typing import NDArray
 
     def patch_ngboost(estimator: NGBoost) -> NGBoost:
         """Patch NGBoost to return only the mean prediction in `predict`
         and the variance in `predict_var` to be consistent with other models.
+        The patch will not apply if the estimator is cloned using `sklearn.base.clone()`
+        and requires re-patching.
 
         Parameters
         ----------
         estimator : NGBoost
             The NGBoost estimator to patch.
 
         Returns
@@ -145,27 +146,30 @@
         setattr(estimator, "predict_std", predict_std)
         return estimator
 
 
 def patch_catboost(estimator: cb.CatBoost) -> cb.CatBoost:
     """Patch CatBoost to return only the mean prediction in `predict`
     and the variance in `predict_var` to be consistent with other models.
+    The patch will not apply if the estimator is cloned using `sklearn.base.clone()`
+    and requires re-patching.
 
     Parameters
     ----------
     estimator : cb.CatBoost
         The CatBoost estimator to patch.
 
     Returns
     -------
     cb.CatBoost
         The patched CatBoost estimator.
     """
     original_predict = estimator.predict
 
+    @functools.wraps(original_predict)
     def predict(
         data: Any,
         prediction_type: Literal[
             "Probability", "Class", "RawFormulaVal", "Exponent", "LogProbability"
         ] = "RawFormulaVal",
         ntree_start: int = 0,
         ntree_end: int = 0,
@@ -221,7 +225,44 @@
             raise ValueError(
                 "prediction_type must be one of ['knowledge', 'data', 'total'], "
                 f"but got {prediction_type}"
             )
 
     setattr(estimator, "predict_var", predict_var)
     return estimator
+
+
+TAny = TypeVar("TAny")
+
+
+def patch(estimator: TAny, *, copy: bool = True, recursive: bool = True) -> TAny:
+    """Patch estimator if it is supported. (`patch_ngboost` and `patch_catboost`.)
+    The patch will not apply if the estimator is cloned using `sklearn.base.clone()`
+    and requires re-patching.
+
+    Parameters
+    ----------
+    estimator : TAny
+        The estimator to patch.
+    copy : bool, optional
+        Whether to copy the estimator before patching, by default True
+    recursive : bool, optional
+        Whether to recursively patch the estimator, by default True
+
+    Returns
+    -------
+    TAny
+        The patched estimator.
+    """
+    if copy:
+        estimator = clone(estimator)
+    if importlib.util.find_spec("ngboost") is not None:
+        if isinstance(estimator, NGBoost):
+            return patch_ngboost(estimator)
+    if isinstance(estimator, cb.CatBoost):
+        return patch_catboost(estimator)
+
+    if recursive and hasattr(estimator, "get_params"):
+        for _, value in estimator.get_params(deep=True).items():
+            patch(value, copy=False, recursive=False)
+
+    return estimator
```

### Comparing `boost_loss-0.1.1/src/boost_loss/torch.py` & `boost_loss-0.2.0/src/boost_loss/torch.py`

 * *Files identical despite different names*

### Comparing `boost_loss-0.1.1/PKG-INFO` & `boost_loss-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 626f 6f73  : 2.1.Name: boos
 00000020: 742d 6c6f 7373 0a56 6572 7369 6f6e 3a20  t-loss.Version: 
-00000030: 302e 312e 310a 5375 6d6d 6172 793a 2055  0.1.1.Summary: U
+00000030: 302e 322e 300a 5375 6d6d 6172 793a 2055  0.2.0.Summary: U
 00000040: 7469 6c69 7469 6573 2066 6f72 2065 6173  tilities for eas
 00000050: 7920 7573 6520 6f66 2063 7573 746f 6d20  y use of custom 
 00000060: 6c6f 7373 6573 2069 6e20 4361 7442 6f6f  losses in CatBoo
 00000070: 7374 2c20 4c69 6768 7447 424d 2c20 5847  st, LightGBM, XG
 00000080: 426f 6f73 740a 486f 6d65 2d70 6167 653a  Boost.Home-page:
 00000090: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 000000a0: 636f 6d2f 3334 6a2f 626f 6f73 742d 6c6f  com/34j/boost-lo
@@ -259,76 +259,160 @@
 00001020: 726b 2e0a 0a23 2320 496e 7374 616c 6c61  rk...## Installa
 00001030: 7469 6f6e 0a0a 496e 7374 616c 6c20 7468  tion..Install th
 00001040: 6973 2076 6961 2070 6970 2028 6f72 2079  is via pip (or y
 00001050: 6f75 7220 6661 766f 7572 6974 6520 7061  our favourite pa
 00001060: 636b 6167 6520 6d61 6e61 6765 7229 3a0a  ckage manager):.
 00001070: 0a60 6060 7368 656c 6c0a 7069 7020 696e  .```shell.pip in
 00001080: 7374 616c 6c20 626f 6f73 742d 6c6f 7373  stall boost-loss
-00001090: 0a60 6060 0a0a 2323 2043 6f6e 7472 6962  .```..## Contrib
-000010a0: 7574 6f72 7320 e29c a80a 0a54 6861 6e6b  utors .....Thank
-000010b0: 7320 676f 6573 2074 6f20 7468 6573 6520  s goes to these 
-000010c0: 776f 6e64 6572 6675 6c20 7065 6f70 6c65  wonderful people
-000010d0: 2028 5b65 6d6f 6a69 206b 6579 5d28 6874   ([emoji key](ht
-000010e0: 7470 733a 2f2f 616c 6c63 6f6e 7472 6962  tps://allcontrib
-000010f0: 7574 6f72 732e 6f72 672f 646f 6373 2f65  utors.org/docs/e
-00001100: 6e2f 656d 6f6a 692d 6b65 7929 293a 0a0a  n/emoji-key)):..
-00001110: 3c21 2d2d 2070 7265 7474 6965 722d 6967  <!-- prettier-ig
-00001120: 6e6f 7265 2d73 7461 7274 202d 2d3e 0a3c  nore-start -->.<
-00001130: 212d 2d20 414c 4c2d 434f 4e54 5249 4255  !-- ALL-CONTRIBU
-00001140: 544f 5253 2d4c 4953 543a 5354 4152 5420  TORS-LIST:START 
-00001150: 2d20 446f 206e 6f74 2072 656d 6f76 6520  - Do not remove 
-00001160: 6f72 206d 6f64 6966 7920 7468 6973 2073  or modify this s
-00001170: 6563 7469 6f6e 202d 2d3e 0a3c 212d 2d20  ection -->.<!-- 
-00001180: 7072 6574 7469 6572 2d69 676e 6f72 652d  prettier-ignore-
-00001190: 7374 6172 7420 2d2d 3e0a 3c21 2d2d 206d  start -->.<!-- m
-000011a0: 6172 6b64 6f77 6e6c 696e 742d 6469 7361  arkdownlint-disa
-000011b0: 626c 6520 2d2d 3e0a 3c74 6162 6c65 3e0a  ble -->.<table>.
-000011c0: 2020 3c74 626f 6479 3e0a 2020 2020 3c74    <tbody>.    <t
-000011d0: 723e 0a20 2020 2020 203c 7464 2061 6c69  r>.      <td ali
-000011e0: 676e 3d22 6365 6e74 6572 2220 7661 6c69  gn="center" vali
-000011f0: 676e 3d22 746f 7022 2077 6964 7468 3d22  gn="top" width="
-00001200: 3134 2e32 3825 223e 3c61 2068 7265 663d  14.28%"><a href=
-00001210: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00001220: 636f 6d2f 3334 6a22 3e3c 696d 6720 7372  com/34j"><img sr
-00001230: 633d 2268 7474 7073 3a2f 2f61 7661 7461  c="https://avata
-00001240: 7273 2e67 6974 6875 6275 7365 7263 6f6e  rs.githubusercon
-00001250: 7465 6e74 2e63 6f6d 2f75 2f35 3533 3338  tent.com/u/55338
-00001260: 3231 353f 763d 343f 733d 3830 2220 7769  215?v=4?s=80" wi
-00001270: 6474 683d 2238 3070 783b 2220 616c 743d  dth="80px;" alt=
-00001280: 2233 346a 222f 3e3c 6272 202f 3e3c 7375  "34j"/><br /><su
-00001290: 623e 3c62 3e33 346a 3c2f 623e 3c2f 7375  b><b>34j</b></su
-000012a0: 623e 3c2f 613e 3c62 7220 2f3e 3c61 2068  b></a><br /><a h
-000012b0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-000012c0: 6875 622e 636f 6d2f 3334 6a2f 626f 6f73  hub.com/34j/boos
-000012d0: 742d 6c6f 7373 2f63 6f6d 6d69 7473 3f61  t-loss/commits?a
-000012e0: 7574 686f 723d 3334 6a22 2074 6974 6c65  uthor=34j" title
-000012f0: 3d22 436f 6465 223e f09f 92bb 3c2f 613e  ="Code">....</a>
-00001300: 203c 6120 6872 6566 3d22 2369 6465 6173   <a href="#ideas
-00001310: 2d33 346a 2220 7469 746c 653d 2249 6465  -34j" title="Ide
-00001320: 6173 2c20 506c 616e 6e69 6e67 2c20 2620  as, Planning, & 
-00001330: 4665 6564 6261 636b 223e f09f a494 3c2f  Feedback">....</
-00001340: 613e 203c 6120 6872 6566 3d22 6874 7470  a> <a href="http
-00001350: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f33  s://github.com/3
-00001360: 346a 2f62 6f6f 7374 2d6c 6f73 732f 636f  4j/boost-loss/co
-00001370: 6d6d 6974 733f 6175 7468 6f72 3d33 346a  mmits?author=34j
-00001380: 2220 7469 746c 653d 2244 6f63 756d 656e  " title="Documen
-00001390: 7461 7469 6f6e 223e f09f 9396 3c2f 613e  tation">....</a>
-000013a0: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
-000013b0: 2020 3c2f 7462 6f64 793e 0a3c 2f74 6162    </tbody>.</tab
-000013c0: 6c65 3e0a 0a3c 212d 2d20 6d61 726b 646f  le>..<!-- markdo
-000013d0: 776e 6c69 6e74 2d72 6573 746f 7265 202d  wnlint-restore -
-000013e0: 2d3e 0a3c 212d 2d20 7072 6574 7469 6572  ->.<!-- prettier
-000013f0: 2d69 676e 6f72 652d 656e 6420 2d2d 3e0a  -ignore-end -->.
-00001400: 0a3c 212d 2d20 414c 4c2d 434f 4e54 5249  .<!-- ALL-CONTRI
-00001410: 4255 544f 5253 2d4c 4953 543a 454e 4420  BUTORS-LIST:END 
-00001420: 2d2d 3e0a 3c21 2d2d 2070 7265 7474 6965  -->.<!-- prettie
-00001430: 722d 6967 6e6f 7265 2d65 6e64 202d 2d3e  r-ignore-end -->
-00001440: 0a0a 5468 6973 2070 726f 6a65 6374 2066  ..This project f
-00001450: 6f6c 6c6f 7773 2074 6865 205b 616c 6c2d  ollows the [all-
-00001460: 636f 6e74 7269 6275 746f 7273 5d28 6874  contributors](ht
-00001470: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001480: 2f61 6c6c 2d63 6f6e 7472 6962 7574 6f72  /all-contributor
-00001490: 732f 616c 6c2d 636f 6e74 7269 6275 746f  s/all-contributo
-000014a0: 7273 2920 7370 6563 6966 6963 6174 696f  rs) specificatio
-000014b0: 6e2e 2043 6f6e 7472 6962 7574 696f 6e73  n. Contributions
-000014c0: 206f 6620 616e 7920 6b69 6e64 2077 656c   of any kind wel
-000014d0: 636f 6d65 210a 0a                        come!..
+00001090: 0a60 6060 0a0a 2323 2055 7361 6765 0a0a  .```..## Usage..
+000010a0: 2323 2320 4261 7369 6320 5573 6167 650a  ### Basic Usage.
+000010b0: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
+000010c0: 7420 6e75 6d70 7920 6173 206e 700a 0a66  t numpy as np..f
+000010d0: 726f 6d20 626f 6f73 745f 6c6f 7373 2069  rom boost_loss i
+000010e0: 6d70 6f72 7420 4c6f 7373 4261 7365 0a66  mport LossBase.f
+000010f0: 726f 6d20 6e75 6d70 792e 7479 7069 6e67  rom numpy.typing
+00001100: 2069 6d70 6f72 7420 4e44 4172 7261 790a   import NDArray.
+00001110: 0a0a 636c 6173 7320 4c32 4c6f 7373 284c  ..class L2Loss(L
+00001120: 6f73 7342 6173 6529 3a0a 2020 2020 6465  ossBase):.    de
+00001130: 6620 6c6f 7373 2873 656c 662c 2079 5f74  f loss(self, y_t
+00001140: 7275 653a 204e 4441 7272 6179 2c20 795f  rue: NDArray, y_
+00001150: 7072 6564 3a20 4e44 4172 7261 7929 202d  pred: NDArray) -
+00001160: 3e20 4e44 4172 7261 793a 0a20 2020 2020  > NDArray:.     
+00001170: 2020 2072 6574 7572 6e20 2879 5f74 7275     return (y_tru
+00001180: 6520 2d20 795f 7072 6564 2920 2a2a 2032  e - y_pred) ** 2
+00001190: 202f 2032 0a0a 2020 2020 6465 6620 6772   / 2..    def gr
+000011a0: 6164 2873 656c 662c 2079 5f74 7275 653a  ad(self, y_true:
+000011b0: 204e 4441 7272 6179 2c20 795f 7072 6564   NDArray, y_pred
+000011c0: 3a20 4e44 4172 7261 7929 202d 3e20 4e44  : NDArray) -> ND
+000011d0: 4172 7261 793a 2023 2064 4c2f 6479 5f70  Array: # dL/dy_p
+000011e0: 7265 640a 2020 2020 2020 2020 7265 7475  red.        retu
+000011f0: 726e 202d 2028 795f 7472 7565 202d 2079  rn - (y_true - y
+00001200: 5f70 7265 6429 0a0a 2020 2020 6465 6620  _pred)..    def 
+00001210: 6865 7373 2873 656c 662c 2079 5f74 7275  hess(self, y_tru
+00001220: 653a 204e 4441 7272 6179 2c20 795f 7072  e: NDArray, y_pr
+00001230: 6564 3a20 4e44 4172 7261 7929 202d 3e20  ed: NDArray) -> 
+00001240: 4e44 4172 7261 793a 2023 2064 5e32 4c2f  NDArray: # d^2L/
+00001250: 6479 5f70 7265 645e 320a 2020 2020 2020  dy_pred^2.      
+00001260: 2020 7265 7475 726e 206e 702e 6f6e 6573    return np.ones
+00001270: 5f6c 696b 6528 795f 7472 7565 290a 6060  _like(y_true).``
+00001280: 600a 0a60 6060 7079 7468 6f6e 0a69 6d70  `..```python.imp
+00001290: 6f72 7420 6c69 6768 7467 626d 2061 7320  ort lightgbm as 
+000012a0: 6c67 620a 0a66 726f 6d20 626f 6f73 745f  lgb..from boost_
+000012b0: 6c6f 7373 2069 6d70 6f72 7420 6170 706c  loss import appl
+000012c0: 795f 6375 7374 6f6d 5f6c 6f73 730a 6672  y_custom_loss.fr
+000012d0: 6f6d 2073 6b6c 6561 726e 2e64 6174 6173  om sklearn.datas
+000012e0: 6574 7320 696d 706f 7274 206c 6f61 645f  ets import load_
+000012f0: 626f 7374 6f6e 0a0a 0a58 2c20 7920 3d20  boston...X, y = 
+00001300: 6c6f 6164 5f62 6f73 746f 6e28 7265 7475  load_boston(retu
+00001310: 726e 5f58 5f79 3d54 7275 6529 0a61 7070  rn_X_y=True).app
+00001320: 6c79 5f63 7573 746f 6d5f 6c6f 7373 286c  ly_custom_loss(l
+00001330: 6762 2e4c 4742 4d52 6567 7265 7373 6f72  gb.LGBMRegressor
+00001340: 2829 2c20 4c32 4c6f 7373 2829 292e 6669  (), L2Loss()).fi
+00001350: 7428 582c 2079 290a 6060 600a 0a42 7569  t(X, y).```..Bui
+00001360: 6c74 2d69 6e20 6c6f 7373 6573 2061 7265  lt-in losses are
+00001370: 2061 7661 696c 6162 6c65 2e20 5b5e 626f   available. [^bo
+00001380: 6b62 6f6b 626f 6b5d 0a0a 6060 6070 7974  kbokbok]..```pyt
+00001390: 686f 6e0a 6672 6f6d 2062 6f6f 7374 5f6c  hon.from boost_l
+000013a0: 6f73 732e 7265 6772 6573 7369 6f6e 2069  oss.regression i
+000013b0: 6d70 6f72 7420 4c6f 6743 6f73 684c 6f73  mport LogCoshLos
+000013c0: 730a 6060 600a 0a23 2323 205b 6074 6f72  s.```..### [`tor
+000013d0: 6368 2e61 7574 6f67 7261 6460 5d28 6874  ch.autograd`](ht
+000013e0: 7470 733a 2f2f 7079 746f 7263 682e 6f72  tps://pytorch.or
+000013f0: 672f 646f 6373 2f73 7461 626c 652f 6175  g/docs/stable/au
+00001400: 746f 6772 6164 2e68 746d 6c29 204c 6f73  tograd.html) Los
+00001410: 7320 5b5e 6175 746f 6772 6164 5d0a 0a60  s [^autograd]..`
+00001420: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+00001430: 746f 7263 680a 0a66 726f 6d20 626f 6f73  torch..from boos
+00001440: 745f 6c6f 7373 2e74 6f72 6368 2069 6d70  t_loss.torch imp
+00001450: 6f72 7420 546f 7263 684c 6f73 7342 6173  ort TorchLossBas
+00001460: 650a 0a0a 636c 6173 7320 4c32 4c6f 7373  e...class L2Loss
+00001470: 546f 7263 6828 546f 7263 684c 6f73 7342  Torch(TorchLossB
+00001480: 6173 6529 3a0a 2020 2020 6465 6620 6c6f  ase):.    def lo
+00001490: 7373 5f74 6f72 6368 2873 656c 662c 2079  ss_torch(self, y
+000014a0: 5f74 7275 653a 2074 6f72 6368 2e54 656e  _true: torch.Ten
+000014b0: 736f 722c 2079 5f70 7265 643a 2074 6f72  sor, y_pred: tor
+000014c0: 6368 2e54 656e 736f 7229 202d 3e20 746f  ch.Tensor) -> to
+000014d0: 7263 682e 5465 6e73 6f72 3a0a 2020 2020  rch.Tensor:.    
+000014e0: 2020 2020 7265 7475 726e 2028 795f 7472      return (y_tr
+000014f0: 7565 202d 2079 5f70 7265 6429 202a 2a20  ue - y_pred) ** 
+00001500: 3220 2f20 320a 6060 600a 0a23 2320 436f  2 / 2.```..## Co
+00001510: 6e74 7269 6275 746f 7273 20e2 9ca8 0a0a  ntributors .....
+00001520: 5468 616e 6b73 2067 6f65 7320 746f 2074  Thanks goes to t
+00001530: 6865 7365 2077 6f6e 6465 7266 756c 2070  hese wonderful p
+00001540: 656f 706c 6520 285b 656d 6f6a 6920 6b65  eople ([emoji ke
+00001550: 795d 2868 7474 7073 3a2f 2f61 6c6c 636f  y](https://allco
+00001560: 6e74 7269 6275 746f 7273 2e6f 7267 2f64  ntributors.org/d
+00001570: 6f63 732f 656e 2f65 6d6f 6a69 2d6b 6579  ocs/en/emoji-key
+00001580: 2929 3a0a 0a3c 212d 2d20 7072 6574 7469  )):..<!-- pretti
+00001590: 6572 2d69 676e 6f72 652d 7374 6172 7420  er-ignore-start 
+000015a0: 2d2d 3e0a 3c21 2d2d 2041 4c4c 2d43 4f4e  -->.<!-- ALL-CON
+000015b0: 5452 4942 5554 4f52 532d 4c49 5354 3a53  TRIBUTORS-LIST:S
+000015c0: 5441 5254 202d 2044 6f20 6e6f 7420 7265  TART - Do not re
+000015d0: 6d6f 7665 206f 7220 6d6f 6469 6679 2074  move or modify t
+000015e0: 6869 7320 7365 6374 696f 6e20 2d2d 3e0a  his section -->.
+000015f0: 3c21 2d2d 2070 7265 7474 6965 722d 6967  <!-- prettier-ig
+00001600: 6e6f 7265 2d73 7461 7274 202d 2d3e 0a3c  nore-start -->.<
+00001610: 212d 2d20 6d61 726b 646f 776e 6c69 6e74  !-- markdownlint
+00001620: 2d64 6973 6162 6c65 202d 2d3e 0a3c 7461  -disable -->.<ta
+00001630: 626c 653e 0a20 203c 7462 6f64 793e 0a20  ble>.  <tbody>. 
+00001640: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
+00001650: 6420 616c 6967 6e3d 2263 656e 7465 7222  d align="center"
+00001660: 2076 616c 6967 6e3d 2274 6f70 2220 7769   valign="top" wi
+00001670: 6474 683d 2231 342e 3238 2522 3e3c 6120  dth="14.28%"><a 
+00001680: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00001690: 7468 7562 2e63 6f6d 2f33 346a 223e 3c69  thub.com/34j"><i
+000016a0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000016b0: 6176 6174 6172 732e 6769 7468 7562 7573  avatars.githubus
+000016c0: 6572 636f 6e74 656e 742e 636f 6d2f 752f  ercontent.com/u/
+000016d0: 3535 3333 3832 3135 3f76 3d34 3f73 3d38  55338215?v=4?s=8
+000016e0: 3022 2077 6964 7468 3d22 3830 7078 3b22  0" width="80px;"
+000016f0: 2061 6c74 3d22 3334 6a22 2f3e 3c62 7220   alt="34j"/><br 
+00001700: 2f3e 3c73 7562 3e3c 623e 3334 6a3c 2f62  /><sub><b>34j</b
+00001710: 3e3c 2f73 7562 3e3c 2f61 3e3c 6272 202f  ></sub></a><br /
+00001720: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
+00001730: 2f2f 6769 7468 7562 2e63 6f6d 2f33 346a  //github.com/34j
+00001740: 2f62 6f6f 7374 2d6c 6f73 732f 636f 6d6d  /boost-loss/comm
+00001750: 6974 733f 6175 7468 6f72 3d33 346a 2220  its?author=34j" 
+00001760: 7469 746c 653d 2243 6f64 6522 3ef0 9f92  title="Code">...
+00001770: bb3c 2f61 3e20 3c61 2068 7265 663d 2223  .</a> <a href="#
+00001780: 6964 6561 732d 3334 6a22 2074 6974 6c65  ideas-34j" title
+00001790: 3d22 4964 6561 732c 2050 6c61 6e6e 696e  ="Ideas, Plannin
+000017a0: 672c 2026 2046 6565 6462 6163 6b22 3ef0  g, & Feedback">.
+000017b0: 9fa4 943c 2f61 3e20 3c61 2068 7265 663d  ...</a> <a href=
+000017c0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000017d0: 636f 6d2f 3334 6a2f 626f 6f73 742d 6c6f  com/34j/boost-lo
+000017e0: 7373 2f63 6f6d 6d69 7473 3f61 7574 686f  ss/commits?autho
+000017f0: 723d 3334 6a22 2074 6974 6c65 3d22 446f  r=34j" title="Do
+00001800: 6375 6d65 6e74 6174 696f 6e22 3ef0 9f93  cumentation">...
+00001810: 963c 2f61 3e3c 2f74 643e 0a20 2020 203c  .</a></td>.    <
+00001820: 2f74 723e 0a20 203c 2f74 626f 6479 3e0a  /tr>.  </tbody>.
+00001830: 3c2f 7461 626c 653e 0a0a 3c21 2d2d 206d  </table>..<!-- m
+00001840: 6172 6b64 6f77 6e6c 696e 742d 7265 7374  arkdownlint-rest
+00001850: 6f72 6520 2d2d 3e0a 3c21 2d2d 2070 7265  ore -->.<!-- pre
+00001860: 7474 6965 722d 6967 6e6f 7265 2d65 6e64  ttier-ignore-end
+00001870: 202d 2d3e 0a0a 3c21 2d2d 2041 4c4c 2d43   -->..<!-- ALL-C
+00001880: 4f4e 5452 4942 5554 4f52 532d 4c49 5354  ONTRIBUTORS-LIST
+00001890: 3a45 4e44 202d 2d3e 0a3c 212d 2d20 7072  :END -->.<!-- pr
+000018a0: 6574 7469 6572 2d69 676e 6f72 652d 656e  ettier-ignore-en
+000018b0: 6420 2d2d 3e0a 0a54 6869 7320 7072 6f6a  d -->..This proj
+000018c0: 6563 7420 666f 6c6c 6f77 7320 7468 6520  ect follows the 
+000018d0: 5b61 6c6c 2d63 6f6e 7472 6962 7574 6f72  [all-contributor
+000018e0: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+000018f0: 622e 636f 6d2f 616c 6c2d 636f 6e74 7269  b.com/all-contri
+00001900: 6275 746f 7273 2f61 6c6c 2d63 6f6e 7472  butors/all-contr
+00001910: 6962 7574 6f72 7329 2073 7065 6369 6669  ibutors) specifi
+00001920: 6361 7469 6f6e 2e20 436f 6e74 7269 6275  cation. Contribu
+00001930: 7469 6f6e 7320 6f66 2061 6e79 206b 696e  tions of any kin
+00001940: 6420 7765 6c63 6f6d 6521 0a0a 5b5e 626f  d welcome!..[^bo
+00001950: 6b62 6f6b 626f 6b5d 3a20 496e 7370 6972  kbokbok]: Inspir
+00001960: 6564 2062 7920 5b6f 7263 6861 7264 6269  ed by [orchardbi
+00001970: 7264 732f 626f 6b62 6f6b 626f 6b5d 2868  rds/bokbokbok](h
+00001980: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001990: 6d2f 6f72 6368 6172 6462 6972 6473 2f62  m/orchardbirds/b
+000019a0: 6f6b 626f 6b62 6f6b 290a 5b5e 6175 746f  okbokbok).[^auto
+000019b0: 6772 6164 5d3a 2049 6e73 7069 7265 6420  grad]: Inspired 
+000019c0: 6279 205b 546f 6d65 7252 6f6e 656e 3334  by [TomerRonen34
+000019d0: 2f74 7265 6562 6f6f 7374 5f61 7574 6f67  /treeboost_autog
+000019e0: 7261 645d 2868 7474 7073 3a2f 2f67 6974  rad](https://git
+000019f0: 6875 622e 636f 6d2f 546f 6d65 7252 6f6e  hub.com/TomerRon
+00001a00: 656e 3334 2f74 7265 6562 6f6f 7374 5f61  en34/treeboost_a
+00001a10: 7574 6f67 7261 6429 0a0a                 utograd)..
```

