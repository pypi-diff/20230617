# Comparing `tmp/ocp_tessellate-1.0.4.tar.gz` & `tmp/ocp_tessellate-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_tessellate-1.0.4.tar", last modified: Mon Jun  5 20:14:58 2023, max compression
+gzip compressed data, was "ocp_tessellate-1.1.0.tar", last modified: Fri Jun 16 20:28:20 2023, max compression
```

## Comparing `ocp_tessellate-1.0.4.tar` & `ocp_tessellate-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-05 20:14:58.776888 ocp_tessellate-1.0.4/
--rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-06-05 20:14:58.776946 ocp_tessellate-1.0.4/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-02-04 10:28:52.000000 ocp_tessellate-1.0.4/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-05 20:14:58.775842 ocp_tessellate-1.0.4/ocp_tessellate/
--rw-r--r--   0 bernhard   (501) staff       (20)     2926 2023-02-11 19:32:38.000000 ocp_tessellate-1.0.4/ocp_tessellate/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1123 2023-06-05 20:14:48.000000 ocp_tessellate-1.0.4/ocp_tessellate/_version.py
--rw-r--r--   0 bernhard   (501) staff       (20)    12980 2023-04-23 07:18:10.000000 ocp_tessellate-1.0.4/ocp_tessellate/cad_objects.py
--rw-r--r--   0 bernhard   (501) staff       (20)    28124 2023-06-05 20:03:27.000000 ocp_tessellate-1.0.4/ocp_tessellate/convert.py
--rw-r--r--   0 bernhard   (501) staff       (20)    10515 2023-04-23 07:18:10.000000 ocp_tessellate-1.0.4/ocp_tessellate/defaults.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-02-11 19:32:38.000000 ocp_tessellate-1.0.4/ocp_tessellate/mp_tess.py
--rw-r--r--   0 bernhard   (501) staff       (20)     3033 2023-02-11 19:32:38.000000 ocp_tessellate-1.0.4/ocp_tessellate/mp_tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)    19996 2023-06-05 19:58:43.000000 ocp_tessellate-1.0.4/ocp_tessellate/ocp_utils.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13370 2023-04-23 10:15:07.000000 ocp_tessellate-1.0.4/ocp_tessellate/stepreader.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13224 2023-04-23 10:15:07.000000 ocp_tessellate-1.0.4/ocp_tessellate/tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)     6223 2023-04-29 10:55:18.000000 ocp_tessellate-1.0.4/ocp_tessellate/utils.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-05 20:14:58.776722 ocp_tessellate-1.0.4/ocp_tessellate.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-06-05 20:14:58.000000 ocp_tessellate-1.0.4/ocp_tessellate.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      561 2023-06-05 20:14:58.000000 ocp_tessellate-1.0.4/ocp_tessellate.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-05 20:14:58.000000 ocp_tessellate-1.0.4/ocp_tessellate.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-05 20:14:58.000000 ocp_tessellate-1.0.4/ocp_tessellate.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)      102 2023-06-05 20:14:58.000000 ocp_tessellate-1.0.4/ocp_tessellate.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       15 2023-06-05 20:14:58.000000 ocp_tessellate-1.0.4/ocp_tessellate.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      671 2023-06-05 20:14:58.777206 ocp_tessellate-1.0.4/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1646 2023-06-05 20:14:48.000000 ocp_tessellate-1.0.4/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-16 20:28:20.584547 ocp_tessellate-1.1.0/
+-rw-r--r--   0 bernhard   (501) staff       (20)      810 2023-06-16 20:28:20.584589 ocp_tessellate-1.1.0/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-02-04 10:28:52.000000 ocp_tessellate-1.1.0/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-16 20:28:20.583840 ocp_tessellate-1.1.0/ocp_tessellate/
+-rw-r--r--   0 bernhard   (501) staff       (20)     2926 2023-02-11 19:32:38.000000 ocp_tessellate-1.1.0/ocp_tessellate/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1123 2023-06-16 06:52:31.000000 ocp_tessellate-1.1.0/ocp_tessellate/_version.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13575 2023-06-15 16:29:54.000000 ocp_tessellate-1.1.0/ocp_tessellate/cad_objects.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    30958 2023-06-16 06:31:35.000000 ocp_tessellate-1.1.0/ocp_tessellate/convert.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    10521 2023-06-16 06:30:40.000000 ocp_tessellate-1.1.0/ocp_tessellate/defaults.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-02-11 19:32:38.000000 ocp_tessellate-1.1.0/ocp_tessellate/mp_tess.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3033 2023-02-11 19:32:38.000000 ocp_tessellate-1.1.0/ocp_tessellate/mp_tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    22358 2023-06-15 21:03:54.000000 ocp_tessellate-1.1.0/ocp_tessellate/ocp_utils.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13370 2023-04-23 10:15:07.000000 ocp_tessellate-1.1.0/ocp_tessellate/stepreader.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13224 2023-04-23 10:15:07.000000 ocp_tessellate-1.1.0/ocp_tessellate/tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     6223 2023-04-29 10:55:18.000000 ocp_tessellate-1.1.0/ocp_tessellate/utils.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-16 20:28:20.584455 ocp_tessellate-1.1.0/ocp_tessellate.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      810 2023-06-16 20:28:20.000000 ocp_tessellate-1.1.0/ocp_tessellate.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      561 2023-06-16 20:28:20.000000 ocp_tessellate-1.1.0/ocp_tessellate.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-16 20:28:20.000000 ocp_tessellate-1.1.0/ocp_tessellate.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-16 20:28:20.000000 ocp_tessellate-1.1.0/ocp_tessellate.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)      102 2023-06-16 20:28:20.000000 ocp_tessellate-1.1.0/ocp_tessellate.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       15 2023-06-16 20:28:20.000000 ocp_tessellate-1.1.0/ocp_tessellate.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      671 2023-06-16 20:28:20.584876 ocp_tessellate-1.1.0/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1646 2023-06-16 06:52:31.000000 ocp_tessellate-1.1.0/setup.py
```

### Comparing `ocp_tessellate-1.0.4/PKG-INFO` & `ocp_tessellate-1.1.0/ocp_tessellate.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
-Name: ocp_tessellate
-Version: 1.0.4
+Name: ocp-tessellate
+Version: 1.1.0
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
+License: UNKNOWN
 Keywords: CAD,cadquery
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Provides-Extra: dev
 
 Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs
+
```

### Comparing `ocp_tessellate-1.0.4/ocp_tessellate/__init__.py` & `ocp_tessellate-1.1.0/ocp_tessellate/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.4/ocp_tessellate/_version.py` & `ocp_tessellate-1.1.0/ocp_tessellate/_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     r = re.compile(
         r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)\-{0,1}(?P<release>\D*)(?P<build>\d*)"
     )
     major, minor, patch, release, build = r.match(version).groups()
     return VersionInfo(major, minor, patch, release, build)
 
 
-__version__ = "1.0.4"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
+__version__ = "1.1.0"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
 __version_info__ = get_version(__version__)
```

### Comparing `ocp_tessellate-1.0.4/ocp_tessellate/cad_objects.py` & `ocp_tessellate-1.1.0/ocp_tessellate/cad_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,21 @@
     bounding_box,
     get_point,
     loc_to_tq,
     get_location,
     np_bbox,
     is_line,
     line,
-    make_compound,
+    axis_to_vecs,
+    loc_to_vecs,
+    vertex,
     identity_location,
+    make_compound,
     cross,
+    normalized,
 )
 from .tessellator import discretize_edge, tessellate, compute_quality
 from .mp_tessellator import is_apply_result, mp_tessellate, init_pool, keymap
 from .defaults import get_default
 
 UNSELECTED = 0
 SELECTED = 1
@@ -438,15 +442,29 @@
             result += obj.compounds()
         return result
 
     def compound(self):
         return make_compound(self.compounds())
 
 
+class CoordAxis(OCP_Edges):
+    def __init__(self, name, origin, z_dir, size=1):
+        o, x, y, z = axis_to_vecs(origin, z_dir)
+        edge = line(o, o + size * z)
+        a2 = line(o + size * z, o + size * 0.9 * z - 0.025 * x)
+        a3 = line(o + size * z, o + size * 0.9 * z + 0.025 * x)
+        a4 = line(o + size * z, o + size * 0.9 * z - 0.025 * y)
+        a5 = line(o + size * z, o + size * 0.9 * z + 0.025 * y)
+        # c = circle((o + size * 0.9 * z).Coord(), z_dir, 0.025)
+        colors = Color("black")
+        super().__init__([edge, a2, a3, a4, a5], name, colors, width=3)
+
+
 class CoordSystem(OCP_Edges):
-    def __init__(self, name, origin, X, Z, size=1):
-        Y = cross(X, Z)
-        x_edge = line(origin, [o + v * size for o, v in zip(origin, X)])
-        y_edge = line(origin, [o + v * size for o, v in zip(origin, Y)])
-        z_edge = line(origin, [o + v * size for o, v in zip(origin, Z)])
+    def __init__(self, name, origin, x_dir, z_dir, size=1):
+        o, x, y, z = loc_to_vecs(origin, x_dir, z_dir)
+        x_edge = line(o, o + size * x)
+        y_edge = line(o, o + size * y)
+        z_edge = line(o, o + size * z)
+
         colors = (Color("red"), Color("green"), Color("blue"))
         super().__init__([x_edge, y_edge, z_edge], name, colors, width=3)
```

### Comparing `ocp_tessellate-1.0.4/ocp_tessellate/convert.py` & `ocp_tessellate-1.1.0/ocp_tessellate/convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from collections.abc import Iterable
 
 import json
 
 from .cad_objects import (
     CoordSystem,
+    CoordAxis,
     OCP_Edges,
     OCP_Faces,
     OCP_Part,
     OCP_PartGroup,
     OCP_Vertices,
     get_instances,
     set_instances,
@@ -37,14 +38,16 @@
     get_downcasted_shape,
     get_edges,
     get_faces,
     get_location,
     get_rgba,
     get_tshape,
     get_tlocation,
+    get_location_coord,
+    get_axis_coord,
     get_tuple,
     identity_location,
     is_build123d_assembly,
     is_build123d_compound,
     is_build123d_shape,
     is_build123d_shell,
     is_build123d,
@@ -68,14 +71,17 @@
     is_topods_shell,
     is_topods_vertex,
     is_topods_wire,
     is_vector,
     is_vertex_list,
     is_wire_list,
     is_wrapped,
+    is_gp_axis,
+    is_gp_plane,
+    is_plane_xy,
     make_compound,
     np_bbox,
     ocp_color,
     vertex,
     loc_to_tq,
 )
 
@@ -454,15 +460,15 @@
 def _to_assembly(
     *cad_objs,
     names=None,
     colors=None,
     alphas=None,
     render_mates=None,
     render_joints=None,
-    mate_scale=1,
+    helper_scale=1,
     default_color=None,
     show_parent=False,
     loc=None,
     mates=None,
     instances=None,
     progress=None,
     is_assembly=False,
@@ -514,81 +520,101 @@
             elif (
                 hasattr(cad_obj, "name")
                 and cad_obj.name is not None
                 and cad_obj.name != ""
             ):
                 obj_name = cad_obj.name
 
+        if is_cadquery(cad_obj) and (
+            len(cad_obj.objects) == 0
+            or (len(cad_obj.objects) == 1 and is_vector(cad_obj.objects[0]))
+        ):  # Workplane:
+            cad_obj = cad_obj.plane.location
+            if obj_name is None:
+                obj_name = "workplane"
+
         if is_cadquery_assembly(cad_obj):
             _debug("to_assembly: cadquery assembly", obj_name)
 
+            add_to_ass = False
+            if is_assembly:
+                ass = pg
+                ass.name = cad_obj.name
+                ass.loc = get_location(cad_obj, as_none=False)
+            else:
+                add_to_ass = True
+                ass = OCP_PartGroup(
+                    [],
+                    name="Group" if obj_name is None else obj_name,
+                    loc=get_location(cad_obj, as_none=False),
+                )
             #
             # Iterate over CadQuery Assembly
             #
             is_assembly = True
 
-            pg.name = cad_obj.name
-            pg.loc = get_location(cad_obj, as_none=False)
-
             if cad_obj.obj is not None:
                 # Get an existing instance id or tessellate this object
 
                 if is_cadquery_massembly(cad_obj):
                     # get_instance fails for MAssemblies when a mate is not at the
                     # shape origin after relocation, see hexapod "top" object
                     # workaround: do not handle TShapes
                     part = conv(cad_obj.obj, cad_obj.name, color, alpha)
                 else:
                     part = get_instance(cad_obj.obj, pg.name, rgba, instances, progress)
-                pg.add(part)
+                ass.add(part)
 
             # render mates
             top_level_mates = None
             if render_mates and hasattr(cad_obj, "mates") and cad_obj.mates is not None:
                 top_level_mates = cad_obj.mates if mates is None else mates
 
                 # create a new part group for mates
                 pg2 = OCP_PartGroup(
                     [
                         CoordSystem(
                             name,
                             get_tuple(mate_def.mate.origin),
                             get_tuple(mate_def.mate.x_dir),
                             get_tuple(mate_def.mate.z_dir),
-                            mate_scale,
+                            helper_scale,
                         )
                         for name, mate_def in top_level_mates.items()
                         if mate_def.assembly == cad_obj
                     ],
                     name="mates",
                     loc=identity_location(),  # mates inherit the parent location, so actually add a no-op
                 )
 
                 # add mates partgroup
                 if pg2.objects:
-                    pg.add(pg2)
+                    ass.add(pg2)
 
             # iterate recursively over all children
             for child in cad_obj.children:
                 part, instances = _to_assembly(
                     child,
                     loc=loc,
                     default_color=default_color,
                     names=[obj_name],
                     colors=[obj_color],
                     alphas=[obj_alpha],
                     mates=top_level_mates,
                     render_mates=render_mates,
                     render_joints=render_joints,
-                    mate_scale=mate_scale,
+                    helper_scale=helper_scale,
                     instances=instances,
                     progress=progress,
                     is_assembly=is_assembly,
                 )
-                pg.add(part)
+                ass.add(part)
+
+            if add_to_ass:
+                pg.add(ass)
 
         elif is_cadquery_sketch(cad_obj):
             _debug("to_assembly: cadquery sketch", obj_name)
             #
             # Special treatment for cadquery sketches
             #
 
@@ -597,52 +623,106 @@
                     child,
                     default_color=default_color,
                     names=[obj_name],
                     colors=[obj_color],
                     alphas=[obj_alpha],
                     render_mates=render_mates,
                     render_joints=render_joints,
-                    mate_scale=mate_scale,
+                    helper_scale=helper_scale,
                     instances=instances,
                     progress=progress,
                 )
                 if len(part.objects) == 1:
                     pg.add(part.objects[0])
                 else:
                     pg.add(part)
 
+        elif (
+            is_build123d(cad_obj)
+            and hasattr(cad_obj, "sketch_local")
+            and not (
+                len(cad_obj.workplanes) == 1
+                and is_plane_xy(cad_obj.workplanes[0].wrapped)
+            )
+        ):
+            _debug("to_assembly: BuildSketch with plane != Plane.XY", obj_name)
+            obj = OCP_PartGroup(
+                [
+                    conv(cad_obj.sketch.faces(), obj_name="sketch"),
+                    conv(
+                        cad_obj.sketch_local.faces(),
+                        obj_name="sketch_local",
+                        obj_alpha=0.2,
+                    ),
+                ],
+                name="sketch" if obj_name is None else obj_name,
+            )
+            pg.add(obj)
+
         # if Iterable but not a Compound and not a ShapeList
         elif (
             isinstance(cad_obj, Iterable)
             and not hasattr(cad_obj, "wrapped")
             and not hasattr(cad_obj, "first")
             and not hasattr(cad_obj, "last")
         ):
             _debug(
                 "to_assembly: iterables other then Compounds and ShapeLists", obj_name
             )
 
+            pg2 = OCP_PartGroup([], name="List" if obj_name is None else obj_name)
             for child in cad_obj:
                 part, instances = _to_assembly(
                     child,
                     default_color=default_color,
                     names=None,
                     colors=[obj_color],
                     alphas=[obj_alpha],
                     render_mates=render_mates,
                     render_joints=render_joints,
-                    mate_scale=mate_scale,
+                    helper_scale=helper_scale,
                     instances=instances,
                     progress=progress,
                     is_assembly=is_assembly,
                 )
                 if isinstance(part, OCP_PartGroup) and len(part.objects) == 1:
-                    pg.add(part.objects[0])
+                    pg2.add(part.objects[0])
                 else:
-                    pg.add(part)
+                    pg2.add(part)
+
+            names = make_unique([obj.name for obj in pg2.objects])
+            for name, obj in zip(names, pg2.objects):
+                obj.name = name
+            pg.add(pg2)
+
+        elif hasattr(cad_obj, "wrapped") and (
+            is_toploc_location(cad_obj.wrapped) or is_gp_plane(cad_obj.wrapped)
+        ):
+            if is_gp_plane(cad_obj.wrapped) and hasattr(cad_obj, "to_location"):
+                cad_obj = cad_obj.to_location()
+
+            coord = get_location_coord(cad_obj.wrapped)
+            obj = CoordSystem(
+                "location" if obj_name is None else obj_name,
+                coord["origin"],
+                coord["x_dir"],
+                coord["z_dir"],
+                size=helper_scale,
+            )
+            pg.add(obj)
+
+        elif hasattr(cad_obj, "wrapped") and is_gp_axis(cad_obj.wrapped):
+            coord = get_axis_coord(cad_obj.wrapped)
+            obj = CoordAxis(
+                "axis" if obj_name is None else obj_name,
+                coord["origin"],
+                coord["z_dir"],
+                size=helper_scale,
+            )
+            pg.add(obj)
 
         elif is_compound(cad_obj):
             _debug("to_assembly: compound")
 
             #
             # Iterate over Compound (includes build123d assemblies)
             #
@@ -658,15 +738,15 @@
                         child,
                         default_color=default_color,
                         names=None,
                         colors=[obj_color],
                         alphas=[obj_alpha],
                         render_mates=render_mates,
                         render_joints=render_joints,
-                        mate_scale=mate_scale,
+                        helper_scale=helper_scale,
                         instances=instances,
                         progress=progress,
                         is_assembly=is_assembly,
                     )
                     if len(part.objects) == 1:
                         if part.objects[0].loc is None:
                             part.objects[0].loc = part.loc
@@ -720,25 +800,25 @@
 
                 if (
                     render_joints
                     and hasattr(cad_obj, "joints")
                     and len(cad_obj.joints) > 0
                 ):
                     _debug("    to_assembly: joints")
-                    if obj_name is not None:
-                        pg.name = obj_name
-                    part.name = "shape"
+                    # if obj_name is not None:
+                    #     pg.name = obj_name
+                    # part.name = "shape"
                     # create a new part group for mates
                     pg2 = OCP_PartGroup(
                         [
                             conv(joint.symbol.wrapped, name)
                             for name, joint in cad_obj.joints.items()
                             if hasattr(joint, "symbol")
                         ],
-                        name="joints",
+                        name=f"{part.name}[joints]",
                         loc=identity_location(),  # mates inherit the parent location, so actually add a no-op
                     )
 
                     # add mates partgroup
                     if pg2.objects:
                         pg.add(pg2)
 
@@ -823,30 +903,30 @@
 def to_assembly(
     *cad_objs,
     names=None,
     colors=None,
     alphas=None,
     render_mates=None,
     render_joints=None,
-    mate_scale=1,
+    helper_scale=1,
     default_color=None,
     show_parent=False,
     loc=None,
     mates=None,
     instances=None,
     progress=None,
 ):
     pg, instances = _to_assembly(
         *cad_objs,
         names=names,
         colors=colors,
         alphas=alphas,
         render_mates=render_mates,
         render_joints=render_joints,
-        mate_scale=mate_scale,
+        helper_scale=helper_scale,
         default_color=default_color,
         show_parent=show_parent,
         loc=loc,
         mates=mates,
         instances=instances,
         progress=progress,
     )
```

### Comparing `ocp_tessellate-1.0.4/ocp_tessellate/defaults.py` & `ocp_tessellate-1.1.0/ocp_tessellate/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         - default_color:      Default face color (default=(232, 176, 36))
         - default_edgecolor:  Default edge color (default="#707070")
         - optimal_bb:         Use optimal bounding box (default=False)
         - render_normals:     Render vertex normals(default=False)
         - render_edges:       Render edges  (default=True)
         - render_mates:       Render mates (for MAssemblies, default=False)
         - render_joints:      Render build12d joints (default=False)
-        - mate_scale:         Scale of rendered mates (for MAssemblies, default=1)
+        - helper_scale:         Scale of rendered mates (for MAssemblies, default=1)
 
         VIEWER OPTIONS
         - control:            Use trackball controls ('trackball') or orbit controls ('orbit') (default='trackball')
         - up:                 Use z-axis ('Z') or y-axis ('Y') as up direction for the camera (or 'L' for legacy z-axis up mode)
         - axes:               Show axes (default=False)
         - axes0:              Show axes at (0,0,0) (default=False)
         - grid:               Show grid (default=[False, False, False])
@@ -124,15 +124,15 @@
             "default_opacity": 0.5,
             "optimal_bb": False,
             "render_normals": False,
             "render_edges": True,
             "render_mates": False,
             "render_joints": False,
             "parallel": False,
-            "mate_scale": 1,
+            "helper_scale": 1,
             #
             # viewer options
             #
             "control": "trackball",
             "up": "Z",
             "axes": False,
             "axes0": False,
@@ -281,15 +281,15 @@
             "default_color",
             "default_edgecolor",
             "optimal_bb",
             "render_normals",
             "render_edges",
             "render_mates",
             "render_joints",
-            "mate_scale",
+            "helper_scale",
             "quality",
             "parallel",
         ]
     }
 
 
 def show_args(config):
```

### Comparing `ocp_tessellate-1.0.4/ocp_tessellate/mp_tess.py` & `ocp_tessellate-1.1.0/ocp_tessellate/mp_tess.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.4/ocp_tessellate/mp_tessellator.py` & `ocp_tessellate-1.1.0/ocp_tessellate/mp_tessellator.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.4/ocp_tessellate/ocp_utils.py` & `ocp_tessellate-1.1.0/ocp_tessellate/ocp_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,26 @@
     BRepBuilderAPI_MakeVertex,
 )
 from OCP.BRepGProp import BRepGProp
 from OCP.BRepMesh import BRepMesh_IncrementalMesh
 from OCP.BRepTools import BRepTools
 from OCP.GCPnts import GCPnts_AbscissaPoint
 from OCP.GeomAbs import GeomAbs_CurveType
-from OCP.gp import gp_Pnt, gp_Quaternion, gp_Trsf, gp_Vec
+from OCP.gp import (
+    gp_Pnt,
+    gp_Quaternion,
+    gp_Trsf,
+    gp_Vec,
+    gp_Ax1,
+    gp_Ax2,
+    gp_Ax3,
+    gp_Dir,
+    gp_Pln,
+    gp_Circ,
+)
 from OCP.GProp import GProp_GProps
 from OCP.Quantity import Quantity_ColorRGBA
 from OCP.StlAPI import StlAPI_Writer
 from OCP.TopAbs import (
     TopAbs_COMPOUND,
     TopAbs_COMPSOLID,
     TopAbs_EDGE,
@@ -155,15 +166,15 @@
 
 
 def is_wrapped(obj):
     return hasattr(obj, "wrapped")
 
 
 def is_build123d(obj):
-    return _has(obj, ["_obj", "_obj_name"])
+    return _has(obj, ["_obj", "_obj_name"]) and not isinstance(obj, type)
 
 
 def is_build123d_shape(obj):
     return _has(obj, ["wrapped", "children"])
 
 
 def is_build123d_shell(obj):
@@ -536,14 +547,28 @@
 # Check TopLoc_Location
 
 
 def is_toploc_location(obj):
     return isinstance(obj, TopLoc_Location)
 
 
+# Check gp_Pln
+
+
+def is_gp_plane(obj):
+    return isinstance(obj, gp_Pln)
+
+
+# Check gp_Ax1
+
+
+def is_gp_axis(obj):
+    return isinstance(obj, gp_Ax1)
+
+
 # Check TopoDS shapes
 
 
 def is_topods_shape(topods_shape):
     return isinstance(topods_shape, TopoDS_Shape)
 
 
@@ -714,23 +739,81 @@
         x, y, z = obj.X(), obj.Y(), obj.Z()
     else:
         x, y, z = obj
 
     return downcast(BRepBuilderAPI_MakeVertex(gp_Pnt(x, y, z)).Vertex())
 
 
+def vector(xyz):
+    return gp_Vec(*xyz)
+
+
 def line(start, end):
-    return downcast(BRepBuilderAPI_MakeEdge(gp_Pnt(*start), gp_Pnt(*end)).Edge())
+    if isinstance(start, (list, tuple)):
+        start = gp_Pnt(*start)
+    if isinstance(end, (list, tuple)):
+        end = gp_Pnt(*end)
+    return downcast(
+        BRepBuilderAPI_MakeEdge(gp_Pnt(*start.Coord()), gp_Pnt(*end.Coord())).Edge()
+    )
+
+
+def circle(origin, z_dir, radius):
+    ax = gp_Ax2(gp_Pnt(*origin), gp_Dir(*z_dir))
+    circle_gp = gp_Circ(ax, radius)
+    return BRepBuilderAPI_MakeEdge(circle_gp).Edge()
+
+
+def axis_to_vecs(origin, z_dir):
+    ax3 = gp_Ax3(gp_Pnt(*origin), gp_Dir(*z_dir))
+    o = gp_Vec(ax3.Location().XYZ())
+    x = gp_Vec(ax3.XDirection().XYZ())
+    y = gp_Vec(ax3.YDirection().XYZ())
+    z = gp_Vec(ax3.Direction().XYZ())
+    return (o, x, y, z)
+
+
+def loc_to_vecs(origin, x_dir, z_dir):
+    ax3 = gp_Ax3(gp_Pnt(*origin), gp_Dir(*z_dir), gp_Dir(*x_dir))
+    o = gp_Vec(ax3.Location().XYZ())
+    x = gp_Vec(ax3.XDirection().XYZ())
+    y = gp_Vec(ax3.YDirection().XYZ())
+    z = gp_Vec(ax3.Direction().XYZ())
+    return (o, x, y, z)
+
+
+def is_same_plane(plane1, plane2):
+    coordSystem1 = plane1.Position()
+    coordSystem2 = plane2.Position()
+
+    return (
+        coordSystem1.Location().IsEqual(coordSystem2.Location(), 1e-6)
+        and coordSystem1.XDirection().IsEqual(coordSystem2.XDirection(), 1e-6)
+        and coordSystem1.YDirection().IsEqual(coordSystem2.YDirection(), 1e-6)
+        and coordSystem1.Direction().IsEqual(coordSystem2.Direction(), 1e-6)
+    )
+
+
+def is_plane_xy(plane):
+    return is_same_plane(
+        plane, gp_Pln(gp_Ax3(gp_Pnt(0, 0, 0), gp_Dir(0, 0, 1), gp_Dir(1, 0, 0)))
+    )
+
+
+def normalized(v):
+    if not isinstance(v, gp_Vec):
+        v = gp_Vec(*v)
+    return v.Normalized()
 
 
 def cross(v1, v2):
-    x = gp_Vec(*v1).Normalized()
-    z = gp_Vec(*v2).Normalized()
+    x = normalized(v1)
+    z = normalized(v2)
     y = x.Crossed(z).Normalized()
-    return (y.X(), y.Y(), y.Z())
+    return y.Coord()
 
 
 def tq_to_loc(t, q):
     T = gp_Trsf()
     Q = gp_Quaternion(*q)
     V = gp_Vec(*t)
     T.SetTransformation(Q, V)
@@ -777,14 +860,39 @@
         return loc.wrapped
     elif isinstance(loc, TopLoc_Location):
         return loc
     else:
         raise TypeError(f"Unknown location typ {type(loc)}")
 
 
+def get_axis_coord(axis):
+    return {
+        "origin": axis.Location().Coord(),
+        "z_dir": axis.Direction().Coord(),
+    }
+
+
+def get_location_coord(loc):
+    trsf = loc.Transformation()
+
+    origin = trsf.TranslationPart()
+    q = trsf.GetRotation()
+
+    x_dir = q * gp_Vec(1, 0, 0)
+    y_dir = q * gp_Vec(0, 1, 0)
+    z_dir = q * gp_Vec(0, 0, 1)
+
+    return {
+        "origin": origin.Coord(),
+        "x_dir": x_dir.Coord(),
+        "y_dir": y_dir.Coord(),
+        "z_dir": z_dir.Coord(),
+    }
+
+
 def copy_shape(obj):
     cls = obj.__class__
     result = cls.__new__(cls)
     result.wrapped = downcast(BRepBuilderAPI_Copy(obj.wrapped).Shape())
     result.wrapped.TShape(obj.wrapped.TShape())
     return result
```

### Comparing `ocp_tessellate-1.0.4/ocp_tessellate/stepreader.py` & `ocp_tessellate-1.1.0/ocp_tessellate/stepreader.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.4/ocp_tessellate/tessellator.py` & `ocp_tessellate-1.1.0/ocp_tessellate/tessellator.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.4/ocp_tessellate/utils.py` & `ocp_tessellate-1.1.0/ocp_tessellate/utils.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.4/ocp_tessellate.egg-info/PKG-INFO` & `ocp_tessellate-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
-Name: ocp-tessellate
-Version: 1.0.4
+Name: ocp_tessellate
+Version: 1.1.0
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
+License: UNKNOWN
 Keywords: CAD,cadquery
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Provides-Extra: dev
 
 Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs
+
```

### Comparing `ocp_tessellate-1.0.4/ocp_tessellate.egg-info/SOURCES.txt` & `ocp_tessellate-1.1.0/ocp_tessellate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.4/setup.cfg` & `ocp_tessellate-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.4
+current_version = 1.1.0
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_tessellate-1.0.4/setup.py` & `ocp_tessellate-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 LONG_DESCRIPTION = (
     "Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs"
 )
 
 setup_args = {
     "name": "ocp_tessellate",
-    "version": "1.0.4",
+    "version": "1.1.0",
     "description": "Tessellate OCP objects",
     "long_description": LONG_DESCRIPTION,
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
         "webcolors~=1.12",
         "numpy",
```

