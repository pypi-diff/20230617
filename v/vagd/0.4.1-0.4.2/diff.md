# Comparing `tmp/vagd-0.4.1.tar.gz` & `tmp/vagd-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vagd-0.4.1.tar", last modified: Sat Jun 17 14:45:12 2023, max compression
+gzip compressed data, was "vagd-0.4.2.tar", last modified: Sat Jun 17 16:00:05 2023, max compression
```

## Comparing `vagd-0.4.1.tar` & `vagd-0.4.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 14:45:12.038369 vagd-0.4.1/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    35149 2023-03-05 14:43:59.000000 vagd-0.4.1/LICENSE
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2906 2023-06-17 14:45:12.038369 vagd-0.4.1/PKG-INFO
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2322 2023-06-17 13:45:28.000000 vagd-0.4.1/README.md
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      880 2023-06-17 14:43:53.000000 vagd-0.4.1/pyproject.toml
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       38 2023-06-17 14:45:12.038369 vagd-0.4.1/setup.cfg
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 14:45:12.035036 vagd-0.4.1/src/
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 14:45:12.035036 vagd-0.4.1/src/vagd/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       53 2023-03-20 14:52:11.000000 vagd-0.4.1/src/vagd/__init__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      220 2023-03-14 11:41:30.000000 vagd-0.4.1/src/vagd/__main__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      939 2023-06-17 11:38:21.000000 vagd-0.4.1/src/vagd/box.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 14:45:12.038369 vagd-0.4.1/src/vagd/gdb/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    20349 2023-03-04 14:19:11.000000 vagd-0.4.1/src/vagd/gdb/__init__.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4178 2023-03-04 12:55:58.000000 vagd-0.4.1/src/vagd/gdb/events.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      983 2023-03-04 12:55:58.000000 vagd-0.4.1/src/vagd/gdb/printing.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       47 2023-03-04 12:55:58.000000 vagd-0.4.1/src/vagd/gdb/prompt.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      865 2023-03-04 12:55:58.000000 vagd-0.4.1/src/vagd/gdb/types.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      135 2023-03-04 12:55:58.000000 vagd-0.4.1/src/vagd/gdb/unwinder.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      844 2023-03-04 12:55:58.000000 vagd-0.4.1/src/vagd/gdb/xmethod.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       44 2023-03-14 14:03:57.000000 vagd-0.4.1/src/vagd/gdb.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1195 2023-04-08 07:51:28.000000 vagd-0.4.1/src/vagd/helper.py
--rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      839 2023-06-17 11:43:56.000000 vagd-0.4.1/src/vagd/template.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1768 2023-06-17 14:32:08.000000 vagd-0.4.1/src/vagd/templates.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 14:45:12.038369 vagd-0.4.1/src/vagd/virts/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      132 2023-03-20 14:52:11.000000 vagd-0.4.1/src/vagd/virts/__init__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     5428 2023-06-17 14:41:31.000000 vagd-0.4.1/src/vagd/virts/dogd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10643 2023-06-17 14:33:49.000000 vagd-0.4.1/src/vagd/virts/pwngd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10853 2023-04-15 14:11:22.000000 vagd-0.4.1/src/vagd/virts/qegd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1345 2023-03-20 14:52:11.000000 vagd-0.4.1/src/vagd/virts/shgd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3592 2023-03-20 14:52:11.000000 vagd-0.4.1/src/vagd/virts/vagd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      843 2023-03-14 14:21:12.000000 vagd-0.4.1/src/vagd/wrapper.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 14:45:12.035036 vagd-0.4.1/src/vagd.egg-info/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2906 2023-06-17 14:45:12.000000 vagd-0.4.1/src/vagd.egg-info/PKG-INFO
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      678 2023-06-17 14:45:12.000000 vagd-0.4.1/src/vagd.egg-info/SOURCES.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)        1 2023-06-17 14:45:12.000000 vagd-0.4.1/src/vagd.egg-info/dependency_links.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       31 2023-06-17 14:45:12.000000 vagd-0.4.1/src/vagd.egg-info/requires.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)        5 2023-06-17 14:45:12.000000 vagd-0.4.1/src/vagd.egg-info/top_level.txt
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 14:45:12.038369 vagd-0.4.1/test/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1074 2023-03-20 14:52:11.000000 vagd-0.4.1/test/test.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 16:00:05.883415 vagd-0.4.2/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    35149 2023-03-05 14:43:59.000000 vagd-0.4.2/LICENSE
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2928 2023-06-17 16:00:05.880082 vagd-0.4.2/PKG-INFO
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2344 2023-06-17 15:28:22.000000 vagd-0.4.2/README.md
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      880 2023-06-17 15:21:56.000000 vagd-0.4.2/pyproject.toml
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       38 2023-06-17 16:00:05.883415 vagd-0.4.2/setup.cfg
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 16:00:05.873415 vagd-0.4.2/src/
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 16:00:05.876748 vagd-0.4.2/src/vagd/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       53 2023-03-20 14:52:11.000000 vagd-0.4.2/src/vagd/__init__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      220 2023-03-14 11:41:30.000000 vagd-0.4.2/src/vagd/__main__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      939 2023-06-17 11:38:21.000000 vagd-0.4.2/src/vagd/box.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 16:00:05.880082 vagd-0.4.2/src/vagd/gdb/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    20349 2023-03-04 14:19:11.000000 vagd-0.4.2/src/vagd/gdb/__init__.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4178 2023-03-04 12:55:58.000000 vagd-0.4.2/src/vagd/gdb/events.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      983 2023-03-04 12:55:58.000000 vagd-0.4.2/src/vagd/gdb/printing.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       47 2023-03-04 12:55:58.000000 vagd-0.4.2/src/vagd/gdb/prompt.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      865 2023-03-04 12:55:58.000000 vagd-0.4.2/src/vagd/gdb/types.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      135 2023-03-04 12:55:58.000000 vagd-0.4.2/src/vagd/gdb/unwinder.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      844 2023-03-04 12:55:58.000000 vagd-0.4.2/src/vagd/gdb/xmethod.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       44 2023-03-14 14:03:57.000000 vagd-0.4.2/src/vagd/gdb.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1195 2023-04-08 07:51:28.000000 vagd-0.4.2/src/vagd/helper.py
+-rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      839 2023-06-17 11:43:56.000000 vagd-0.4.2/src/vagd/template.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1759 2023-06-17 14:59:31.000000 vagd-0.4.2/src/vagd/templates.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 16:00:05.880082 vagd-0.4.2/src/vagd/virts/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      132 2023-03-20 14:52:11.000000 vagd-0.4.2/src/vagd/virts/__init__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     5683 2023-06-17 15:38:36.000000 vagd-0.4.2/src/vagd/virts/dogd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10666 2023-06-17 15:51:31.000000 vagd-0.4.2/src/vagd/virts/pwngd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10849 2023-06-17 15:49:55.000000 vagd-0.4.2/src/vagd/virts/qegd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1345 2023-03-20 14:52:11.000000 vagd-0.4.2/src/vagd/virts/shgd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3592 2023-03-20 14:52:11.000000 vagd-0.4.2/src/vagd/virts/vagd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      843 2023-03-14 14:21:12.000000 vagd-0.4.2/src/vagd/wrapper.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 16:00:05.876748 vagd-0.4.2/src/vagd.egg-info/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2928 2023-06-17 16:00:05.000000 vagd-0.4.2/src/vagd.egg-info/PKG-INFO
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      678 2023-06-17 16:00:05.000000 vagd-0.4.2/src/vagd.egg-info/SOURCES.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)        1 2023-06-17 16:00:05.000000 vagd-0.4.2/src/vagd.egg-info/dependency_links.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       31 2023-06-17 16:00:05.000000 vagd-0.4.2/src/vagd.egg-info/requires.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)        5 2023-06-17 16:00:05.000000 vagd-0.4.2/src/vagd.egg-info/top_level.txt
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 16:00:05.880082 vagd-0.4.2/test/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1206 2023-06-17 15:43:05.000000 vagd-0.4.2/test/test.py
```

### Comparing `vagd-0.4.1/LICENSE` & `vagd-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vagd-0.4.1/PKG-INFO` & `vagd-0.4.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagd
-Version: 0.4.1
+Version: 0.4.2
 Summary: VirtuAlization GDb integrations in pwntools
 Author-email: 0x6fe1be2 <author@example.com>
 Project-URL: Homepage, https://github.com/gfelber/vagd
 Project-URL: Documentation, https://gfelber.github.io/vagd/
 Project-URL: Bug Tracker, https://github.com/gfelber/vagd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -73,15 +73,15 @@
   * DOCKER_JAMMY = 'ubuntu:jammy'
   * DOCKER_FOCAL = 'ubuntu:focal'
   * DOCKER_BIONIC = 'ubuntu:bionic'
   * DOCKER_XENIAL = 'ubuntu:xenial'
   * DOCKER_ALPINE_316 = 'alpine:3.16.6'
 
 
-currently only distributions that use `apt` are supported
+currently only distributions that use `apt` and alpine for Docker are supported
 
 
 
 ## Future plans
 
 ### pre configured Vagrant boxes / QEMU Images / Docker Image
```

### Comparing `vagd-0.4.1/README.md` & `vagd-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
   * DOCKER_JAMMY = 'ubuntu:jammy'
   * DOCKER_FOCAL = 'ubuntu:focal'
   * DOCKER_BIONIC = 'ubuntu:bionic'
   * DOCKER_XENIAL = 'ubuntu:xenial'
   * DOCKER_ALPINE_316 = 'alpine:3.16.6'
 
 
-currently only distributions that use `apt` are supported
+currently only distributions that use `apt` and alpine for Docker are supported
 
 
 
 ## Future plans
 
 ### pre configured Vagrant boxes / QEMU Images / Docker Image
```

### Comparing `vagd-0.4.1/pyproject.toml` & `vagd-0.4.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vagd"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="0x6fe1be2", email="author@example.com" },
 ]
 description = "VirtuAlization GDb integrations in pwntools"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ['pwntools', 'python-vagrant', 'docker']
```

### Comparing `vagd-0.4.1/src/vagd/box.py` & `vagd-0.4.2/src/vagd/box.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.1/src/vagd/gdb/__init__.pyi` & `vagd-0.4.2/src/vagd/gdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.4.1/src/vagd/gdb/events.pyi` & `vagd-0.4.2/src/vagd/gdb/events.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.4.1/src/vagd/gdb/printing.pyi` & `vagd-0.4.2/src/vagd/gdb/printing.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.4.1/src/vagd/gdb/types.pyi` & `vagd-0.4.2/src/vagd/gdb/types.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.4.1/src/vagd/gdb/xmethod.pyi` & `vagd-0.4.2/src/vagd/gdb/xmethod.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.4.1/src/vagd/helper.py` & `vagd-0.4.2/src/vagd/helper.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.1/src/vagd/template.txt` & `vagd-0.4.2/src/vagd/template.txt`

 * *Files identical despite different names*

### Comparing `vagd-0.4.1/src/vagd/templates.py` & `vagd-0.4.2/src/vagd/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,15 @@
     cd ..;\
     rm -rf gdb-build/;
 
 # install ssh server support and keys
 RUN apk add --no-cache openssh
 
 EXPOSE 22
-EXPOSE 22
-RUN adduser -h /home/vagd -s /bin/sh -D vagd
+RUN adduser -h /home/vagd -s /bin/ash -D vagd
 RUN echo "vagd:vagd" | chpasswd
 
 USER vagd
 
 WORKDIR /home/vagd
 
 COPY keyfile.pub .ssh/authorized_keys
```

#### html2text {}

```diff
@@ -11,12 +11,12 @@
 need make and linux-headers to compile gdb RUN apk add python3 RUN apk add --
 no-cache musl-dbg RUN apk add --no-cache make RUN apk add --no-cache linux-
 headers RUN apk add --no-cache texinfo RUN apk add --no-cache gcc RUN apk add -
 -no-cache g++ RUN apk add --no-cache gfortran # install gdb # RUN apk add --no-
 cache gdb RUN mkdir gdb-build ;\ cd gdb-build;\ wget http://ftp.gnu.org/gnu/
 gdb/gdb-7.11.tar.xz;\ tar -xvf gdb-7.11.tar.xz;\ cd gdb-7.11;\ ./configure --
 prefix=/usr;\ make;\ make -C gdb install;\ cd ..;\ rm -rf gdb-build/; # install
-ssh server support and keys RUN apk add --no-cache openssh EXPOSE 22 EXPOSE 22
-RUN adduser -h /home/vagd -s /bin/sh -D vagd RUN echo "vagd:vagd" | chpasswd
-USER vagd WORKDIR /home/vagd COPY keyfile.pub .ssh/authorized_keys USER root
-RUN ssh-keygen -A RUN mkdir -p /run/sshd && \ chmod 755 /run/sshd CMD /usr/
-sbin/sshd; \ while true; do sleep 1m; done '''
+ssh server support and keys RUN apk add --no-cache openssh EXPOSE 22 RUN
+adduser -h /home/vagd -s /bin/ash -D vagd RUN echo "vagd:vagd" | chpasswd USER
+vagd WORKDIR /home/vagd COPY keyfile.pub .ssh/authorized_keys USER root RUN
+ssh-keygen -A RUN mkdir -p /run/sshd && \ chmod 755 /run/sshd CMD /usr/sbin/
+sshd; \ while true; do sleep 1m; done '''
```

### Comparing `vagd-0.4.1/src/vagd/virts/dogd.py` & `vagd-0.4.2/src/vagd/virts/dogd.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class Dogd(Shgd):
     """
     | Docker virtualization for pwntools
     | SSH from cmd
     .. code-block:: bash
 
-        ssh -o "StrictHostKeyChecking=no" -i .vagd/keyfile -p $(cut .vagd/docker.lock -d":" -f 2) vagd@0.0.0.0
+        ssh -o "StrictHostKeyChecking=no" -i ~/.vagd/keyfile -p $(cut .vagd/docker.lock -d":" -f 2) vagd@0.0.0.0
 
     | connect with docker exec
     .. code-block:: bash
 
        docker exec -it $(cut ./.vagd/docker.lock -d":" -f 1) /bin/bash
 
     | Kill from cmd:
@@ -57,22 +57,24 @@
 
     def _create_dockerfile(self):
 
         pwn.log.info(f'create new Dockerfile at f{self._dockerfile}')
         if not os.path.exists(Pwngd.KEYFILE):
             helper.generate_keypair()
 
+        if not os.path.exists(self._dockerdir + "keyfile.pub"):
+            os.link(Pwngd.PUBKEYFILE, self._dockerdir + "keyfile.pub")
         template = templates.DOCKER_ALPINE_TEMPLATE if self._isalpine else templates.DOCKER_TEMPLATE
 
         with open(self._dockerfile, 'w') as dockerfile:
             dockerfile.write(
                 template.format(image=self._image,
                                 packages=' '.join(Dogd.DEFAULT_PACKAGES),
                                 user=self._user,
-                                keyfile=os.path.basename(Pwngd.KEYFILE + '.pub')))
+                                keyfile=os.path.basename(self._dockerdir + "keyfile.pub")))
 
     def _create_docker_instance(self):
         pwn.log.info('starting docker instance')
         self._port = helper.first_free_port(Dogd.DEFAULT_PORT)
         self._forward.update({'22/tcp': self._port})
         if self._isalpine:
             self._forward.update({f'{Pwngd.STATIC_GDBSRV_PORT}/tcp': Pwngd.STATIC_GDBSRV_PORT})
@@ -80,15 +82,15 @@
         self._id = container.id
         pwn.log.info(f'started docker instance {container.short_id}')
         with open(Dogd.LOCKFILE, 'w') as lockfile:
             lockfile.write(container.id + ':' + str(self._port))
 
     def _build_image(self):
         pwn.log.info('building docker image')
-        return self._client.images.build(path=os.path.dirname(self._dockerfile))[0]
+        return self._client.images.build(path=os.path.dirname(self._dockerfile), tag=f'vagd/{self._image}')[0]
 
     def _vm_create(self):
 
         if not os.path.exists(self._dockerfile):
             self._create_dockerfile()
 
         self._bimage = self._build_image()
@@ -101,16 +103,16 @@
             pwn.log.info(f'No Lockfile {Dogd.LOCKFILE} found, creating new Docker Instance')
             self._vm_create()
         else:
             with open(Dogd.LOCKFILE, 'r') as lockfile:
                 data = lockfile.readline().split(':')
                 self._id = data[0]
                 self._port = int(data[1])
-            if not helper.is_port_in_use(self._port):
-                pwn.log.info(f'Lockfile {Dogd.LOCKFILE} found, port not used, creating new container')
+            if not self._client.containers.list(filters={'id':self._id}):
+                pwn.log.info(f'Lockfile {Dogd.LOCKFILE} found, container not running, creating new one')
                 self._vm_create()
             else:
                 pwn.log.info(
                     f'Lockfile {Dogd.LOCKFILE} found, Docker Instance f{self._client.containers.get(self._id).short_id}')
 
     def __init__(self,
                  binary: str,
@@ -141,13 +143,14 @@
         if self._isalpine and not self._ex:
             pwn.log.error("Docker alpine images requires experimental features")
         if self._forward is None:
            self._forward = dict()
 
         self._vm_setup()
 
+        gdbsrvport = Pwngd.STATIC_GDBSRV_PORT if self._isalpine else None
         super().__init__(binary=binary,
                          user=self._user,
                          port=self._port,
                          ex=ex,
-                         gdbsrvport=Pwngd.STATIC_GDBSRV_PORT,
+                         gdbsrvport=gdbsrvport,
                          **kwargs)
```

### Comparing `vagd-0.4.1/src/vagd/virts/pwngd.py` & `vagd-0.4.2/src/vagd/virts/pwngd.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 class Pwngd(ABC):
     LOCAL_DIR = './.vagd/'
     HOME_DIR = os.path.expanduser('~/.vagd/')
     SYSROOT = LOCAL_DIR + 'sysroot/'
     SYSROOT_LIB = SYSROOT + 'lib/'
     SYSROOT_LIB_DEBUG = SYSROOT + 'lib/debug'
-    KEYFILE = LOCAL_DIR + 'keyfile'
+    KEYFILE = HOME_DIR + 'keyfile'
+    PUBKEYFILE = KEYFILE + '.pub'
     DEFAULT_PORT = 2222
     STATIC_GDBSRV_PORT = 42069
 
     _path: str
     _gdbsrvport: int
     _binary: str
     _ssh: pwn.ssh
@@ -54,15 +55,15 @@
         mount remote dir on local wiith sshfs
         :param remote_dir: directory on remote to mount
         :param local_dir: local mount point
         """
         if not which('sshfs'):
             pwn.log.error('sshfs isn\'t installed')
         cmd = Pwngd._SSHFS_TEMPLATE.format(port=self._ssh.port,
-                                           keyfile="$PWD/" + self._ssh.keyfile,
+                                           keyfile=self._ssh.keyfile,
                                            user=self._ssh.user,
                                            host=self._ssh.host,
                                            remote_dir=remote_dir,
                                            local_dir=local_dir)
         pwn.log.info(cmd)
         os.system(cmd)
```

### Comparing `vagd-0.4.1/src/vagd/virts/qegd.py` & `vagd-0.4.2/src/vagd/virts/qegd.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class Qegd(Pwngd):
     """
     | QEMU Virtualization for pwntools
     | SSH from cmd
 
     .. code-block:: bash
 
-        ssh -o "StrictHostKeyChecking=no" -i .vagd/keyfile -p $(cat .vagd/qemu.lock) ubuntu@0.0.0.0
+        ssh -o "StrictHostKeyChecking=no" -i ~/.vagd/keyfile -p $(cat .vagd/qemu.lock) ubuntu@0.0.0.0
 
     | Kill from cmd:
 
     .. code-block:: bash
 
         kill $(pgrep qemu)
 
@@ -132,15 +132,15 @@
                 pwn.log.info(f"{Qegd.METADATA_FILE} not found generating new one")
                 with open(Qegd.METADATA_FILE, 'w') as metadata_file:
                     metadata_file.write(Qegd._METADATA)
             if not os.path.exists(Qegd.USER_DATA_FILE):
                 pwn.log.info(f"{Qegd.USER_DATA_FILE} not found generating new one")
                 helper.generate_keypair()
                 with open(Qegd.USER_DATA_FILE, 'w') as user_data_file:
-                    with open(Pwngd.KEYFILE + '.pub', 'r') as pubkey_file:
+                    with open(Pwngd.PUBKEYFILE, 'r') as pubkey_file:
                         pubkey = pubkey_file.readline()
                     user_data_file.write(Qegd._USER_DATA.format(pubkey=pubkey))
             os.system(Qegd._GENERATE_SEED_IMG)
 
     _QEMU_PORT_FORWARDING = ',hostfwd=tcp::{host}-:{guest}'
     _QEMU_START = "{qemu} " \
                   + "{machine} " \
```

### Comparing `vagd-0.4.1/src/vagd/virts/shgd.py` & `vagd-0.4.2/src/vagd/virts/shgd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.1/src/vagd/virts/vagd.py` & `vagd-0.4.2/src/vagd/virts/vagd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.1/src/vagd/wrapper.py` & `vagd-0.4.2/src/vagd/wrapper.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.1/src/vagd.egg-info/PKG-INFO` & `vagd-0.4.2/src/vagd.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagd
-Version: 0.4.1
+Version: 0.4.2
 Summary: VirtuAlization GDb integrations in pwntools
 Author-email: 0x6fe1be2 <author@example.com>
 Project-URL: Homepage, https://github.com/gfelber/vagd
 Project-URL: Documentation, https://gfelber.github.io/vagd/
 Project-URL: Bug Tracker, https://github.com/gfelber/vagd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -73,15 +73,15 @@
   * DOCKER_JAMMY = 'ubuntu:jammy'
   * DOCKER_FOCAL = 'ubuntu:focal'
   * DOCKER_BIONIC = 'ubuntu:bionic'
   * DOCKER_XENIAL = 'ubuntu:xenial'
   * DOCKER_ALPINE_316 = 'alpine:3.16.6'
 
 
-currently only distributions that use `apt` are supported
+currently only distributions that use `apt` and alpine for Docker are supported
 
 
 
 ## Future plans
 
 ### pre configured Vagrant boxes / QEMU Images / Docker Image
```

### Comparing `vagd-0.4.1/src/vagd.egg-info/SOURCES.txt` & `vagd-0.4.2/src/vagd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vagd-0.4.1/test/test.py` & `vagd-0.4.2/test/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,36 +13,41 @@
 ENV = {}
 API = True
 GDB = f"""
 b main
 c"""
 
 context.binary = exe = ELF(BINARY, checksec=False)
-context.aslr = False
+context.aslr = True
 
 byt = lambda x: str(x).encode()
 
 
 def vms():
+    log.info("Testing Vagrant")
     vm = Vagd(exe.path, vbox=Box.UBUNTU_FOCAL64, tmp=True, fast=True, ex=True)
     yield vm
     vm._v.halt()
-    vm = Dogd(exe.path, user='ubuntu', image=Box.DOCKER_FOCAL, tmp=True, ex=True, fast=True)
+    log.info("Testing Docker for Ubuntu")
+    vm = Dogd(exe.path, image=Box.DOCKER_FOCAL, tmp=True, ex=True, fast=True)
     yield vm
     vm._client.containers.get(vm._id).kill()
-    vm = Qegd(exe.path, user='ubuntu', img=Box.CLOUDIMAGE_FOCAL, tmp=True, ex=True, fast=True)
+    log.info("Testing Qemu")
+    vm = Qegd(exe.path, img=Box.CLOUDIMAGE_FOCAL, tmp=True, ex=True, fast=True)
     yield vm
+    log.info("Testing SSH")
     yield Shgd(exe.path, user=vm._user, port=vm._port, tmp=True, ex=True, fast=True)
     os.system('kill $(pgrep qemu)')
     yield wrapper.Empty()
 
 
 for vm in vms():
     t = vm.start(argv=ARGS, env=ENV, gdbscript=GDB, api=API)
 
+    sleep(1)
     g = wrapper.GDB(t)
     g.execute('p "PWN"')
     g.execute('c')
 
-    t.recvall()
+    log.info(t.recvall().decode())
 
 print("Everything executed without errors")
```

