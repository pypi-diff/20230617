# Comparing `tmp/boardgen-0.7.0.tar.gz` & `tmp/boardgen-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boardgen-0.7.0.tar", max compression
+gzip compressed data, was "boardgen-0.7.1.tar", max compression
```

## Comparing `boardgen-0.7.0.tar` & `boardgen-0.7.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0     1076 2023-06-15 18:45:53.655918 boardgen-0.7.0/LICENSE
--rw-r--r--   0        0        0     4785 2023-06-15 18:45:53.655918 boardgen-0.7.0/README.md
--rw-r--r--   0        0        0      353 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/__init__.py
--rw-r--r--   0        0        0     9220 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/cli.py
--rw-r--r--   0        0        0       92 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/core/__init__.py
--rw-r--r--   0        0        0     2543 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/core/cache.py
--rw-r--r--   0        0        0     9760 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/core/core.py
--rw-r--r--   0        0        0     1325 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/core/getters.py
--rw-r--r--   0        0        0     1891 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/draw_util.py
--rw-r--r--   0        0        0      773 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/mixins.py
--rw-r--r--   0        0        0      439 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/models/__init__.py
--rw-r--r--   0        0        0     1705 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/models/board.py
--rw-r--r--   0        0        0     1015 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/models/enums.py
--rw-r--r--   0        0        0     1156 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/models/flash_region.py
--rw-r--r--   0        0        0     1257 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/models/pcb.py
--rw-r--r--   0        0        0     2348 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/models/role.py
--rw-r--r--   0        0        0      358 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/models/template.py
--rw-r--r--   0        0        0      117 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/readme/__init__.py
--rw-r--r--   0        0        0     2229 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/readme/parts.py
--rw-r--r--   0        0        0     8123 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/readme/writer.py
--rw-r--r--   0        0        0      109 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/boards/README.md
--rw-r--r--   0        0        0      589 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/flash.json
--rw-r--r--   0        0        0      831 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/presets.json
--rw-r--r--   0        0        0     1497 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/roles.json
--rw-r--r--   0        0        0      398 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/label_line_2mm_down.json
--rw-r--r--   0        0        0      412 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/label_line_2mm_up.json
--rw-r--r--   0        0        0      690 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/labels_horz5_2mm.json
--rw-r--r--   0        0        0      829 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/labels_horz6_2mm.json
--rw-r--r--   0        0        0      967 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/labels_horz7_2mm.json
--rw-r--r--   0        0        0     1106 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/labels_horz8_2mm.json
--rw-r--r--   0        0        0      133 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pad_10x25.json
--rw-r--r--   0        0        0      525 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pads_horz5_2mm.json
--rw-r--r--   0        0        0      631 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pads_horz6_2mm.json
--rw-r--r--   0        0        0      386 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pin_horz_2mm_cast_hole.json
--rw-r--r--   0        0        0      244 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pin_horz_2mm_cast_nohole.json
--rw-r--r--   0        0        0      388 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pin_vert_2mm_cast_hole.json
--rw-r--r--   0        0        0      245 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pin_vert_2mm_cast_nohole.json
--rw-r--r--   0        0        0      540 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pins_horz5_2mm_0.7mm.json
--rw-r--r--   0        0        0      649 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pins_horz6_2mm_0.7mm.json
--rw-r--r--   0        0        0      757 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pins_horz7_2mm_0.7mm.json
--rw-r--r--   0        0        0      866 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pins_horz8_2mm_0.7mm.json
--rw-r--r--   0        0        0      789 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pins_vert7_2mm_0.7mm.json
--rw-r--r--   0        0        0      902 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/pins_vert8_2mm_0.7mm.json
--rw-r--r--   0        0        0       80 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/test_pad_1mm.json
--rw-r--r--   0        0        0      980 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/shapes/tuya2-pcb.json
--rw-r--r--   0        0        0     2931 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/custom-20x24-22.json
--rw-r--r--   0        0        0     2594 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/esp12e-21.json
--rw-r--r--   0        0        0     2640 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/esp12e-22.json
--rw-r--r--   0        0        0      256 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/esp12e-shield-nohole.json
--rw-r--r--   0        0        0      233 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/esp12e-shield.json
--rw-r--r--   0        0        0      233 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/esp12s-shield.json
--rw-r--r--   0        0        0     1666 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/esp12s.json
--rw-r--r--   0        0        0     1222 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/rf-15mm-type1.json
--rw-r--r--   0        0        0     1224 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/rf-16mm-type1.json
--rw-r--r--   0        0        0     1226 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/rf-20mm-type1.json
--rw-r--r--   0        0        0      450 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/tuya-16x24.json
--rw-r--r--   0        0        0      227 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/tuya2-shield.json
--rw-r--r--   0        0        0     1308 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/tuya2.json
--rw-r--r--   0        0        0      229 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/tuya2l-shield.json
--rw-r--r--   0        0        0      909 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/res/templates/tuya2l.json
--rw-r--r--   0        0        0      341 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/shapes/__init__.py
--rw-r--r--   0        0        0     4369 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/shapes/base.py
--rw-r--r--   0        0        0     1158 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/shapes/circle.py
--rw-r--r--   0        0        0     1283 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/shapes/fill_style.py
--rw-r--r--   0        0        0     2268 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/shapes/group.py
--rw-r--r--   0        0        0      182 2023-06-15 18:45:53.655918 boardgen-0.7.0/boardgen/shapes/label/__init__.py
--rw-r--r--   0        0        0     1745 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/shapes/label/block.py
--rw-r--r--   0        0        0      543 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/shapes/label/io_line.py
--rw-r--r--   0        0        0     3306 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/shapes/label/label.py
--rw-r--r--   0        0        0     1120 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/shapes/rect.py
--rw-r--r--   0        0        0      867 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/shapes/text.py
--rw-r--r--   0        0        0     2238 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/utils.py
--rw-r--r--   0        0        0      119 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/variant/__init__.py
--rw-r--r--   0        0        0      362 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/variant/features.py
--rw-r--r--   0        0        0     6271 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/variant/parts.py
--rw-r--r--   0        0        0      319 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/variant/section.py
--rw-r--r--   0        0        0     8502 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/variant/writer.py
--rw-r--r--   0        0        0     8765 2023-06-15 18:45:53.659918 boardgen-0.7.0/boardgen/vector.py
--rw-r--r--   0        0        0      503 2023-06-15 18:45:53.659918 boardgen-0.7.0/ltctplugin/boardgen/__init__.py
--rw-r--r--   0        0        0     4140 2023-06-15 18:45:53.659918 boardgen-0.7.0/ltctplugin/boardgen/boardgen.wxui
--rw-r--r--   0        0        0     5230 2023-06-15 18:45:53.659918 boardgen-0.7.0/ltctplugin/boardgen/boardgen.xrc
--rw-r--r--   0        0        0    11614 2023-06-15 18:45:53.659918 boardgen-0.7.0/ltctplugin/boardgen/gui.py
--rw-r--r--   0        0        0     1321 2023-06-15 18:45:53.659918 boardgen-0.7.0/ltctplugin/boardgen/svg.py
--rw-r--r--   0        0        0     3555 2023-06-15 18:45:53.659918 boardgen-0.7.0/ltctplugin/boardgen/utils.py
--rw-r--r--   0        0        0      668 2023-06-15 18:45:53.659918 boardgen-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5463 1970-01-01 00:00:00.000000 boardgen-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-16 20:44:22.097910 boardgen-0.7.1/LICENSE
+-rw-r--r--   0        0        0     4785 2023-06-16 20:44:22.097910 boardgen-0.7.1/README.md
+-rw-r--r--   0        0        0      353 2023-06-16 20:44:22.097910 boardgen-0.7.1/boardgen/__init__.py
+-rw-r--r--   0        0        0     9220 2023-06-16 20:44:22.097910 boardgen-0.7.1/boardgen/cli.py
+-rw-r--r--   0        0        0       92 2023-06-16 20:44:22.097910 boardgen-0.7.1/boardgen/core/__init__.py
+-rw-r--r--   0        0        0     2872 2023-06-16 20:44:22.097910 boardgen-0.7.1/boardgen/core/cache.py
+-rw-r--r--   0        0        0     9752 2023-06-16 20:44:22.097910 boardgen-0.7.1/boardgen/core/core.py
+-rw-r--r--   0        0        0     1325 2023-06-16 20:44:22.097910 boardgen-0.7.1/boardgen/core/getters.py
+-rw-r--r--   0        0        0     1891 2023-06-16 20:44:22.097910 boardgen-0.7.1/boardgen/draw_util.py
+-rw-r--r--   0        0        0      773 2023-06-16 20:44:22.097910 boardgen-0.7.1/boardgen/mixins.py
+-rw-r--r--   0        0        0      439 2023-06-16 20:44:22.097910 boardgen-0.7.1/boardgen/models/__init__.py
+-rw-r--r--   0        0        0     1705 2023-06-16 20:44:22.097910 boardgen-0.7.1/boardgen/models/board.py
+-rw-r--r--   0        0        0     1015 2023-06-16 20:44:22.097910 boardgen-0.7.1/boardgen/models/enums.py
+-rw-r--r--   0        0        0     1156 2023-06-16 20:44:22.097910 boardgen-0.7.1/boardgen/models/flash_region.py
+-rw-r--r--   0        0        0     1257 2023-06-16 20:44:22.097910 boardgen-0.7.1/boardgen/models/pcb.py
+-rw-r--r--   0        0        0     2348 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/models/role.py
+-rw-r--r--   0        0        0      358 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/models/template.py
+-rw-r--r--   0        0        0      117 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/readme/__init__.py
+-rw-r--r--   0        0        0     2229 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/readme/parts.py
+-rw-r--r--   0        0        0     8123 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/readme/writer.py
+-rw-r--r--   0        0        0      109 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/boards/README.md
+-rw-r--r--   0        0        0      589 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/flash.json
+-rw-r--r--   0        0        0      831 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/presets.json
+-rw-r--r--   0        0        0     1497 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/roles.json
+-rw-r--r--   0        0        0      398 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/label_line_2mm_down.json
+-rw-r--r--   0        0        0      412 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/label_line_2mm_up.json
+-rw-r--r--   0        0        0      690 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/labels_horz5_2mm.json
+-rw-r--r--   0        0        0      829 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/labels_horz6_2mm.json
+-rw-r--r--   0        0        0      967 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/labels_horz7_2mm.json
+-rw-r--r--   0        0        0     1106 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/labels_horz8_2mm.json
+-rw-r--r--   0        0        0      133 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/pad_10x25.json
+-rw-r--r--   0        0        0      525 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/pads_horz5_2mm.json
+-rw-r--r--   0        0        0      631 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/pads_horz6_2mm.json
+-rw-r--r--   0        0        0      386 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/pin_horz_2mm_cast_hole.json
+-rw-r--r--   0        0        0      244 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/pin_horz_2mm_cast_nohole.json
+-rw-r--r--   0        0        0      388 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/pin_vert_2mm_cast_hole.json
+-rw-r--r--   0        0        0      245 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/pin_vert_2mm_cast_nohole.json
+-rw-r--r--   0        0        0      540 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/pins_horz5_2mm_0.7mm.json
+-rw-r--r--   0        0        0      649 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/pins_horz6_2mm_0.7mm.json
+-rw-r--r--   0        0        0      757 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/pins_horz7_2mm_0.7mm.json
+-rw-r--r--   0        0        0      866 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/pins_horz8_2mm_0.7mm.json
+-rw-r--r--   0        0        0      789 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/pins_vert7_2mm_0.7mm.json
+-rw-r--r--   0        0        0      902 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/pins_vert8_2mm_0.7mm.json
+-rw-r--r--   0        0        0       80 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/test_pad_1mm.json
+-rw-r--r--   0        0        0      980 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/shapes/tuya2-pcb.json
+-rw-r--r--   0        0        0     2931 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/templates/custom-20x24-22.json
+-rw-r--r--   0        0        0     2594 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/templates/esp12e-21.json
+-rw-r--r--   0        0        0     2640 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/templates/esp12e-22.json
+-rw-r--r--   0        0        0      256 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/templates/esp12e-shield-nohole.json
+-rw-r--r--   0        0        0      233 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/templates/esp12e-shield.json
+-rw-r--r--   0        0        0      233 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/templates/esp12s-shield.json
+-rw-r--r--   0        0        0     1666 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/templates/esp12s.json
+-rw-r--r--   0        0        0     1222 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/templates/rf-15mm-type1.json
+-rw-r--r--   0        0        0     1224 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/templates/rf-16mm-type1.json
+-rw-r--r--   0        0        0     1226 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/templates/rf-20mm-type1.json
+-rw-r--r--   0        0        0      450 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/templates/tuya-16x24.json
+-rw-r--r--   0        0        0      227 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/templates/tuya2-shield.json
+-rw-r--r--   0        0        0     1308 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/templates/tuya2.json
+-rw-r--r--   0        0        0      229 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/templates/tuya2l-shield.json
+-rw-r--r--   0        0        0      909 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/res/templates/tuya2l.json
+-rw-r--r--   0        0        0      341 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/shapes/__init__.py
+-rw-r--r--   0        0        0     4369 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/shapes/base.py
+-rw-r--r--   0        0        0     1158 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/shapes/circle.py
+-rw-r--r--   0        0        0     1283 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/shapes/fill_style.py
+-rw-r--r--   0        0        0     2268 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/shapes/group.py
+-rw-r--r--   0        0        0      182 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/shapes/label/__init__.py
+-rw-r--r--   0        0        0     1745 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/shapes/label/block.py
+-rw-r--r--   0        0        0      543 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/shapes/label/io_line.py
+-rw-r--r--   0        0        0     3306 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/shapes/label/label.py
+-rw-r--r--   0        0        0     1120 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/shapes/rect.py
+-rw-r--r--   0        0        0      867 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/shapes/text.py
+-rw-r--r--   0        0        0     2238 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/utils.py
+-rw-r--r--   0        0        0      119 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/variant/__init__.py
+-rw-r--r--   0        0        0      362 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/variant/features.py
+-rw-r--r--   0        0        0     6271 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/variant/parts.py
+-rw-r--r--   0        0        0      319 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/variant/section.py
+-rw-r--r--   0        0        0     8502 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/variant/writer.py
+-rw-r--r--   0        0        0     8765 2023-06-16 20:44:22.101910 boardgen-0.7.1/boardgen/vector.py
+-rw-r--r--   0        0        0      503 2023-06-16 20:44:22.101910 boardgen-0.7.1/ltctplugin/boardgen/__init__.py
+-rw-r--r--   0        0        0     7728 2023-06-16 20:44:22.101910 boardgen-0.7.1/ltctplugin/boardgen/boardgen.wxui
+-rw-r--r--   0        0        0     9241 2023-06-16 20:44:22.101910 boardgen-0.7.1/ltctplugin/boardgen/boardgen.xrc
+-rw-r--r--   0        0        0    29584 2023-06-16 20:44:22.101910 boardgen-0.7.1/ltctplugin/boardgen/gui.py
+-rw-r--r--   0        0        0     1321 2023-06-16 20:44:22.101910 boardgen-0.7.1/ltctplugin/boardgen/svg.py
+-rw-r--r--   0        0        0     4046 2023-06-16 20:44:22.101910 boardgen-0.7.1/ltctplugin/boardgen/utils.py
+-rw-r--r--   0        0        0      668 2023-06-16 20:44:22.101910 boardgen-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     5463 1970-01-01 00:00:00.000000 boardgen-0.7.1/PKG-INFO
```

### Comparing `boardgen-0.7.0/LICENSE` & `boardgen-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/README.md` & `boardgen-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/cli.py` & `boardgen-0.7.1/boardgen/cli.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/core/cache.py` & `boardgen-0.7.1/boardgen/core/cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 # Copyright (c) Kuba Szczodrzyński 2022-05-12.
 
 from abc import ABC
 from glob import glob
-from os.path import basename, isfile, join
+from os.path import isfile, join, relpath
 from typing import Callable, Optional
 
 from ..utils import load_json, merge_dicts
 
 
 class CoreCache(ABC):
     _cache: dict[str, dict[str, dict]] = {
         "boards": {},
         "board_objs": {},
         "shapes": {},
         "templates": {},
     }
     json_hook: Optional[Callable[[str, str, dict, Optional[str]], None]] = None
 
+    def clear_cache(self) -> None:
+        for obj in self._cache.values():
+            obj.clear()
+        self._presets = None
+        self._roles = None
+        self._flash = None
+
     def get_dirs(self, type: str) -> list[str]:
         attr_name = f"_dirs_{type}"
         if not hasattr(self, attr_name):
             return []
         return getattr(self, attr_name)
 
-    def list_json(self, type: str) -> set[str]:
+    def list_json(self, type: str, recursive: bool = False) -> set[str]:
         dirs = self.get_dirs(type)
         files = set()
         for dir in dirs:
-            for file in glob(join(dir, "*.json")):
-                files.add(basename(file).rpartition(".")[0])
+            for file in glob(
+                join(dir, "**/*.json" if recursive else "*.json"),
+                recursive=recursive,
+            ):
+                files.add(relpath(file, dir).replace("\\", "/").rpartition(".")[0])
         return files
 
     def load_json(self, type: str, name: str) -> dict | None:
         if name in self._cache[type]:
             if self.json_hook:
                 self.json_hook(type, name, self._cache[type][name], None)
             return self._cache[type][name]
```

### Comparing `boardgen-0.7.0/boardgen/core/core.py` & `boardgen-0.7.1/boardgen/core/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,35 +21,35 @@
 from .getters import CoreGetters
 
 
 class Core(CoreCache, CoreGetters):
     shape_ctors: dict[ShapeType, type]
     is_libretiny: bool = False
 
-    _dir_base: str
+    dir_base: str
     _dirs_boards: list[str]
     _dirs_shapes: list[str]
     _dirs_templates: list[str]
 
     def __init__(self) -> None:
-        self._dir_base = join(dirname(__file__), "..", "res")
+        self.dir_base = join(dirname(__file__), "..", "res")
         self._dirs_boards = [
             join(dirname(__file__), "..", "..", "..", "..", "boards"),
-            join(self._dir_base, "boards"),
+            join(self.dir_base, "boards"),
             "boards",
         ]
         self._dirs_shapes = [
-            join(self._dir_base, "shapes"),
+            join(self.dir_base, "shapes"),
         ]
         self._dirs_templates = [
-            join(self._dir_base, "templates"),
+            join(self.dir_base, "templates"),
         ]
-        self._file_presets = join(self._dir_base, "presets.json")
-        self._file_roles = join(self._dir_base, "roles.json")
-        self._file_flash = join(self._dir_base, "flash.json")
+        self._file_presets = join(self.dir_base, "presets.json")
+        self._file_roles = join(self.dir_base, "roles.json")
+        self._file_flash = join(self.dir_base, "flash.json")
         self.shape_ctors = {
             ShapeType.RECT: Rect,
             ShapeType.CIRCLE: Circle,
             ShapeType.SUBSHAPE: ShapeGroup,
             ShapeType.TEXT: Text,
         }
         self.is_libretiny = isfile(
```

### Comparing `boardgen-0.7.0/boardgen/core/getters.py` & `boardgen-0.7.1/boardgen/core/getters.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/draw_util.py` & `boardgen-0.7.1/boardgen/draw_util.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/mixins.py` & `boardgen-0.7.1/boardgen/mixins.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/models/board.py` & `boardgen-0.7.1/boardgen/models/board.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/models/enums.py` & `boardgen-0.7.1/boardgen/models/enums.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/models/flash_region.py` & `boardgen-0.7.1/boardgen/models/flash_region.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/models/pcb.py` & `boardgen-0.7.1/boardgen/models/pcb.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/models/role.py` & `boardgen-0.7.1/boardgen/models/role.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/readme/parts.py` & `boardgen-0.7.1/boardgen/readme/parts.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/readme/writer.py` & `boardgen-0.7.1/boardgen/readme/writer.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/flash.json` & `boardgen-0.7.1/boardgen/res/flash.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/presets.json` & `boardgen-0.7.1/boardgen/res/presets.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/roles.json` & `boardgen-0.7.1/boardgen/res/roles.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/shapes/labels_horz5_2mm.json` & `boardgen-0.7.1/boardgen/res/shapes/labels_horz5_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/shapes/labels_horz6_2mm.json` & `boardgen-0.7.1/boardgen/res/shapes/labels_horz6_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/shapes/labels_horz7_2mm.json` & `boardgen-0.7.1/boardgen/res/shapes/labels_horz7_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/shapes/labels_horz8_2mm.json` & `boardgen-0.7.1/boardgen/res/shapes/labels_horz8_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/shapes/pads_horz5_2mm.json` & `boardgen-0.7.1/boardgen/res/shapes/pads_horz5_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/shapes/pads_horz6_2mm.json` & `boardgen-0.7.1/boardgen/res/shapes/pads_horz6_2mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/shapes/pins_horz5_2mm_0.7mm.json` & `boardgen-0.7.1/boardgen/res/shapes/pins_horz5_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/shapes/pins_horz6_2mm_0.7mm.json` & `boardgen-0.7.1/boardgen/res/shapes/pins_horz6_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/shapes/pins_horz7_2mm_0.7mm.json` & `boardgen-0.7.1/boardgen/res/shapes/pins_horz7_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/shapes/pins_horz8_2mm_0.7mm.json` & `boardgen-0.7.1/boardgen/res/shapes/pins_horz8_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/shapes/pins_vert7_2mm_0.7mm.json` & `boardgen-0.7.1/boardgen/res/shapes/pins_vert7_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/shapes/pins_vert8_2mm_0.7mm.json` & `boardgen-0.7.1/boardgen/res/shapes/pins_vert8_2mm_0.7mm.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/shapes/tuya2-pcb.json` & `boardgen-0.7.1/boardgen/res/shapes/tuya2-pcb.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/templates/custom-20x24-22.json` & `boardgen-0.7.1/boardgen/res/templates/custom-20x24-22.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/templates/esp12e-21.json` & `boardgen-0.7.1/boardgen/res/templates/esp12e-21.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/templates/esp12e-22.json` & `boardgen-0.7.1/boardgen/res/templates/esp12e-22.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/templates/esp12s.json` & `boardgen-0.7.1/boardgen/res/templates/esp12s.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/templates/rf-15mm-type1.json` & `boardgen-0.7.1/boardgen/res/templates/rf-15mm-type1.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/templates/rf-16mm-type1.json` & `boardgen-0.7.1/boardgen/res/templates/rf-16mm-type1.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/templates/rf-20mm-type1.json` & `boardgen-0.7.1/boardgen/res/templates/rf-20mm-type1.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/templates/tuya2.json` & `boardgen-0.7.1/boardgen/res/templates/tuya2.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/res/templates/tuya2l.json` & `boardgen-0.7.1/boardgen/res/templates/tuya2l.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/shapes/base.py` & `boardgen-0.7.1/boardgen/shapes/base.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/shapes/circle.py` & `boardgen-0.7.1/boardgen/shapes/circle.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/shapes/fill_style.py` & `boardgen-0.7.1/boardgen/shapes/fill_style.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/shapes/group.py` & `boardgen-0.7.1/boardgen/shapes/group.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/shapes/label/block.py` & `boardgen-0.7.1/boardgen/shapes/label/block.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/shapes/label/io_line.py` & `boardgen-0.7.1/boardgen/shapes/label/io_line.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/shapes/label/label.py` & `boardgen-0.7.1/boardgen/shapes/label/label.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/shapes/rect.py` & `boardgen-0.7.1/boardgen/shapes/rect.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/shapes/text.py` & `boardgen-0.7.1/boardgen/shapes/text.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/utils.py` & `boardgen-0.7.1/boardgen/utils.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/variant/parts.py` & `boardgen-0.7.1/boardgen/variant/parts.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/variant/writer.py` & `boardgen-0.7.1/boardgen/variant/writer.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/boardgen/vector.py` & `boardgen-0.7.1/boardgen/vector.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/ltctplugin/boardgen/svg.py` & `boardgen-0.7.1/ltctplugin/boardgen/svg.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.0/ltctplugin/boardgen/utils.py` & `boardgen-0.7.1/ltctplugin/boardgen/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -109,14 +109,30 @@
         obj = json.loads(s)
         return find_marker(obj)
     except json.JSONDecodeError:
         pass
     return None
 
 
+def jsonwalk(obj: dict | list, path: str) -> tuple[dict | list, str | int] | None:
+    while "." in path:
+        key, _, path = path.partition(".")
+        if isinstance(obj, list) and key.isnumeric():
+            obj = obj[int(key)]
+        elif isinstance(obj, dict):
+            obj = obj[key]
+        else:
+            return None
+    if isinstance(obj, list) and path.isnumeric():
+        path = int(path)
+    elif not isinstance(obj, dict):
+        return None
+    return obj, path
+
+
 def test_jsonpath():
     json_data = """
     {
         "mask_black": {
             "fill": {
                 "lgrad": ["1,0", "#4D4D4D", "0,1", "#0F0F0F"]
             },
```

### Comparing `boardgen-0.7.0/pyproject.toml` & `boardgen-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boardgen"
-version = "0.7.0"
+version = "0.7.1"
 description = "Board pinout diagram generator (with ltchiptool plugin GUI editor)"
 authors = ["Kuba Szczodrzyński <kuba@szczodrzynski.pl>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "boardgen" },
     { include = "ltctplugin/boardgen" },
```

### Comparing `boardgen-0.7.0/PKG-INFO` & `boardgen-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boardgen
-Version: 0.7.0
+Version: 0.7.1
 Summary: Board pinout diagram generator (with ltchiptool plugin GUI editor)
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

