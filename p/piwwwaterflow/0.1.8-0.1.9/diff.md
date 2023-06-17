# Comparing `tmp/piwwwaterflow-0.1.8.tar.gz` & `tmp/piwwwaterflow-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwwwaterflow-0.1.8.tar", last modified: Tue Jun 13 06:54:37 2023, max compression
+gzip compressed data, was "piwwwaterflow-0.1.9.tar", last modified: Sat Jun 17 14:35:08 2023, max compression
```

## Comparing `piwwwaterflow-0.1.8.tar` & `piwwwaterflow-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.773601 piwwwaterflow-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-13 06:54:37.773601 piwwwaterflow-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.769601 piwwwaterflow-0.1.8/piwwwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.769601 piwwwaterflow-0.1.8/piwwwaterflow/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.769601 piwwwaterflow-0.1.8/piwwwaterflow/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/css/iepngfix.htc
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.773601 piwwwaterflow-0.1.8/piwwwaterflow/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/img/blank.gif
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/img/bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/img/icon-256.png
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/img/icon-32.png
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/img/piwaterflow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/img/play.png
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/img/shadow.gif
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/img/top.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.773601 piwwwaterflow-0.1.8/piwwwaterflow/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/static/js/code.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.773601 piwwwaterflow-0.1.8/piwwwaterflow/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/webservice.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/piwwwaterflow/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.769601 piwwwaterflow-0.1.8/piwwwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-13 06:54:37.000000 piwwwaterflow-0.1.8/piwwwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-13 06:54:37.000000 piwwwaterflow-0.1.8/piwwwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:54:37.000000 piwwwaterflow-0.1.8/piwwwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-13 06:54:37.000000 piwwwaterflow-0.1.8/piwwwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 06:54:37.000000 piwwwaterflow-0.1.8/piwwwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:54:37.773601 piwwwaterflow-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:37.773601 piwwwaterflow-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:25.000000 piwwwaterflow-0.1.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.734823 piwwwaterflow-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-17 14:35:08.734823 piwwwaterflow-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.730823 piwwwaterflow-0.1.9/piwwwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.730823 piwwwaterflow-0.1.9/piwwwaterflow/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.730823 piwwwaterflow-0.1.9/piwwwaterflow/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/css/iepngfix.htc
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.734823 piwwwaterflow-0.1.9/piwwwaterflow/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/img/blank.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/img/bottom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/img/icon-256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/img/icon-32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/img/piwaterflow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/img/play.png
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/img/shadow.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/img/top.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.734823 piwwwaterflow-0.1.9/piwwwaterflow/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    10461 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/js/code.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.734823 piwwwaterflow-0.1.9/piwwwaterflow/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/webservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.730823 piwwwaterflow-0.1.9/piwwwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-17 14:35:08.000000 piwwwaterflow-0.1.9/piwwwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-17 14:35:08.000000 piwwwaterflow-0.1.9/piwwwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:35:08.000000 piwwwaterflow-0.1.9/piwwwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-17 14:35:08.000000 piwwwaterflow-0.1.9/piwwwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-17 14:35:08.000000 piwwwaterflow-0.1.9/piwwwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:35:08.734823 piwwwaterflow-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.734823 piwwwaterflow-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/tests/__init__.py
```

### Comparing `piwwwaterflow-0.1.8/PKG-INFO` & `piwwwaterflow-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.1.8
+Version: 0.1.9
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.1.8/piwwwaterflow/static/css/iepngfix.htc` & `piwwwaterflow-0.1.9/piwwwaterflow/static/css/iepngfix.htc`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.8/piwwwaterflow/static/css/view.css` & `piwwwaterflow-0.1.9/piwwwaterflow/static/css/view.css`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.8/piwwwaterflow/static/img/icon-256.png` & `piwwwaterflow-0.1.9/piwwwaterflow/static/img/icon-256.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.8/piwwwaterflow/static/img/icon-32.png` & `piwwwaterflow-0.1.9/piwwwaterflow/static/img/icon-32.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.8/piwwwaterflow/static/img/piwaterflow.svg` & `piwwwaterflow-0.1.9/piwwwaterflow/static/img/piwaterflow.svg`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.8/piwwwaterflow/static/img/play.png` & `piwwwaterflow-0.1.9/piwwwaterflow/static/img/play.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.8/piwwwaterflow/static/js/code.js` & `piwwwaterflow-0.1.9/piwwwaterflow/static/js/code.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -97,16 +97,16 @@
 
 setInterval("update(false);", 30000);
 
 function update(first_time) {
     socket.emit('service_request', function service(response) {
         // Version label update
         var versionlabel = document.getElementById('version');
-        frontend = '1.4.0'
-        backend = response.version
+        frontend = response.version_frontend
+        backend = response.version_backend
         versionlabel.textContent = `PiWaterflow ${frontend} (Backend ${backend})`
 
         // Status line update
         now = new Date()
         formattedNow = _datestringFromDate(now).slice(0, 10)
         tomorrow = new Date(now.getTime())
         tomorrow.setDate(now.getDate() + 1)
```

### Comparing `piwwwaterflow-0.1.8/piwwwaterflow/templates/form.html` & `piwwwaterflow-0.1.9/piwwwaterflow/templates/form.html`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	<div id="form_container" align="center">
 		<div class="mainheader">
 			<!--<img src="static/img/icon-256.png" alt="Icon" width="90em" height="90em">-->
 			<img src="static/img/piwaterflow.svg" alt="Icon" width="90em" height="90em">
 			<label id = 'version'> PiWaterflow loading... </label>
 		</div>
 		<form id="waterflow_form" style=" margin-block-end: 0em;" method="POST" action="">
-			<div class="form_description" style="margin-bottom: -;margin-bottom: 0px; margin-top: 0px;">
+			<div class="form_description" style="margin-bottom: 0px; margin-top: 0px;">
 				<label id = 'status'>Status: Retrieving status...</label>
 			</div>
 
 			<table class="table" id="tablacontroles"  style="width:100%">
 				<tr>
 					<td>
 						<table id="programsandforce" style="width:100%;height:100%; border-bottom:1px dotted #ccc;">
@@ -27,26 +27,26 @@
 									<table class="table" id="programstable" style="height:100%;" cellpadding="0" cellspacing="5">
 										<tr border="0px" id="headers">
 											<th width="10%"></th>
 											<th width="30%">
 												<label class="programheader">Start time </label>
 											</th>
 											<th width="30%">
-												<label class="programheader" id="valve1trigger" onclick="forceValve(this,0)">Valve 1</label>
+												<label class="programheader" id="valve1trigger" onclick="forceValve(this, document.getElementById('valve1trigger').textContent)">Valve 1</label>
 											</th>
 											<th width="30%">
-												<label class="programheader" id="valve2trigger" onclick="forceValve(this,1)">Valve 2</label>
+												<label class="programheader" id="valve2trigger" onclick="forceValve(this, document.getElementById('valve2trigger').textContent)">Valve 2</label>
 											</th >
 											<th width="5%">
 												<label class="programheader" >Enabled</label>
 											</th>
 										</tr>
 										<tr border="0px" id="prog1row">
 											<td>
-												<label class="programheader" id="program1trigger" onclick="forceProgram(this,0)">Prog 1</label>
+												<label class="programheader" id="program1trigger" onclick="forceProgram(this, document.getElementById('program1trigger').textContent)">Prog 1</label>
 											</td>
 											<td>
 												<input type="time" class="timeclass copperround" id="time1" name="time1" required>
 											</td>
 											<td>
 												<input id="valve11" name="valve11" class="number copperround" type="number"  min="0" max="10">
 											</td>
@@ -55,15 +55,15 @@
 											</td>
 											<td>
 												<input type="checkbox" id="prog1enabled" name="prog1enabled" value="True" class="checkstyle">
 											</td>
 										</tr>
 										<tr border="0px" id="prog2row">
 											<td>
-												<label class="programheader" id="program2trigger" onclick="forceProgram(this,1)">Prog 2</label>
+												<label class="programheader" id="program2trigger" onclick="forceProgram(this, document.getElementById('program2trigger').textContent)">Prog 2</label>
 											</td>
 											<td>
 												<input type="time" class="timeclass copperround" id="time2" name="time2" required>
 											</td>
 											<td>
 												<input id="valve21" name="valve21" class="number copperround"  type="number" min="0" max="10">
 											</td>
```

### Comparing `piwwwaterflow-0.1.8/piwwwaterflow/webservice.py` & `piwwwaterflow-0.1.9/piwwwaterflow/webservice.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,40 +61,50 @@
         Args:
             data (dict):'first_time': This value is only bypassed to the caller
         Returns:
             dict:Dictionary with all the information about the status of the waterflow system
         """
         self.logger.info('Service requested...')
         try:
-            ver = version('piwaterflow')
+            ver_backend = version('piwaterflow')
+            ver_frontend = version('piwwwwaterflow')
         except PackageNotFoundError:
-            ver = '?.?.?'
+            ver_backend = '?.?.?'
+            ver_frontend = '?.?.?'
+
+        responsedict = None
+
+        try:
+            responsedict = {'log': self.waterflow.get_log(),
+                            'forced': self.waterflow.get_forced_info(),
+                            'stop': self.waterflow.stop_requested(),
+                            'config': self._get_public_config(),
+                            'lastlooptime': self.waterflow.last_loop_time().strftime('%Y-%m-%dT%H:%M:%S'),
+                            'version_backend': ver_backend,
+                            'version_frontend': ver_frontend
+                            }
+            # Change to string so that javascript can manage with it
+            for program in responsedict['config']['programs']:
+                program['start_time'] = program['start_time'].strftime('%H:%M')
+        except Exception as ex:
+            self.logger.error('Error calculating service request: %s', ex)
+            raise RuntimeError(f'Exception on service request: {ex}') from ex
 
-        responsedict = {'log': self.waterflow.get_log(),
-                        'forced': self.waterflow.get_forced_info(),
-                        'stop': self.waterflow.stop_requested(),
-                        'config': self._get_public_config(),
-                        'lastlooptime': self.waterflow.last_loop_time().strftime('%Y-%m-%dT%H:%M:%S'),
-                        'version': ver
-                        }
-        # Change to string so that javascript can manage with it
-        for program in responsedict['config']['programs']:
-            program['start_time'] = program['start_time'].strftime('%H:%M')
         return responsedict
 
     def on_force(self, data: dict):
         """ On force action request
         Args:
             data (dict): 'type': Must be 'valve' or 'program'
                          'value': Must be the index of the program or value to be forced
         """
         print(f'Force requested... {data}')
         type_force = data['type']
         value_force = data['value']
-        self.waterflow.force(type_force, int(value_force))
+        self.waterflow.force(type_force, value_force)
 
     def on_stop(self):
         """ Event to stop current operation """
         print('Stop requested...')
         self.waterflow.stop()
 
     def on_save(self, data):
```

### Comparing `piwwwaterflow-0.1.8/piwwwaterflow/wsgi.py` & `piwwwaterflow-0.1.9/piwwwaterflow/wsgi.py`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.8/piwwwaterflow.egg-info/PKG-INFO` & `piwwwaterflow-0.1.9/piwwwaterflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.1.8
+Version: 0.1.9
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.1.8/piwwwaterflow.egg-info/SOURCES.txt` & `piwwwaterflow-0.1.9/piwwwaterflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.8/setup.py` & `piwwwaterflow-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="piwwwaterflow",
-    version="0.1.8",
+    version="0.1.9",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Waterflow resilient system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/piwwwaterflow",
     packages=setuptools.find_packages(),
```

