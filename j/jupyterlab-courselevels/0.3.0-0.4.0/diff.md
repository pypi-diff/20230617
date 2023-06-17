# Comparing `tmp/jupyterlab_courselevels-0.3.0.tar.gz` & `tmp/jupyterlab_courselevels-0.4.0.tar.gz`

## Comparing `jupyterlab_courselevels-0.3.0.tar` & `jupyterlab_courselevels-0.4.0.tar`

### file list

```diff
@@ -1,132 +1,135 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/.eslintrc.js
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/.prettierignore
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/.stylelintrc
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/RELEASE.md
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/install.json
--rw-r--r--   0        0        0   164800 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/package-lock.json
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/package.json
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/package.json.version
--rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/release-to-pypi.sh
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/tsconfig.json
--rw-r--r--   0        0        0   209231 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/yarn.lock
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/examples/admonitions.ipynb
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/examples/courselevels.ipynb
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/_version.py
--rw-r--r--   0        0        0    21249 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/build_log.json
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/package.json
--rw-r--r--   0        0        0    15705 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.03e2a055a4787bf8010c.js
--rw-r--r--   0        0        0    13712 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.03e2a055a4787bf8010c.js.map
--rw-r--r--   0        0        0    15685 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.231e9c11adf913854203.js
--rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.231e9c11adf913854203.js.map
--rw-r--r--   0        0        0    15239 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.33ce47933f8c6b71922c.js
--rw-r--r--   0        0        0    13170 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.33ce47933f8c6b71922c.js.map
--rw-r--r--   0        0        0    15757 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.3968f999bb84e356595c.js
--rw-r--r--   0        0        0    13779 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.3968f999bb84e356595c.js.map
--rw-r--r--   0        0        0    15256 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.3a7abe98f591ab39344b.js
--rw-r--r--   0        0        0    13187 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.3a7abe98f591ab39344b.js.map
--rw-r--r--   0        0        0    15241 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.3a86705e19eabe4150fc.js
--rw-r--r--   0        0        0    13177 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.3a86705e19eabe4150fc.js.map
--rw-r--r--   0        0        0    15257 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.4dea3ad073c72cc3a779.js
--rw-r--r--   0        0        0    13188 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.4dea3ad073c72cc3a779.js.map
--rw-r--r--   0        0        0    15722 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.4e707f1bcb403e057938.js
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.4e707f1bcb403e057938.js.map
--rw-r--r--   0        0        0    15655 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.565a3d697199e369d999.js
--rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.565a3d697199e369d999.js.map
--rw-r--r--   0        0        0    15690 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.5a6e21d4692790444867.js
--rw-r--r--   0        0        0    13700 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.5a6e21d4692790444867.js.map
--rw-r--r--   0        0        0    15237 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.623d3c3da0698cae21a4.js
--rw-r--r--   0        0        0    13168 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.623d3c3da0698cae21a4.js.map
--rw-r--r--   0        0        0    15722 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.62bf13948d92f937dae0.js
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.62bf13948d92f937dae0.js.map
--rw-r--r--   0        0        0    14987 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.6c06e04cb286dac2dd61.js
--rw-r--r--   0        0        0    12866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.6c06e04cb286dac2dd61.js.map
--rw-r--r--   0        0        0    15691 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.7b3aa40ec4d42ec3984b.js
--rw-r--r--   0        0        0    13701 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.7b3aa40ec4d42ec3984b.js.map
--rw-r--r--   0        0        0    15255 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.7d9effddd678fd8ca6fb.js
--rw-r--r--   0        0        0    13186 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.7d9effddd678fd8ca6fb.js.map
--rw-r--r--   0        0        0    15685 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.83fbc9ad7312d3a7a1aa.js
--rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.83fbc9ad7312d3a7a1aa.js.map
--rw-r--r--   0        0        0    15685 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.8a89d001c8b189978b91.js
--rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.8a89d001c8b189978b91.js.map
--rw-r--r--   0        0        0    15245 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.93c49e4bf06d889f1516.js
--rw-r--r--   0        0        0    13186 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.93c49e4bf06d889f1516.js.map
--rw-r--r--   0        0        0    14989 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.9bca3068ff07dda3c398.js
--rw-r--r--   0        0        0    12869 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.9bca3068ff07dda3c398.js.map
--rw-r--r--   0        0        0    15687 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.9e7b66e25b9b9ba02fcb.js
--rw-r--r--   0        0        0    13697 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.9e7b66e25b9b9ba02fcb.js.map
--rw-r--r--   0        0        0    15722 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.a53fe4d36cd49e8ea6f0.js
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.a53fe4d36cd49e8ea6f0.js.map
--rw-r--r--   0        0        0    15653 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.b30fe0144d8412985738.js
--rw-r--r--   0        0        0    13657 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.b30fe0144d8412985738.js.map
--rw-r--r--   0        0        0    15240 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.b387682af14440564db4.js
--rw-r--r--   0        0        0    13176 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.b387682af14440564db4.js.map
--rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.ba8f368cf64b2e4275e8.js
--rw-r--r--   0        0        0    13158 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.ba8f368cf64b2e4275e8.js.map
--rw-r--r--   0        0        0    14986 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.bc24297beb7490cbabef.js
--rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.bc24297beb7490cbabef.js.map
--rw-r--r--   0        0        0    15238 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.be1d1e701a460a83ce36.js
--rw-r--r--   0        0        0    13169 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.be1d1e701a460a83ce36.js.map
--rw-r--r--   0        0        0    15722 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.c5998f6761fd0152962d.js
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.c5998f6761fd0152962d.js.map
--rw-r--r--   0        0        0    15722 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.d6331f143a8f7db234bf.js
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.d6331f143a8f7db234bf.js.map
--rw-r--r--   0        0        0    15200 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.e6f6fd3185b8b9840a8d.js
--rw-r--r--   0        0        0    13135 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.e6f6fd3185b8b9840a8d.js.map
--rw-r--r--   0        0        0    15682 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.ec3e5d243a949fa3e05b.js
--rw-r--r--   0        0        0    13680 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.ec3e5d243a949fa3e05b.js.map
--rw-r--r--   0        0        0    15247 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.f545c5b5e389bfd44f1a.js
--rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.f545c5b5e389bfd44f1a.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.0ed75c9504acfd0f263b.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.10d8182bf5137b4db1b9.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.13d10706596b450a5d66.js.map
--rw-r--r--   0        0        0    29980 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.15671b6ebd987ce9d8cc.js
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.15671b6ebd987ce9d8cc.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.222d921eb7b88b9fa537.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.27da1884e13e86365b34.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.3c9f80103831f1e43f7e.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.3fe296612009e197627d.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.44824a82cec1d4b63cef.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.610617f3abf4dc2cc544.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.61acc15842d07d6a4a61.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.6e399c92cdd14946c60f.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.720dd603f494aa76ca77.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.736d7d395d3a21838c2a.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.77991feae957710d4356.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.77b1947e54dfef3bd08a.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.78fff1ff77e72cab0144.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.7e558d44cf36505aa904.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.8e77dbc23851b6aafc0b.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.9c5463dce5da3f9b0fa1.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.abff7f1d5ea0b07a80e8.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.bf0e3e5d4f3f0faba7a9.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.cf937e63835a6ba72c23.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.d26f3ec81fd823809a9f.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.d993f7c3729d0f5d56f6.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.e62263ec2a04b73ddfc8.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.e876e101a44cc0d19e2d.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.ee3287a799c2f4d087d2.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.efdfa5dad67ef6404a01.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.f0bfee77f9abffdabc31.js.map
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.f9f602a9c411d8725ac4.js.map
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/style.js
--rw-r--r--   0        0        0    21447 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/style_index_js.84816b6f9c775026e9fc.js
--rw-r--r--   0        0        0    17555 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/style_index_js.84816b6f9c775026e9fc.js.map
--rw-r--r--   0        0        0    25905 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/vendors-node_modules_jupyterlab-celltagsclasses_lib_index_js.ddf2f0c11b072e5871d4.js
--rw-r--r--   0        0        0    24137 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/vendors-node_modules_jupyterlab-celltagsclasses_lib_index_js.ddf2f0c11b072e5871d4.js.map
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/src/admonitions.ts
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/src/index.js
--rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/src/index.ts
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/style/index.js
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/LICENSE
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/README.md
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/.eslintrc.js
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/.prettierignore
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/.stylelintrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/RELEASE.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/install.json
+-rw-r--r--   0        0        0   164800 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/package-lock.json
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/package.json
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/package.json.version
+-rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/release-to-pypi.sh
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/tsconfig.json
+-rw-r--r--   0        0        0   209231 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/yarn.lock
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/examples/admonitions.ipynb
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/examples/courselevels.ipynb
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/_version.py
+-rw-r--r--   0        0        0    21249 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/build_log.json
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/install.json
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/package.json
+-rw-r--r--   0        0        0    15705 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.03e2a055a4787bf8010c.js
+-rw-r--r--   0        0        0    13712 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.03e2a055a4787bf8010c.js.map
+-rw-r--r--   0        0        0    15685 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.231e9c11adf913854203.js
+-rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.231e9c11adf913854203.js.map
+-rw-r--r--   0        0        0    15239 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.33ce47933f8c6b71922c.js
+-rw-r--r--   0        0        0    13170 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.33ce47933f8c6b71922c.js.map
+-rw-r--r--   0        0        0    15757 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.3968f999bb84e356595c.js
+-rw-r--r--   0        0        0    13779 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.3968f999bb84e356595c.js.map
+-rw-r--r--   0        0        0    15256 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.3a7abe98f591ab39344b.js
+-rw-r--r--   0        0        0    13187 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.3a7abe98f591ab39344b.js.map
+-rw-r--r--   0        0        0    15241 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.3a86705e19eabe4150fc.js
+-rw-r--r--   0        0        0    13177 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.3a86705e19eabe4150fc.js.map
+-rw-r--r--   0        0        0    15257 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.4dea3ad073c72cc3a779.js
+-rw-r--r--   0        0        0    13188 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.4dea3ad073c72cc3a779.js.map
+-rw-r--r--   0        0        0    15722 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.4e707f1bcb403e057938.js
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.4e707f1bcb403e057938.js.map
+-rw-r--r--   0        0        0    15655 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.565a3d697199e369d999.js
+-rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.565a3d697199e369d999.js.map
+-rw-r--r--   0        0        0    15690 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.5a6e21d4692790444867.js
+-rw-r--r--   0        0        0    13700 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.5a6e21d4692790444867.js.map
+-rw-r--r--   0        0        0    15237 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.623d3c3da0698cae21a4.js
+-rw-r--r--   0        0        0    13168 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.623d3c3da0698cae21a4.js.map
+-rw-r--r--   0        0        0    15722 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.62bf13948d92f937dae0.js
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.62bf13948d92f937dae0.js.map
+-rw-r--r--   0        0        0    14987 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.6c06e04cb286dac2dd61.js
+-rw-r--r--   0        0        0    12866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.6c06e04cb286dac2dd61.js.map
+-rw-r--r--   0        0        0    15691 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.7b3aa40ec4d42ec3984b.js
+-rw-r--r--   0        0        0    13701 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.7b3aa40ec4d42ec3984b.js.map
+-rw-r--r--   0        0        0    15255 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.7d9effddd678fd8ca6fb.js
+-rw-r--r--   0        0        0    13186 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.7d9effddd678fd8ca6fb.js.map
+-rw-r--r--   0        0        0    15685 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.83fbc9ad7312d3a7a1aa.js
+-rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.83fbc9ad7312d3a7a1aa.js.map
+-rw-r--r--   0        0        0    15685 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.8a89d001c8b189978b91.js
+-rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.8a89d001c8b189978b91.js.map
+-rw-r--r--   0        0        0    15245 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.93c49e4bf06d889f1516.js
+-rw-r--r--   0        0        0    13186 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.93c49e4bf06d889f1516.js.map
+-rw-r--r--   0        0        0    14989 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.9bca3068ff07dda3c398.js
+-rw-r--r--   0        0        0    12869 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.9bca3068ff07dda3c398.js.map
+-rw-r--r--   0        0        0    15687 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.9e7b66e25b9b9ba02fcb.js
+-rw-r--r--   0        0        0    13697 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.9e7b66e25b9b9ba02fcb.js.map
+-rw-r--r--   0        0        0    15722 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.a53fe4d36cd49e8ea6f0.js
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.a53fe4d36cd49e8ea6f0.js.map
+-rw-r--r--   0        0        0    15653 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.b30fe0144d8412985738.js
+-rw-r--r--   0        0        0    13657 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.b30fe0144d8412985738.js.map
+-rw-r--r--   0        0        0    15240 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.b387682af14440564db4.js
+-rw-r--r--   0        0        0    13176 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.b387682af14440564db4.js.map
+-rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.ba8f368cf64b2e4275e8.js
+-rw-r--r--   0        0        0    13158 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.ba8f368cf64b2e4275e8.js.map
+-rw-r--r--   0        0        0    14986 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.bc24297beb7490cbabef.js
+-rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.bc24297beb7490cbabef.js.map
+-rw-r--r--   0        0        0    15238 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.be1d1e701a460a83ce36.js
+-rw-r--r--   0        0        0    13169 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.be1d1e701a460a83ce36.js.map
+-rw-r--r--   0        0        0    15722 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.c5998f6761fd0152962d.js
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.c5998f6761fd0152962d.js.map
+-rw-r--r--   0        0        0    15722 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.d6331f143a8f7db234bf.js
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.d6331f143a8f7db234bf.js.map
+-rw-r--r--   0        0        0    15200 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.e6f6fd3185b8b9840a8d.js
+-rw-r--r--   0        0        0    13135 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.e6f6fd3185b8b9840a8d.js.map
+-rw-r--r--   0        0        0    15682 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.ec3e5d243a949fa3e05b.js
+-rw-r--r--   0        0        0    13680 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.ec3e5d243a949fa3e05b.js.map
+-rw-r--r--   0        0        0    15247 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.f545c5b5e389bfd44f1a.js
+-rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.f545c5b5e389bfd44f1a.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.0ed75c9504acfd0f263b.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.10d8182bf5137b4db1b9.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.13d10706596b450a5d66.js.map
+-rw-r--r--   0        0        0    29980 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.15671b6ebd987ce9d8cc.js
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.15671b6ebd987ce9d8cc.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.222d921eb7b88b9fa537.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.27da1884e13e86365b34.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.3c9f80103831f1e43f7e.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.3fe296612009e197627d.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.44824a82cec1d4b63cef.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.610617f3abf4dc2cc544.js.map
+-rw-r--r--   0        0        0    29980 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.616cf8d6bfdd2e339431.js
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.616cf8d6bfdd2e339431.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.61acc15842d07d6a4a61.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.6e399c92cdd14946c60f.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.720dd603f494aa76ca77.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.736d7d395d3a21838c2a.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.77991feae957710d4356.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.77b1947e54dfef3bd08a.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.78fff1ff77e72cab0144.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.7e558d44cf36505aa904.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.8e77dbc23851b6aafc0b.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.9c5463dce5da3f9b0fa1.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.abff7f1d5ea0b07a80e8.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.bf0e3e5d4f3f0faba7a9.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.cf937e63835a6ba72c23.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.d26f3ec81fd823809a9f.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.d993f7c3729d0f5d56f6.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.e62263ec2a04b73ddfc8.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.e876e101a44cc0d19e2d.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.ee3287a799c2f4d087d2.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.efdfa5dad67ef6404a01.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.f0bfee77f9abffdabc31.js.map
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.f9f602a9c411d8725ac4.js.map
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/style.js
+-rw-r--r--   0        0        0    21447 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/style_index_js.84816b6f9c775026e9fc.js
+-rw-r--r--   0        0        0    17555 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/style_index_js.84816b6f9c775026e9fc.js.map
+-rw-r--r--   0        0        0    25905 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/vendors-node_modules_jupyterlab-celltagsclasses_lib_index_js.ddf2f0c11b072e5871d4.js
+-rw-r--r--   0        0        0    24137 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/vendors-node_modules_jupyterlab-celltagsclasses_lib_index_js.ddf2f0c11b072e5871d4.js.map
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/src/admonitions.ts
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/src/index.js
+-rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/src/index.ts
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/style/index.js
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/README.md
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 jupyterlab_courselevels-0.4.0/PKG-INFO
```

### Comparing `jupyterlab_courselevels-0.3.0/.eslintrc.js` & `jupyterlab_courselevels-0.4.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/RELEASE.md` & `jupyterlab_courselevels-0.4.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/package-lock.json` & `jupyterlab_courselevels-0.4.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/package.json` & `jupyterlab_courselevels-0.4.0/package.json.version`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.2.0'"}*

```diff
@@ -91,9 +91,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "0.2.0"
 }
```

### Comparing `jupyterlab_courselevels-0.3.0/package.json.version` & `jupyterlab_courselevels-0.4.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9669047619047619%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/notebook': '^4.0.0'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0'}",*

 * * "'version'": "'0.4.0'"}*

```diff
@@ -3,23 +3,23 @@
         "email": "thierry.parmentelat@inria.fr",
         "name": "Thierry Parmentelat"
     },
     "bugs": {
         "url": "https://github.com/parmentelat/jupyterlab-courselevels/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^4.0.0-rc.1",
-        "@jupyterlab/apputils": "^4.0.0-rc.1",
-        "@jupyterlab/notebook": "^4.0.0-rc.1",
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/notebook": "^4.0.0",
         "@lumino/widgets": "^2.0.1",
         "jupyterlab-celltagsclasses": "^0.3.0"
     },
     "description": "Jlab extension for showing course levels and structure",
     "devDependencies": {
-        "@jupyterlab/builder": "^4.0.0-rc.1",
+        "@jupyterlab/builder": "^4.0.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@typescript-eslint/eslint-plugin": "^5.55.0",
         "@typescript-eslint/parser": "^5.55.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
         "eslint-config-prettier": "^8.7.0",
@@ -91,9 +91,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.4.0"
 }
```

### Comparing `jupyterlab_courselevels-0.3.0/release-to-pypi.sh` & `jupyterlab_courselevels-0.4.0/release-to-pypi.sh`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/tsconfig.json` & `jupyterlab_courselevels-0.4.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/yarn.lock` & `jupyterlab_courselevels-0.4.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/examples/admonitions.ipynb` & `jupyterlab_courselevels-0.4.0/examples/admonitions.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/examples/courselevels.ipynb` & `jupyterlab_courselevels-0.4.0/examples/courselevels.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/build_log.json` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/package.json` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.03e2a055a4787bf8010c.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.03e2a055a4787bf8010c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.03e2a055a4787bf8010c.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.03e2a055a4787bf8010c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.231e9c11adf913854203.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.231e9c11adf913854203.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.231e9c11adf913854203.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.231e9c11adf913854203.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.33ce47933f8c6b71922c.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.33ce47933f8c6b71922c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.33ce47933f8c6b71922c.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.33ce47933f8c6b71922c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.3968f999bb84e356595c.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.3968f999bb84e356595c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.3968f999bb84e356595c.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.3968f999bb84e356595c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.3a7abe98f591ab39344b.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.3a7abe98f591ab39344b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.3a7abe98f591ab39344b.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.3a7abe98f591ab39344b.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.3a86705e19eabe4150fc.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.3a86705e19eabe4150fc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.3a86705e19eabe4150fc.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.3a86705e19eabe4150fc.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.4dea3ad073c72cc3a779.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.4dea3ad073c72cc3a779.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.4dea3ad073c72cc3a779.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.4dea3ad073c72cc3a779.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.4e707f1bcb403e057938.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.4e707f1bcb403e057938.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.4e707f1bcb403e057938.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.4e707f1bcb403e057938.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.565a3d697199e369d999.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.565a3d697199e369d999.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.565a3d697199e369d999.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.565a3d697199e369d999.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.5a6e21d4692790444867.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.5a6e21d4692790444867.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.5a6e21d4692790444867.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.5a6e21d4692790444867.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.623d3c3da0698cae21a4.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.623d3c3da0698cae21a4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.623d3c3da0698cae21a4.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.623d3c3da0698cae21a4.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.62bf13948d92f937dae0.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.62bf13948d92f937dae0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.62bf13948d92f937dae0.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.62bf13948d92f937dae0.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.6c06e04cb286dac2dd61.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.6c06e04cb286dac2dd61.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.6c06e04cb286dac2dd61.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.6c06e04cb286dac2dd61.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.7b3aa40ec4d42ec3984b.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.7b3aa40ec4d42ec3984b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.7b3aa40ec4d42ec3984b.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.7b3aa40ec4d42ec3984b.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.7d9effddd678fd8ca6fb.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.7d9effddd678fd8ca6fb.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.7d9effddd678fd8ca6fb.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.7d9effddd678fd8ca6fb.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.83fbc9ad7312d3a7a1aa.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.83fbc9ad7312d3a7a1aa.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.83fbc9ad7312d3a7a1aa.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.83fbc9ad7312d3a7a1aa.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.8a89d001c8b189978b91.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.8a89d001c8b189978b91.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.8a89d001c8b189978b91.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.8a89d001c8b189978b91.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.93c49e4bf06d889f1516.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.93c49e4bf06d889f1516.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.93c49e4bf06d889f1516.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.93c49e4bf06d889f1516.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.9bca3068ff07dda3c398.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.9bca3068ff07dda3c398.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.9bca3068ff07dda3c398.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.9bca3068ff07dda3c398.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.9e7b66e25b9b9ba02fcb.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.9e7b66e25b9b9ba02fcb.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.9e7b66e25b9b9ba02fcb.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.9e7b66e25b9b9ba02fcb.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.a53fe4d36cd49e8ea6f0.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.a53fe4d36cd49e8ea6f0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.a53fe4d36cd49e8ea6f0.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.a53fe4d36cd49e8ea6f0.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.b30fe0144d8412985738.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.b30fe0144d8412985738.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.b30fe0144d8412985738.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.b30fe0144d8412985738.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.b387682af14440564db4.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.b387682af14440564db4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.b387682af14440564db4.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.b387682af14440564db4.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.ba8f368cf64b2e4275e8.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.ba8f368cf64b2e4275e8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.ba8f368cf64b2e4275e8.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.ba8f368cf64b2e4275e8.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.bc24297beb7490cbabef.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.bc24297beb7490cbabef.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.bc24297beb7490cbabef.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.bc24297beb7490cbabef.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.be1d1e701a460a83ce36.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.be1d1e701a460a83ce36.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.be1d1e701a460a83ce36.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.be1d1e701a460a83ce36.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.c5998f6761fd0152962d.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.c5998f6761fd0152962d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.c5998f6761fd0152962d.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.c5998f6761fd0152962d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.d6331f143a8f7db234bf.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.d6331f143a8f7db234bf.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.d6331f143a8f7db234bf.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.d6331f143a8f7db234bf.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.e6f6fd3185b8b9840a8d.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.e6f6fd3185b8b9840a8d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.e6f6fd3185b8b9840a8d.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.e6f6fd3185b8b9840a8d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.ec3e5d243a949fa3e05b.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.ec3e5d243a949fa3e05b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.ec3e5d243a949fa3e05b.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.ec3e5d243a949fa3e05b.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.f545c5b5e389bfd44f1a.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.f545c5b5e389bfd44f1a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/lib_index_js.f545c5b5e389bfd44f1a.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/lib_index_js.f545c5b5e389bfd44f1a.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.0ed75c9504acfd0f263b.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.0ed75c9504acfd0f263b.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.10d8182bf5137b4db1b9.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.10d8182bf5137b4db1b9.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.13d10706596b450a5d66.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.13d10706596b450a5d66.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.15671b6ebd987ce9d8cc.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.15671b6ebd987ce9d8cc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.15671b6ebd987ce9d8cc.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.15671b6ebd987ce9d8cc.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.222d921eb7b88b9fa537.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.222d921eb7b88b9fa537.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.27da1884e13e86365b34.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.27da1884e13e86365b34.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.3c9f80103831f1e43f7e.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.3c9f80103831f1e43f7e.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.3fe296612009e197627d.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.3fe296612009e197627d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.44824a82cec1d4b63cef.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.44824a82cec1d4b63cef.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.610617f3abf4dc2cc544.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.610617f3abf4dc2cc544.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.61acc15842d07d6a4a61.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.61acc15842d07d6a4a61.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.6e399c92cdd14946c60f.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.6e399c92cdd14946c60f.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.720dd603f494aa76ca77.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.720dd603f494aa76ca77.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.736d7d395d3a21838c2a.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.736d7d395d3a21838c2a.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.77991feae957710d4356.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.77991feae957710d4356.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.77b1947e54dfef3bd08a.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.77b1947e54dfef3bd08a.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.78fff1ff77e72cab0144.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.78fff1ff77e72cab0144.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.7e558d44cf36505aa904.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.7e558d44cf36505aa904.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.8e77dbc23851b6aafc0b.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.8e77dbc23851b6aafc0b.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.9c5463dce5da3f9b0fa1.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.9c5463dce5da3f9b0fa1.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.abff7f1d5ea0b07a80e8.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.abff7f1d5ea0b07a80e8.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.bf0e3e5d4f3f0faba7a9.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.bf0e3e5d4f3f0faba7a9.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.cf937e63835a6ba72c23.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.cf937e63835a6ba72c23.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.d26f3ec81fd823809a9f.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.d26f3ec81fd823809a9f.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.d993f7c3729d0f5d56f6.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.d993f7c3729d0f5d56f6.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.e62263ec2a04b73ddfc8.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.e62263ec2a04b73ddfc8.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.e876e101a44cc0d19e2d.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.e876e101a44cc0d19e2d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.ee3287a799c2f4d087d2.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.ee3287a799c2f4d087d2.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.efdfa5dad67ef6404a01.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.efdfa5dad67ef6404a01.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.f0bfee77f9abffdabc31.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.f0bfee77f9abffdabc31.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/remoteEntry.f9f602a9c411d8725ac4.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/remoteEntry.f9f602a9c411d8725ac4.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/style_index_js.84816b6f9c775026e9fc.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/style_index_js.84816b6f9c775026e9fc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/style_index_js.84816b6f9c775026e9fc.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/style_index_js.84816b6f9c775026e9fc.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/vendors-node_modules_jupyterlab-celltagsclasses_lib_index_js.ddf2f0c11b072e5871d4.js` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/vendors-node_modules_jupyterlab-celltagsclasses_lib_index_js.ddf2f0c11b072e5871d4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/jupyterlab_courselevels/labextension/static/vendors-node_modules_jupyterlab-celltagsclasses_lib_index_js.ddf2f0c11b072e5871d4.js.map` & `jupyterlab_courselevels-0.4.0/jupyterlab_courselevels/labextension/static/vendors-node_modules_jupyterlab-celltagsclasses_lib_index_js.ddf2f0c11b072e5871d4.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/src/admonitions.ts` & `jupyterlab_courselevels-0.4.0/src/admonitions.ts`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
   let cell_source = model.sharedModel.getSource()
   // remove trailing newlines
   while (cell_source.endsWith('\n')) {
     cell_source = cell_source.slice(0, -1)
   }
   // does it start with an admonition?
-  const turning_off = (cell_source.startsWith(':::') || cell_source.startsWith('```'))
+  const turning_off = (cell_source.startsWith(':::') || cell_source.startsWith('````'))
 
   console.log('turning_off', turning_off)
 
   // a function that removes any initial white line, and any trailing white line
   // a line is considered white if it is empty or only contains whitespace
   const tidy = (dirty: string): string => {
     const lines = dirty.split('\n')
@@ -36,18 +36,19 @@
   }
 
   if (turning_off) {
     model.sharedModel.setSource(
       tidy(
         cell_source
           .replace(RegExp(`^::: *{[a-zA-Z]+}`), '')
-          .replace(RegExp(`^\`\`\` *{[a-zA-Z]+}`), '')
-          .replace(RegExp('```.*$'), '')
-          .replace(RegExp(':::.*$'), '')
+          .replace(RegExp(`^\`\`\`\` *{[a-zA-Z]+}`), '')
+          // .replace(RegExp('````.*$'), '')
+          // .replace(RegExp('```.*$'), '')
+          // .replace(RegExp(':::.*$'), '')
       )
     )
   } else {
     model.sharedModel.setSource(
-      `\`\`\`{${admonition}}\n${tidy(cell_source)}\n\`\`\``
+      `\`\`\`\`{${admonition}}\n${tidy(cell_source)}\n\`\`\`\``
     )
   }
 }
```

### Comparing `jupyterlab_courselevels-0.3.0/src/index.js` & `jupyterlab_courselevels-0.4.0/src/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/src/index.ts` & `jupyterlab_courselevels-0.4.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/style/base.css` & `jupyterlab_courselevels-0.4.0/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/.gitignore` & `jupyterlab_courselevels-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/LICENSE` & `jupyterlab_courselevels-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/README.md` & `jupyterlab_courselevels-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_courselevels-0.3.0/pyproject.toml` & `jupyterlab_courselevels-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling>=1.5.0", "jupyterlab>=4.0.0rc0,<5", "hatch-nodejs-version"]
+requires = ["hatchling>=1.5.0", "jupyterlab>=4.0.0,<5", "hatch-nodejs-version"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyterlab_courselevels"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
@@ -63,15 +63,15 @@
 build_dir = "jupyterlab_courselevels/labextension"
 
 [tool.jupyter-releaser.options]
 version_cmd = "hatch version"
 
 [tool.jupyter-releaser.hooks]
 before-build-npm = [
-    "python -m pip install 'jupyterlab>=4.0.0b0,<5'",
+    "python -m pip install 'jupyterlab>=4.0.0,<5'",
     "jlpm",
     "jlpm build:prod"
 ]
 before-build-python = ["jlpm clean:all"]
 
 [tool.check-wheel-contents]
 ignore = ["W002"]
```

### Comparing `jupyterlab_courselevels-0.3.0/PKG-INFO` & `jupyterlab_courselevels-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_courselevels
-Version: 0.3.0
+Version: 0.4.0
 Summary: Jlab extension for showing course levels and structure
 Project-URL: Homepage, https://github.com/parmentelat/jupyterlab-courselevels
 Project-URL: Bug Tracker, https://github.com/parmentelat/jupyterlab-courselevels/issues
 Project-URL: Repository, https://github.com/parmentelat/jupyterlab-courselevels.git
 Author-email: Thierry Parmentelat <thierry.parmentelat@inria.fr>
 License: BSD 3-Clause License
```

