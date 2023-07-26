# Comparing `tmp/Flask-SocketIO-5.3.4.tar.gz` & `tmp/Flask-SocketIO-5.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-SocketIO-5.3.4.tar", last modified: Wed May  3 10:34:08 2023, max compression
+gzip compressed data, was "Flask-SocketIO-5.3.5.tar", last modified: Wed Jul 26 18:14:16 2023, max compression
```

## Comparing `Flask-SocketIO-5.3.4.tar` & `Flask-SocketIO-5.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-05-03 10:34:08.560341 Flask-SocketIO-5.3.4/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1082 2019-11-17 19:18:09.000000 Flask-SocketIO-5.3.4/LICENSE
--rw-r--r--   0 mgrinberg   (502) staff       (20)       26 2019-11-17 19:18:09.000000 Flask-SocketIO-5.3.4/MANIFEST.in
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2504 2023-05-03 10:34:08.560571 Flask-SocketIO-5.3.4/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1867 2021-06-13 15:46:50.000000 Flask-SocketIO-5.3.4/README.md
--rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-13 15:46:50.000000 Flask-SocketIO-5.3.4/pyproject.toml
--rw-r--r--   0 mgrinberg   (502) staff       (20)      845 2023-05-03 10:34:08.561552 Flask-SocketIO-5.3.4/setup.cfg
--rw-r--r--   0 mgrinberg   (502) staff       (20)       38 2021-07-17 09:46:45.000000 Flask-SocketIO-5.3.4/setup.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-05-03 10:34:08.548192 Flask-SocketIO-5.3.4/src/
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-05-03 10:34:08.555686 Flask-SocketIO-5.3.4/src/Flask_SocketIO.egg-info/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2504 2023-05-03 10:34:08.000000 Flask-SocketIO-5.3.4/src/Flask_SocketIO.egg-info/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)      410 2023-05-03 10:34:08.000000 Flask-SocketIO-5.3.4/src/Flask_SocketIO.egg-info/SOURCES.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2023-05-03 10:34:08.000000 Flask-SocketIO-5.3.4/src/Flask_SocketIO.egg-info/dependency_links.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-07 19:15:18.000000 Flask-SocketIO-5.3.4/src/Flask_SocketIO.egg-info/not-zip-safe
--rw-r--r--   0 mgrinberg   (502) staff       (20)       34 2023-05-03 10:34:08.000000 Flask-SocketIO-5.3.4/src/Flask_SocketIO.egg-info/requires.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)       15 2023-05-03 10:34:08.000000 Flask-SocketIO-5.3.4/src/Flask_SocketIO.egg-info/top_level.txt
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-05-03 10:34:08.559372 Flask-SocketIO-5.3.4/src/flask_socketio/
--rw-r--r--   0 mgrinberg   (502) staff       (20)    54782 2023-03-21 19:59:26.000000 Flask-SocketIO-5.3.4/src/flask_socketio/__init__.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2020 2021-06-13 15:46:50.000000 Flask-SocketIO-5.3.4/src/flask_socketio/namespace.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    10274 2023-05-03 10:28:48.000000 Flask-SocketIO-5.3.4/src/flask_socketio/test_client.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-26 18:14:16.724852 Flask-SocketIO-5.3.5/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1082 2023-06-13 09:40:37.000000 Flask-SocketIO-5.3.5/LICENSE
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       26 2023-06-13 09:40:37.000000 Flask-SocketIO-5.3.5/MANIFEST.in
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2525 2023-07-26 18:14:16.724852 Flask-SocketIO-5.3.5/PKG-INFO
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1867 2023-06-13 09:40:37.000000 Flask-SocketIO-5.3.5/README.md
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      104 2023-06-13 09:40:37.000000 Flask-SocketIO-5.3.5/pyproject.toml
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      887 2023-07-26 18:14:16.724852 Flask-SocketIO-5.3.5/setup.cfg
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       38 2023-06-13 09:40:37.000000 Flask-SocketIO-5.3.5/setup.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-26 18:14:16.724852 Flask-SocketIO-5.3.5/src/
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-26 18:14:16.724852 Flask-SocketIO-5.3.5/src/Flask_SocketIO.egg-info/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2525 2023-07-26 18:14:16.000000 Flask-SocketIO-5.3.5/src/Flask_SocketIO.egg-info/PKG-INFO
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      410 2023-07-26 18:14:16.000000 Flask-SocketIO-5.3.5/src/Flask_SocketIO.egg-info/SOURCES.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2023-07-26 18:14:16.000000 Flask-SocketIO-5.3.5/src/Flask_SocketIO.egg-info/dependency_links.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2023-06-13 10:11:43.000000 Flask-SocketIO-5.3.5/src/Flask_SocketIO.egg-info/not-zip-safe
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       49 2023-07-26 18:14:16.000000 Flask-SocketIO-5.3.5/src/Flask_SocketIO.egg-info/requires.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       15 2023-07-26 18:14:16.000000 Flask-SocketIO-5.3.5/src/Flask_SocketIO.egg-info/top_level.txt
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-26 18:14:16.724852 Flask-SocketIO-5.3.5/src/flask_socketio/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    54731 2023-07-26 18:01:29.000000 Flask-SocketIO-5.3.5/src/flask_socketio/__init__.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2020 2023-06-13 09:40:37.000000 Flask-SocketIO-5.3.5/src/flask_socketio/namespace.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    10274 2023-06-13 09:40:37.000000 Flask-SocketIO-5.3.5/src/flask_socketio/test_client.py
```

### Comparing `Flask-SocketIO-5.3.4/LICENSE` & `Flask-SocketIO-5.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-SocketIO-5.3.4/PKG-INFO` & `Flask-SocketIO-5.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: Flask-SocketIO
-Version: 5.3.4
+Version: 5.3.5
 Summary: Socket.IO integration for Flask applications
 Home-page: https://github.com/miguelgrinberg/flask-socketio
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/flask-socketio/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: docs
 License-File: LICENSE
 
 Flask-SocketIO
 ==============
 
 [![Build status](https://github.com/miguelgrinberg/flask-socketio/workflows/build/badge.svg)](https://github.com/miguelgrinberg/Flask-SocketIO/actions) [![codecov](https://codecov.io/gh/miguelgrinberg/flask-socketio/branch/main/graph/badge.svg)](https://codecov.io/gh/miguelgrinberg/flask-socketio)
```

### Comparing `Flask-SocketIO-5.3.4/README.md` & `Flask-SocketIO-5.3.5/README.md`

 * *Files identical despite different names*

### Comparing `Flask-SocketIO-5.3.4/setup.cfg` & `Flask-SocketIO-5.3.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Flask-SocketIO
-version = 5.3.4
+version = 5.3.5
 author = Miguel Grinberg
 author_email = miguel.grinberg@gmail.com
 description = Socket.IO integration for Flask applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/miguelgrinberg/flask-socketio
 project_urls = 
@@ -26,11 +26,15 @@
 install_requires = 
 	Flask >= 0.9
 	python-socketio >= 5.0.2
 
 [options.packages.find]
 where = src
 
+[options.extras_require]
+docs = 
+	sphinx
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `Flask-SocketIO-5.3.4/src/Flask_SocketIO.egg-info/PKG-INFO` & `Flask-SocketIO-5.3.5/src/Flask_SocketIO.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: Flask-SocketIO
-Version: 5.3.4
+Version: 5.3.5
 Summary: Socket.IO integration for Flask applications
 Home-page: https://github.com/miguelgrinberg/flask-socketio
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/flask-socketio/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: docs
 License-File: LICENSE
 
 Flask-SocketIO
 ==============
 
 [![Build status](https://github.com/miguelgrinberg/flask-socketio/workflows/build/badge.svg)](https://github.com/miguelgrinberg/Flask-SocketIO/actions) [![codecov](https://codecov.io/gh/miguelgrinberg/flask-socketio/branch/main/graph/badge.svg)](https://codecov.io/gh/miguelgrinberg/flask-socketio)
```

### Comparing `Flask-SocketIO-5.3.4/src/flask_socketio/__init__.py` & `Flask-SocketIO-5.3.5/src/flask_socketio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,23 +623,22 @@
             #    \  middleware
             #     o
             #  Flask-SocketIO WebSocket handler
             #
             self.sockio_mw.wsgi_app = DebuggedApplication(
                 self.sockio_mw.wsgi_app, evalex=True)
 
+        allow_unsafe_werkzeug = kwargs.pop('allow_unsafe_werkzeug', False)
         if self.server.eio.async_mode == 'threading':
             try:
                 import simple_websocket  # noqa: F401
             except ImportError:
                 from werkzeug._internal import _log
                 _log('warning', 'WebSocket transport not available. Install '
                                 'simple-websocket for improved performance.')
-            allow_unsafe_werkzeug = kwargs.pop('allow_unsafe_werkzeug',
-                                               False)
             if not sys.stdin or not sys.stdin.isatty():  # pragma: no cover
                 if not allow_unsafe_werkzeug:
                     raise RuntimeError('The Werkzeug web server is not '
                                        'designed to run in production. Pass '
                                        'allow_unsafe_werkzeug=True to the '
                                        'run() method to disable this error.')
                 else:
```

### Comparing `Flask-SocketIO-5.3.4/src/flask_socketio/namespace.py` & `Flask-SocketIO-5.3.5/src/flask_socketio/namespace.py`

 * *Files identical despite different names*

### Comparing `Flask-SocketIO-5.3.4/src/flask_socketio/test_client.py` & `Flask-SocketIO-5.3.5/src/flask_socketio/test_client.py`

 * *Files identical despite different names*

