# Comparing `tmp/deqr-0.2.1.tar.gz` & `tmp/deqr-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deqr-0.2.1.tar", max compression
+gzip compressed data, was "deqr-0.2.2.tar", max compression
```

## Comparing `deqr-0.2.1.tar` & `deqr-0.2.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0      722 2022-01-21 08:15:45.243004 deqr-0.2.1/LICENSE.isc
--rw-r--r--   0        0        0    26433 2022-01-21 08:15:45.243004 deqr-0.2.1/LICENSE.lgpl
--rw-r--r--   0        0        0      287 2022-01-21 08:15:45.243004 deqr-0.2.1/README.md
--rw-r--r--   0        0        0     1669 2022-01-21 08:15:45.243004 deqr-0.2.1/build.py
--rw-r--r--   0        0        0     5054 2022-01-21 08:15:46.483037 deqr-0.2.1/deps/qrdec/src/bch15_5.c
--rw-r--r--   0        0        0      864 2022-01-21 08:15:46.487037 deqr-0.2.1/deps/qrdec/src/bch15_5.h
--rw-r--r--   0        0        0    19246 2022-01-21 08:15:46.487037 deqr-0.2.1/deps/qrdec/src/binarize.c
--rw-r--r--   0        0        0      627 2022-01-21 08:15:46.487037 deqr-0.2.1/deps/qrdec/src/binarize.h
--rw-r--r--   0        0        0     4411 2022-01-21 08:15:46.487037 deqr-0.2.1/deps/qrdec/src/image.c
--rw-r--r--   0        0        0      555 2022-01-21 08:15:46.487037 deqr-0.2.1/deps/qrdec/src/image.h
--rw-r--r--   0        0        0     3807 2022-01-21 08:15:46.487037 deqr-0.2.1/deps/qrdec/src/isaac.c
--rw-r--r--   0        0        0     1096 2022-01-21 08:15:46.487037 deqr-0.2.1/deps/qrdec/src/isaac.h
--rw-r--r--   0        0        0     6739 2022-01-21 08:15:46.487037 deqr-0.2.1/deps/qrdec/src/qrcode.h
--rw-r--r--   0        0        0   142003 2022-01-21 08:15:46.487037 deqr-0.2.1/deps/qrdec/src/qrdec.c
--rw-r--r--   0        0        0    14083 2022-01-21 08:15:46.487037 deqr-0.2.1/deps/qrdec/src/qrdectxt.c
--rw-r--r--   0        0        0     4215 2022-01-21 08:15:46.487037 deqr-0.2.1/deps/qrdec/src/reader.c
--rw-r--r--   0        0        0    26337 2022-01-21 08:15:46.487037 deqr-0.2.1/deps/qrdec/src/rs.c
--rw-r--r--   0        0        0     2650 2022-01-21 08:15:46.487037 deqr-0.2.1/deps/qrdec/src/rs.h
--rw-r--r--   0        0        0     3320 2022-01-21 08:15:46.487037 deqr-0.2.1/deps/qrdec/src/util.c
--rw-r--r--   0        0        0     2240 2022-01-21 08:15:46.487037 deqr-0.2.1/deps/qrdec/src/util.h
--rw-r--r--   0        0        0    21432 2022-01-21 08:15:47.419072 deqr-0.2.1/deps/quirc/lib/decode.c
--rw-r--r--   0        0        0    27610 2022-01-21 08:15:47.419072 deqr-0.2.1/deps/quirc/lib/identify.c
--rw-r--r--   0        0        0     4510 2022-01-21 08:15:47.419072 deqr-0.2.1/deps/quirc/lib/quirc.c
--rw-r--r--   0        0        0     5402 2022-01-21 08:15:47.419072 deqr-0.2.1/deps/quirc/lib/quirc.h
--rw-r--r--   0        0        0     3114 2022-01-21 08:15:47.419072 deqr-0.2.1/deps/quirc/lib/quirc_internal.h
--rw-r--r--   0        0        0    11779 2022-01-21 08:15:47.419072 deqr-0.2.1/deps/quirc/lib/version_db.c
--rw-r--r--   0        0        0      431 2022-01-21 08:16:18.539458 deqr-0.2.1/deqr/__init__.py
--rw-r--r--   0        0        0      891 2022-01-21 08:15:45.243004 deqr-0.2.1/deqr/binarize.pxd
--rw-r--r--   0        0        0     1458 2022-01-21 08:15:45.243004 deqr-0.2.1/deqr/binarize.pyx
--rw-r--r--   0        0        0     5050 2022-01-21 08:15:45.243004 deqr-0.2.1/deqr/datatypes.py
--rw-r--r--   0        0        0     4006 2022-01-21 08:15:45.243004 deqr-0.2.1/deqr/image.py
--rw-r--r--   0        0        0     7261 2022-01-21 08:15:45.243004 deqr-0.2.1/deqr/qrdec.pyx
--rw-r--r--   0        0        0     3370 2022-01-21 08:15:45.243004 deqr-0.2.1/deqr/qrdecdecl.pxd
--rw-r--r--   0        0        0     7746 2022-01-21 08:15:45.243004 deqr-0.2.1/deqr/quirc.pyx
--rw-r--r--   0        0        0     3275 2022-01-21 08:15:45.243004 deqr-0.2.1/deqr/quircdecl.pxd
--rw-r--r--   0        0        0     1177 2022-01-21 08:16:18.539458 deqr-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      884 2022-01-21 08:16:18.657196 deqr-0.2.1/setup.py
--rw-r--r--   0        0        0      924 2022-01-21 08:16:18.657455 deqr-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3022 2023-06-17 21:13:17.873533 deqr-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0      722 2023-06-17 21:13:17.873533 deqr-0.2.2/LICENSE.isc
+-rw-r--r--   0        0        0    26433 2023-06-17 21:13:17.873533 deqr-0.2.2/LICENSE.lgpl
+-rw-r--r--   0        0        0      287 2023-06-17 21:13:17.873533 deqr-0.2.2/README.md
+-rw-r--r--   0        0        0     1669 2023-06-17 21:13:17.873533 deqr-0.2.2/build.py
+-rw-r--r--   0        0        0     5054 2023-06-17 21:13:19.229541 deqr-0.2.2/deps/qrdec/src/bch15_5.c
+-rw-r--r--   0        0        0      864 2023-06-17 21:13:19.229541 deqr-0.2.2/deps/qrdec/src/bch15_5.h
+-rw-r--r--   0        0        0    19246 2023-06-17 21:13:19.229541 deqr-0.2.2/deps/qrdec/src/binarize.c
+-rw-r--r--   0        0        0      627 2023-06-17 21:13:19.229541 deqr-0.2.2/deps/qrdec/src/binarize.h
+-rw-r--r--   0        0        0     4411 2023-06-17 21:13:19.229541 deqr-0.2.2/deps/qrdec/src/image.c
+-rw-r--r--   0        0        0      555 2023-06-17 21:13:19.229541 deqr-0.2.2/deps/qrdec/src/image.h
+-rw-r--r--   0        0        0     3807 2023-06-17 21:13:19.229541 deqr-0.2.2/deps/qrdec/src/isaac.c
+-rw-r--r--   0        0        0     1096 2023-06-17 21:13:19.229541 deqr-0.2.2/deps/qrdec/src/isaac.h
+-rw-r--r--   0        0        0     6739 2023-06-17 21:13:19.229541 deqr-0.2.2/deps/qrdec/src/qrcode.h
+-rw-r--r--   0        0        0   142003 2023-06-17 21:13:19.233541 deqr-0.2.2/deps/qrdec/src/qrdec.c
+-rw-r--r--   0        0        0    14083 2023-06-17 21:13:19.233541 deqr-0.2.2/deps/qrdec/src/qrdectxt.c
+-rw-r--r--   0        0        0     4215 2023-06-17 21:13:19.233541 deqr-0.2.2/deps/qrdec/src/reader.c
+-rw-r--r--   0        0        0    26337 2023-06-17 21:13:19.233541 deqr-0.2.2/deps/qrdec/src/rs.c
+-rw-r--r--   0        0        0     2650 2023-06-17 21:13:19.233541 deqr-0.2.2/deps/qrdec/src/rs.h
+-rw-r--r--   0        0        0     3320 2023-06-17 21:13:19.233541 deqr-0.2.2/deps/qrdec/src/util.c
+-rw-r--r--   0        0        0     2240 2023-06-17 21:13:19.233541 deqr-0.2.2/deps/qrdec/src/util.h
+-rw-r--r--   0        0        0    21512 2023-06-17 21:13:19.249541 deqr-0.2.2/deps/quirc/lib/decode.c
+-rw-r--r--   0        0        0    28248 2023-06-17 21:13:19.249541 deqr-0.2.2/deps/quirc/lib/identify.c
+-rw-r--r--   0        0        0     4510 2023-06-17 21:13:19.249541 deqr-0.2.2/deps/quirc/lib/quirc.c
+-rw-r--r--   0        0        0     5402 2023-06-17 21:13:19.249541 deqr-0.2.2/deps/quirc/lib/quirc.h
+-rw-r--r--   0        0        0     3720 2023-06-17 21:13:19.249541 deqr-0.2.2/deps/quirc/lib/quirc_internal.h
+-rw-r--r--   0        0        0    11779 2023-06-17 21:13:19.249541 deqr-0.2.2/deps/quirc/lib/version_db.c
+-rw-r--r--   0        0        0      210 2023-06-17 21:13:17.873533 deqr-0.2.2/deqr/__init__.py
+-rw-r--r--   0        0        0      891 2023-06-17 21:13:17.873533 deqr-0.2.2/deqr/binarize.pxd
+-rw-r--r--   0        0        0     1458 2023-06-17 21:13:17.873533 deqr-0.2.2/deqr/binarize.pyx
+-rw-r--r--   0        0        0     5050 2023-06-17 21:13:17.873533 deqr-0.2.2/deqr/datatypes.py
+-rw-r--r--   0        0        0     4006 2023-06-17 21:13:17.873533 deqr-0.2.2/deqr/image.py
+-rw-r--r--   0        0        0     7261 2023-06-17 21:13:17.873533 deqr-0.2.2/deqr/qrdec.pyx
+-rw-r--r--   0        0        0     3370 2023-06-17 21:13:17.873533 deqr-0.2.2/deqr/qrdecdecl.pxd
+-rw-r--r--   0        0        0     7746 2023-06-17 21:13:17.873533 deqr-0.2.2/deqr/quirc.pyx
+-rw-r--r--   0        0        0     3275 2023-06-17 21:13:17.873533 deqr-0.2.2/deqr/quircdecl.pxd
+-rw-r--r--   0        0        0      972 2023-06-17 21:13:17.873533 deqr-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3986 1970-01-01 00:00:00.000000 deqr-0.2.2/setup.py
+-rw-r--r--   0        0        0     3998 1970-01-01 00:00:00.000000 deqr-0.2.2/PKG-INFO
```

### Comparing `deqr-0.2.1/LICENSE.isc` & `deqr-0.2.2/LICENSE.isc`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/LICENSE.lgpl` & `deqr-0.2.2/LICENSE.lgpl`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/build.py` & `deqr-0.2.2/build.py`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/qrdec/src/bch15_5.c` & `deqr-0.2.2/deps/qrdec/src/bch15_5.c`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/qrdec/src/bch15_5.h` & `deqr-0.2.2/deps/qrdec/src/bch15_5.h`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/qrdec/src/binarize.c` & `deqr-0.2.2/deps/qrdec/src/binarize.c`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/qrdec/src/binarize.h` & `deqr-0.2.2/deps/qrdec/src/binarize.h`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/qrdec/src/image.c` & `deqr-0.2.2/deps/qrdec/src/image.c`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/qrdec/src/image.h` & `deqr-0.2.2/deps/qrdec/src/image.h`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/qrdec/src/isaac.c` & `deqr-0.2.2/deps/qrdec/src/isaac.c`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/qrdec/src/isaac.h` & `deqr-0.2.2/deps/qrdec/src/isaac.h`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/qrdec/src/qrcode.h` & `deqr-0.2.2/deps/qrdec/src/qrcode.h`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/qrdec/src/qrdec.c` & `deqr-0.2.2/deps/qrdec/src/qrdec.c`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/qrdec/src/qrdectxt.c` & `deqr-0.2.2/deps/qrdec/src/qrdectxt.c`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/qrdec/src/reader.c` & `deqr-0.2.2/deps/qrdec/src/reader.c`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/qrdec/src/rs.c` & `deqr-0.2.2/deps/qrdec/src/rs.c`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/qrdec/src/rs.h` & `deqr-0.2.2/deps/qrdec/src/rs.h`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/qrdec/src/util.c` & `deqr-0.2.2/deps/qrdec/src/util.c`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/qrdec/src/util.h` & `deqr-0.2.2/deps/qrdec/src/util.h`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/quirc/lib/decode.c` & `deqr-0.2.2/deps/quirc/lib/decode.c`

 * *Files 1% similar despite different names*

```diff
@@ -882,14 +882,17 @@
 
 quirc_decode_error_t quirc_decode(const struct quirc_code *code,
 				  struct quirc_data *data)
 {
 	quirc_decode_error_t err;
 	struct datastream ds;
 
+	if (code->size > QUIRC_MAX_GRID_SIZE)
+		return QUIRC_ERROR_INVALID_GRID_SIZE;
+
 	if ((code->size - 17) % 4)
 		return QUIRC_ERROR_INVALID_GRID_SIZE;
 
 	memset(data, 0, sizeof(*data));
 	memset(&ds, 0, sizeof(ds));
 
 	data->version = (code->size - 17) / 4;
```

### Comparing `deqr-0.2.1/deps/quirc/lib/identify.c` & `deqr-0.2.2/deps/quirc/lib/identify.c`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,19 @@
  * OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
  */
 
 #include <limits.h>
 #include <string.h>
 #include <stdbool.h>
 #include <stdlib.h>
+#ifdef QUIRC_USE_TGMATH
+#include <tgmath.h>
+#else
 #include <math.h>
+#endif // QUIRC_USE_TGMATH
 #include "quirc_internal.h"
 
 /************************************************************************
  * Linear algebra routines
  */
 
 static int line_intersect(const struct quirc_point *p0,
@@ -58,29 +62,29 @@
 
 	r->x = (d * e - b * f) / det;
 	r->y = (-c * e + a * f) / det;
 
 	return 1;
 }
 
-static void perspective_setup(double *c,
+static void perspective_setup(quirc_float_t *c,
 			      const struct quirc_point *rect,
-			      double w, double h)
+			      quirc_float_t w, quirc_float_t h)
 {
-	double x0 = rect[0].x;
-	double y0 = rect[0].y;
-	double x1 = rect[1].x;
-	double y1 = rect[1].y;
-	double x2 = rect[2].x;
-	double y2 = rect[2].y;
-	double x3 = rect[3].x;
-	double y3 = rect[3].y;
+	quirc_float_t x0 = rect[0].x;
+	quirc_float_t y0 = rect[0].y;
+	quirc_float_t x1 = rect[1].x;
+	quirc_float_t y1 = rect[1].y;
+	quirc_float_t x2 = rect[2].x;
+	quirc_float_t y2 = rect[2].y;
+	quirc_float_t x3 = rect[3].x;
+	quirc_float_t y3 = rect[3].y;
 
-	double wden = w * (x2*y3 - x3*y2 + (x3-x2)*y1 + x1*(y2-y3));
-	double hden = h * (x2*y3 + x1*(y2-y3) - x3*y2 + (x3-x2)*y1);
+	quirc_float_t wden = w * (x2*y3 - x3*y2 + (x3-x2)*y1 + x1*(y2-y3));
+	quirc_float_t hden = h * (x2*y3 + x1*(y2-y3) - x3*y2 + (x3-x2)*y1);
 
 	c[0] = (x1*(x2*y3-x3*y2) + x0*(-x2*y3+x3*y2+(x2-x3)*y1) +
 		x1*(x3-x2)*y0) / wden;
 	c[1] = -(x0*(x2*y3+x1*(y2-y3)-x2*y1) - x1*x3*y2 + x2*x3*y1
 		 + (x1*x3-x2*x3)*y0) / hden;
 	c[2] = x0;
 	c[3] = (y0*(x1*(y3-y2)-x2*y3+x3*y2) + y1*(x2*y3-x3*y2) +
@@ -89,32 +93,32 @@
 		y0*(x3*y2-x1*y2+(x2-x3)*y1)) / hden;
 	c[5] = y0;
 	c[6] = (x1*(y3-y2) + x0*(y2-y3) + (x2-x3)*y1 + (x3-x2)*y0) / wden;
 	c[7] = (-x2*y3 + x1*y3 + x3*y2 + x0*(y1-y2) - x3*y1 + (x2-x1)*y0) /
 		hden;
 }
 
-static void perspective_map(const double *c,
-			    double u, double v, struct quirc_point *ret)
+static void perspective_map(const quirc_float_t *c,
+			    quirc_float_t u, quirc_float_t v, struct quirc_point *ret)
 {
-	double den = c[6]*u + c[7]*v + 1.0;
-	double x = (c[0]*u + c[1]*v + c[2]) / den;
-	double y = (c[3]*u + c[4]*v + c[5]) / den;
+	quirc_float_t den = c[6]*u + c[7]*v + 1.0;
+	quirc_float_t x = (c[0]*u + c[1]*v + c[2]) / den;
+	quirc_float_t y = (c[3]*u + c[4]*v + c[5]) / den;
 
 	ret->x = (int) rint(x);
 	ret->y = (int) rint(y);
 }
 
-static void perspective_unmap(const double *c,
+static void perspective_unmap(const quirc_float_t *c,
 			      const struct quirc_point *in,
-			      double *u, double *v)
+			      quirc_float_t *u, quirc_float_t *v)
 {
-	double x = in->x;
-	double y = in->y;
-	double den = -c[0]*c[7]*y + c[1]*c[6]*y + (c[3]*c[7]-c[4]*c[6])*x +
+	quirc_float_t x = in->x;
+	quirc_float_t y = in->y;
+	quirc_float_t den = -c[0]*c[7]*y + c[1]*c[6]*y + (c[3]*c[7]-c[4]*c[6])*x +
 		c[0]*c[4] - c[1]*c[3];
 
 	*u = -(c[1]*(y-c[5]) - c[2]*c[7]*y + (c[5]*c[7]-c[4])*x + c[2]*c[4]) /
 		den;
 	*v = (c[0]*(y-c[5]) - c[2]*c[6]*y + (c[5]*c[6]-c[3])*x + c[2]*c[3]) /
 		den;
 }
@@ -295,41 +299,41 @@
 	unsigned int length = numPixels;
 	while (length--) {
 		uint8_t value = *ptr++;
 		histogram[value]++;
 	}
 
 	// Calculate weighted sum of histogram values
-	double sum = 0;
+	quirc_float_t sum = 0;
 	unsigned int i = 0;
 	for (i = 0; i <= UINT8_MAX; ++i) {
 		sum += i * histogram[i];
 	}
 
 	// Compute threshold
-	double sumB = 0;
+	quirc_float_t sumB = 0;
 	unsigned int q1 = 0;
-	double max = 0;
+	quirc_float_t max = 0;
 	uint8_t threshold = 0;
 	for (i = 0; i <= UINT8_MAX; ++i) {
 		// Weighted background
 		q1 += histogram[i];
 		if (q1 == 0)
 			continue;
 
 		// Weighted foreground
 		const unsigned int q2 = numPixels - q1;
 		if (q2 == 0)
 			break;
 
 		sumB += i * histogram[i];
-		const double m1 = sumB / q1;
-		const double m2 = (sum - sumB) / q2;
-		const double m1m2 = m1 - m2;
-		const double variance = m1m2 * m1m2 * q1 * q2;
+		const quirc_float_t m1 = sumB / q1;
+		const quirc_float_t m2 = (sum - sumB) / q2;
+		const quirc_float_t m1m2 = m1 - m2;
+		const quirc_float_t variance = m1m2 * m1m2 * q1 * q2;
 		if (variance >= max) {
 			threshold = i;
 			max = variance;
 		}
 	}
 
 	return threshold;
@@ -578,15 +582,15 @@
 	struct quirc_capstone *c2 = &q->capstones[qr->caps[2]];
 	struct quirc_point a;
 	struct quirc_point b;
 	struct quirc_point c;
 	int size_estimate;
 	int step_size = 1;
 	int dir = 0;
-	double u, v;
+	quirc_float_t u, v;
 
 	/* Grab our previous estimate of the alignment pattern corner */
 	memcpy(&b, &qr->align, sizeof(b));
 
 	/* Guess another two corners of the alignment pattern so that we
 	 * can estimate its size.
 	 */
@@ -644,39 +648,43 @@
 			psd->scores[0] = d;
 			psd->corners[0].x = xs[i];
 			psd->corners[0].y = y;
 		}
 	}
 }
 
-static double distance(struct quirc_point a, struct quirc_point b)
+static quirc_float_t length(struct quirc_point a, struct quirc_point b)
 {
-	return sqrt((a.x - b.x)*(a.x - b.x) +  (a.y - b.y)*(a.y - b.y));
+	quirc_float_t x = abs(a.x - b.x) + 1;
+	quirc_float_t y = abs(a.y - b.y) + 1;
+	return sqrt(x * x +  y * y);
 }
 /* Estimate grid size by determing distance between capstones
  */
 static void measure_grid_size(struct quirc *q, int index)
 {
 	struct quirc_grid *qr = &q->grids[index];
 
 	struct quirc_capstone *a = &(q->capstones[qr->caps[0]]);
 	struct quirc_capstone *b = &(q->capstones[qr->caps[1]]);
 	struct quirc_capstone *c = &(q->capstones[qr->caps[2]]);
 
-	double ab = distance(b->corners[0], a->corners[3]);
-	double capstone_ab_size = (distance(b->corners[0], b->corners[3]) + distance(a->corners[0], a->corners[3]))/2.0;
-	double ver_grid = 7.0 * ab / capstone_ab_size;
-
-	double bc = distance(b->corners[0], c->corners[1]);
-	double capstone_bc_size = (distance(b->corners[0], b->corners[1]) + distance(c->corners[0], c->corners[1]))/2.0;
-	double hor_grid = 7.0 * bc / capstone_bc_size;
+	quirc_float_t ab = length(b->corners[0], a->corners[3]);
+	quirc_float_t capstone_ab_size = (length(b->corners[0], b->corners[3]) + length(a->corners[0], a->corners[3]))/2.0;
+	quirc_float_t ver_grid = 7.0 * ab / capstone_ab_size;
+
+	quirc_float_t bc = length(b->corners[0], c->corners[1]);
+	quirc_float_t capstone_bc_size = (length(b->corners[0], b->corners[1]) + length(c->corners[0], c->corners[1]))/2.0;
+	quirc_float_t hor_grid = 7.0 * bc / capstone_bc_size;
 	
-	double grid_size_estimate = (ver_grid + hor_grid) / 2;
+	quirc_float_t grid_size_estimate = (ver_grid + hor_grid) / 2;
+
+	int ver = (int)((grid_size_estimate - 17.0 + 2.0) / 4.0);
 	
-	qr->grid_size =  4*((int)(grid_size_estimate - 17.0 + 2.0) / 4) + 17;
+	qr->grid_size =  4*ver + 17;
 }
 
 /* Read a cell from a grid using the currently set perspective
  * transform. Returns +/- 1 for black/white, 0 for cells which are
  * out of image bounds.
  */
 static int read_cell(const struct quirc *q, int index, int x, int y)
@@ -695,15 +703,15 @@
 {
 	const struct quirc_grid *qr = &q->grids[index];
 	int score = 0;
 	int u, v;
 
 	for (v = 0; v < 3; v++)
 		for (u = 0; u < 3; u++) {
-			static const double offsets[] = {0.3, 0.5, 0.7};
+			static const quirc_float_t offsets[] = {0.3, 0.5, 0.7};
 			struct quirc_point p;
 
 			perspective_map(qr->c, x + offsets[u],
 					       y + offsets[v], &p);
 			if (p.y < 0 || p.y >= q->h || p.x < 0 || p.x >= q->w)
 				continue;
 
@@ -798,27 +806,27 @@
 }
 
 static void jiggle_perspective(struct quirc *q, int index)
 {
 	struct quirc_grid *qr = &q->grids[index];
 	int best = fitness_all(q, index);
 	int pass;
-	double adjustments[8];
+	quirc_float_t adjustments[8];
 	int i;
 
 	for (i = 0; i < 8; i++)
 		adjustments[i] = qr->c[i] * 0.02;
 
 	for (pass = 0; pass < 5; pass++) {
 		for (i = 0; i < 16; i++) {
 			int j = i >> 1;
 			int test;
-			double old = qr->c[j];
-			double step = adjustments[j];
-			double new;
+			quirc_float_t old = qr->c[j];
+			quirc_float_t step = adjustments[j];
+			quirc_float_t new;
 
 			if (i & 1)
 				new = old + step;
 			else
 				new = old - step;
 
 			qr->c[j] = new;
@@ -990,15 +998,15 @@
 	for (i = 0; i < 3; i++)
 		q->capstones[qr->caps[i]].qr_grid = -1;
 	q->num_grids--;
 }
 
 struct neighbour {
 	int		index;
-	double		distance;
+	quirc_float_t		distance;
 };
 
 struct neighbour_list {
 	struct neighbour	n[QUIRC_MAX_CAPSTONES];
 	int			count;
 };
 
@@ -1007,15 +1015,15 @@
 			    const struct neighbour_list *vlist)
 {
 	/* Test each possible grouping */
 	for (int j = 0; j < hlist->count; j++) {
 		const struct neighbour *hn = &hlist->n[j];
 		for (int k = 0; k < vlist->count; k++) {
 			const struct neighbour *vn = &vlist->n[k];
-			double squareness = fabs(1.0 - hn->distance / vn->distance);
+			quirc_float_t squareness = fabs(1.0 - hn->distance / vn->distance);
 			if (squareness < 0.2)
 				record_qr_grid(q, hn->index, i, vn->index);
 		}
 	}
 }
 
 static void test_grouping(struct quirc *q, unsigned int i)
@@ -1029,15 +1037,15 @@
 	vlist.count = 0;
 
 	/* Look for potential neighbours by examining the relative gradients
 	 * from this capstone to others.
 	 */
 	for (j = 0; j < q->num_capstones; j++) {
 		struct quirc_capstone *c2 = &q->capstones[j];
-		double u, v;
+		quirc_float_t u, v;
 
 		if (i == j)
 			continue;
 
 		perspective_unmap(c1->c, &c2->center, &u, &v);
 
 		u = fabs(u - 3.5);
@@ -1110,27 +1118,33 @@
 void quirc_extract(const struct quirc *q, int index,
 		   struct quirc_code *code)
 {
 	const struct quirc_grid *qr = &q->grids[index];
 	int y;
 	int i = 0;
 
+	memset(code, 0, sizeof(*code));
+
 	if (index < 0 || index > q->num_grids)
 		return;
 
-	memset(code, 0, sizeof(*code));
-
 	perspective_map(qr->c, 0.0, 0.0, &code->corners[0]);
 	perspective_map(qr->c, qr->grid_size, 0.0, &code->corners[1]);
 	perspective_map(qr->c, qr->grid_size, qr->grid_size,
 			&code->corners[2]);
 	perspective_map(qr->c, 0.0, qr->grid_size, &code->corners[3]);
 
 	code->size = qr->grid_size;
 
+	/* Skip out early so as not to overrun the buffer. quirc_decode
+	 * will return an error on interpreting the code.
+	 */
+	if (code->size > QUIRC_MAX_GRID_SIZE)
+		return;
+
 	for (y = 0; y < qr->grid_size; y++) {
 		int x;
 		for (x = 0; x < qr->grid_size; x++) {
 			if (read_cell(q, index, x, y) > 0) {
 				code->cell_bitmap[i >> 3] |= (1 << (i & 7));
 			}
 			i++;
```

### Comparing `deqr-0.2.1/deps/quirc/lib/quirc.c` & `deqr-0.2.2/deps/quirc/lib/quirc.c`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/quirc/lib/quirc.h` & `deqr-0.2.2/deps/quirc/lib/quirc.h`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deps/quirc/lib/quirc_internal.h` & `deqr-0.2.2/deps/quirc/lib/quirc_internal.h`

 * *Files 12% similar despite different names*

```diff
@@ -42,27 +42,41 @@
 #elif QUIRC_MAX_REGIONS < UINT16_MAX
 #define QUIRC_PIXEL_ALIAS_IMAGE	0
 typedef uint16_t quirc_pixel_t;
 #else
 #error "QUIRC_MAX_REGIONS > 65534 is not supported"
 #endif
 
+#ifdef QUIRC_FLOAT_TYPE
+/* Quirc uses double precision floating point internally by default.
+ * On platforms with a single precision FPU but no double precision FPU,
+ * this can be changed to float by defining QUIRC_FLOAT_TYPE.
+ *
+ * When setting QUIRC_FLOAT_TYPE to 'float', consider also defining QUIRC_USE_TGMATH.
+ * This will use the type-generic math functions (tgmath.h, C99 or later) instead of the normal ones,
+ * which will allow the compiler to use the correct overloaded functions for the type.
+ */
+typedef QUIRC_FLOAT_TYPE quirc_float_t;
+#else
+typedef double quirc_float_t;
+#endif
+
 struct quirc_region {
 	struct quirc_point	seed;
 	int			count;
 	int			capstone;
 };
 
 struct quirc_capstone {
 	int			ring;
 	int			stone;
 
 	struct quirc_point	corners[4];
 	struct quirc_point	center;
-	double			c[QUIRC_PERSPECTIVE_PARAMS];
+	quirc_float_t		c[QUIRC_PERSPECTIVE_PARAMS];
 
 	int			qr_grid;
 };
 
 struct quirc_grid {
 	/* Capstone indices */
 	int			caps[3];
@@ -72,15 +86,15 @@
 	struct quirc_point	align;
 
 	/* Timing pattern endpoints */
 	struct quirc_point	tpep[3];
 
 	/* Grid size and perspective transform */
 	int			grid_size;
-	double			c[QUIRC_PERSPECTIVE_PARAMS];
+	quirc_float_t		c[QUIRC_PERSPECTIVE_PARAMS];
 };
 
 struct quirc_flood_fill_vars {
 	int y;
 	int right;
 	int left_up;
 	int left_down;
```

### Comparing `deqr-0.2.1/deps/quirc/lib/version_db.c` & `deqr-0.2.2/deps/quirc/lib/version_db.c`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deqr/binarize.pxd` & `deqr-0.2.2/deqr/binarize.pxd`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deqr/binarize.pyx` & `deqr-0.2.2/deqr/binarize.pyx`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deqr/datatypes.py` & `deqr-0.2.2/deqr/datatypes.py`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deqr/image.py` & `deqr-0.2.2/deqr/image.py`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deqr/qrdec.pyx` & `deqr-0.2.2/deqr/qrdec.pyx`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deqr/qrdecdecl.pxd` & `deqr-0.2.2/deqr/qrdecdecl.pxd`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deqr/quirc.pyx` & `deqr-0.2.2/deqr/quirc.pyx`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/deqr/quircdecl.pxd` & `deqr-0.2.2/deqr/quircdecl.pxd`

 * *Files identical despite different names*

### Comparing `deqr-0.2.1/pyproject.toml` & `deqr-0.2.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,40 @@
 [tool.poetry]
 name = "deqr"
-version = "0.2.1"
+version = "0.2.2"
 description = "qr code decoding library"
 authors = ["torque <torque@users.noreply.github.com>"]
 license = "LGPL-2.1-or-later"
-readme = "README.md"
+readme = ["README.md", "CHANGELOG.md"]
 repository = "https://github.com/torque/deqr"
 documentation = "https://torque.github.io/deqr-docs/"
-build = "build.py"
+build = {script = "build.py", generate-setup-file = true}
 include = [
-    "deps/qrdec/src",
-    "deps/quirc/lib",
+    {path = "deps/qrdec/src", format = "sdist"},
+    {path = "deps/quirc/lib", format = "sdist"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
-Cython = {version = "3.0.0a10", allow-prereleases = true}
+Cython = {version = "3.0.0b3", allow-prereleases = true}
 
 # tests
-pytest = "^6.0.0"
+pytest = ">=7.0.0"
 Pillow = ">=8.0.0"
 numpy = ">=1.20.0"
 
 # documentation
-Sphinx = "^4.0.0"
+sphinx = "^4.0.0"
 sphinx-copybutton = "^0.4.0"
 furo = "^2022.1.2"
 sphinx-inline-tabs = ">=2022.1.2-beta.11"
 
-[tool.poetry-dynamic-versioning]
-enable = false
-vcs = "git"
-pattern = "^(?P<base>\\d+\\.\\d+\\.\\d+)"
-style = "semver"
-latest-tag = true
-
-[tool.poetry-dynamic-versioning.substitution]
-files = ["deqr/__init__.py"]
-patterns = ["(^__version__\\s+=\\s+['\"])__PLACEHOLDER__(['\"])"]
-
 [build-system]
 requires = [
-    "cython==3.0.0a10",
-    "poetry-core>=1.0.0",
-    "poetry-dynamic-versioning>=0.13.0",
+    "cython==3.0.0b3",
+    "poetry-core>=1.6.0,<1.7.0",
     "setuptools>=40.9.0",
     "wheel",
 ]
 build-backend = "poetry.core.masonry.api"
```

