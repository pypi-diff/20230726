# Comparing `tmp/openstg-1.19.0.tar.gz` & `tmp/openstg-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openstg-1.19.0.tar", last modified: Wed Jul 26 14:13:31 2023, max compression
+gzip compressed data, was "dist/openstg-1.2.0.tar", last modified: Thu Feb 27 08:51:19 2020, max compression
```

## Comparing `openstg-1.19.0.tar` & `openstg-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,24 @@
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2023-07-26 14:13:31.000000 openstg-1.19.0/
--rw-rw-r--   0 afita     (1000) afita     (1000)      291 2023-07-26 14:13:31.000000 openstg-1.19.0/PKG-INFO
--rw-rw-r--   0 afita     (1000) afita     (1000)       38 2023-07-26 14:13:31.000000 openstg-1.19.0/setup.cfg
--rw-rw-r--   0 afita     (1000) afita     (1000)      648 2023-07-26 14:12:08.000000 openstg-1.19.0/setup.py
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2023-07-26 14:13:31.000000 openstg-1.19.0/openstg/
--rw-r--r--   0 afita     (1000) afita     (1000)      210 2020-07-07 08:22:35.000000 openstg-1.19.0/openstg/app.py
--rw-rw-r--   0 afita     (1000) afita     (1000)     1267 2023-06-30 06:41:26.000000 openstg-1.19.0/openstg/SqliteCounter.py
--rw-rw-r--   0 afita     (1000) afita     (1000)     7806 2023-07-26 14:11:42.000000 openstg-1.19.0/openstg/ws_stg.py
--rw-r--r--   0 afita     (1000) afita     (1000)      218 2020-07-07 08:22:35.000000 openstg-1.19.0/openstg/stgapp.py
--rw-rw-r--   0 afita     (1000) afita     (1000)     1566 2023-07-06 13:29:34.000000 openstg-1.19.0/openstg/utils.py
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2023-07-26 14:13:31.000000 openstg-1.19.0/openstg/api/
--rw-rw-r--   0 afita     (1000) afita     (1000)     1367 2023-07-26 14:11:42.000000 openstg-1.19.0/openstg/api/constants.py
--rw-rw-r--   0 afita     (1000) afita     (1000)    35431 2023-07-26 14:11:42.000000 openstg-1.19.0/openstg/api/__init__.py
--rw-rw-r--   0 afita     (1000) afita     (1000)     5181 2023-07-26 14:11:42.000000 openstg-1.19.0/openstg/api/rtu.py
--rw-r--r--   0 afita     (1000) afita     (1000)       14 2020-02-27 08:49:02.000000 openstg-1.19.0/openstg/__init__.py
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2023-07-26 14:13:31.000000 openstg-1.19.0/openstg/stg/
--rw-r--r--   0 afita     (1000) afita     (1000)     4943 2020-07-07 08:22:35.000000 openstg-1.19.0/openstg/stg/__init__.py
--rw-rw-r--   0 afita     (1000) afita     (1000)     2211 2023-07-26 14:11:42.000000 openstg-1.19.0/openstg/config.py
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2023-07-26 14:13:31.000000 openstg-1.19.0/openstg/services/
--rw-rw-r--   0 afita     (1000) afita     (1000)      459 2023-06-22 07:56:51.000000 openstg-1.19.0/openstg/services/__init__.py
--rw-rw-r--   0 afita     (1000) afita     (1000)     4170 2022-10-25 18:11:13.000000 openstg-1.19.0/openstg/erpapi.py
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2023-07-26 14:13:31.000000 openstg-1.19.0/openstg.egg-info/
--rw-r--r--   0 afita     (1000) afita     (1000)        8 2023-07-26 14:13:31.000000 openstg-1.19.0/openstg.egg-info/top_level.txt
--rw-r--r--   0 afita     (1000) afita     (1000)      442 2023-07-26 14:13:31.000000 openstg-1.19.0/openstg.egg-info/SOURCES.txt
--rw-r--r--   0 afita     (1000) afita     (1000)      291 2023-07-26 14:13:31.000000 openstg-1.19.0/openstg.egg-info/PKG-INFO
--rw-r--r--   0 afita     (1000) afita     (1000)        1 2023-07-26 14:13:31.000000 openstg-1.19.0/openstg.egg-info/dependency_links.txt
--rw-r--r--   0 afita     (1000) afita     (1000)      154 2023-07-26 14:13:31.000000 openstg-1.19.0/openstg.egg-info/requires.txt
--rw-r--r--   0 afita     (1000) afita     (1000)      380 2020-07-07 08:22:35.000000 openstg-1.19.0/README.md
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-02-27 08:51:19.000000 openstg-1.2.0/
+-rw-r--r--   0 afita     (1000) afita     (1000)      290 2020-02-27 08:51:19.000000 openstg-1.2.0/PKG-INFO
+-rw-r--r--   0 afita     (1000) afita     (1000)       38 2020-02-27 08:51:19.000000 openstg-1.2.0/setup.cfg
+-rw-r--r--   0 afita     (1000) afita     (1000)      653 2020-02-27 08:49:24.000000 openstg-1.2.0/setup.py
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg/
+-rw-r--r--   0 afita     (1000) afita     (1000)      163 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/app.py
+-rw-r--r--   0 afita     (1000) afita     (1000)     4672 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/server.py
+-rw-r--r--   0 afita     (1000) afita     (1000)     1102 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/SqliteCounter.py
+-rw-r--r--   0 afita     (1000) afita     (1000)     1381 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/utils.py
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg/api/
+-rw-r--r--   0 afita     (1000) afita     (1000)    19729 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/api/__init__.py
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg/serializers/
+-rw-r--r--   0 afita     (1000) afita     (1000)      687 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/serializers/__init__.py
+-rw-r--r--   0 afita     (1000) afita     (1000)       14 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/__init__.py
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg/models/
+-rw-r--r--   0 afita     (1000) afita     (1000)     1771 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/models/__init__.py
+-rw-r--r--   0 afita     (1000) afita     (1000)     1568 2020-02-27 08:49:02.000000 openstg-1.2.0/openstg/config.py
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg.egg-info/
+-rw-r--r--   0 afita     (1000) afita     (1000)        8 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg.egg-info/top_level.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      368 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg.egg-info/SOURCES.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      290 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg.egg-info/PKG-INFO
+-rw-r--r--   0 afita     (1000) afita     (1000)        1 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg.egg-info/dependency_links.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      160 2020-02-27 08:51:19.000000 openstg-1.2.0/openstg.egg-info/requires.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)       98 2020-02-27 08:49:02.000000 openstg-1.2.0/README.md
```

### Comparing `openstg-1.19.0/setup.py` & `openstg-1.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='openstg',
-    version='1.19.0',
+    version='1.2.0',
     packages=find_packages(),
     url='https://github.com/gisce/openstg',
     license='GNU Affero General Public License v3',
     author='GISCE-TI, S.L.',
     author_email='devel@gisce.net',
     install_requires=[
-        'ERPpeek',
+        'ERPpeek==1.6.3',
         'Flask==0.12.2',
         'Flask-Cors==3.0.2',
         'Flask-Login==0.2.11',
         'Flask-RESTful==0.3.5',
         'flask-restplus==0.10.1',
-        'primestg>=1.40.0',
+        'primestg>=1.3.0',
         'marshmallow<3',
         'osconf==0.1.3',
         'pytz',
     ],
     description='API for STG-Protocol-DC Interface Specification'
 )
```

### Comparing `openstg-1.19.0/openstg/SqliteCounter.py` & `openstg-1.2.0/openstg/SqliteCounter.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,45 +2,37 @@
 import random
 import os
 import time
 
 
 default_filename = 'sqlite_counter.db'
 
-
-class SqliteCounter:
+class SqliteCounter():
     def __init__(self, filename):
         if not os.path.isfile(filename):
             self.db_init(filename)
         else:
             self.con = sqlite3.connect(filename)
 
     def next(self):
         with self.con:
             self.con.execute('UPDATE counter SET value = (value + 1) % 4294967295')
             for row in self.con.execute('SELECT value FROM counter WHERE name="stg"'):
                 return row[0]
 
-    def current(self):
-        with self.con:
-            for row in self.con.execute('SELECT value FROM counter WHERE name="stg"'):
-                return row[0]
-
     def db_init(self, filename):
         self.con = sqlite3.connect(filename)
         with self.con:
             self.con.execute('CREATE TABLE counter (id PRIMARY KEY, value integer, name varchar)')
             self.con.execute('INSERT INTO counter VALUES (1,0,"stg")')
 
-
 def work():
     counter = SqliteCounter(default_filename)
     pid = os.getpid()
     for num in range(1, 25):
         wait_time = random.randint(0, 2)
         time.sleep(wait_time/100.0)
         res = counter.next()
         print('{}: {}'.format(pid, res))
 
-
 if __name__ == '__main__':
     work()
```

### Comparing `openstg-1.19.0/openstg/stg/__init__.py` & `openstg-1.2.0/openstg/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# coding: utf-8
 from flask import Flask, request
-from flask_restplus import Api, Resource
 import xml.dom.minidom as xmlmd
 import time
 import os
-
+app = Flask(__name__)
 
 dc_status = {
         '0': "SUCCESS: The request with ID {} for the concentrator {} have "
              "finished successfully. {}",
         '1': "WORKING: The request with ID {} for the concentrator {} is "
              "still in progress. {}",
         '2': "ERROR: The request with ID {} for the concentrator {} has "
@@ -41,41 +39,31 @@
              "ID {}. But any report after it is missing",
         '3': "ERROR: The meter {} couldn't finish serving the request with "
              "ID {}. Order partially applied (part of the data sent in the "
              "order were not correctly applied in the meter)."
     }
 
 
-class Stg(Api):
-    def _register_doc(self, app_or_blueprint):
-        #We have to
-        pass
-
-
 def getText(nodelist):
     rc = []
     for node in nodelist:
         if node.nodeType == node.TEXT_NODE:
             rc.append(node.data)
     return ''.join(rc)
 
 
-class WSStgResource(Resource):
-
-    def post(self):
-        f_name = '/tmp/post-{}'.format(time.time())
-        if isinstance(request.data, bytes):
-            # Python3 backwards compatibility
-            request.data = request.data.decode()
-        with open(f_name, 'w') as f:
-            f.write(request.data)
-        out_msg = manage_request()
-        os.remove(f_name)
-        print(out_msg)
-        return "Ok", 200
+@app.route('/', methods=['POST'])
+def allrequests():
+    f_name = 'post-{}'.format(time.time())
+    with open(f_name, 'w') as f:
+        f.write(request.data)
+    out_msg = manage_request()
+    os.remove(f_name)
+    print out_msg
+    return "Ok", 200
 
 
 def manage_request_status(info):
     if 'Reference' not in info:
         info['Reference'] = ''
     default = "ERROR: The request with ID {} for the concentrator {}. has " \
               "suffered an UNKNOWN error {}".format(info['IdPet'],
@@ -124,10 +112,9 @@
         dc_status.get(info['ReqStatus'], default).format(info['IdPet'],
                                                          info['IdDC'],
                                                          info['Reference']))
 
     # TODO: Connect to ERP to read the S15 report received
 
 
-resources = [
-    (WSStgResource, '/ws')
-]
+if __name__ == '__main__':
+    app.run(host='0.0.0.0', port=5656, debug=True)
```

