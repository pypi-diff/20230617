# Comparing `tmp/json_tricks-3.7.0.tar.gz` & `tmp/json_tricks-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/json_tricks-3.7.0.tar", last modified: Thu Jan 19 14:26:22 2017, max compression
+gzip compressed data, was "dist/json_tricks-3.8.0.tar", last modified: Fri Jan 20 08:36:32 2017, max compression
```

## Comparing `json_tricks-3.7.0.tar` & `json_tricks-3.8.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2017-01-19 14:26:22.000000 json_tricks-3.7.0/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2017-01-19 14:26:22.000000 json_tricks-3.7.0/json_tricks/
--rw-rw-r--   0 mark      (1000) mark      (1000)     8333 2017-01-18 21:37:08.000000 json_tricks-3.7.0/json_tricks/nonp.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1058 2016-11-30 16:44:47.000000 json_tricks-3.7.0/json_tricks/np_utils.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4836 2017-01-18 21:38:05.000000 json_tricks-3.7.0/json_tricks/np.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      295 2016-11-30 16:33:52.000000 json_tricks-3.7.0/json_tricks/utils.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      735 2016-11-30 14:40:38.000000 json_tricks-3.7.0/json_tricks/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     6133 2017-01-18 20:59:50.000000 json_tricks-3.7.0/json_tricks/encoders.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     5688 2017-01-18 21:03:59.000000 json_tricks-3.7.0/json_tricks/decoders.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      833 2016-10-19 17:40:27.000000 json_tricks-3.7.0/json_tricks/comment.py
--rw-rw-r--   0 mark      (1000) mark      (1000)    13603 2017-01-19 14:26:22.000000 json_tricks-3.7.0/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)    10529 2017-01-18 21:31:36.000000 json_tricks-3.7.0/README.rst
--rw-rw-r--   0 mark      (1000) mark      (1000)      130 2017-01-19 14:26:22.000000 json_tricks-3.7.0/setup.cfg
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2017-01-19 14:26:22.000000 json_tricks-3.7.0/json_tricks.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)      381 2017-01-19 14:26:22.000000 json_tricks-3.7.0/json_tricks.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)    13603 2017-01-19 14:26:22.000000 json_tricks-3.7.0/json_tricks.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2017-01-19 14:26:22.000000 json_tricks-3.7.0/json_tricks.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2016-10-19 20:31:09.000000 json_tricks-3.7.0/json_tricks.egg-info/not-zip-safe
--rw-rw-r--   0 mark      (1000) mark      (1000)       12 2017-01-19 14:26:22.000000 json_tricks-3.7.0/json_tricks.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)     1394 2017-01-18 21:33:03.000000 json_tricks-3.7.0/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2017-01-20 08:36:32.000000 json_tricks-3.8.0/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2017-01-20 08:36:32.000000 json_tricks-3.8.0/json_tricks/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     8442 2017-01-19 22:08:37.000000 json_tricks-3.8.0/json_tricks/nonp.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1058 2016-11-30 16:44:47.000000 json_tricks-3.8.0/json_tricks/np_utils.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     5069 2017-01-19 22:08:37.000000 json_tricks-3.8.0/json_tricks/np.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1037 2017-01-19 20:51:07.000000 json_tricks-3.8.0/json_tricks/utils.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      735 2016-11-30 14:40:38.000000 json_tricks-3.8.0/json_tricks/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     7010 2017-01-19 22:08:37.000000 json_tricks-3.8.0/json_tricks/encoders.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     5688 2017-01-18 21:03:59.000000 json_tricks-3.8.0/json_tricks/decoders.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      833 2016-10-19 17:40:27.000000 json_tricks-3.8.0/json_tricks/comment.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)    17250 2017-01-20 08:36:32.000000 json_tricks-3.8.0/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)    13124 2017-01-19 22:11:43.000000 json_tricks-3.8.0/README.rst
+-rw-rw-r--   0 mark      (1000) mark      (1000)      130 2017-01-20 08:36:32.000000 json_tricks-3.8.0/setup.cfg
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2017-01-20 08:36:32.000000 json_tricks-3.8.0/json_tricks.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      381 2017-01-20 08:36:32.000000 json_tricks-3.8.0/json_tricks.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)    17250 2017-01-20 08:36:30.000000 json_tricks-3.8.0/json_tricks.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2017-01-20 08:36:30.000000 json_tricks-3.8.0/json_tricks.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2017-01-19 19:20:15.000000 json_tricks-3.8.0/json_tricks.egg-info/not-zip-safe
+-rw-rw-r--   0 mark      (1000) mark      (1000)       12 2017-01-20 08:36:30.000000 json_tricks-3.8.0/json_tricks.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1878 2017-01-19 22:14:25.000000 json_tricks-3.8.0/setup.py
```

### Comparing `json_tricks-3.7.0/json_tricks/nonp.py` & `json_tricks-3.8.0/json_tricks/nonp.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ENCODING = 'UTF-8'
 
 
 class NoNumpyException(Exception):
 		""" Trying to use numpy features, but numpy cannot be found. """
 
 
-def nonumpy_encode(obj):
+def nonumpy_encode(obj, primitives=False):
 	"""
 	Emits a warning for numpy arrays, no other effect.
 	"""
 	if 'ndarray' in str(type(obj)):
 		raise NoNumpyException(('Trying to encode {0:} which appears to be a numpy array ({1:}), but numpy ' +
 			'support is not enabled. Make sure that numpy is installed and that you import from json_tricks.np.')
 			.format(obj, type(obj)))
@@ -50,21 +50,21 @@
 			'support is not enabled. Make sure that numpy is installed and that you import from json_tricks.np.')
 			.format(', '.join(dct.keys()[:10])))
 	return dct
 
 
 _cih_instance = ClassInstanceHook()
 DEFAULT_ENCODERS = (json_date_time_encode, class_instance_encode, json_complex_encode, json_set_encode, numeric_types_encode,)
-DEFAULT_NONP_ENCODERS = DEFAULT_ENCODERS + (nonumpy_encode,)
+DEFAULT_NONP_ENCODERS = (nonumpy_encode,) + DEFAULT_ENCODERS
 DEFAULT_HOOKS = (json_date_time_hook, _cih_instance, json_complex_hook, json_set_hook, numeric_types_hook,)
 DEFAULT_NONP_HOOKS = (json_nonumpy_obj_hook,) + DEFAULT_HOOKS
 
 
 def dumps(obj, sort_keys=None, cls=TricksEncoder, obj_encoders=DEFAULT_NONP_ENCODERS, extra_obj_encoders=(),
-		compression=None, allow_nan=False, **jsonkwargs):
+		primitives=False, compression=None, allow_nan=False, **jsonkwargs):
 	"""
 	Convert a nested data structure to a json string.
 
 	:param obj: The Python object to convert.
 	:param sort_keys: Keep this False if you want order to be preserved.
 	:param cls: The json encoder class to use, defaults to NoNumpyEncoder which gives a warning for numpy arrays.
 	:param obj_encoders: Iterable of encoders to use to convert arbitrary objects into json-able promitives.
@@ -73,43 +73,44 @@
 	:return: The string containing the json-encoded version of obj.
 
 	Other arguments are passed on to `cls`. Note that `sort_keys` should be false if you want to preserve order.
 
 	Use `json_tricks.np.dumps` instead if you want encoding of numpy arrays.
 	"""
 	encoders = tuple(extra_obj_encoders) + tuple(obj_encoders)
-	string = cls(sort_keys=sort_keys, obj_encoders=encoders, allow_nan=allow_nan, **jsonkwargs).encode(obj)
+	string = cls(sort_keys=sort_keys, obj_encoders=encoders, allow_nan=allow_nan,
+		primitives=primitives, **jsonkwargs).encode(obj)
 	if not compression:
 		return string
 	if compression is True:
 		compression = 5
 	if is_py3:
 		string = bytes(string, encoding=ENCODING)
 	sh = BytesIO()
 	with GzipFile(mode='wb', fileobj=sh, compresslevel=compression) as zh:
 		zh.write(string)
 	gzstring = sh.getvalue()
 	return gzstring
 
 
 def dump(obj, fp, sort_keys=None, cls=TricksEncoder, obj_encoders=DEFAULT_NONP_ENCODERS, extra_obj_encoders=(),
-		compression=None, force_flush=False, allow_nan=False, **jsonkwargs):
+         primitives=False, compression=None, force_flush=False, allow_nan=False, **jsonkwargs):
 	"""
 	Convert a nested data structure to a json string.
 
 	:param fp: File handle or path to write to.
 	:param compression: The gzip compression level, or None for no compression.
 	:param force_flush: If True, flush the file handle used, when possibly also in the operating system (default False).
 	
 	The other arguments are identical to `dumps`.
 
 	Use `json_tricks.np.dump` instead if you want encoding of numpy arrays.
 	"""
 	string = dumps(obj, sort_keys=sort_keys, cls=cls, obj_encoders=obj_encoders, extra_obj_encoders=extra_obj_encoders,
-		compression=compression, allow_nan=allow_nan, **jsonkwargs)
+		primitives=primitives, compression=compression, allow_nan=allow_nan, **jsonkwargs)
 	if isinstance(fp, str_type):
 		fh = open(fp, 'wb+')
 	else:
 		fh = fp
 	try:
 		try:
 			fh.write(string)
```

### Comparing `json_tricks-3.7.0/json_tricks/np_utils.py` & `json_tricks-3.8.0/json_tricks/np_utils.py`

 * *Files identical despite different names*

### Comparing `json_tricks-3.7.0/json_tricks/np.py` & `json_tricks-3.8.0/json_tricks/np.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 
 from logging import warning
+from . import nonp
+from .nonp import NoNumpyException, DEFAULT_ENCODERS, DEFAULT_HOOKS
 from .utils import hashodict
 from .comment import strip_comment_line_with_symbol, strip_comments  # keep 'unused' imports
 from .encoders import TricksEncoder, json_date_time_encode, class_instance_encode, ClassInstanceEncoder  # keep 'unused' imports
 from .decoders import DuplicateJsonKeyException, TricksPairHook, json_date_time_hook, ClassInstanceHook, \
 	json_complex_hook, json_set_hook  # keep 'unused' imports
-from .nonp import NoNumpyException, DEFAULT_ENCODERS, _cih_instance, DEFAULT_HOOKS
-from . import nonp
 
 try:
 	from numpy import ndarray, asarray, generic
 	import numpy as nptypes
 except ImportError:
 	raise NoNumpyException('Could not load numpy, maybe it is not installed? If you do not want to use numpy encoding '
 		'or decoding, you can import the functions from json_tricks.nonp instead, which do not need numpy.')
 
 
-def numpy_encode(obj):
+def numpy_encode(obj, primitives=False):
 	"""
 	Encodes numpy `ndarray`s as lists with meta data.
 	
 	Encodes numpy scalar types as Python equivalents. Special encoding is not possible,
 	because int64 (in py2) and float64 (in py2 and py3) are subclasses of primitives,
 	which never reach the encoder.
+	
+	:param primitives: If True, arrays are serialized as (nested) lists without meta info.
 	"""
 	if isinstance(obj, ndarray):
-		dct = hashodict((
-			('__ndarray__', obj.tolist()),
-			('dtype', str(obj.dtype)),
-			('shape', obj.shape),
-		))
-		if len(obj.shape) > 1:
-			dct['Corder'] = obj.flags['C_CONTIGUOUS']
-		return dct
+		if primitives:
+			return obj.tolist()
+		else:
+			dct = hashodict((
+				('__ndarray__', obj.tolist()),
+				('dtype', str(obj.dtype)),
+				('shape', obj.shape),
+			))
+			if len(obj.shape) > 1:
+				dct['Corder'] = obj.flags['C_CONTIGUOUS']
+			return dct
 	elif isinstance(obj, generic):
 		if NumpyEncoder.SHOW_SCALAR_WARNING:
 			NumpyEncoder.SHOW_SCALAR_WARNING = False
 			warning('json-tricks: numpy scalar serialization is experimental and may work differently in future versions')
 		return obj.item()
 	return obj
 
@@ -77,32 +82,33 @@
 
 
 DEFAULT_NP_ENCODERS = (numpy_encode,) + DEFAULT_ENCODERS  # numpy encode needs to be before complex
 DEFAULT_NP_HOOKS = (json_numpy_obj_hook,) + DEFAULT_HOOKS
 
 
 def dumps(obj, sort_keys=None, cls=TricksEncoder, obj_encoders=DEFAULT_NP_ENCODERS,
-		extra_obj_encoders=(), compression=None, allow_nan=False, **jsonkwargs):
+		extra_obj_encoders=(), primitives=False, compression=None, allow_nan=False,
+		**jsonkwargs):
 	"""
 	Just like `nonp.dumps` but with numpy functionality enabled.
 	"""
 	return nonp.dumps(obj, sort_keys=sort_keys, cls=cls, obj_encoders=obj_encoders,
-		extra_obj_encoders=extra_obj_encoders, compression=compression,
-		allow_nan=allow_nan, **jsonkwargs)
+		extra_obj_encoders=extra_obj_encoders, primitives=primitives,
+		compression=compression, allow_nan=allow_nan, **jsonkwargs)
 
 
 def dump(obj, fp, sort_keys=None, cls=TricksEncoder, obj_encoders=DEFAULT_NP_ENCODERS,
-		extra_obj_encoders=(), compression=None, force_flush=False, allow_nan=False,
-		**jsonkwargs):
+		extra_obj_encoders=(), primitives=False, compression=None, force_flush=False,
+		allow_nan=False, **jsonkwargs):
 	"""
 	Just like `nonp.dump` but with numpy functionality enabled.
 	"""
 	return nonp.dump(obj, fp, sort_keys=sort_keys, cls=cls, obj_encoders=obj_encoders,
-		extra_obj_encoders=extra_obj_encoders, compression=compression,
-		force_flush=force_flush, allow_nan=allow_nan, **jsonkwargs)
+		extra_obj_encoders=extra_obj_encoders, primitives=primitives,
+		compression=compression, force_flush=force_flush, allow_nan=allow_nan, **jsonkwargs)
 
 
 def loads(string, preserve_order=True, ignore_comments=True, decompression=None, obj_pairs_hooks=DEFAULT_NP_HOOKS,
 		extra_obj_pairs_hooks=(), cls_lookup_map=None, allow_duplicates=True, **jsonkwargs):
 	"""
 	Just like `nonp.loads` but with numpy functionality enabled.
 	"""
```

### Comparing `json_tricks-3.7.0/json_tricks/__init__.py` & `json_tricks-3.8.0/json_tricks/__init__.py`

 * *Files identical despite different names*

### Comparing `json_tricks-3.7.0/json_tricks/encoders.py` & `json_tricks-3.8.0/json_tricks/encoders.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,103 @@
 
 from datetime import datetime, date, time, timedelta
 from fractions import Fraction
 from logging import warning
 from json import JSONEncoder
 from sys import version
-
 from decimal import Decimal
-
-from .utils import hashodict
+from .utils import hashodict, call_with_optional_kwargs
 
 
 class TricksEncoder(JSONEncoder):
 	"""
 	Encoder that runs any number of encoder functions or instances on
 	the objects that are being encoded.
 
 	Each encoder should make any appropriate changes and return an object,
 	changed or not. This will be passes to the other encoders.
 	"""
-	def __init__(self, obj_encoders=None, silence_typeerror=False, **json_kwargs):
+	def __init__(self, obj_encoders=None, silence_typeerror=False, primitives=False, **json_kwargs):
 		"""
 		:param obj_encoders: An iterable of functions or encoder instances to try.
 		:param silence_typeerror: If set to True, ignore the TypeErrors that Encoder instances throw (default False).
 		"""
 		self.obj_encoders = []
 		if obj_encoders:
 			self.obj_encoders = list(obj_encoders)
 		self.silence_typeerror = silence_typeerror
+		self.primitives = primitives
 		super(TricksEncoder, self).__init__(**json_kwargs)
 
 	def default(self, obj, *args, **kwargs):
 		"""
 		This is the method of JSONEncoders that is called for each object; it calls
 		all the encoders with the previous one's output used as input.
 
 		It works for Encoder instances, but they are expected not to throw
-		TypeErrorfor unrecognized types (the super method does that by default).
+		`TypeError` for unrecognized types (the super method does that by default).
 
 		It never calls the `super` method so if there are non-primitive types
 		left at the end, you'll get an encoding error.
 		"""
 		prev_id = id(obj)
 		for encoder in self.obj_encoders:
 			if hasattr(encoder, 'default'):
-				# hope no TypeError is thrown
 				try:
-					obj = encoder.default(obj)
+					obj = call_with_optional_kwargs(encoder.default, obj, primitives=self.primitives)
 				except TypeError as err:
 					if not self.silence_typeerror:
 						raise
 			elif hasattr(encoder, '__call__'):
-				obj = encoder(obj)
+				obj = call_with_optional_kwargs(encoder, obj, primitives=self.primitives)
 			else:
 				raise TypeError('`obj_encoder` {0:} does not have `default` method and is not callable'.format(encoder))
 		if id(obj) == prev_id:
 			raise TypeError('Object of type {0:} could not be encoded by {1:} using encoders [{2:s}]'.format(
 				type(obj), self.__class__.__name__, ', '.join(str(encoder) for encoder in self.obj_encoders)))
 		return obj
 
 
-def json_date_time_encode(obj):
+def json_date_time_encode(obj, primitives=False):
 	"""
 	Encode a date, time, datetime or timedelta to a string of a json dictionary, including optional timezone.
 
 	:param obj: date/time/datetime/timedelta obj
 	:return: (dict) json primitives representation of date, time, datetime or timedelta
 	"""
+	if primitives and isinstance(obj, (date, time, datetime)):
+		return obj.isoformat()
 	if isinstance(obj, datetime):
 		dct = hashodict([('__datetime__', None), ('year', obj.year), ('month', obj.month),
 			('day', obj.day), ('hour', obj.hour), ('minute', obj.minute),
 			('second', obj.second), ('microsecond', obj.microsecond)])
 		if obj.tzinfo:
 			dct['tzinfo'] = obj.tzinfo.zone
 	elif isinstance(obj, date):
 		dct = hashodict([('__date__', None), ('year', obj.year), ('month', obj.month), ('day', obj.day)])
 	elif isinstance(obj, time):
 		dct = hashodict([('__time__', None), ('hour', obj.hour), ('minute', obj.minute),
 			('second', obj.second), ('microsecond', obj.microsecond)])
 		if obj.tzinfo:
 			dct['tzinfo'] = obj.tzinfo.zone
 	elif isinstance(obj, timedelta):
-		dct = hashodict([('__timedelta__', None), ('days', obj.days), ('seconds', obj.seconds),
-			('microseconds', obj.microseconds)])
+		if primitives:
+			return obj.total_seconds()
+		else:
+			dct = hashodict([('__timedelta__', None), ('days', obj.days), ('seconds', obj.seconds),
+				('microseconds', obj.microseconds)])
 	else:
 		return obj
 	for key, val in tuple(dct.items()):
 		if not key.startswith('__') and not val:
 			del dct[key]
 	return dct
 
 
-def class_instance_encode(obj):
+def class_instance_encode(obj, primitives=False):
 	"""
 	Encodes a class instance to json. Note that it can only be recovered if the environment allows the class to be
 	imported in the same way.
 	"""
 	if isinstance(obj, list) or isinstance(obj, dict):
 		return obj
 	if hasattr(obj, '__class__') and hasattr(obj, '__dict__'):
@@ -114,41 +117,58 @@
 				' that it\'s module/import path is unknown, so you might have to provide cls_lookup_map when '
 				'decoding').format(obj.__class__))
 		name = obj.__class__.__name__
 		if hasattr(obj, '__json_encode__'):
 			attrs = obj.__json_encode__()
 		else:
 			attrs = hashodict(obj.__dict__.items())
-		return hashodict((('__instance_type__', (mod, name)), ('attributes', attrs)))
+		if primitives:
+			return attrs
+		else:
+			return hashodict((('__instance_type__', (mod, name)), ('attributes', attrs)))
 	return obj
 
 
-def json_complex_encode(obj):
+def json_complex_encode(obj, primitives=False):
 	"""
 	Encode a complex number as a json dictionary of it's real and imaginary part.
 
 	:param obj: complex number, e.g. `2+1j`
 	:return: (dict) json primitives representation of `obj`
 	"""
 	if isinstance(obj, complex):
-		return hashodict(__complex__=[obj.real, obj.imag])
+		if primitives:
+			return [obj.real, obj.imag]
+		else:
+			return hashodict(__complex__=[obj.real, obj.imag])
 	return obj
 
 
-def numeric_types_encode(obj):
+def numeric_types_encode(obj, primitives=False):
+	"""
+	Encode Decimal and Fraction.
+	
+	:param primitives: Encode decimals and fractions as standard floats. You may lose precision. If you do this, you may need to enable `allow_nan` (decimals always allow NaNs but floats do not).
+	"""
 	if isinstance(obj, Decimal):
-		return {
-			'__decimal__': str(obj.canonical()),
-		}
+		if primitives:
+			return float(obj)
+		else:
+			return {
+				'__decimal__': str(obj.canonical()),
+			}
 	if isinstance(obj, Fraction):
-		return {
-			'__fraction__': True,
-			'numerator': obj.numerator,
-			'denominator': obj.denominator,
-		}
+		if primitives:
+			return float(obj)
+		else:
+			return hashodict((
+				('__fraction__', True),
+				('numerator', obj.numerator),
+				('denominator', obj.denominator),
+			))
 	return obj
 
 
 class ClassInstanceEncoder(JSONEncoder):
 	"""
 	See `class_instance_encoder`.
 	"""
@@ -158,22 +178,25 @@
 
 	def default(self, obj, *args, **kwargs):
 		if self.encode_cls_instances:
 			obj = class_instance_encode(obj)
 		return super(ClassInstanceEncoder, self).default(obj, *args, **kwargs)
 
 
-def json_set_encode(obj):
+def json_set_encode(obj, primitives=False):
 	"""
 	Encode python sets as dictionary with key __set__ and a list of the values.
 
 	Try to sort the set to get a consistent json representation, use arbitrary order if the data is not ordinal.
 	"""
 	if isinstance(obj, set):
 		try:
 			repr = sorted(obj)
 		except Exception:
 			repr = list(obj)
-		return hashodict(__set__=repr)
+		if primitives:
+			return repr
+		else:
+			return hashodict(__set__=repr)
 	return obj
```

### Comparing `json_tricks-3.7.0/json_tricks/decoders.py` & `json_tricks-3.8.0/json_tricks/decoders.py`

 * *Files identical despite different names*

### Comparing `json_tricks-3.7.0/json_tricks/comment.py` & `json_tricks-3.8.0/json_tricks/comment.py`

 * *Files identical despite different names*

### Comparing `json_tricks-3.7.0/PKG-INFO` & `json_tricks-3.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 1.1
 Name: json_tricks
-Version: 3.7.0
+Version: 3.8.0
 Summary: Add features to json: en/decoding of numpy arrays, preservation of ordering and ignoring of comments in input
 Home-page: https://github.com/mverleg/pyjson_tricks
 Author: (the author)
 Author-email: mdilligaf@gmail.com
 License: Revised BSD License (LICENSE.txt)
 Description: JSON tricks (python)
         ---------------------------------------
         
-        The `pyjson-tricks` package brings four pieces of functionality to python handling of json files:
+        The `pyjson-tricks` package brings several pieces of functionality to python handling of json files:
         
         1. **Store and load numpy arrays** in human-readable format.
         2. **Store and load class instances** both generic and customized.
         3. **Store and load date/times** as a dictionary (including timezone).
         4. **Preserve map order** `{}` using `OrderedDict`.
         5. **Allow for comments** in json files by starting lines with `#`.
         6. Sets, complex numbers, Decimal, Fraction, compression, duplicate keys, ...
@@ -51,14 +51,116 @@
         
         	from json_tricks.np import dump, dumps, load, loads, strip_comments
         
         If you do not have numpy and want to use only order preservation and commented json reading, you should **``import from json_tricks.nonp`` instead**.
         
         The exact signatures of these functions are in the documentation_.
         
+        Preserve type vs use primitive
+        -------------------------------
+        
+        By default, types are encoded such that they can be restored to their original type when loaded with `json-tricks. Example encodings in this documentation refer to that format.
+        
+        You can also choose to store things as their closest primitive type (e.g. arrays and sets as lists, decimals as floats). This may be desirable if you don't care about the exact type, or you are loading the json in another language (which doesn't restore python types). It's also smaller.
+        
+        To forego meta data and store primitives instead, pass `primitives` to `dump(s)`. This is available in version `3.8` and later. Example:
+        
+        .. code-block:: python
+        
+        	data = [
+        		arange(0, 10, 1, dtype=int).reshape((2, 5)),
+        		datetime(year=2017, month=1, day=19, hour=23, minute=00, second=00),
+        		1 + 2j,
+        		Decimal(42),
+        		Fraction(1, 3),
+        		MyTestCls(s='ub', dct={'7': 7}),  # see later
+        		set(range(7)),
+        	]
+        	print(dumps(data, indent=2))
+        
+        .. code-block:: javascript
+        
+            // (comments added and indenting changed)
+            [
+              // numpy array
+              {
+                "__ndarray__": [
+                    [0, 1, 2, 3, 4],
+                    [5, 6, 7, 8, 9]],
+                "dtype": "int64",
+                "shape": [2, 5],
+                "Corder": true
+              },
+              // datetime (naive)
+              {
+                "__datetime__": null,
+                "year": 2017,
+                "month": 1,
+                "day": 19,
+                "hour": 23
+              },
+              // complex number
+              {
+                "__complex__": [1.0, 2.0]
+              },
+              // decimal & fraction
+              {
+                "__decimal__": "42"
+              },
+              {
+                "__fraction__": true
+                "numerator": 1,
+                "denominator": 3,
+              },
+              // class instance
+              {
+                "__instance_type__": [
+                  "tests.test_class",
+                  "MyTestCls"
+                ],
+                "attributes": {
+                  "s": "ub",
+                  "dct": {"7": 7}
+                }
+              },
+              // set
+              {
+                "__set__": [0, 1, 2, 3, 4, 5, 6]
+              }
+            ]
+        
+        .. code-block:: python
+        
+            print(dumps(data, indent=2, primitives=True))
+        
+        .. code-block:: javascript
+        
+            // (comments added and indentation changed)
+            [
+              // numpy array
+              [[0, 1, 2, 3, 4],
+               [5, 6, 7, 8, 9]],
+              // datetime (naive)
+              "2017-01-19T23:00:00",
+              // complex number
+              [1.0, 2.0],
+              // decimal & fraction
+              42.0,
+              0.3333333333333333,
+              // class instance
+              {
+                "s": "ub",
+                "dct": {"7": 7}
+              },
+              // set
+              [0, 1, 2, 3, 4, 5, 6]
+            ]
+        
+        Note that valid json is produced either way: `json-tricks` stores meta data as normal json, but other packages probably won't interpret it.
+        
         Features
         ---------------------------------------
         
         Numpy arrays
         +++++++++++++++++++++++++++++++++++++++
         
         The array is encoded in sort-of-readable and very flexible and portable format, like so:
@@ -253,20 +355,24 @@
         .. _encode_scalars_inplace: https://json-tricks.readthedocs.io/en/latest/#json_tricks.np_utils.encode_scalars_inplace
         
         
         
 Keywords: json,numpy,OrderedDict,comments
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `json_tricks-3.7.0/README.rst` & `json_tricks-3.8.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 JSON tricks (python)
 ---------------------------------------
 
-The `pyjson-tricks` package brings four pieces of functionality to python handling of json files:
+The `pyjson-tricks` package brings several pieces of functionality to python handling of json files:
 
 1. **Store and load numpy arrays** in human-readable format.
 2. **Store and load class instances** both generic and customized.
 3. **Store and load date/times** as a dictionary (including timezone).
 4. **Preserve map order** `{}` using `OrderedDict`.
 5. **Allow for comments** in json files by starting lines with `#`.
 6. Sets, complex numbers, Decimal, Fraction, compression, duplicate keys, ...
@@ -43,14 +43,116 @@
 
 	from json_tricks.np import dump, dumps, load, loads, strip_comments
 
 If you do not have numpy and want to use only order preservation and commented json reading, you should **``import from json_tricks.nonp`` instead**.
 
 The exact signatures of these functions are in the documentation_.
 
+Preserve type vs use primitive
+-------------------------------
+
+By default, types are encoded such that they can be restored to their original type when loaded with `json-tricks. Example encodings in this documentation refer to that format.
+
+You can also choose to store things as their closest primitive type (e.g. arrays and sets as lists, decimals as floats). This may be desirable if you don't care about the exact type, or you are loading the json in another language (which doesn't restore python types). It's also smaller.
+
+To forego meta data and store primitives instead, pass `primitives` to `dump(s)`. This is available in version `3.8` and later. Example:
+
+.. code-block:: python
+
+	data = [
+		arange(0, 10, 1, dtype=int).reshape((2, 5)),
+		datetime(year=2017, month=1, day=19, hour=23, minute=00, second=00),
+		1 + 2j,
+		Decimal(42),
+		Fraction(1, 3),
+		MyTestCls(s='ub', dct={'7': 7}),  # see later
+		set(range(7)),
+	]
+	print(dumps(data, indent=2))
+
+.. code-block:: javascript
+
+    // (comments added and indenting changed)
+    [
+      // numpy array
+      {
+        "__ndarray__": [
+            [0, 1, 2, 3, 4],
+            [5, 6, 7, 8, 9]],
+        "dtype": "int64",
+        "shape": [2, 5],
+        "Corder": true
+      },
+      // datetime (naive)
+      {
+        "__datetime__": null,
+        "year": 2017,
+        "month": 1,
+        "day": 19,
+        "hour": 23
+      },
+      // complex number
+      {
+        "__complex__": [1.0, 2.0]
+      },
+      // decimal & fraction
+      {
+        "__decimal__": "42"
+      },
+      {
+        "__fraction__": true
+        "numerator": 1,
+        "denominator": 3,
+      },
+      // class instance
+      {
+        "__instance_type__": [
+          "tests.test_class",
+          "MyTestCls"
+        ],
+        "attributes": {
+          "s": "ub",
+          "dct": {"7": 7}
+        }
+      },
+      // set
+      {
+        "__set__": [0, 1, 2, 3, 4, 5, 6]
+      }
+    ]
+
+.. code-block:: python
+
+    print(dumps(data, indent=2, primitives=True))
+
+.. code-block:: javascript
+
+    // (comments added and indentation changed)
+    [
+      // numpy array
+      [[0, 1, 2, 3, 4],
+       [5, 6, 7, 8, 9]],
+      // datetime (naive)
+      "2017-01-19T23:00:00",
+      // complex number
+      [1.0, 2.0],
+      // decimal & fraction
+      42.0,
+      0.3333333333333333,
+      // class instance
+      {
+        "s": "ub",
+        "dct": {"7": 7}
+      },
+      // set
+      [0, 1, 2, 3, 4, 5, 6]
+    ]
+
+Note that valid json is produced either way: `json-tricks` stores meta data as normal json, but other packages probably won't interpret it.
+
 Features
 ---------------------------------------
 
 Numpy arrays
 +++++++++++++++++++++++++++++++++++++++
 
 The array is encoded in sort-of-readable and very flexible and portable format, like so:
```

### Comparing `json_tricks-3.7.0/json_tricks.egg-info/PKG-INFO` & `json_tricks-3.8.0/json_tricks.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 1.1
 Name: json-tricks
-Version: 3.7.0
+Version: 3.8.0
 Summary: Add features to json: en/decoding of numpy arrays, preservation of ordering and ignoring of comments in input
 Home-page: https://github.com/mverleg/pyjson_tricks
 Author: (the author)
 Author-email: mdilligaf@gmail.com
 License: Revised BSD License (LICENSE.txt)
 Description: JSON tricks (python)
         ---------------------------------------
         
-        The `pyjson-tricks` package brings four pieces of functionality to python handling of json files:
+        The `pyjson-tricks` package brings several pieces of functionality to python handling of json files:
         
         1. **Store and load numpy arrays** in human-readable format.
         2. **Store and load class instances** both generic and customized.
         3. **Store and load date/times** as a dictionary (including timezone).
         4. **Preserve map order** `{}` using `OrderedDict`.
         5. **Allow for comments** in json files by starting lines with `#`.
         6. Sets, complex numbers, Decimal, Fraction, compression, duplicate keys, ...
@@ -51,14 +51,116 @@
         
         	from json_tricks.np import dump, dumps, load, loads, strip_comments
         
         If you do not have numpy and want to use only order preservation and commented json reading, you should **``import from json_tricks.nonp`` instead**.
         
         The exact signatures of these functions are in the documentation_.
         
+        Preserve type vs use primitive
+        -------------------------------
+        
+        By default, types are encoded such that they can be restored to their original type when loaded with `json-tricks. Example encodings in this documentation refer to that format.
+        
+        You can also choose to store things as their closest primitive type (e.g. arrays and sets as lists, decimals as floats). This may be desirable if you don't care about the exact type, or you are loading the json in another language (which doesn't restore python types). It's also smaller.
+        
+        To forego meta data and store primitives instead, pass `primitives` to `dump(s)`. This is available in version `3.8` and later. Example:
+        
+        .. code-block:: python
+        
+        	data = [
+        		arange(0, 10, 1, dtype=int).reshape((2, 5)),
+        		datetime(year=2017, month=1, day=19, hour=23, minute=00, second=00),
+        		1 + 2j,
+        		Decimal(42),
+        		Fraction(1, 3),
+        		MyTestCls(s='ub', dct={'7': 7}),  # see later
+        		set(range(7)),
+        	]
+        	print(dumps(data, indent=2))
+        
+        .. code-block:: javascript
+        
+            // (comments added and indenting changed)
+            [
+              // numpy array
+              {
+                "__ndarray__": [
+                    [0, 1, 2, 3, 4],
+                    [5, 6, 7, 8, 9]],
+                "dtype": "int64",
+                "shape": [2, 5],
+                "Corder": true
+              },
+              // datetime (naive)
+              {
+                "__datetime__": null,
+                "year": 2017,
+                "month": 1,
+                "day": 19,
+                "hour": 23
+              },
+              // complex number
+              {
+                "__complex__": [1.0, 2.0]
+              },
+              // decimal & fraction
+              {
+                "__decimal__": "42"
+              },
+              {
+                "__fraction__": true
+                "numerator": 1,
+                "denominator": 3,
+              },
+              // class instance
+              {
+                "__instance_type__": [
+                  "tests.test_class",
+                  "MyTestCls"
+                ],
+                "attributes": {
+                  "s": "ub",
+                  "dct": {"7": 7}
+                }
+              },
+              // set
+              {
+                "__set__": [0, 1, 2, 3, 4, 5, 6]
+              }
+            ]
+        
+        .. code-block:: python
+        
+            print(dumps(data, indent=2, primitives=True))
+        
+        .. code-block:: javascript
+        
+            // (comments added and indentation changed)
+            [
+              // numpy array
+              [[0, 1, 2, 3, 4],
+               [5, 6, 7, 8, 9]],
+              // datetime (naive)
+              "2017-01-19T23:00:00",
+              // complex number
+              [1.0, 2.0],
+              // decimal & fraction
+              42.0,
+              0.3333333333333333,
+              // class instance
+              {
+                "s": "ub",
+                "dct": {"7": 7}
+              },
+              // set
+              [0, 1, 2, 3, 4, 5, 6]
+            ]
+        
+        Note that valid json is produced either way: `json-tricks` stores meta data as normal json, but other packages probably won't interpret it.
+        
         Features
         ---------------------------------------
         
         Numpy arrays
         +++++++++++++++++++++++++++++++++++++++
         
         The array is encoded in sort-of-readable and very flexible and portable format, like so:
@@ -253,20 +355,24 @@
         .. _encode_scalars_inplace: https://json-tricks.readthedocs.io/en/latest/#json_tricks.np_utils.encode_scalars_inplace
         
         
         
 Keywords: json,numpy,OrderedDict,comments
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `json_tricks-3.7.0/setup.py` & `json_tricks-3.8.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,62 @@
 # -*- coding: utf-8 -*-
 
+from sys import version_info
 from setuptools import setup
 
 
 with open('README.rst', 'r') as fh:
 	readme = fh.read()
 
 
+requires = []
+if version_info < (2, 7, 0):
+	requires.append('ordereddict')
+
+
 setup(
 	name='json_tricks',
 	description='Add features to json: en/decoding of numpy arrays, ' +
 		'preservation of ordering and ignoring of comments in input',
 	long_description=readme,
 	url='https://github.com/mverleg/pyjson_tricks',
 	author='Mark V',
 	maintainer='(the author)',
 	author_email='mdilligaf@gmail.com',
 	license='Revised BSD License (LICENSE.txt)',
 	keywords=['json', 'numpy', 'OrderedDict', 'comments',],
-	version='3.7.0',
+	version='3.8.0',
 	packages=['json_tricks'],
 	include_package_data=True,
 	zip_safe=False,
 	classifiers=[
 		'Development Status :: 5 - Production/Stable',
+		'Development Status :: 6 - Mature',
 		'Intended Audience :: Developers',
 		'Natural Language :: English',
 		'License :: OSI Approved :: BSD License',
 		'Operating System :: OS Independent',
 		'Programming Language :: Python',
 		'Programming Language :: Python :: 2',
-		'Programming Language :: Python :: 2.6',
+		'Programming Language :: Python :: 2.6',  # it should work, but there's a problem with tests
 		'Programming Language :: Python :: 2.7',
 		'Programming Language :: Python :: 3',
 		'Programming Language :: Python :: 3.3',
 		'Programming Language :: Python :: 3.4',
 		'Programming Language :: Python :: 3.5',
+		'Programming Language :: Python :: 3.6',
+		'Programming Language :: Python :: Implementation :: CPython',
+		'Programming Language :: Python :: Implementation :: PyPy',
 		'Topic :: Software Development :: Libraries :: Python Modules',
+		# 'Topic :: Documentation',
+		# 'Topic :: Documentation :: Sphinx',
+		# 'Topic :: Utilities',
 	],
-	install_requires=[
+	install_requires=requires,
 		# pytz for timezones (and tests)
 		# pytest for tests
+		# tox for tests
 		# sphinx for documentation
 		# numpy for numpy functionality
-	],
 )
```

