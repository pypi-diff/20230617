# Comparing `tmp/oneat-5.9.9.tar.gz` & `tmp/oneat-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneat-5.9.9.tar", last modified: Thu Dec  1 17:03:17 2022, max compression
+gzip compressed data, was "oneat-6.0.0.tar", last modified: Thu Dec  1 17:14:24 2022, max compression
```

## Comparing `oneat-5.9.9.tar` & `oneat-6.0.0.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.937475 oneat-5.9.9/
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2022-12-01 17:02:59.000000 oneat-5.9.9/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-01 17:02:59.000000 oneat-5.9.9/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.917475 oneat-5.9.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.921475 oneat-5.9.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2022-12-01 17:02:59.000000 oneat-5.9.9/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2022-12-01 17:02:59.000000 oneat-5.9.9/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.921475 oneat-5.9.9/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-01 17:02:59.000000 oneat-5.9.9/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      509 2022-12-01 17:02:59.000000 oneat-5.9.9/.idea/Yoloneat.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.921475 oneat-5.9.9/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2022-12-01 17:02:59.000000 oneat-5.9.9/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2022-12-01 17:02:59.000000 oneat-5.9.9/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      268 2022-12-01 17:02:59.000000 oneat-5.9.9/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2022-12-01 17:02:59.000000 oneat-5.9.9/.idea/other.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2022-12-01 17:02:59.000000 oneat-5.9.9/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2022-12-01 17:02:59.000000 oneat-5.9.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2022-12-01 17:02:59.000000 oneat-5.9.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-01 17:02:59.000000 oneat-5.9.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2022-12-01 17:03:17.937475 oneat-5.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2022-12-01 17:02:59.000000 oneat-5.9.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.925475 oneat-5.9.9/images/
--rw-r--r--   0 runner    (1001) docker     (123)   190057 2022-12-01 17:02:59.000000 oneat-5.9.9/images/Xenopus_example.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   752746 2022-12-01 17:02:59.000000 oneat-5.9.9/images/Xenopus_example.png
--rw-r--r--   0 runner    (1001) docker     (123)    33384 2022-12-01 17:02:59.000000 oneat-5.9.9/images/ch_0_crop.png
--rw-r--r--   0 runner    (1001) docker     (123)    34434 2022-12-01 17:02:59.000000 oneat-5.9.9/images/ch_1_crop.png
--rw-r--r--   0 runner    (1001) docker     (123)    64858 2022-12-01 17:02:59.000000 oneat-5.9.9/images/ch_2_crop.png
--rw-r--r--   0 runner    (1001) docker     (123)    79433 2022-12-01 17:02:59.000000 oneat-5.9.9/images/ch_3_crop.png
--rw-r--r--   0 runner    (1001) docker     (123)    50517 2022-12-01 17:02:59.000000 oneat-5.9.9/images/ch_4_crop.png
--rw-r--r--   0 runner    (1001) docker     (123)    33211 2022-12-01 17:02:59.000000 oneat-5.9.9/images/ch_5_crop.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.925475 oneat-5.9.9/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-12-01 17:02:59.000000 oneat-5.9.9/licenses/Apache-2
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2022-12-01 17:02:59.000000 oneat-5.9.9/licenses/BSD-3
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2022-12-01 17:02:59.000000 oneat-5.9.9/licenses/GPL-3
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2022-12-01 17:02:59.000000 oneat-5.9.9/licenses/LGPL-3
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2022-12-01 17:02:59.000000 oneat-5.9.9/licenses/MIT
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2022-12-01 17:02:59.000000 oneat-5.9.9/licenses/MPL-2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.917475 oneat-5.9.9/logs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.921475 oneat-5.9.9/logs/fit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.917475 oneat-5.9.9/logs/fit/20221123-151122/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.925475 oneat-5.9.9/logs/fit/20221123-151122/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:02:59.000000 oneat-5.9.9/logs/fit/20221123-151122/train/events.out.tfevents.1669212683.KAPOORLABS.12084.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.917475 oneat-5.9.9/logs/fit/20221123-151247/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.925475 oneat-5.9.9/logs/fit/20221123-151247/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:02:59.000000 oneat-5.9.9/logs/fit/20221123-151247/train/events.out.tfevents.1669212767.KAPOORLABS.6468.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.917475 oneat-5.9.9/logs/fit/20221123-152314/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.925475 oneat-5.9.9/logs/fit/20221123-152314/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:02:59.000000 oneat-5.9.9/logs/fit/20221123-152314/train/events.out.tfevents.1669213394.KAPOORLABS.37528.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.917475 oneat-5.9.9/logs/fit/20221123-152337/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.925475 oneat-5.9.9/logs/fit/20221123-152337/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:02:59.000000 oneat-5.9.9/logs/fit/20221123-152337/train/events.out.tfevents.1669213417.KAPOORLABS.17652.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.917475 oneat-5.9.9/logs/fit/20221123-152411/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.925475 oneat-5.9.9/logs/fit/20221123-152411/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:02:59.000000 oneat-5.9.9/logs/fit/20221123-152411/train/events.out.tfevents.1669213451.KAPOORLABS.20748.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.917475 oneat-5.9.9/logs/fit/20221123-152525/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.925475 oneat-5.9.9/logs/fit/20221123-152525/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22381 2022-12-01 17:02:59.000000 oneat-5.9.9/logs/fit/20221123-152525/train/events.out.tfevents.1669213525.Kapoorlabs.1753.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.917475 oneat-5.9.9/logs/fit/20221123-153101/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.925475 oneat-5.9.9/logs/fit/20221123-153101/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22381 2022-12-01 17:02:59.000000 oneat-5.9.9/logs/fit/20221123-153101/train/events.out.tfevents.1669213861.Kapoorlabs.1839.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.917475 oneat-5.9.9/logs/fit/20221123-153142/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.925475 oneat-5.9.9/logs/fit/20221123-153142/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22381 2022-12-01 17:02:59.000000 oneat-5.9.9/logs/fit/20221123-153142/train/events.out.tfevents.1669213902.Kapoorlabs.1925.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.917475 oneat-5.9.9/logs/fit/20221123-153330/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.925475 oneat-5.9.9/logs/fit/20221123-153330/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22381 2022-12-01 17:02:59.000000 oneat-5.9.9/logs/fit/20221123-153330/train/events.out.tfevents.1669214010.Kapoorlabs.2330.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.921475 oneat-5.9.9/logs/fit/20221123-153435/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.925475 oneat-5.9.9/logs/fit/20221123-153435/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:02:59.000000 oneat-5.9.9/logs/fit/20221123-153435/train/events.out.tfevents.1669214075.KAPOORLABS.24332.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.921475 oneat-5.9.9/logs/fit/20221123-153515/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.925475 oneat-5.9.9/logs/fit/20221123-153515/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:02:59.000000 oneat-5.9.9/logs/fit/20221123-153515/train/events.out.tfevents.1669214115.KAPOORLABS.40224.0.v2
--rw-r--r--   0 runner    (1001) docker     (123)      255 2022-12-01 17:02:59.000000 oneat-5.9.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2022-12-01 17:03:17.937475 oneat-5.9.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.921475 oneat-5.9.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.929475 oneat-5.9.9/src/oneat/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.929475 oneat-5.9.9/src/oneat/NEATModels/
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/.neat_focus.py.swp
--rw-r--r--   0 runner    (1001) docker     (123)      554 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/MidogConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/Staticconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/TrainConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/gen_anchors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13041 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    38176 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/neat_densevollnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    40718 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/neat_dynamic_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    27082 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/neat_focus.py
--rw-r--r--   0 runner    (1001) docker     (123)    21313 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/neat_focus_microscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    39187 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/neat_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/neat_microscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    23305 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/neat_static_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    38167 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/neat_vollnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    40628 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATModels/nets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.933475 oneat-5.9.9/src/oneat/NEATUtils/
--rw-r--r--   0 runner    (1001) docker     (123)    24113 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/HolovizNapari.py
--rw-r--r--   0 runner    (1001) docker     (123)    51302 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/MovieCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/NMS.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/VisualizeDetections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/Zmapgen.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.933475 oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    25380 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    20890 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.933475 oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    25029 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    70487 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/NEATUtils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.933475 oneat-5.9.9/src/oneat/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/_tests/test_nets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/_tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.937475 oneat-5.9.9/src/oneat/_tests/variables/
--rw-r--r--   0 runner    (1001) docker     (123)  5142983 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/_tests/variables/variables.data-00000-of-00001
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/_tests/variables/variables.index
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-01 17:03:17.000000 oneat-5.9.9/src/oneat/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/caped.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2022-12-01 17:02:59.000000 oneat-5.9.9/src/oneat/pretrained.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:03:17.929475 oneat-5.9.9/src/oneat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2022-12-01 17:03:17.000000 oneat-5.9.9/src/oneat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2022-12-01 17:03:17.000000 oneat-5.9.9/src/oneat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-01 17:03:17.000000 oneat-5.9.9/src/oneat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-01 17:03:17.000000 oneat-5.9.9/src/oneat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2022-12-01 17:03:17.000000 oneat-5.9.9/src/oneat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-01 17:03:17.000000 oneat-5.9.9/src/oneat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2022-12-01 17:02:59.000000 oneat-5.9.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.969071 oneat-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2022-12-01 17:14:07.000000 oneat-6.0.0/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-01 17:14:07.000000 oneat-6.0.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.945070 oneat-6.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2022-12-01 17:14:07.000000 oneat-6.0.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2022-12-01 17:14:07.000000 oneat-6.0.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-01 17:14:07.000000 oneat-6.0.0/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2022-12-01 17:14:07.000000 oneat-6.0.0/.idea/Yoloneat.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2022-12-01 17:14:07.000000 oneat-6.0.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2022-12-01 17:14:07.000000 oneat-6.0.0/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2022-12-01 17:14:07.000000 oneat-6.0.0/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2022-12-01 17:14:07.000000 oneat-6.0.0/.idea/other.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2022-12-01 17:14:07.000000 oneat-6.0.0/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2022-12-01 17:14:07.000000 oneat-6.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2022-12-01 17:14:07.000000 oneat-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-01 17:14:07.000000 oneat-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2022-12-01 17:14:24.969071 oneat-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2022-12-01 17:14:07.000000 oneat-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   190057 2022-12-01 17:14:07.000000 oneat-6.0.0/images/Xenopus_example.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   752746 2022-12-01 17:14:07.000000 oneat-6.0.0/images/Xenopus_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33384 2022-12-01 17:14:07.000000 oneat-6.0.0/images/ch_0_crop.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34434 2022-12-01 17:14:07.000000 oneat-6.0.0/images/ch_1_crop.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64858 2022-12-01 17:14:07.000000 oneat-6.0.0/images/ch_2_crop.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79433 2022-12-01 17:14:07.000000 oneat-6.0.0/images/ch_3_crop.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50517 2022-12-01 17:14:07.000000 oneat-6.0.0/images/ch_4_crop.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33211 2022-12-01 17:14:07.000000 oneat-6.0.0/images/ch_5_crop.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-12-01 17:14:07.000000 oneat-6.0.0/licenses/Apache-2
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2022-12-01 17:14:07.000000 oneat-6.0.0/licenses/BSD-3
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2022-12-01 17:14:07.000000 oneat-6.0.0/licenses/GPL-3
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2022-12-01 17:14:07.000000 oneat-6.0.0/licenses/LGPL-3
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2022-12-01 17:14:07.000000 oneat-6.0.0/licenses/MIT
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2022-12-01 17:14:07.000000 oneat-6.0.0/licenses/MPL-2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.945070 oneat-6.0.0/logs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.945070 oneat-6.0.0/logs/fit/20221123-151122/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/logs/fit/20221123-151122/train/
+-rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-151122/train/events.out.tfevents.1669212683.KAPOORLABS.12084.0.v2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-151247/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/logs/fit/20221123-151247/train/
+-rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-151247/train/events.out.tfevents.1669212767.KAPOORLABS.6468.0.v2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-152314/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/logs/fit/20221123-152314/train/
+-rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-152314/train/events.out.tfevents.1669213394.KAPOORLABS.37528.0.v2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-152337/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/logs/fit/20221123-152337/train/
+-rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-152337/train/events.out.tfevents.1669213417.KAPOORLABS.17652.0.v2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-152411/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/logs/fit/20221123-152411/train/
+-rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-152411/train/events.out.tfevents.1669213451.KAPOORLABS.20748.0.v2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-152525/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.957070 oneat-6.0.0/logs/fit/20221123-152525/train/
+-rw-r--r--   0 runner    (1001) docker     (123)    22381 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-152525/train/events.out.tfevents.1669213525.Kapoorlabs.1753.0.v2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-153101/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.957070 oneat-6.0.0/logs/fit/20221123-153101/train/
+-rw-r--r--   0 runner    (1001) docker     (123)    22381 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-153101/train/events.out.tfevents.1669213861.Kapoorlabs.1839.0.v2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-153142/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.957070 oneat-6.0.0/logs/fit/20221123-153142/train/
+-rw-r--r--   0 runner    (1001) docker     (123)    22381 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-153142/train/events.out.tfevents.1669213902.Kapoorlabs.1925.0.v2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-153330/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.957070 oneat-6.0.0/logs/fit/20221123-153330/train/
+-rw-r--r--   0 runner    (1001) docker     (123)    22381 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-153330/train/events.out.tfevents.1669214010.Kapoorlabs.2330.0.v2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-153435/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.957070 oneat-6.0.0/logs/fit/20221123-153435/train/
+-rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-153435/train/events.out.tfevents.1669214075.KAPOORLABS.24332.0.v2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-153515/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.957070 oneat-6.0.0/logs/fit/20221123-153515/train/
+-rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-153515/train/events.out.tfevents.1669214115.KAPOORLABS.40224.0.v2
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2022-12-01 17:14:07.000000 oneat-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2022-12-01 17:14:24.969071 oneat-6.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.957070 oneat-6.0.0/src/oneat/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.961070 oneat-6.0.0/src/oneat/NEATModels/
+-rw-r--r--   0 runner    (1001) docker     (123)    20480 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/.neat_focus.py.swp
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/MidogConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/Staticconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/TrainConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/gen_anchors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13041 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38176 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/neat_densevollnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40718 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/neat_dynamic_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27082 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/neat_focus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21313 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/neat_focus_microscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39187 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/neat_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15758 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/neat_microscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23305 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/neat_static_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38167 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/neat_vollnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40628 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/nets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.961070 oneat-6.0.0/src/oneat/NEATUtils/
+-rw-r--r--   0 runner    (1001) docker     (123)    24113 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/HolovizNapari.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51303 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/MovieCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/NMS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/VisualizeDetections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/Zmapgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.961070 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25380 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20890 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.961070 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25029 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70487 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.961070 oneat-6.0.0/src/oneat/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/_tests/test_nets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/_tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.969071 oneat-6.0.0/src/oneat/_tests/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)  5142983 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/_tests/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/_tests/variables/variables.index
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-01 17:14:24.000000 oneat-6.0.0/src/oneat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/caped.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/pretrained.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.957070 oneat-6.0.0/src/oneat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2022-12-01 17:14:24.000000 oneat-6.0.0/src/oneat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2022-12-01 17:14:24.000000 oneat-6.0.0/src/oneat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-01 17:14:24.000000 oneat-6.0.0/src/oneat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-01 17:14:24.000000 oneat-6.0.0/src/oneat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2022-12-01 17:14:24.000000 oneat-6.0.0/src/oneat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-01 17:14:24.000000 oneat-6.0.0/src/oneat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2022-12-01 17:14:07.000000 oneat-6.0.0/tox.ini
```

### Comparing `oneat-5.9.9/.DS_Store` & `oneat-6.0.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/.github/workflows/test_and_deploy.yml` & `oneat-6.0.0/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/.gitignore` & `oneat-6.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/.pre-commit-config.yaml` & `oneat-6.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/LICENSE` & `oneat-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/PKG-INFO` & `oneat-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 5.9.9
+Version: 6.0.0
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-5.9.9/README.md` & `oneat-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/images/Xenopus_example.jpg` & `oneat-6.0.0/images/Xenopus_example.jpg`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/images/Xenopus_example.png` & `oneat-6.0.0/images/Xenopus_example.png`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/images/ch_0_crop.png` & `oneat-6.0.0/images/ch_0_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/images/ch_1_crop.png` & `oneat-6.0.0/images/ch_1_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/images/ch_2_crop.png` & `oneat-6.0.0/images/ch_2_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/images/ch_3_crop.png` & `oneat-6.0.0/images/ch_3_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/images/ch_4_crop.png` & `oneat-6.0.0/images/ch_4_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/images/ch_5_crop.png` & `oneat-6.0.0/images/ch_5_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/licenses/Apache-2` & `oneat-6.0.0/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/licenses/BSD-3` & `oneat-6.0.0/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/licenses/GPL-3` & `oneat-6.0.0/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/licenses/LGPL-3` & `oneat-6.0.0/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/licenses/MIT` & `oneat-6.0.0/licenses/MIT`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/licenses/MPL-2` & `oneat-6.0.0/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/logs/fit/20221123-151122/train/events.out.tfevents.1669212683.KAPOORLABS.12084.0.v2` & `oneat-6.0.0/logs/fit/20221123-151122/train/events.out.tfevents.1669212683.KAPOORLABS.12084.0.v2`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/logs/fit/20221123-151247/train/events.out.tfevents.1669212767.KAPOORLABS.6468.0.v2` & `oneat-6.0.0/logs/fit/20221123-151247/train/events.out.tfevents.1669212767.KAPOORLABS.6468.0.v2`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/logs/fit/20221123-152314/train/events.out.tfevents.1669213394.KAPOORLABS.37528.0.v2` & `oneat-6.0.0/logs/fit/20221123-152314/train/events.out.tfevents.1669213394.KAPOORLABS.37528.0.v2`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/logs/fit/20221123-152337/train/events.out.tfevents.1669213417.KAPOORLABS.17652.0.v2` & `oneat-6.0.0/logs/fit/20221123-152337/train/events.out.tfevents.1669213417.KAPOORLABS.17652.0.v2`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/logs/fit/20221123-152411/train/events.out.tfevents.1669213451.KAPOORLABS.20748.0.v2` & `oneat-6.0.0/logs/fit/20221123-152411/train/events.out.tfevents.1669213451.KAPOORLABS.20748.0.v2`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/logs/fit/20221123-152525/train/events.out.tfevents.1669213525.Kapoorlabs.1753.0.v2` & `oneat-6.0.0/logs/fit/20221123-152525/train/events.out.tfevents.1669213525.Kapoorlabs.1753.0.v2`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/logs/fit/20221123-153101/train/events.out.tfevents.1669213861.Kapoorlabs.1839.0.v2` & `oneat-6.0.0/logs/fit/20221123-153101/train/events.out.tfevents.1669213861.Kapoorlabs.1839.0.v2`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/logs/fit/20221123-153142/train/events.out.tfevents.1669213902.Kapoorlabs.1925.0.v2` & `oneat-6.0.0/logs/fit/20221123-153142/train/events.out.tfevents.1669213902.Kapoorlabs.1925.0.v2`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/logs/fit/20221123-153330/train/events.out.tfevents.1669214010.Kapoorlabs.2330.0.v2` & `oneat-6.0.0/logs/fit/20221123-153330/train/events.out.tfevents.1669214010.Kapoorlabs.2330.0.v2`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/logs/fit/20221123-153435/train/events.out.tfevents.1669214075.KAPOORLABS.24332.0.v2` & `oneat-6.0.0/logs/fit/20221123-153435/train/events.out.tfevents.1669214075.KAPOORLABS.24332.0.v2`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/logs/fit/20221123-153515/train/events.out.tfevents.1669214115.KAPOORLABS.40224.0.v2` & `oneat-6.0.0/logs/fit/20221123-153515/train/events.out.tfevents.1669214115.KAPOORLABS.40224.0.v2`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/setup.cfg` & `oneat-6.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 	pandas
 	vollseg-napari
 	scipy
 	tifffile
 	matplotlib
 	imagecodecs
 	napari[all]
-	
 	scikit-learn
 	dask
 	natsort
 	napari-animation
 	pydot
 	graphviz
 	oneat-augmentations
@@ -59,15 +58,14 @@
 [options.entry_points]
 caped.manifest = 
 	oneat = oneat:caped.yaml
 
 [options.extras_require]
 testing = 
 	tox
-	oneat
 	pytest  # https://docs.pytest.org/en/latest/contents.html
 	pytest-cov  # https://pytest-cov.readthedocs.io/en/latest/
 
 [options.package_data]
 * = *.yaml
 
 [egg_info]
```

### Comparing `oneat-5.9.9/src/oneat/NEATModels/.neat_focus.py.swp` & `oneat-6.0.0/src/oneat/NEATModels/.neat_focus.py.swp`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATModels/MidogConfig.py` & `oneat-6.0.0/src/oneat/NEATModels/MidogConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATModels/Staticconfig.py` & `oneat-6.0.0/src/oneat/NEATModels/Staticconfig.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATModels/TrainConfig.py` & `oneat-6.0.0/src/oneat/NEATModels/TrainConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATModels/__init__.py` & `oneat-6.0.0/src/oneat/NEATModels/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATModels/config.py` & `oneat-6.0.0/src/oneat/NEATModels/config.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATModels/gen_anchors.py` & `oneat-6.0.0/src/oneat/NEATModels/gen_anchors.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATModels/loss.py` & `oneat-6.0.0/src/oneat/NEATModels/loss.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATModels/neat_densevollnet.py` & `oneat-6.0.0/src/oneat/NEATModels/neat_densevollnet.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATModels/neat_dynamic_resnet.py` & `oneat-6.0.0/src/oneat/NEATModels/neat_dynamic_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATModels/neat_focus.py` & `oneat-6.0.0/src/oneat/NEATModels/neat_focus.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATModels/neat_focus_microscope.py` & `oneat-6.0.0/src/oneat/NEATModels/neat_focus_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATModels/neat_lstm.py` & `oneat-6.0.0/src/oneat/NEATModels/neat_lstm.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATModels/neat_microscope.py` & `oneat-6.0.0/src/oneat/NEATModels/neat_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATModels/neat_static_resnet.py` & `oneat-6.0.0/src/oneat/NEATModels/neat_static_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATModels/neat_vollnet.py` & `oneat-6.0.0/src/oneat/NEATModels/neat_vollnet.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATModels/nets.py` & `oneat-6.0.0/src/oneat/NEATModels/nets.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATUtils/HolovizNapari.py` & `oneat-6.0.0/src/oneat/NEATUtils/HolovizNapari.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATUtils/MovieCreator.py` & `oneat-6.0.0/src/oneat/NEATUtils/MovieCreator.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 from PIL import Image
 from skimage import measure
+
 from sklearn.model_selection import train_test_split
 from tifffile import imread, imwrite
 from tqdm import tqdm
 
 from .utils import normalizeFloatZeroOne
```

### Comparing `oneat-5.9.9/src/oneat/NEATUtils/NMS.py` & `oneat-6.0.0/src/oneat/NEATUtils/NMS.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATUtils/VisualizeDetections.py` & `oneat-6.0.0/src/oneat/NEATUtils/VisualizeDetections.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATUtils/Zmapgen.py` & `oneat-6.0.0/src/oneat/NEATUtils/Zmapgen.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py` & `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py` & `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py` & `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py` & `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py` & `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py` & `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py` & `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py` & `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py` & `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATUtils/plotters.py` & `oneat-6.0.0/src/oneat/NEATUtils/plotters.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/NEATUtils/utils.py` & `oneat-6.0.0/src/oneat/NEATUtils/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/__init__.py` & `oneat-6.0.0/src/oneat/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/_tests/test_nets.py` & `oneat-6.0.0/src/oneat/_tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/_tests/utils.py` & `oneat-6.0.0/src/oneat/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/_tests/variables/variables.data-00000-of-00001` & `oneat-6.0.0/src/oneat/_tests/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/_tests/variables/variables.index` & `oneat-6.0.0/src/oneat/_tests/variables/variables.index`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat/pretrained.py` & `oneat-6.0.0/src/oneat/pretrained.py`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/src/oneat.egg-info/PKG-INFO` & `oneat-6.0.0/src/oneat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 5.9.9
+Version: 6.0.0
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-5.9.9/src/oneat.egg-info/SOURCES.txt` & `oneat-6.0.0/src/oneat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oneat-5.9.9/tox.ini` & `oneat-6.0.0/tox.ini`

 * *Files identical despite different names*

