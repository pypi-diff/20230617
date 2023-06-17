# Comparing `tmp/gmcapsule-0.4.1.tar.gz` & `tmp/gmcapsule-0.5.0.tar.gz`

## Comparing `gmcapsule-0.4.1.tar` & `gmcapsule-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 gmcapsule-0.4.1/example.ini
--rw-r--r--   0        0        0    25496 2020-02-02 00:00:00.000000 gmcapsule-0.4.1/gmcapsule/__init__.py
--rw-r--r--   0        0        0    24608 2020-02-02 00:00:00.000000 gmcapsule-0.4.1/gmcapsule/gemini.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 gmcapsule-0.4.1/gmcapsule/markdown.py
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 gmcapsule-0.4.1/gmcapsule/modules/10_rewrite.py
--rwxr-xr-x   0        0        0    18589 2020-02-02 00:00:00.000000 gmcapsule-0.4.1/gmcapsule/modules/80_gitview.py
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 gmcapsule-0.4.1/gmcapsule/modules/90_cgi.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 gmcapsule-0.4.1/gmcapsule/modules/99_static.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 gmcapsule-0.4.1/.gitignore
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 gmcapsule-0.4.1/README.md
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gmcapsule-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 gmcapsule-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/example.ini
+-rw-r--r--   0        0        0    21684 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/gmcapsule/__init__.py
+-rw-r--r--   0        0        0    33472 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/gmcapsule/gemini.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/gmcapsule/markdown.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/gmcapsule/modules/10_rewrite.py
+-rwxr-xr-x   0        0        0    18619 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/gmcapsule/modules/80_gitview.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/gmcapsule/modules/90_cgi.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/gmcapsule/modules/99_static.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/.gitignore
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/README.md
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 gmcapsule-0.5.0/PKG-INFO
```

### Comparing `gmcapsule-0.4.1/example.ini` & `gmcapsule-0.5.0/example.ini`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 ; to specify some other configuration file.
 
 [server]
 ;host = localhost
 ;address = 0.0.0.0
 ;port = 1965
 ;certs = .certs
-;modules =
+;modules = 
 ;threads = 5
+;processes = 2
 
 [static]
 root = .
 
 [titan]
 ;upload_limit = 10485760
 
+[cgi]
+bin_root	= ./cgi-bin
+
 [cgi.booster]
 protocol        = titan
 host            = localhost
 path            = /gemlog/* /plan.gmi
 command         = /usr/bin/python3 ../booster/booster.py
 
 [cgi.printenv]
```

### Comparing `gmcapsule-0.4.1/gmcapsule/__init__.py` & `gmcapsule-0.5.0/gmcapsule/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,14 +98,22 @@
     to `.certs`.
 
 modules : path [path...]
     One or more directories to load extension modules from.
 
 threads : int
     Number of worker threads. At least 1 is required. Defaults to 5.
+    Determines how many clients can be responded to at the same time.
+
+processes : int
+    Number of request handler processes. Defaults to 2. Request handler
+    processes run independently of the main process, allowing multiple
+    long-running requests to be handled concurrently. If zero, the worker
+    threads handle requests synchronously and are able to only do I/O
+    operations concurrently.
 
 
 titan
 -----
 
 Settings for Titan requests.
 
@@ -366,15 +374,16 @@
 - ``QUERY_STRING``
 - ``PATH_INFO``
 - ``SCRIPT_NAME``
 - ``SERVER_PROTOCOL``
 - ``SERVER_NAME``
 - ``SERVER_PORT``
 - ``AUTH_TYPE``
-- ``REMOTE_IDENT`` (when client certificate provided)
+- ``TLS_CLIENT_HASH`` (when client certificate provided)
+- ``REMOTE_IDENT`` (fingerprints of client certificate and public key)
 - ``REMOTE_USER`` (when client certificate provided)
 - ``CONTENT_LENGTH`` (Titan only)
 - ``CONTENT_TYPE`` (Titan only)
 - ``TITAN_TOKEN`` (Titan only)
 
 The CGI programs's stdout is used as the response to the request. The response
 is expected to begin with a valid meta line (status code and meta text), but
@@ -409,30 +418,34 @@
     `NN_extmod.py`
 
 That is, the name of the extension ("extmod") is prefixed with two numbers
 `NN` and an underscore. This naming gives more control over the order in
 which modules are loaded. The ones loaded first have precedence over
 registered URL entry points.
 
+If the server has been configured to use multiple processes, each process
+loads the extensions separately. This may require synchronizing access to
+external resources accessed by extensions.
+
 
 Initialization
 --------------
 
 Each extension module is required to have an initialization function:
 
-.. py:function:: extmod.init(capsule)
+.. py:function:: extmod.init(context)
 
     Initialize the extension module.
 
     This is called once immediately after the extension has been loaded.
 
-    :param capsule: Server instance. The extension can use this to access
+    :param context: Worker context. The extension can use this to access
         configuration parameters, install caches, and register entry
-        points.
-    :type capsule: gmcapsule.Capsule
+        points and custom scheme handlers.
+    :type context: gmcapsule.Context
 
 
 Requests
 --------
 
 An extension module is responsible for handling requests arriving at its
 registered entry points. A :class:`~gmcapsule.gemini.Request` object is
@@ -443,31 +456,28 @@
 to the client:
 
 - Returning ``bytes`` or ``str`` means that the response is UTF-8 encoded
   "text/gemini", and the status code is 20.
 - Returning a two-element tuple is interpreted as (status code, meta).
   The response body will be empty. This is useful for error messages and
   redirects.
-- Returning a three-element tuple is interpreted as (status code, meta,
-  body). If the body type is ``str``, it will be UTF-8 encoded before sending.
-  Otherwise, the body is sent as-is. If the body type isn't ``bytes`` or
-  ``bytearray``, it is assumed to be a buffered file-like object. In this
-  case, the entire body is not read in memory first, and ``close()`` will be
-  called on the object afterwards to release its resources.
+- Returning a three-element tuple is interpreted as (status, meta, body).
+  If the body type is ``str``, it will be UTF-8 encoded before sending.
+  If the body type is ``pathlib.Path``, the referenced file is opened and
+  its contents are streamed to the client without reading the entire file
+  to memory. Otherwise, the body type must be ``bytes`` or ``bytearray``.
 
 
 Future improvements
 *******************
 
 The following limitations could/should be lifted in the future:
 
 - Enable value interpolation in the `configparser`, allowing access to
   defined values and environment variables.
-- Add Titan configuration option to not require a client certificate.
-- Extension modules should be reloadable. Add a ``deinit()`` method.
 - `gitview` should have a URL path prefix.
 - Caches should be informed of identities and queries; content might still
   be cacheable.
 
 """
 
 import configparser
@@ -477,21 +487,21 @@
 import mimetypes
 import os
 import re
 import shlex
 import subprocess
 from pathlib import Path
 
-from .gemini import Server, Cache
+from .gemini import Server, Cache, Context
 from .markdown import to_gemtext as markdown_to_gemtext
 
 
-__version__ = '0.4.1'
+__version__ = '0.5.0'
 __all__ = [
-    'Config', 'Capsule', 'Cache',
+    'Config', 'Cache', 'Context',
     'get_mime_type', 'markdown_to_gemtext'
 ]
 
 
 class Config:
     """
     Server configuration.
@@ -504,20 +514,24 @@
             Extension modules can use this to access additional custom
             config parameters. See `configparser
             <https://docs.python.org/3/library/configparser.html>`_
             for details.
     """
 
     def __init__(self, config_path):
-        self.debug_memtrace = False
+        self.config_path = config_path
+        self.reload()
+
+    def reload(self):
         self.ini = configparser.ConfigParser()
-        if os.path.exists(config_path):
-            self.ini.read(config_path)
+        if os.path.exists(self.config_path):
+            print('Configuration:', self.config_path)
+            self.ini.read(self.config_path)
         else:
-            print(config_path, 'not found -- using defaults')
+            print(self.config_path, 'not found -- using defaults')
 
     def hostnames(self):
         """
         Returns:
             list(str): All the configured hostnames. The first listed hostname
             is considered the default to be used when a hostname is not
             otherwise specified.
@@ -549,17 +563,23 @@
     def mod_dirs(self):
         return [Path(p).resolve() for p in shlex.split(
             self.ini.get('server', 'modules', fallback='.'))]
 
     def num_threads(self):
         return self.ini.getint('server', 'threads', fallback=5)
 
+    def num_processes(self):
+        return self.ini.getint('server', 'processes', fallback=2)
+
     def max_upload_size(self):
         return self.ini.getint('titan', 'upload_limit', fallback=10 * 1024 * 1024)
 
+    def require_upload_identity(self):
+        return self.ini.getboolean('titan', 'require_identity', fallback=True)
+
     def section(self, name):
         """
         Find a section in the config INI file.
 
         Args:
             name (str): Name of the section.
 
@@ -603,145 +623,24 @@
     :func:`~gmcapsule.Capsule.run` method to begin accepting incoming
     connections.
 
     Args:
         cfg (Config): Server configuration.
     """
 
-    _capsule = None
-
     def __init__(self, cfg):
-        Capsule._capsule = self
         self.cfg = cfg
-        self.sv = Server(
-            cfg.hostnames(),
-            cfg.certs_dir() / 'cert.pem',
-            cfg.certs_dir() / 'key.pem',
-            address=cfg.address(),
-            port=cfg.port(),
-            session_id=f'GmCapsule:{cfg.port()}'.encode('utf-8'),
-            max_upload_size=cfg.max_upload_size(),
-            num_threads=cfg.num_threads()
-        )
-        # Modules define the entrypoints.
-        self.load_modules()
-
-    @staticmethod
-    def config():
-        """
-        Returns:
-            Config: Server configuration.
-        """
-        return Capsule._capsule.cfg
-
-    def add(self, path, entrypoint, hostname=None, protocol='gemini'):
-        """
-        Register a URL entry point.
-
-        Extension modules must call this to become visible in the server's
-        path hierarchy. Entry points are looked up in the order the modules
-        were loaded, with earlier modules getting precedence.
-
-        Args:
-            path (str): URL path. Must begin with a slash (``/``). Asterisk
-                wildcards (``*``) are supported. Note that if the path
-                ``/*`` is registered, it will match any requested URL.
-            entrypoint (callable): Function or other callable object that
-                gets called when a request is processed with a matching
-                URL path. A :class:`~gmcapsule.gemini.Request` is passed in as the
-                only argument.
-            hostname (str): Hostname for the entry point. If omitted,
-                the entry point applies to all configured hostnames.
-            protocol (str): Protocol for the entry point.
-        """
-        if hostname:
-            self.sv.add_entrypoint(protocol, hostname, path, entrypoint)
-        else:
-            for hostname in self.cfg.hostnames():
-                if not hostname:
-                    raise Exception(f'invalid hostname: "{hostname}"')
-                self.sv.add_entrypoint(protocol, hostname, path, entrypoint)
-
-    def add_cache(self, cache):
-        """
-        Install a cache.
-
-        All installed caches will attempt to save and load content until one
-        succeeds. The caches installed first get precedence.
-
-        Args:
-            cache (Cache): Cache instance.
-        """
-        self.sv.add_cache(cache)
-
-    def load_modules(self):
-        # The configuration can override default priorities.
-        mod_priority = {}
-        if 'priority' in self.cfg.ini:
-            for name, priority in self.cfg.section('priority').items():
-                mod_priority[name] = int(priority)
-
-        # We will load all recognized modules.
-        name_pattern = re.compile(r'([0-9][0-9])_(.*)\.py')
-        dirs = []
-        for user_dir in self.cfg.mod_dirs():
-            if user_dir not in dirs:
-                dirs.append(user_dir)
-        dirs += [Path(__file__).parent.resolve() / 'modules']
-        mods = []
-        for mdir in dirs:
-            for mod_file in sorted(os.listdir(mdir)):
-                m = name_pattern.match(mod_file)
-                if m:
-                    path = (mdir / mod_file).resolve()
-                    name = m.group(2)
-                    loader = importlib.machinery.SourceFileLoader(name, str(path))
-                    spec = importlib.util.spec_from_loader(name, loader)
-                    mod = importlib.util.module_from_spec(spec)
-                    loader.exec_module(mod)
-                    if name in mod_priority:
-                        priority = mod_priority[name]
-                    else:
-                        priority = int(m.group(1))
-                    mods.append((priority, name, mod))
-
-        # Initialize in priority order.
-        for _, _, mod in sorted(mods):
-            print(f'Init:', mod.__doc__)
-            mod.init(self)
-
-    def shutdown_event(self):
-        """
-        Returns:
-            threading.Event: Event that is set when the server is
-            shutting down. Background workers must wait on this and stop
-            when the event is set.
-        """
-        return self.sv.shutdown_event
-
-    def call_entrypoint(self, request):
-        """
-        Calls the registered entry point for a request.
-
-        Args:
-            request (Request): Request object.
-
-        Returns:
-            Tuple with (response, cache). The response can be binary data, text,
-            tuple with status and meta string, or tuple with status, meta, and body.
-            The cache is None if the data was not read from a cache.
-        """
-        return self.sv.call_entrypoint(request)
+        self.sv = Server(cfg)
 
     def run(self):
         """
         Start worker threads and begin accepting incoming connections. The
         server will run until stopped with a KeyboardInterrupt (^C).
         """
-        self.sv.run(memtrace=self.cfg.debug_memtrace)
+        self.sv.run()
 
 
 def get_mime_type(path):
     """
     Determine the MIME type of a file. A handful of common file extensions
     are detected as special cases, such as ".gmi" and ".txt". Other files
     are detected with Python's ``mimetypes`` standard library module, and as
@@ -791,16 +690,14 @@
                       help='Configuration file to load at startup')
     argp.add_argument('--trace-malloc',
                       action='store_true',
                       help='Enable memory allocation tracing (for debugging)')
     args = argp.parse_args()
 
     cfg = Config(args.config_file)
-    cfg.debug_memtrace = args.trace_malloc
-
     try:
         capsule = Capsule(cfg)
         capsule.run()
         return 0
     except Exception as er:
         print('ERROR:', er)
         return -1
```

### Comparing `gmcapsule-0.4.1/gmcapsule/gemini.py` & `gmcapsule-0.5.0/gmcapsule/gemini.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # Copyright (c) 2021-2022 Jaakko Keränen <jaakko.keranen@iki.fi>
 # License: BSD-2-Clause
 
 import fnmatch
-import gc
 import hashlib
-import queue
+import importlib
 import os.path
 import select
 import socket
+import multiprocessing as mp
 import threading
+import queue
+import re
+import signal
 import time
+from pathlib import Path
 from urllib.parse import urlparse
 
 import OpenSSL.crypto
 from OpenSSL import SSL, crypto
 
 
 class GeminiError(Exception):
@@ -66,66 +70,79 @@
         except OpenSSL.SSL.WantWriteError:
             pass
         except OpenSSL.SSL.WantX509LookupError:
             pass
     return data
 
 
+def is_bytes(data):
+    return type(data) == bytes or type(data) == bytearray
+
+
 def safe_sendall(stream, data, stall_timeout=30):
     """
     Send data over an SSL connection, accounting for stalls and retries
     required by OpenSSL.
 
     Args:
         stream (OpenSSL.SSL.Connection): Network stream.
         data (bytes or file-like): Data to sent. If not a bytes/bytearray,
             ``read()`` will be called to get more data.
         stall_timeout (float): Number of seconds to wait until
             terminating a stalled send.
     """
-    if type(data) == bytes or type(data) == bytearray:
-        streaming = False
-    else:
-        streaming = True
-
-    # We may need to retry sending with the exact same buffer,
-    # so keep it around until successful.
-    BUF_LEN = 32768
-    if streaming:
-        send_buf = data.read(BUF_LEN)
-    else:
-        send_buf = data[:BUF_LEN]
+    try:
+        if is_bytes(data):
+            streaming = False
+        else:
+            streaming = True
+            if isinstance(data, Path):
+                print('opening', data)
+                data = open(data, 'rb')
+
+        # We may need to retry sending with the exact same buffer,
+        # so keep it around until successful.
+        BUF_LEN = 32768
+        if streaming:
+            send_buf = data.read(BUF_LEN)
+        else:
+            send_buf = data[:BUF_LEN]
 
-    last_time = time.time()
-    pos = 0
-    while len(send_buf) > 0:
-        try:
-            if time.time() - last_time > stall_timeout:
-                raise AbortedIOError('stalled')
-            sent = stream.send(send_buf)
-            if sent < 0:
-                raise AbortedIOError('failed to send')
-            pos += sent
-            if streaming:
-                send_buf = send_buf[sent:]
-                if len(send_buf) < BUF_LEN / 2:
-                    send_buf += data.read(BUF_LEN)
-            else:
-                send_buf = data[pos : pos + BUF_LEN]
-            if sent > 0:
-                last_time = time.time()
-            else:
+        last_time = time.time()
+        pos = 0
+        while len(send_buf) > 0:
+            try:
+                if time.time() - last_time > stall_timeout:
+                    raise AbortedIOError('stalled')
+                sent = stream.send(send_buf)
+                if sent < 0:
+                    raise AbortedIOError('failed to send')
+                pos += sent
+                if streaming:
+                    send_buf = send_buf[sent:]
+                    if len(send_buf) < BUF_LEN / 2:
+                        send_buf += data.read(BUF_LEN)
+                else:
+                    send_buf = data[pos : pos + BUF_LEN]
+                if sent > 0:
+                    last_time = time.time()
+                else:
+                    wait_for_write(stream, stall_timeout)
+            except OpenSSL.SSL.WantReadError:
+                pass
+            except OpenSSL.SSL.WantWriteError:
+                # Wait until the socket is ready for writing.
                 wait_for_write(stream, stall_timeout)
-        except OpenSSL.SSL.WantReadError:
-            pass
-        except OpenSSL.SSL.WantWriteError:
-            # Wait until the socket is ready for writing.
-            wait_for_write(stream, stall_timeout)
-        except OpenSSL.SSL.WantX509LookupError:
-            pass
+            except OpenSSL.SSL.WantX509LookupError:
+                pass
+
+    finally:
+        # Close resources and handles.
+        if data and hasattr(data, 'close'):
+            data.close()
 
 
 def safe_close(stream):
     if not stream:
         return
     try:
         stream.shutdown()
@@ -140,109 +157,68 @@
 def report_error(stream, code, msg):
     print(time.strftime('%Y-%m-%d %H:%M:%S'), f'   ', '--', code, msg)
     #stream.sendall(f'{code} {msg}\r\n'.encode('utf-8'))
     safe_sendall(stream, f'{code} {msg}\r\n'.encode('utf-8'))
     safe_close(stream)
 
 
-memtrace_lock = threading.Lock()
-
-
-def display_memtop(snapshot, prev_snapshot, key_type='lineno', limit=1000):
-    import tracemalloc
-    import linecache
-    filters = (
-        tracemalloc.Filter(False, "<frozen importlib._bootstrap>"),
-        tracemalloc.Filter(False, "<unknown>"),
-        tracemalloc.Filter(False, "*/linecache.py"),
-        tracemalloc.Filter(False, "*/tracemalloc.py")
-    )
-    snapshot = snapshot.filter_traces(filters)
-    if prev_snapshot:
-        prev_snapshot = prev_snapshot.filter_traces(filters)
-        top_stats = snapshot.compare_to(prev_snapshot, key_type)
-        top_type = 'delta'
-        limit = 200
-    else:
-        top_stats = snapshot.statistics('traceback') #key_type)
-        top_type = 'malloc'
-
-    with memtrace_lock:
-        print("\n\nTop %s %s" % (limit, top_type))
-        for index, stat in enumerate(top_stats[:limit], 1):
-            if prev_snapshot:
-                frame = stat.traceback[0]
-                if stat.size_diff <= 0:
-                    continue
-                print("#%s: \x1b[1m%.1f\x1b[0m KiB (%+.1f KiB) count=%d (%+d)"
-                    % (index,
-                       stat.size / 1024, stat.size_diff / 1024, stat.count, stat.count_diff))
-            else:
-                print("#%s: \x1b[1m%.1f\x1b[0m KiB count=%d"
-                      % (index, stat.size / 1024, stat.count))
-            for frame in stat.traceback:
-                line = linecache.getline(frame.filename, frame.lineno).strip()
-                if 'python3.' in frame.filename: continue
-                if line:
-                    print('\x1b[0;31m  %35s:%-5s ' % (frame.filename[-35:], str(frame.lineno) + ':'))
-                    print('\x1b[0;36m    %s\x1b[0m' % line)
-
-        other = top_stats[limit:]
-        if other:
-            size = sum(stat.size for stat in other)
-            print("%s other: %.1f KiB" % (len(other), size / 1024))
-        total = sum(stat.size for stat in top_stats)
-        print("Total size: %.1f KiB\n\n" % (total / 1024))
+def cert_subject(cert):
+    comps = {}
+    for name, value in cert.get_subject().get_components():
+        comps[name.decode()] = value.decode()
+    return comps
+
+def cert_issuer(cert):
+    comps = {}
+    for name, value in cert.get_issuer().get_components():
+        comps[name.decode()] = value.decode()
+    return comps
 
 
 class Identity:
     """
     Client certificate.
 
     SHA-256 hashes are calculated automatically for the whole certificate and
     just for the public key.
 
     Attributes:
-        cert (OpenSSL.SSL.X509): Certificate.
-        pubkey (OpenSSL.SSL.PKey): Public key.
+        cert (bytes): Certificate (DER format).
+        pubkey (bytes): Public key (DER format).
         fp_cert (str): SHA-256 hash of the certificate.
         fp_pubkey (str): SHA-256 hash of the public key.
     """
     def __init__(self, cert):
-        self.cert = cert
+        self._subject = cert_subject(cert)
+        self._issuer = cert_issuer(cert)
+        self.cert = crypto.dump_certificate(crypto.FILETYPE_ASN1, cert)
         m = hashlib.sha256()
-        m.update(crypto.dump_certificate(crypto.FILETYPE_ASN1, self.cert))
+        m.update(self.cert)
         self.fp_cert = m.hexdigest()
-        self.pubkey = self.cert.get_pubkey()
+        self.pubkey = crypto.dump_publickey(crypto.FILETYPE_ASN1, cert.get_pubkey())
         m = hashlib.sha256()
-        m.update(crypto.dump_publickey(crypto.FILETYPE_ASN1, self.pubkey))
+        m.update(self.pubkey)
         self.fp_pubkey = m.hexdigest()
 
     def __str__(self):
         return f"{self.fp_cert};{self.fp_pubkey}"
 
     def subject(self):
         """
         Returns:
-            dict: Name components of the certificate subject, e.g.: ``{'CN': 'Name'}``
+            dict: Name components of the certificate subject, e.g.: ``{'CN': 'Name'}``.
         """
-        comps = {}
-        for name, value in self.cert.get_subject().get_components():
-            comps[name.decode()] = value.decode()
-        return comps
+        return self._subject
 
     def issuer(self):
         """
         Returns:
-            dict: Name components of the certificate issuer, e.g.: ``{'CN': 'Name'}``
+            dict: Name components of the certificate issuer, e.g.: ``{'CN': 'Name'}``.
         """
-        comps = {}
-        for name, value in self.cert.get_issuer().get_components():
-            comps[name.decode()] = value.decode()
-        return comps
+        return self._issuer
 
 
 class Request:
     """
     Request received from a client.
 
     Request objects are used to pass information to entry points handlers.
@@ -262,24 +238,26 @@
         content_token (str): Encoded token specified in Titan URLs.
             May be ``None``.
         content_mime (str): MIME type specified in Titan URls. May be ``None``.
         content (bytes): Content uploaded by the client in a Titan request.
             May be ``None``.
     """
     def __init__(self, identity=None, scheme='gemini', hostname='', path='', query=None,
-                 remote_address=None, content_token=None, content_mime=None, content=None):
+                 remote_address=None, content_token=None, content_mime=None, content=None,
+                 worker_id=None):
         self.remote_address = remote_address
         self.scheme = scheme
         self.identity = identity
         self.hostname = hostname
         self.path = path
         self.query = query
         self.content_token = content_token
         self.content_mime = content_mime
         self.content = content
+        self.worker_id = worker_id
 
     def url(self):
         return f'{self.scheme}://{self.hostname}{self.path}{"?" + self.query if self.query else ""}'
 
 
 def verify_callback(connection, cert, err_num, err_depth, ret_code):
     #print("verify_callback:", connection, cert, ret_code)
@@ -294,14 +272,18 @@
     methods to save and load response content as appropriate.
 
     The server will not try to load or save cached content when a request
     includes a query string or a client certificate is provided. When multiple
     Cache objects have been installed, the save/load operation is attempted
     on each in turn until one cache succeeds in saving or loading content.
 
+    Each server worker thread constructs their own Cache objects. If there
+    is a shared backing store like a file system or a database, proper care
+    should be taken to synchronize access to it from the Cache objects.
+
     The mapping from URLs to cache paths is::
 
         gemini://example.com/path/file.gmi
          ↓
         /example.com/path/file.gmi
 
     """
@@ -335,59 +317,417 @@
         Returns:
             tuple(str, bytes): Content MIME type and data. Returns
             (None, None) if nothing is cached for the given path.
         """
         return None, None
 
 
-class Worker(threading.Thread):
-    """Thread that processes incoming requests from clients."""
+def handle_gemini_or_titan_request(request_data):
+    worker = request_data.worker
+    stream = request_data.stream
+    data = request_data.buffered_data
+    from_addr = request_data.from_addr
+    identity = request_data.identity
+    request = request_data.request
+    expected_size = 0
+    req_token = None
+    req_mime = None
+
+    if request.startswith('titan:'):
+        if identity is None and worker.cfg.require_upload_identity():
+            report_error(stream, 60, "Client certificate required for upload")
+            return
+        # Read the rest of the data.
+        parms = request.split(';')
+        request = parms[0]
+        for p in parms:
+            if p.startswith('size='):
+                expected_size = int(p[5:])
+            elif p.startswith('token='):
+                req_token = p[6:]
+            elif p.startswith('mime='):
+                req_mime = p[5:]
+        worker.log(f'Receiving Titan content: {expected_size}')
+        max_upload_size = worker.cfg.max_upload_size()
+        if expected_size > max_upload_size and max_upload_size > 0:
+            report_error(stream, 59, "Maximum content length exceeded")
+            return
+        while len(data) < expected_size:
+            incoming = safe_recv(stream, 65536)
+            if len(incoming) == 0:
+                break
+            data += incoming
+        if len(data) != expected_size:
+            report_error(stream, 59, "Invalid content length")
+            return
+    else:
+        # No Payload in Gemini.
+        if len(data):
+            report_error(stream, 59, "Bad request")
+            return
+
+    url = urlparse(request)
+    path = url.path
+    if path == '':
+        path = '/'
+    hostname = url.hostname
+
+    if url.port != None and url.port != worker.port:
+        report_error(stream, 59, "Invalid port number")
+        return
+    if not stream.get_servername():
+        # Server name indication is required.
+        report_error(stream, 59, "Missing TLS server name indication")
+        return
+    if stream.get_servername().decode() != hostname:
+        report_error(stream, 53, "Proxy request refused")
+        return
+
+    try:
+        status, meta, body, from_cache = worker.context.call_entrypoint(Request(
+            identity,
+            remote_address=from_addr,
+            scheme=url.scheme,
+            hostname=hostname,
+            path=path,
+            query=url.query if '?' in request else None,
+            content_token=req_token,
+            content_mime=req_mime,
+            content=data if len(data) else None,
+            worker_id=request_data.worker.id
+        ))
+
+        output = f'{status} {meta}\r\n'.encode('utf-8')
+        if is_bytes(body):
+            safe_sendall(stream, output + body)
+        else:
+            # `body` is some sort of streamable data, cannot send in one call.
+            safe_sendall(stream, output)
+            safe_sendall(stream, body)
+
+        # Save to cache.
+        if not from_cache and status == 20 and is_bytes(body):
+            for cache in worker.context.caches:
+                if cache.save(hostname + path, meta, body):
+                    break
+
+    except GeminiError as error:
+        report_error(stream, error.status, str(error))
+        return
+
+
+def unpack_response(response):
+    if type(response) == tuple:
+        if len(response) == 2:
+            status, meta = response
+            response = ''
+        else:
+            status, meta, response = response
+    else:
+        status = 20
+        meta = 'text/gemini; charset=utf-8'
+
+    if response == None:
+        body = b''
+    elif type(response) == str:
+        body = response.encode('utf-8')
+    else:
+        body = response
+
+    return status, meta, body
+
+
+class Context:
+    def __init__(self, cfg, allow_extension_workers=False, handler_queue=None,
+                 response_queues=None):
+        self.cfg = cfg
+        self.is_quiet = True
+        self.allow_extension_workers = allow_extension_workers
+        if allow_extension_workers:
+            self.shutdown = threading.Event()
+        self.hostnames = cfg.hostnames()
+        self.entrypoints = {'gemini': {}, 'titan': {}}
+        for proto in ['gemini', 'titan']:
+            self.entrypoints[proto] = {}
+            for hostname in self.hostnames:
+                self.entrypoints[proto][hostname] = []
+        self.caches = []
+        self.protocols = {}
+        self.add_protocol('gemini', handle_gemini_or_titan_request)
+        self.add_protocol('titan', handle_gemini_or_titan_request)
+        # Queue for pending handler jobs.
+        self.job_lock = threading.Lock()
+        self.job_id = 0
+        self.handler_queue = handler_queue
+        self.response_queues = response_queues
+
+    def config(self):
+        return self.cfg
+
+    def is_background_work_allowed(self):
+        """
+        Determines whether extension modules are allowed to start workers.
+        """
+        return self.allow_extension_workers
+
+    def shutdown_event(self):
+        """
+        Returns:
+            threading.Event: Extension modules must check this to be notified
+            when the server is being shut down.
+        """
+        if not self.is_background_work_allowed():
+            raise Exception("background work not allowed")
+        # This is used in a parser thread that is allowed to launch workers.
+        return self.shutdown
+
+    def set_quiet(self, is_quiet):
+        self.is_quiet = is_quiet
+
+    def print(self, *args):
+        if not self.is_quiet:
+            print(*args)
 
-    def __init__(self, id, server):
+    def add_entrypoint(self, protocol, hostname, path_pattern, entrypoint):
+        self.entrypoints[protocol][hostname].append((path_pattern, entrypoint))
+
+    def __setitem__(self, key, value):
+        for hostname in self.hostnames:
+            self.add_entrypoint('gemini', hostname, key, value)
+
+    def add_cache(self, cache):
+        """
+        Install a cache.
+
+        All installed caches will attempt to save and load content until one
+        succeeds. The caches installed first get precedence.
+
+        Args:
+            cache (Cache): Cache instance.
+        """
+        self.caches.append(cache)
+
+    def add_protocol(self, scheme, handler):
+        """
+        Registers a new protocol handler.
+
+        Args:
+            scheme (str): URL scheme of the protocol.
+            handler (callable): Handler to be called when a request with the
+                specified scheme is received. The handler must return the
+                response to be sent to the client (bytes).
+        """
+        self.protocols[scheme] = handler
+
+    def add(self, path, entrypoint, hostname=None, protocol='gemini'):
+        """
+        Register a URL entry point.
+
+        Extension modules must call this to become visible in the server's
+        path hierarchy. Entry points are looked up in the order the modules
+        were loaded, with earlier modules getting precedence.
+
+        Args:
+            path (str): URL path. Must begin with a slash (``/``). Asterisk
+                wildcards (``*``) are supported. Note that if the path
+                ``/*`` is registered, it will match any requested URL.
+            entrypoint (callable): Function or other callable object that
+                gets called when a request is processed with a matching
+                URL path. A :class:`~gmcapsule.gemini.Request` is passed in as the
+                only argument.
+            hostname (str): Hostname for the entry point. If omitted,
+                the entry point applies to all configured hostnames.
+            protocol (str): Protocol for the entry point.
+        """
+        if hostname:
+            self.add_entrypoint(protocol, hostname, path, entrypoint)
+        else:
+            for hostname in self.cfg.hostnames():
+                if not hostname:
+                    raise Exception(f'invalid hostname: "{hostname}"')
+                self.add_entrypoint(protocol, hostname, path, entrypoint)
+
+    def load_modules(self):
+        # The configuration can override default priorities.
+        mod_priority = {}
+        if 'priority' in self.cfg.ini:
+            for name, priority in self.cfg.section('priority').items():
+                mod_priority[name] = int(priority)
+
+        # We will load all recognized modules.
+        name_pattern = re.compile(r'([0-9][0-9])_(.*)\.py')
+        dirs = []
+        for user_dir in self.cfg.mod_dirs():
+            if user_dir not in dirs:
+                dirs.append(user_dir)
+        dirs += [Path(__file__).parent.resolve() / 'modules']
+        mods = []
+        for mdir in dirs:
+            for mod_file in sorted(os.listdir(mdir)):
+                m = name_pattern.match(mod_file)
+                if m:
+                    path = (mdir / mod_file).resolve()
+                    name = m.group(2)
+                    loader = importlib.machinery.SourceFileLoader(name, str(path))
+                    spec = importlib.util.spec_from_loader(name, loader)
+                    mod = importlib.util.module_from_spec(spec)
+                    loader.exec_module(mod)
+                    if name in mod_priority:
+                        priority = mod_priority[name]
+                    else:
+                        priority = int(m.group(1))
+                    mods.append((priority, name, mod))
+
+        # Initialize in priority order.
+        for _, name, mod in sorted(mods):
+            self.print(f'Init:', mod.__doc__ if mod.__doc__ else name)
+            mod.init(self)
+
+    def find_entrypoint(self, protocol, hostname, path):
+        try:
+            for entry in self.entrypoints[protocol][hostname]:
+                path_pattern, handler = entry
+                if handler != None:
+                    # A path string, possibly with wildcards.
+                    if len(path_pattern) == 0 or fnmatch.fnmatch(path, path_pattern):
+                        return handler
+                else:
+                    # A callable generic path matcher.
+                    handler = path_pattern(path)
+                    if handler:
+                        return handler
+        except Exception as x:
+            print(x)
+            return None
+
+        return None
+
+    def call_entrypoint(self, request):
+        """
+        Calls the registered entry point for a request.
+
+        Args:
+            request (Request): Request object.
+
+        Returns:
+            tuple: (status, meta, body, cache). The type of body can be bytes,
+            bytearray, or pathlib.Path. Returning a pathlib.Path means that
+            the body will be read from the referenced file. The cache is None
+            if the data was not read from a cache.
+        """
+        entrypoint = self.find_entrypoint(request.scheme, request.hostname, request.path)
+
+        caches = self.caches if (request.scheme == 'gemini' and
+                                 not request.identity and
+                                 not request.query) else []
+        from_cache = None
+
+        if entrypoint:
+            # Check the caches first.
+            for cache in caches:
+                media, content = cache.try_load(request.hostname + request.path)
+                if not media is None:
+                    if hasattr(content, '__len__'):
+                        self.print('%d bytes from cache, %s' % (len(content), media))
+                    else:
+                        self.print('stream from cache,', media)
+                    return 20, media, content, cache
+
+            # Process the request normally if there is nothing cached.
+            if not from_cache:
+                try:
+                    if not self.handler_queue:
+                        # Handle in the same thread/process synchronously. This is probably
+                        # running under a RequestHandler process.
+                        response = entrypoint(request)
+                    else:
+                        # Put it in the handler queue and wait for completion. Parser threads use
+                        # this to hand work off to the handler processes.
+                        with self.job_lock:
+                            # The job ID is for verifying we are getting the right response.
+                            self.job_id += 1
+                            job_id = self.job_id
+
+                        self.handler_queue.put((job_id, request, request.worker_id))
+                        result_id, response = self.response_queues[request.worker_id].get()
+
+                        if result_id != job_id:
+                            raise Exception('response queue out of sync: request handler returned wrong job ID')
+                        if isinstance(response, Exception):
+                            raise response
+
+                    status, meta, body = unpack_response(response)
+
+                    return status, meta, body, None
+
+                except Exception as x:
+                    import traceback
+                    traceback.print_exception(x)
+                    raise GeminiError(40, 'Temporary failure')
+
+        raise GeminiError(50, 'Permanent failure')
+
+
+class RequestData:
+    """Encapsules data about an incoming request, before it has been fully parsed."""
+
+    def __init__(self, worker, stream, buffered_data, from_addr, identity, request):
+        self.worker = worker
+        self.stream = stream
+        self.buffered_data = buffered_data
+        self.from_addr = from_addr
+        self.identity = identity
+        self.request = request
+
+
+class RequestParser(threading.Thread):
+    """Thread that parses incoming requests from clients."""
+
+    def __init__(self, id, context, job_queue):
         super().__init__()
         self.id = id
-        self.server = server
-        self.jobs = server.work_queue
+        self.context = context
+        self.cfg = context.cfg
+        self.port = self.cfg.port()
+        self.jobs = job_queue
 
     def run(self):
-        while True:
-            stream, from_addr = self.jobs.get()
-            if stream is None:
-                break
-
-            try:
-                self.process_request(stream, from_addr)
-            except OpenSSL.SSL.SysCallError as error:
-                self.log(f'OpenSSL error: ' + str(error))
-            except AbortedIOError as error:
-                self.log(f'Send aborted: ' + str(error))
-            except Exception as error:
-                self.log(f'Problem: ' + str(error))
-                # Some unexpected problem...
-                #import traceback
-                #traceback.print_exc()
-                # try:
-                #     report_error(stream, 42, str(error))
-                # except:
-                #     pass
-
-            safe_close(stream)
-            stream, from_addr = None, None
+        try:
+            while True:
+                stream, from_addr = self.jobs.get()
+                if stream is None:
+                    break
+                try:
+                    self.process_request(stream, from_addr)
+                except OpenSSL.SSL.SysCallError as error:
+                    self.log(f'OpenSSL error: ' + str(error))
+                except AbortedIOError as error:
+                    self.log(f'Send aborted: ' + str(error))
+                except Exception as error:
+                    self.log(f'Problem: ' + str(error))
+                    # Some unexpected problem...
+                    #import traceback
+                    #traceback.print_exc()
+                    # try:
+                    #     report_error(stream, 42, str(error))
+                    # except:
+                    #     pass
+                safe_close(stream)
+                stream, from_addr = None, None
+        except KeyboardInterrupt:
+            pass
 
     def log(self, *args):
         print(time.strftime('%Y-%m-%d %H:%M:%S'), f'[{self.id}]', '--', *args)
 
     def process_request(self, stream, from_addr):
         data = bytes()
-        MAX_LEN = 1024
+        MAX_LEN = 1024  # TODO: Gemini/Titan limitation only.
         MAX_RECV = MAX_LEN + 2  # includes terminator "\r\n"
         request = None
-        expected_size = 0
-        req_token = None
-        req_mime = None
         incoming = safe_recv(stream, MAX_RECV)
 
         try:
             while len(data) < MAX_RECV:
                 data += incoming
                 crlf_pos = data.find(b'\r\n')
                 if crlf_pos >= 0:
@@ -404,187 +744,114 @@
                 if len(incoming) <= 0:
                     break
         except UnicodeDecodeError:
             report_error(stream, 59, "Request contains malformed UTF-8")
             return
 
         if not request or len(data) > MAX_RECV:
-            report_error(stream, 59, "Invalid request")
-            return
-        if not (request.startswith('gemini:') or request.startswith('titan:')):
-            report_error(stream, 59, "Unsupported protocol")
+            report_error(stream, 59, "Bad request")
             return
 
         cl_cert = stream.get_peer_certificate()
         identity = Identity(cl_cert) if cl_cert else None
 
-        if request.startswith('titan:'):
-            if identity is None and self.server.require_upload_identity:
-                report_error(stream, 60, "Client certificate required for upload")
+        for scheme, handler in self.context.protocols.items():
+            if request.startswith(scheme + ':'):
+                self.log(request)
+                response = handler(RequestData(self, stream, data, from_addr, identity, request))
+                if not response is None:
+                    safe_sendall(stream, response)
                 return
 
-            # Read the rest of the data.
-            parms = request.split(';')
-            request = parms[0]
-            for p in parms:
-                if p.startswith('size='):
-                    expected_size = int(p[5:])
-                elif p.startswith('token='):
-                    req_token = p[6:]
-                elif p.startswith('mime='):
-                    req_mime = p[5:]
-            self.log(f'Receiving Titan content: {expected_size}')
-            if expected_size > self.server.max_upload_size and self.server.max_upload_size > 0:
-                report_error(stream, 59, "Maximum content length exceeded")
-                return
-            while len(data) < expected_size:
-                incoming = safe_recv(stream, 65536)
-                if len(incoming) == 0:
-                    break
-                data += incoming
-            if len(data) != expected_size:
-                report_error(stream, 59, "Invalid content length")
-                return
-        else:
-            # No Payload in Gemini.
-            if len(data):
-                report_error(stream, 59, "Gemini disallows request content")
-                return
+        report_error(stream, 59, "Unsupported protocol")
 
-        self.log(request)
 
-        url = urlparse(request)
-        path = url.path
-        if path == '':
-            path = '/'
-        hostname = url.hostname
+class ServerRestarter:
+    def __init__(self, server):
+        self.server = server
 
-        if url.port != None and url.port != self.server.port:
-            report_error(stream, 59, "Invalid port number")
-            return
-        if not stream.get_servername():
-            # Server name indication is required.
-            report_error(stream, 59, "Missing TLS server name indication")
-            return
-        if stream.get_servername().decode() != hostname:
-            report_error(stream, 53, "Proxy request refused")
-            return
+    def __call__(self, signum, frame):
+        if signum == signal.SIGHUP:
+            print('--- SIGHUP ---')
+            self.server.restart_workers()
 
+
+class RequestHandler(mp.Process):
+    def __init__(self, id, cfg, job_queue, result_queues):
+        super().__init__(target=RequestHandler._run, args=(self,))
+        self.id = id
+        self.cfg = cfg
+        self.jobs = job_queue
+        self.results = result_queues
+        self.context = None
+
+    def _run(self):
+        self.context = Context(self.cfg)
+        self.context.load_modules()
+
+        # Wait for request processing jobs.
         try:
-            request = Request(
-                identity,
-                remote_address=from_addr,
-                scheme=url.scheme,
-                hostname=hostname,
-                path=path,
-                query=url.query if '?' in request else None,
-                content_token=req_token,
-                content_mime=req_mime,
-                content=data if len(data) else None
-            )
-            response, from_cache = self.server.call_entrypoint(request)
-
-            # Determine status code, meta line, and body content.
-            if type(response) == tuple:
-                if len(response) == 2:
-                    status, meta = response
-                    response = ''
-                else:
-                    status, meta, response = response
-            else:
-                status = 20
-                meta = 'text/gemini; charset=utf-8'
-
-            if response == None:
-                response_data = b''
-            elif type(response) == str:
-                response_data = response.encode('utf-8')
-            else:
-                response_data = response
-
-            safe_sendall(stream, f'{status} {meta}\r\n'.encode('utf-8'))
-            safe_sendall(stream, response_data)
-
-            # Save to cache.
-            if not from_cache and status == 20 and \
-                    (type(response_data) == bytes or type(response_data) == bytearray):
-                for cache in self.server.caches:
-                    if cache.save(hostname + path, meta, response_data):
-                        break
-
-            # Close handles.
-            if hasattr(response_data, 'close'):
-                response_data.close()
+            while True:
+                job_id, request, queue_id = self.jobs.get()
+                if job_id is None:
+                    break
+                result_queue = self.results[queue_id]
+                entrypoint = self.context.find_entrypoint(request.scheme, request.hostname, request.path)
+                if not entrypoint:
+                    result_queue.put((job_id, Exception("Missing entrypoint: " + request.url())))
+                    continue
+                try:
+                    response = unpack_response(entrypoint(request))
+                    result_queue.put((job_id, response))
 
-        except GeminiError as error:
-            report_error(stream, error.status, str(error))
-            return
+                except Exception as error:
+                    result_queue.put((job_id, error))
+
+        except KeyboardInterrupt:
+            pass
 
 
 class Server:
-    def __init__(self, hostname_or_hostnames, cert_path, key_path,
-                 address='localhost', port=1965,
-                 cache=None, session_id=None, max_upload_size=0, num_threads=1,
-                 require_upload_identity=True):
-        self.hostnames = [hostname_or_hostnames] \
-            if type(hostname_or_hostnames) == str else hostname_or_hostnames
-        self.address = address
-        self.port = port
-        self.entrypoints = {'gemini': {}, 'titan': {}}
-        for proto in ['gemini', 'titan']:
-            self.entrypoints[proto] = {}
-            for hostname in self.hostnames:
-                self.entrypoints[proto][hostname] = []
-        self.caches = []
-        if cache:
-            self.caches.append(cache)
-        self.max_upload_size = max_upload_size
-        self.require_upload_identity = require_upload_identity
+    def __init__(self, cfg):
+        mp.set_start_method('spawn')
+
+        self.cfg = cfg
+        self.address = cfg.address()
+        self.port = cfg.port()
+
+        cert_path = cfg.certs_dir() / 'cert.pem'
+        key_path = cfg.certs_dir() / 'key.pem'
 
         if not os.path.exists(cert_path):
             raise Exception("certificate file not found: " + str(cert_path))
         if not os.path.exists(key_path):
             raise Exception("private key file not found: " + str(key_path))
 
         self.context = SSL.Context(SSL.TLS_SERVER_METHOD)
         self.context.use_certificate_file(str(cert_path))
         self.context.use_privatekey_file(str(key_path))
         self.context.set_verify(SSL.VERIFY_PEER, verify_callback)
-        if session_id:
-            if type(session_id) != bytes:
-                raise Exception("session_id type must be `bytes`")
-            self.context.set_session_id(session_id)
+
+        session_id = f'GmCapsule:{cfg.port()}'.encode('utf-8')
+        #if type(session_id) != bytes:
+        #    raise Exception("session_id type must be `bytes`")
+        self.context.set_session_id(session_id)
 
         # Spawn the worker threads.
-        self.shutdown_event = threading.Event()
-        self.workers = []
-        self.work_queue = queue.Queue()
-        for worker_id in range(max(num_threads, 1)):
-            worker = Worker(worker_id, self)
-            self.workers.append(worker)
+        self.parser_queue = queue.Queue()
+        self.handler_queue = mp.Queue()
+        self.init_parser_context()
+        self.parsers = []
+        self.handlers = []
+        self.create_workers(cfg)
 
         self.sock = None
         self.sv_conn = None
 
-    def add_cache(self, cache):
-        self.caches.append(cache)
-
-    def add_entrypoint(self, protocol, hostname, path_pattern, entrypoint):
-        self.entrypoints[protocol][hostname].append((path_pattern, entrypoint))
-
-    def __setitem__(self, key, value):
-        for hostname in self.hostnames:
-            self.add_entrypoint('gemini', hostname, key, value)
-
-    def run(self, memtrace=False):
-        self.memtrace = memtrace
-        if self.memtrace:
-            import tracemalloc
-            tracemalloc.start(10)
-
+    def run(self):
         attempts = 60
         print(f'Opening port {self.port}...')
         while True:
             try:
                 self.sock = socket.socket()
                 self.sock.bind((self.address, self.port))
                 self.sock.listen(5)
@@ -595,117 +862,105 @@
                 attempts -= 1
                 if attempts == 0:
                     raise Exception(f'Failed to open port {self.port} for listening')
                 time.sleep(2.0)
                 print('...')
         print(f'Server started on port {self.port}')
 
-        MULTITHREAD = True
+        self.start_workers()
 
-        if MULTITHREAD:
-            for worker in self.workers:
-                worker.start()
-            print(len(self.workers), 'worker(s) started')
-
-        snapshot = None
+        try:
+            signal.signal(signal.SIGHUP, ServerRestarter(self))
+        except ValueError:
+            print('Restarting with SIGHUP not supported')
 
         while True:
             stream = None
             try:
                 stream, from_addr = self.sv_conn.accept()
                 stream._socket.settimeout(10)
-                self.work_queue.put((stream, from_addr))
-
-                if not MULTITHREAD:
-                    self.work_queue.put((None, None)) # single iteration only
-                    self.workers[0].run()
-
+                self.parser_queue.put((stream, from_addr))
                 del stream
                 del from_addr
             except KeyboardInterrupt:
                 print('\nStopping the server...')
                 break
             except Exception as ex:
                 #import traceback
                 #traceback.print_exc()
                 print(ex)
 
-            if self.memtrace:
-                old_snapshot = snapshot
-                gc.collect()
-                snapshot = tracemalloc.take_snapshot()
-                filters = (
-                    tracemalloc.Filter(False, "<frozen importlib._bootstrap>"),
-                    tracemalloc.Filter(False, "<unknown>"),
-                    tracemalloc.Filter(False, "*/linecache.py"),
-                    tracemalloc.Filter(False, "*/tracemalloc.py"),
-                    tracemalloc.Filter(False, "*/mimetypes.py"),
-                    tracemalloc.Filter(False, "*/fnmatch.py")
-                )
-                snapshot = snapshot.filter_traces(filters)
-                top_stats = snapshot.statistics('lineno')
-                display_memtop(snapshot, None) #old_snapshot)
-
         # Close the server socket.
         self.sv_conn = None
         self.sock.close()
         self.sock = None
 
         # Stop all workers.
-        self.shutdown_event.set()
-        if MULTITHREAD:
-            for i in range(len(self.workers)):
-                self.work_queue.put((None, None))
-            for worker in self.workers:
-                worker.join()
+        self.stop_workers()
 
         print('Done')
 
-    def find_entrypoint(self, protocol, hostname, path):
-        try:
-            for entry in self.entrypoints[protocol][hostname]:
-                path_pattern, handler = entry
-                if handler != None:
-                    # A path string, possibly with wildcards.
-                    if len(path_pattern) == 0 or fnmatch.fnmatch(path, path_pattern):
-                        return handler
-                else:
-                    # A callable generic path matcher.
-                    handler = path_pattern(path)
-                    if handler:
-                        return handler
-        except Exception as x:
-            print(x)
-            return None
-
-        return None
-
-    def call_entrypoint(self, request):
-        entrypoint = self.find_entrypoint(request.scheme, request.hostname, request.path)
-
-        caches = self.caches if (request.scheme == 'gemini' and
-                                 not request.identity and
-                                 not request.query) else []
-        from_cache = None
-
-        if entrypoint:
-            # Check the caches first.
-            for cache in caches:
-                media, content = cache.try_load(request.hostname + request.path)
-                if not media is None:
-                    response = 20, media, content
-                    if hasattr(content, '__len__'):
-                        print('%d bytes from cache, %s' % (len(content), media))
-                    else:
-                        print('stream from cache,', media)
-                    return response, cache
-
-            # Process the request normally if there is nothing cached.
-            if not from_cache:
-                try:
-                    return entrypoint(request), None
-                except Exception as x:
-                    import traceback
-                    traceback.print_exception(x)
-                    raise GeminiError(40, 'Temporary failure')
+    def init_parser_context(self):
+        self.handler_results = []
+        if self.is_using_handler_processes():
+            for _ in range(max(self.cfg.num_threads(), 1)):
+                # Handler processes put results in these queues.
+                self.handler_results.append(mp.Queue())
+        self.parser_context = Context(self.cfg,
+                                      allow_extension_workers=True,
+                                      handler_queue=self.handler_queue if self.is_using_handler_processes() else None,
+                                      response_queues=self.handler_results if self.is_using_handler_processes() else None)
+        self.parser_context.set_quiet(False)
+        self.parser_context.load_modules()
 
-        raise GeminiError(50, 'Permanent failure')
+    def restart_workers(self):
+        """
+        Restarts workers with an updated configuration. The server socket or
+        TLS configuration are not modified, even if the values have changed
+        in the configuration file.
+        """
+        self.stop_workers()
+        self.cfg.reload()
+        self.init_parser_context()
+        self.create_workers(self.cfg)
+        self.start_workers()
+
+    def is_using_handler_processes(self):
+        return self.cfg.num_processes() > 0
+
+    def create_workers(self, cfg):
+        for proc_id in range(max(cfg.num_processes(), 0)):
+            proc = RequestHandler(proc_id, cfg, self.handler_queue, self.handler_results)
+            self.handlers.append(proc)
+
+        for parser_id in range(max(cfg.num_threads(), 1)):
+            # Threads share one context (note: GIL).
+            parser = RequestParser(parser_id, self.parser_context, self.parser_queue)
+            self.parsers.append(parser)
+
+    def start_workers(self):
+        for handler in self.handlers:
+            handler.start()
+        for parser in self.parsers:
+            parser.start()
+
+        print(len(self.parsers), 'parser(s) and', len(self.handlers), 'handler(s) started')
+
+    def stop_workers(self):
+        self.parser_context.shutdown.set()
+
+        # Stop parsers first so all ongoing handler processes get to finish, and no new
+        # requests can come in.
+        for _ in range(len(self.parsers)):
+            self.parser_queue.put((None, None))
+        for _ in range(len(self.handlers)):
+            self.handler_queue.put((None, None, None))
+
+        for p in self.parsers:
+            p.join()
+        for h in self.handlers:
+            h.join()
+
+        print(len(self.parsers), 'parser(s) and', len(self.handlers), 'handler(s) stopped')
+        self.parsers = []
+        self.handlers = []
+        self.parser_context.shutdown.clear()
```

### Comparing `gmcapsule-0.4.1/gmcapsule/markdown.py` & `gmcapsule-0.5.0/gmcapsule/markdown.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.4.1/gmcapsule/modules/80_gitview.py` & `gmcapsule-0.5.0/gmcapsule/modules/80_gitview.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import pickle
 import re
 import subprocess
 import time
 import urllib
 from pathlib import Path
 
-from gmcapsule import Cache, Capsule, markdown_to_gemtext
+from gmcapsule import Cache, markdown_to_gemtext
 
 pjoin = os.path.join
 
 
 class GitViewCache(Cache):
     """
     File-based cache that stores content using ``pickle``.
@@ -65,14 +65,15 @@
             return False
         storage_path = pjoin(self.file_root, self.storage_path(path))
         os.makedirs(os.path.dirname(storage_path), exist_ok=True)
         pickle.dump((media_type, content), open(storage_path, 'wb'))
         return True
 
 
+CONFIG = None
 GIT = '/usr/bin/git'
 HOSTNAME = 'localhost'
 NUM_COMMITS_FRONT = 8
 NUM_COMMITS_PER_PAGE = 25
 NUM_COMMITS_PER_TAG = 10
 
 # Link Icons
@@ -91,15 +92,15 @@
 def preformat(raw, alt_text=''):
     raw = raw.replace('\n```', '\n ```')
     return f'```{alt_text}\n' + raw + '\n```\n'
 
 
 def repositories():
     roots = []
-    for name, cfg in Capsule.config().prefixed_sections('gitview.').items():
+    for name, cfg in CONFIG.prefixed_sections('gitview.').items():
         url = cfg['url_root']
         if not url.startswith('/'): url = '/' + url
         if not url.endswith('/'): url += '/'
         roots.append((name, url, cfg))
     return roots
 
 
@@ -338,15 +339,15 @@
             return 51, "Not Found"
         info = info[0]
         hash = info['hash']
         full_hash = info['fullHash']
         email_subject = urllib.parse.quote(f"{req.cfg['title']} commit {hash}")
         email_body = urllib.parse.quote("=> gemini://%s:%d%scommits/%s" %
             (HOSTNAME,
-            Capsule.config().port(),
+            CONFIG.port(),
             req.url_root + req.ubranch,
             full_hash)
         )
         tags = []
         for ref in info['refs'].split(','):
             ref = ref.strip()
             if ref.startswith('tag:'):
@@ -461,32 +462,36 @@
     for name, url_root, repo_cfg in sorted(repositories()):
         page += f"\n=> {url_root + repo_cfg['default_branch'].replace('/', '%2F') + '/'} {repo_cfg['title']}\n"
         if 'brief' in repo_cfg:
             page += repo_cfg['brief'] + '\n'
     return page
 
 
-def init(capsule):
-    cfg = capsule.config()
+def init(context):
+    cfg = context.config()
+
+    global CONFIG
+    CONFIG = cfg
+
     try:
         mod_cfg = cfg.section('gitview')
 
         global GIT
         GIT = mod_cfg.get('git', fallback=GIT)
 
         global HOSTNAME
         HOSTNAME = mod_cfg.get('host', fallback=None)
         if HOSTNAME is None:
             HOSTNAME = cfg.hostnames()[0]
 
         if 'cache_path' in mod_cfg:
-            capsule.add_cache(GitViewCache(HOSTNAME, mod_cfg['cache_path']))
+            context.add_cache(GitViewCache(HOSTNAME, mod_cfg['cache_path']))
 
         for name, url_root, _ in repositories():
-            print(f'  Adding repository "{name}"...')
-            capsule.add('/', main_page, hostname=HOSTNAME)
-            capsule.add(url_root[:-1], redirect_to_default, hostname=HOSTNAME)
-            capsule.add(url_root + '*', handle_request, hostname=HOSTNAME)
+            context.print(f'  Adding repository "{name}"...')
+            context.add('/', main_page, hostname=HOSTNAME)
+            context.add(url_root[:-1], redirect_to_default, hostname=HOSTNAME)
+            context.add(url_root + '*', handle_request, hostname=HOSTNAME)
 
     except KeyError:
         # GitView not configured.
         pass
```

### Comparing `gmcapsule-0.4.1/gmcapsule/modules/90_cgi.py` & `gmcapsule-0.5.0/gmcapsule/modules/90_cgi.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 import os
 import pathlib
 import shlex
 import subprocess
 import urllib.parse
 
 import gmcapsule
-from gmcapsule import Capsule
 
 
 class CgiContext:
-    def __init__(self, url_path, args, work_dir=None):
+    def __init__(self, port, url_path, args, work_dir=None):
+        self.port = port
         self.args = args
         self.base_path = url_path
         if self.base_path.endswith('/*'):
             self.base_path = self.base_path[:-2]
         self.work_dir = work_dir
 
     def __call__(self, req):
@@ -31,15 +31,15 @@
             if req.query != None:
                 env_vars['QUERY_STRING'] = req.query
             env_vars['PATH_INFO'] = req.path
             env_vars['SCRIPT_NAME'] = self.base_path
             env_vars['SERVER_SOFTWARE'] = 'GmCapsule/' + gmcapsule.__version__
             env_vars['SERVER_PROTOCOL'] = req.scheme.upper()
             env_vars['SERVER_NAME'] = req.hostname
-            env_vars['SERVER_PORT'] = str(Capsule.config().port())
+            env_vars['SERVER_PORT'] = str(self.port)
             env_vars[req.scheme.upper() + '_URL'] = f"{req.scheme}://{req.hostname}{req.path}" + (
                 '?' + req.query if req.query != None else '')
             env_vars[req.scheme.upper() + '_URL_PATH'] = req.path
 
             # TLS client certificate.
             if req.identity:
                 env_vars['AUTH_TYPE'] = 'Certificate'
@@ -85,71 +85,72 @@
                 except:
                     return 20, 'application/octet-stream', result
         except Exception as er:
             return 42, "CGI error: " + str(er)
 
 
 class CgiTreeMapper:
-    def __init__(self, protocol, host, root_dir):
+    def __init__(self, protocol, host, port, root_dir):
         self.protocol = protocol
         self.host = host
+        self.port = port
         self.root_dir = pathlib.Path(root_dir)
 
     def __call__(self, url_path):
         # Check if url_path is a valid CGI entrypoint and return
         # a CgiContext for it.
         fn = str(self.root_dir) + url_path
         if self.protocol == 'titan':
             fn += ',titan'
         if os.path.isdir(fn):
             return None
         if os.access(fn, os.X_OK):
-            return CgiContext(url_path, [fn], work_dir=os.path.dirname(fn))
+            return CgiContext(self.port, url_path, [fn], work_dir=os.path.dirname(fn))
         return None
 
 
 # # NOTE: This require restarting the server when binaries are added/removed.
-# def add_cgibin_entrypoints_recursively(capsule, host, base, cur_dir=None):
+# def add_cgibin_entrypoints_recursively(context, host, base, cur_dir=None):
 #     if cur_dir is None:
 #         cur_dir = base
 #     for name in os.listdir(cur_dir):
 #         fn = cur_dir / name
 #         if os.path.isdir(fn):
-#             add_cgibin_entrypoints_recursively(capsule, host, base, fn)
+#             add_cgibin_entrypoints_recursively(context, host, base, fn)
 #         elif os.access(fn, os.X_OK):
 #             protocol = 'gemini'
 #             if name.endswith(',titan'):
 #                 protocol = 'titan'
 #             # Remove the base directory from the entry path.
 #             path = str(fn)[len(str(base)):]
 #             args = [str(fn)]
 #             if protocol == 'titan':
 #                 path = path[:-6]
 #             print(f'  {protocol}://{host}{path} ->', args)
-#             capsule.add(path, CgiContext(path, args, work_dir=cur_dir), host, protocol)
+#             context.add(path, CgiContext(path, args, work_dir=cur_dir), host, protocol)
 
 
-def init(capsule):
-    cfg = Capsule.config()
+def init(context):
+    cfg = context.config()
     default_host = cfg.hostnames()[0]
 
     # Custom entrypoints for specific URLs.
-    for section in Capsule.config().prefixed_sections('cgi.').values():
+    for section in cfg.prefixed_sections('cgi.').values():
         protocol = section.get('protocol', fallback='gemini')
         host = section.get('host', fallback=default_host)
         work_dir = section.get('cwd', fallback=None)
         args = shlex.split(section.get('command'))
         for path in shlex.split(section.get('path', fallback='/*')):
-            print(f'  {protocol}://{host}{path} ->', args)
-            capsule.add(path, CgiContext(path, args, work_dir),
+            context.print(f'  {protocol}://{host}{path} ->', args)
+            context.add(path, CgiContext(cfg.port(), path, args, work_dir),
                         host, protocol)
 
     # Automatic entrypoints for all executables.
-    bin_root = Capsule.config().ini.get('cgi', 'bin_root', fallback=None)
+    bin_root = cfg.ini.get('cgi', 'bin_root', fallback=None)
     if bin_root != None:
         bin_root = pathlib.Path(bin_root).resolve()
-        for host in Capsule.config().hostnames():
+        for host in cfg.hostnames():
             host_bin_root = bin_root / host
             for protocol in ['gemini', 'titan']:
-                capsule.add(
-                    CgiTreeMapper(protocol, host, host_bin_root), None,
+                context.add(
+                    CgiTreeMapper(protocol, host, cfg.port(), host_bin_root), None,
                     host, protocol)
```

### Comparing `gmcapsule-0.4.1/gmcapsule/modules/99_static.py` & `gmcapsule-0.5.0/gmcapsule/modules/99_static.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 
 """Static files"""
 
 import fnmatch
 import os.path
 import string
 
-from gmcapsule import Capsule, get_mime_type
+from gmcapsule import get_mime_type
 from pathlib import Path
 
 META = '.meta'
+CONFIG = None
 
 
 def check_meta_rules(path, hostname):
-    cfg = Capsule.config()
-    root = cfg.root_dir() / hostname
+    root = CONFIG.root_dir() / hostname
     dir = Path(path).parent
     while True:
-        if not str(dir).startswith(str(cfg.root_dir())):
+        if not str(dir).startswith(str(CONFIG.root_dir())):
             break
         if (dir / META).exists():
             for rule in open(dir / META, 'rt').readlines():
                 rule = rule.strip()
                 if len(rule) == 0: continue
                 pos = rule.find(':')
                 if pos < 0: continue
@@ -37,15 +37,15 @@
     return 20, get_mime_type(path)
 
 
 def serve_file(req):
     if req.scheme != 'gemini':
         return 59, "Only Gemini requests allowed"
 
-    cfg = Capsule.config()
+    cfg = CONFIG
     if req.path == '':
         return 31, '/'
 
     for seg in req.path.split('/'):
         if seg != '.' and seg != '..' and seg.startswith('.'):
             return 51, "Not found"
 
@@ -62,17 +62,19 @@
     status, meta = check_meta_rules(path, req.hostname)
     if status and status != 20:
         return status, meta
 
     if not os.path.exists(path):
         return 51, "Not found"
 
-    # Note: We return the file object so the sender doesn't have to buffer
+    # Note: We return a Path object so the sender doesn't have to buffer
     # the entire file in memory first.
-    return status, meta, (open(path, 'rb') if status == 20 else None)
+    return status, meta, (Path(path) if status == 20 else None)
 
 
-def init(capsule):
-    cfg = capsule.config()
+def init(context):
+    cfg = context.config()
+    global CONFIG
+    CONFIG = cfg
     if 'static' in cfg.ini and 'root' in cfg.section('static'):
-        print('  Content directory:', cfg.root_dir() / '{hostname}')
-        capsule.add('/*', serve_file)
+        context.print('  Content directory:', cfg.root_dir() / '{hostname}')
+        context.add('/*', serve_file)
```

### Comparing `gmcapsule-0.4.1/README.md` & `gmcapsule-0.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     [Unit]
     Description=GmCapsule: extensible Gemini/Titan server
     After=network.target
 
     [Service]
     Type=simple
     ExecStart=<YOUR-INSTALL-PATH>/gmcapsuled
+    ExecReload=/bin/kill -HUP $MAINPID
     Restart=always
     Environment="PYTHONUNBUFFERED=1"
     StandardOutput=syslog
     StandardError=syslog
     SyslogIdentifier=gmcapsule
 
     [Install]
@@ -42,14 +43,22 @@
 
 The log can be viewed via journalctl (or syslog):
 
     journalctl -xe --user-unit=gmcapsule
 
 ## Change log
 
+### v0.5
+
+* Added `processes` to the `[server]` section to configure how many request handler processes are started.
+* Extension modules can register new protocols in addition to the built-in Gemini and Titan.
+* SIGHUP causes the configuration file to be reloaded and workers to be restarted. The listening socket remains open, so the socket and TLS parameters cannot be changed.
+* API change: Extension modules get initialized separately in each worker thread. Instead of a `Capsule`, the extension module `init` method is passed a `Context`. `Capsule` is no longer available as global state.
+* API change: `Identity` no longer contains OpenSSL objects for the certificate and public key. Instead, they are provided as serialized in DER format.
+
 ### v0.4
 
 * Added built-in module "rewrite" that matches regular expressions against the request path and can rewrite the path or return a custom status for redirection, "Gone" messages, or other exceptional situations.
 * Extension module load order is determined after locating all modules from all directories. Previously, the order was local to each directory.
 * Added a new configuration section `[priority]` for overriding default module priorities determined from file names. This is useful for changing the priority of the built-in modules.
 
 v0.4.1:
```

### Comparing `gmcapsule-0.4.1/pyproject.toml` & `gmcapsule-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.4.1/PKG-INFO` & `gmcapsule-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmcapsule
-Version: 0.4.1
+Version: 0.5.0
 Summary: Extensible Gemini/Titan server
 Project-URL: Home-page, https://geminispace.org/gmcapsule/
 Project-URL: Documentation, https://geminispace.org/gmcapsule/gmcapsule.html
 Project-URL: Source, https://codeberg.org/skyjake/gmcapsule
 Project-URL: Issues, https://codeberg.org/skyjake/gmcapsule/issues
 Author-email: Jaakko Keränen <jaakko.keranen@iki.fi>
 Keywords: gemini,internet,server,titan
@@ -41,14 +41,15 @@
     [Unit]
     Description=GmCapsule: extensible Gemini/Titan server
     After=network.target
 
     [Service]
     Type=simple
     ExecStart=<YOUR-INSTALL-PATH>/gmcapsuled
+    ExecReload=/bin/kill -HUP $MAINPID
     Restart=always
     Environment="PYTHONUNBUFFERED=1"
     StandardOutput=syslog
     StandardError=syslog
     SyslogIdentifier=gmcapsule
 
     [Install]
@@ -64,14 +65,22 @@
 
 The log can be viewed via journalctl (or syslog):
 
     journalctl -xe --user-unit=gmcapsule
 
 ## Change log
 
+### v0.5
+
+* Added `processes` to the `[server]` section to configure how many request handler processes are started.
+* Extension modules can register new protocols in addition to the built-in Gemini and Titan.
+* SIGHUP causes the configuration file to be reloaded and workers to be restarted. The listening socket remains open, so the socket and TLS parameters cannot be changed.
+* API change: Extension modules get initialized separately in each worker thread. Instead of a `Capsule`, the extension module `init` method is passed a `Context`. `Capsule` is no longer available as global state.
+* API change: `Identity` no longer contains OpenSSL objects for the certificate and public key. Instead, they are provided as serialized in DER format.
+
 ### v0.4
 
 * Added built-in module "rewrite" that matches regular expressions against the request path and can rewrite the path or return a custom status for redirection, "Gone" messages, or other exceptional situations.
 * Extension module load order is determined after locating all modules from all directories. Previously, the order was local to each directory.
 * Added a new configuration section `[priority]` for overriding default module priorities determined from file names. This is useful for changing the priority of the built-in modules.
 
 v0.4.1:
```

