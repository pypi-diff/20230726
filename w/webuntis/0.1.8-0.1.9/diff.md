# Comparing `tmp/webuntis-0.1.8.tar.gz` & `tmp/webuntis-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/webuntis-0.1.8.tar", last modified: Mon Sep  9 22:25:05 2013, max compression
+gzip compressed data, was "dist/webuntis-0.1.9.tar", last modified: Wed Jan 22 16:15:00 2014, max compression
```

## Comparing `webuntis-0.1.8.tar` & `webuntis-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2013-09-09 22:25:05.000000 webuntis-0.1.8/
--rw-r--r--   0 untitaker  (1000) users      (100)      915 2013-04-23 17:01:53.000000 webuntis-0.1.8/README.rst
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2013-09-09 22:25:05.000000 webuntis-0.1.8/webuntis/
--rw-r--r--   0 untitaker  (1000) users      (100)    16815 2013-06-26 15:30:19.000000 webuntis-0.1.8/webuntis/objects.py
--rwxr-xr-x   0 untitaker  (1000) users      (100)      208 2013-09-09 22:13:27.000000 webuntis-0.1.8/webuntis/__init__.py
--rwxr-xr-x   0 untitaker  (1000) users      (100)    12849 2013-06-26 15:31:36.000000 webuntis-0.1.8/webuntis/session.py
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2013-09-09 22:25:05.000000 webuntis-0.1.8/webuntis/tests/
--rw-r--r--   0 untitaker  (1000) users      (100)     4732 2013-07-05 12:17:42.000000 webuntis-0.1.8/webuntis/tests/__init__.py
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2013-09-09 22:25:05.000000 webuntis-0.1.8/webuntis/tests/static/
--rw-r--r--   0 untitaker  (1000) users      (100)      331 2013-07-05 12:17:42.000000 webuntis-0.1.8/webuntis/tests/static/getdepartments_mock.json
--rw-r--r--   0 untitaker  (1000) users      (100)      985 2013-07-05 12:17:42.000000 webuntis-0.1.8/webuntis/tests/static/getstatusdata_mock.json
--rw-r--r--   0 untitaker  (1000) users      (100)     1536 2013-07-05 12:17:42.000000 webuntis-0.1.8/webuntis/tests/static/getholidays_mock.json
--rw-r--r--   0 untitaker  (1000) users      (100)     1723 2013-07-05 12:17:42.000000 webuntis-0.1.8/webuntis/tests/static/getklassen_mock.json
--rw-r--r--   0 untitaker  (1000) users      (100)      825 2013-07-05 12:17:42.000000 webuntis-0.1.8/webuntis/tests/static/getschoolyears_mock.json
--rw-r--r--   0 untitaker  (1000) users      (100)     9878 2013-07-05 12:17:42.000000 webuntis-0.1.8/webuntis/tests/static/getteachers_mock.json
--rw-r--r--   0 untitaker  (1000) users      (100)     5850 2013-07-05 12:17:42.000000 webuntis-0.1.8/webuntis/tests/static/getsubjects_mock.json
--rw-r--r--   0 untitaker  (1000) users      (100)     8607 2013-07-05 12:17:42.000000 webuntis-0.1.8/webuntis/tests/static/gettimegrid_mock.json
--rw-r--r--   0 untitaker  (1000) users      (100)    55579 2013-07-05 12:17:42.000000 webuntis-0.1.8/webuntis/tests/static/gettimetables_mock.json
--rw-r--r--   0 untitaker  (1000) users      (100)     4578 2013-07-05 12:17:42.000000 webuntis-0.1.8/webuntis/tests/static/getrooms_mock.json
--rw-r--r--   0 untitaker  (1000) users      (100)     8655 2013-07-05 12:17:42.000000 webuntis-0.1.8/webuntis/tests/test_session.py
--rw-r--r--   0 untitaker  (1000) users      (100)     8402 2013-07-05 12:17:42.000000 webuntis-0.1.8/webuntis/tests/test_objects.py
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2013-09-09 22:25:05.000000 webuntis-0.1.8/webuntis/utils/
--rw-r--r--   0 untitaker  (1000) users      (100)      364 2013-04-23 15:07:02.000000 webuntis-0.1.8/webuntis/utils/__init__.py
--rw-r--r--   0 untitaker  (1000) users      (100)      711 2012-12-24 19:17:52.000000 webuntis-0.1.8/webuntis/utils/third_party.py
--rwxr-xr-x   0 untitaker  (1000) users      (100)     4473 2013-06-26 15:38:17.000000 webuntis-0.1.8/webuntis/utils/misc.py
--rw-r--r--   0 untitaker  (1000) users      (100)     1245 2013-02-24 15:49:14.000000 webuntis-0.1.8/webuntis/utils/timetable_utils.py
--rwxr-xr-x   0 untitaker  (1000) users      (100)     1266 2013-06-26 15:37:59.000000 webuntis-0.1.8/webuntis/utils/datetime_utils.py
--rwxr-xr-x   0 untitaker  (1000) users      (100)     4191 2013-07-25 10:08:26.000000 webuntis-0.1.8/webuntis/utils/remote.py
--rw-r--r--   0 untitaker  (1000) users      (100)     1712 2013-06-26 14:27:37.000000 webuntis-0.1.8/webuntis/utils/userinput.py
--rw-r--r--   0 untitaker  (1000) users      (100)      498 2012-12-15 18:56:15.000000 webuntis-0.1.8/webuntis/utils/logger.py
--rwxr-xr-x   0 untitaker  (1000) users      (100)      795 2013-06-26 15:01:33.000000 webuntis-0.1.8/webuntis/errors.py
-drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2013-09-09 22:25:05.000000 webuntis-0.1.8/webuntis.egg-info/
--rwxr-xr-x   0 untitaker  (1000) users      (100)        9 2013-09-09 22:25:05.000000 webuntis-0.1.8/webuntis.egg-info/top_level.txt
--rwxr-xr-x   0 untitaker  (1000) users      (100)     2144 2013-09-09 22:25:05.000000 webuntis-0.1.8/webuntis.egg-info/PKG-INFO
--rwxr-xr-x   0 untitaker  (1000) users      (100)        1 2013-09-09 22:25:05.000000 webuntis-0.1.8/webuntis.egg-info/dependency_links.txt
--rwxr-xr-x   0 untitaker  (1000) users      (100)     1017 2013-09-09 22:25:05.000000 webuntis-0.1.8/webuntis.egg-info/SOURCES.txt
--rwxr-xr-x   0 untitaker  (1000) users      (100)     1394 2013-09-09 22:13:21.000000 webuntis-0.1.8/setup.py
--rw-r--r--   0 untitaker  (1000) users      (100)     2144 2013-09-09 22:25:05.000000 webuntis-0.1.8/PKG-INFO
--rw-r--r--   0 untitaker  (1000) users      (100)       77 2012-11-29 16:18:21.000000 webuntis-0.1.8/MANIFEST.in
--rw-r--r--   0 untitaker  (1000) users      (100)     1464 2013-01-09 12:11:03.000000 webuntis-0.1.8/LICENSE
--rwxr-xr-x   0 untitaker  (1000) users      (100)       97 2013-09-09 22:25:05.000000 webuntis-0.1.8/setup.cfg
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2014-01-22 16:15:00.000000 webuntis-0.1.9/
+-rw-r--r--   0 untitaker  (1000) users      (100)     1041 2013-12-31 10:29:22.000000 webuntis-0.1.9/README.rst
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2014-01-22 16:15:00.000000 webuntis-0.1.9/webuntis/
+-rw-r--r--   0 untitaker  (1000) users      (100)    16815 2013-10-10 20:33:02.000000 webuntis-0.1.9/webuntis/objects.py
+-rwxr-xr-x   0 untitaker  (1000) users      (100)      208 2014-01-22 16:13:35.000000 webuntis-0.1.9/webuntis/__init__.py
+-rwxr-xr-x   0 untitaker  (1000) users      (100)    12917 2013-10-17 10:26:13.000000 webuntis-0.1.9/webuntis/session.py
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2014-01-22 16:15:00.000000 webuntis-0.1.9/webuntis/tests/
+-rw-r--r--   0 untitaker  (1000) users      (100)     4732 2013-07-05 12:17:42.000000 webuntis-0.1.9/webuntis/tests/__init__.py
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2014-01-22 16:15:00.000000 webuntis-0.1.9/webuntis/tests/static/
+-rw-r--r--   0 untitaker  (1000) users      (100)      331 2013-07-05 12:17:42.000000 webuntis-0.1.9/webuntis/tests/static/getdepartments_mock.json
+-rw-r--r--   0 untitaker  (1000) users      (100)      985 2013-07-05 12:17:42.000000 webuntis-0.1.9/webuntis/tests/static/getstatusdata_mock.json
+-rw-r--r--   0 untitaker  (1000) users      (100)     1536 2013-07-05 12:17:42.000000 webuntis-0.1.9/webuntis/tests/static/getholidays_mock.json
+-rw-r--r--   0 untitaker  (1000) users      (100)     1723 2013-07-05 12:17:42.000000 webuntis-0.1.9/webuntis/tests/static/getklassen_mock.json
+-rw-r--r--   0 untitaker  (1000) users      (100)      825 2013-07-05 12:17:42.000000 webuntis-0.1.9/webuntis/tests/static/getschoolyears_mock.json
+-rw-r--r--   0 untitaker  (1000) users      (100)     9878 2013-07-05 12:17:42.000000 webuntis-0.1.9/webuntis/tests/static/getteachers_mock.json
+-rw-r--r--   0 untitaker  (1000) users      (100)     5850 2013-07-05 12:17:42.000000 webuntis-0.1.9/webuntis/tests/static/getsubjects_mock.json
+-rw-r--r--   0 untitaker  (1000) users      (100)     8607 2013-07-05 12:17:42.000000 webuntis-0.1.9/webuntis/tests/static/gettimegrid_mock.json
+-rw-r--r--   0 untitaker  (1000) users      (100)    55579 2013-07-05 12:17:42.000000 webuntis-0.1.9/webuntis/tests/static/gettimetables_mock.json
+-rw-r--r--   0 untitaker  (1000) users      (100)     4578 2013-07-05 12:17:42.000000 webuntis-0.1.9/webuntis/tests/static/getrooms_mock.json
+-rw-r--r--   0 untitaker  (1000) users      (100)     8655 2013-07-05 12:17:42.000000 webuntis-0.1.9/webuntis/tests/test_session.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     8402 2013-07-05 12:17:42.000000 webuntis-0.1.9/webuntis/tests/test_objects.py
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2014-01-22 16:15:00.000000 webuntis-0.1.9/webuntis/utils/
+-rw-r--r--   0 untitaker  (1000) users      (100)      364 2013-04-23 15:07:02.000000 webuntis-0.1.9/webuntis/utils/__init__.py
+-rw-r--r--   0 untitaker  (1000) users      (100)      558 2013-10-19 11:05:42.000000 webuntis-0.1.9/webuntis/utils/third_party.py
+-rwxr-xr-x   0 untitaker  (1000) users      (100)     4473 2013-09-16 17:44:40.000000 webuntis-0.1.9/webuntis/utils/misc.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     1245 2013-10-10 20:33:02.000000 webuntis-0.1.9/webuntis/utils/timetable_utils.py
+-rwxr-xr-x   0 untitaker  (1000) users      (100)     1266 2013-06-26 15:37:59.000000 webuntis-0.1.9/webuntis/utils/datetime_utils.py
+-rwxr-xr-x   0 untitaker  (1000) users      (100)     4079 2013-12-31 10:15:06.000000 webuntis-0.1.9/webuntis/utils/remote.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     1714 2013-10-17 10:26:47.000000 webuntis-0.1.9/webuntis/utils/userinput.py
+-rw-r--r--   0 untitaker  (1000) users      (100)      498 2012-12-15 18:56:15.000000 webuntis-0.1.9/webuntis/utils/logger.py
+-rwxr-xr-x   0 untitaker  (1000) users      (100)      795 2013-06-26 15:01:33.000000 webuntis-0.1.9/webuntis/errors.py
+drwxr-xr-x   0 untitaker  (1000) users      (100)        0 2014-01-22 16:15:00.000000 webuntis-0.1.9/webuntis.egg-info/
+-rwxr-xr-x   0 untitaker  (1000) users      (100)        9 2014-01-22 16:14:57.000000 webuntis-0.1.9/webuntis.egg-info/top_level.txt
+-rwxr-xr-x   0 untitaker  (1000) users      (100)     2302 2014-01-22 16:14:57.000000 webuntis-0.1.9/webuntis.egg-info/PKG-INFO
+-rwxr-xr-x   0 untitaker  (1000) users      (100)        1 2014-01-22 16:14:57.000000 webuntis-0.1.9/webuntis.egg-info/dependency_links.txt
+-rw-r--r--   0 untitaker  (1000) users      (100)        8 2014-01-22 16:14:57.000000 webuntis-0.1.9/webuntis.egg-info/requires.txt
+-rwxr-xr-x   0 untitaker  (1000) users      (100)     1048 2014-01-22 16:14:59.000000 webuntis-0.1.9/webuntis.egg-info/SOURCES.txt
+-rwxr-xr-x   0 untitaker  (1000) users      (100)     1404 2014-01-22 16:13:27.000000 webuntis-0.1.9/setup.py
+-rw-r--r--   0 untitaker  (1000) users      (100)     2302 2014-01-22 16:15:00.000000 webuntis-0.1.9/PKG-INFO
+-rw-r--r--   0 untitaker  (1000) users      (100)       77 2012-11-29 16:18:21.000000 webuntis-0.1.9/MANIFEST.in
+-rw-r--r--   0 untitaker  (1000) users      (100)     1464 2013-01-09 12:11:03.000000 webuntis-0.1.9/LICENSE
+-rwxr-xr-x   0 untitaker  (1000) users      (100)       82 2014-01-22 16:15:00.000000 webuntis-0.1.9/setup.cfg
```

### Comparing `webuntis-0.1.8/README.rst` & `webuntis-0.1.9/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 ===============
 python-webuntis
 ===============
 
+.. image:: https://travis-ci.org/untitaker/python-webuntis.png?branch=master
+   :target: https://travis-ci.org/untitaker/python-webuntis
+
+
 Bindings for WebUntis API
 =========================
 
 ::
 
     import webuntis
 
@@ -44,11 +48,11 @@
 
 
 Unittests
 +++++++++
 
 ::
 
-    $ python run-tests.py
+    $ pytest
 
 For the single testsuites and their descriptions, look at the docstrings of the
 modules in ``webuntis.tests``.
```

### Comparing `webuntis-0.1.8/webuntis/objects.py` & `webuntis-0.1.9/webuntis/objects.py`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis/session.py` & `webuntis-0.1.9/webuntis/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,28 +297,34 @@
 
     :type password: str
     :param password: The password used for the API.
 
     :type server: str
     :param server: A host name, a URL, or a URL without path.
 
-            >>> s = webuntis.Session(..., server='thalia.webuntis.com')
-            >>> s.config['server']
-            'http://thalia.webuntis.com/WebUntis/jsonrpc.do'
-            >>> # notice that there's NO SLASH at the end!
-            >>> s.config['server'] = 'https://thalia.webuntis.com'
-            >>> s.config['server']
-            'https://thalia.webuntis.com/WebUntis/jsonrpc.do'
-            >>> s.config['server'] = 'https://thalia.webuntis.com/'
-            >>> # because a slash gets interpreted as the full path to the API
-            >>> # endpoint, which would crash during login
-            >>> s.config['server']
-            'http://thalia.webuntis.com/'
-            >>> s.config['server'] = '!"$%/WebUntis/jsonrpc.do'
-            Traceback blah blah something ValueError
+        ::
+
+            s = webuntis.Session(..., server='thalia.webuntis.com')
+            # 'https://thalia.webuntis.com/WebUntis/jsonrpc.do'
+
+            # Want to disable SSL?
+            # make sure there's NO SLASH at the end!
+            s.config['server'] = 'http://thalia.webuntis.com'
+            # 'http://thalia.webuntis.com/WebUntis/jsonrpc.do'
+
+            # or maybe use a completely different API endpoint?
+            s.config['server'] = 'http://thalia.webuntis.com/WebUntis/jsonrpc2.do'
+            # 'http://thalia.webuntis.com/WebUntis/jsonrpc2.do'
+
+            # or just change the path?
+            s.config['server'] = 'thalia.webuntis.com/WebUntis/jsonrpc2.do'
+            # 'https://thalia.webuntis.com/WebUntis/jsonrpc2.do'
+
+            s.config['server'] = '!"$%/WebUntis/jsonrpc.do'
+            # ValueError: Not a valid hostname
 
     :type school: str
     :param school: A valid school name.
 
     :type useragent: str
     :param useragent: A string containing a useragent. Please include useful
         information, such as an email address, for the server maintainer. Just
```

### Comparing `webuntis-0.1.8/webuntis/tests/__init__.py` & `webuntis-0.1.9/webuntis/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis/tests/static/getstatusdata_mock.json` & `webuntis-0.1.9/webuntis/tests/static/getstatusdata_mock.json`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis/tests/static/getholidays_mock.json` & `webuntis-0.1.9/webuntis/tests/static/getholidays_mock.json`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis/tests/static/getklassen_mock.json` & `webuntis-0.1.9/webuntis/tests/static/getklassen_mock.json`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis/tests/static/getschoolyears_mock.json` & `webuntis-0.1.9/webuntis/tests/static/getschoolyears_mock.json`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis/tests/static/getteachers_mock.json` & `webuntis-0.1.9/webuntis/tests/static/getteachers_mock.json`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis/tests/static/getsubjects_mock.json` & `webuntis-0.1.9/webuntis/tests/static/getsubjects_mock.json`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis/tests/static/gettimegrid_mock.json` & `webuntis-0.1.9/webuntis/tests/static/gettimegrid_mock.json`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis/tests/static/gettimetables_mock.json` & `webuntis-0.1.9/webuntis/tests/static/gettimetables_mock.json`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis/tests/static/getrooms_mock.json` & `webuntis-0.1.9/webuntis/tests/static/getrooms_mock.json`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis/tests/test_session.py` & `webuntis-0.1.9/webuntis/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis/tests/test_objects.py` & `webuntis-0.1.9/webuntis/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis/utils/third_party.py` & `webuntis-0.1.9/webuntis/utils/third_party.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,15 +13,11 @@
 try:
     import json  # Python >= 2.6
 except ImportError:
     import simplejson as json  # from dependency "simplejson"
 
 try:
     # Python 3
-    import urllib.request as urlrequest
-    import urllib.error as urlerrors  # pragma: no cover
     import urllib.parse as urlparse  # pragma: no cover
 except ImportError:
     # Python 2
-    import urllib2
     import urlparse
-    urlrequest = urlerrors = urllib2
```

### Comparing `webuntis-0.1.8/webuntis/utils/misc.py` & `webuntis-0.1.9/webuntis/utils/misc.py`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis/utils/timetable_utils.py` & `webuntis-0.1.9/webuntis/utils/timetable_utils.py`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis/utils/datetime_utils.py` & `webuntis-0.1.9/webuntis/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis/utils/remote.py` & `webuntis-0.1.9/webuntis/utils/remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
     :copyright: (c) 2012 by Markus Unterwaditzer.
     :license: BSD, see LICENSE for more details.
 '''
 from webuntis import errors
 from webuntis.utils import log
 from webuntis.utils.userinput import unicode_string, bytestring
-from webuntis.utils.third_party import json, urlrequest
+from webuntis.utils.third_party import json
 
 import datetime
+import requests
 
 
 _errorcodes = {
     -32601: errors.MethodNotFoundError,
     -8504: errors.BadCredentialsError,
     -8520: errors.NotLoggedInError
 }
@@ -124,19 +125,17 @@
 
 
 def _send_request(url, data, headers):
     '''Sends a POST request given the endpoint URL, JSON-encodable data and
     a dictionary with headers.
     '''
 
-    request = urlrequest.Request(url, json.dumps(data).encode(), headers)
-    # this will eventually raise errors, e.g. if there's an unexpected http
-    # status code
-    result_obj = urlrequest.urlopen(request)
-    result = result_obj.read().decode('utf-8')
+    r = requests.post(url, data=json.dumps(data), headers=headers)
+    result = r.text
+    # this will eventually raise errors, e.g. on timeout
 
     try:
         result_data = json.loads(result)
         log('debug', 'Valid JSON found')
     except ValueError:
         raise errors.RemoteError('Invalid JSON', result)
     else:
```

### Comparing `webuntis-0.1.8/webuntis/utils/userinput.py` & `webuntis-0.1.9/webuntis/utils/userinput.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from .logger import log
 from .third_party import urlparse
 
 
 def server(url):
     if not re.match(r'^http(s?)\:\/\/', url):  # if we just have the hostname
         log('debug', 'The URL given doesn\'t seem to be a valid URL, just '
-                     'gonna prepend "http://"')
+                     'gonna prepend "https://"')
 
         # append the http prefix and hope for the best
-        url = 'http://' + url
+        url = 'https://' + url
 
     urlobj = urlparse.urlparse(url)
 
     if not urlobj.scheme or not urlobj.netloc:
         # urlparse failed
         raise ValueError('Not a valid URL or hostname')
```

### Comparing `webuntis-0.1.8/webuntis/errors.py` & `webuntis-0.1.9/webuntis/errors.py`

 * *Files identical despite different names*

### Comparing `webuntis-0.1.8/webuntis.egg-info/PKG-INFO` & `webuntis-0.1.9/webuntis.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 1.1
 Name: webuntis
-Version: 0.1.8
+Version: 0.1.9
 Summary: Bindings for WebUntis API
 Home-page: http://dev.unterwaditzer.net/python-webuntis/
 Author: Markus Unterwaditzer
 Author-email: markus@unterwaditzer.net
 License: new-style BSD
 Description: ===============
         python-webuntis
         ===============
         
+        .. image:: https://travis-ci.org/untitaker/python-webuntis.png?branch=master
+           :target: https://travis-ci.org/untitaker/python-webuntis
+        
+        
         Bindings for WebUntis API
         =========================
         
         ::
         
             import webuntis
         
@@ -52,15 +56,15 @@
         
         
         Unittests
         +++++++++
         
         ::
         
-            $ python run-tests.py
+            $ pytest
         
         For the single testsuites and their descriptions, look at the docstrings of the
         modules in ``webuntis.tests``.
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `webuntis-0.1.8/webuntis.egg-info/SOURCES.txt` & `webuntis-0.1.9/webuntis.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 webuntis/__init__.py
 webuntis/errors.py
 webuntis/objects.py
 webuntis/session.py
 webuntis.egg-info/PKG-INFO
 webuntis.egg-info/SOURCES.txt
 webuntis.egg-info/dependency_links.txt
+webuntis.egg-info/requires.txt
 webuntis.egg-info/top_level.txt
 webuntis/tests/__init__.py
 webuntis/tests/test_objects.py
 webuntis/tests/test_session.py
 webuntis/tests/static/getdepartments_mock.json
 webuntis/tests/static/getholidays_mock.json
 webuntis/tests/static/getklassen_mock.json
```

### Comparing `webuntis-0.1.8/setup.py` & `webuntis-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
     :copyright: (c) 2012 by Markus Unterwaditzer.
     :license: BSD, see LICENSE for more details.
 '''
 
 from setuptools import setup
 from sys import version_info
 
-dependencies = []
+dependencies = ['requests']
 
 if version_info < (2,6):
     dependencies.append('simplejson')
 
 if version_info < (2,7):
     dependencies.append('ordereddict')
 
 setup(
     name='webuntis',
-    version='0.1.8',
+    version='0.1.9',
     author='Markus Unterwaditzer',
     author_email='markus@unterwaditzer.net',
     packages=['webuntis', 'webuntis.utils', 'webuntis.tests'],
     include_package_data=True,
     url='http://dev.unterwaditzer.net/python-webuntis/',
     license='new-style BSD',
     description='Bindings for WebUntis API',
```

### Comparing `webuntis-0.1.8/PKG-INFO` & `webuntis-0.1.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 1.1
 Name: webuntis
-Version: 0.1.8
+Version: 0.1.9
 Summary: Bindings for WebUntis API
 Home-page: http://dev.unterwaditzer.net/python-webuntis/
 Author: Markus Unterwaditzer
 Author-email: markus@unterwaditzer.net
 License: new-style BSD
 Description: ===============
         python-webuntis
         ===============
         
+        .. image:: https://travis-ci.org/untitaker/python-webuntis.png?branch=master
+           :target: https://travis-ci.org/untitaker/python-webuntis
+        
+        
         Bindings for WebUntis API
         =========================
         
         ::
         
             import webuntis
         
@@ -52,15 +56,15 @@
         
         
         Unittests
         +++++++++
         
         ::
         
-            $ python run-tests.py
+            $ pytest
         
         For the single testsuites and their descriptions, look at the docstrings of the
         modules in ``webuntis.tests``.
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `webuntis-0.1.8/LICENSE` & `webuntis-0.1.9/LICENSE`

 * *Files identical despite different names*

