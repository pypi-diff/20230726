# Comparing `tmp/openshift-0.9.2.tar.gz` & `tmp/openshift-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openshift-0.9.2.tar", last modified: Wed Sep  4 19:32:07 2019, max compression
+gzip compressed data, was "dist/openshift-0.9.3.tar", last modified: Fri Feb 28 21:59:57 2020, max compression
```

## Comparing `openshift-0.9.2.tar` & `openshift-0.9.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-04 19:32:07.000000 openshift-0.9.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12939 2019-09-04 19:31:35.000000 openshift-0.9.2/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     2474 2019-09-04 19:31:35.000000 openshift-0.9.2/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-04 19:32:07.000000 openshift-0.9.2/openshift.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2019-09-04 19:32:07.000000 openshift-0.9.2/openshift.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2019-09-04 19:32:07.000000 openshift-0.9.2/openshift.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      889 2019-09-04 19:32:07.000000 openshift-0.9.2/openshift.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-09-04 19:32:07.000000 openshift-0.9.2/openshift.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2019-09-04 19:32:07.000000 openshift-0.9.2/openshift.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      481 2019-09-04 19:32:07.000000 openshift-0.9.2/openshift.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      722 2019-09-04 19:32:07.000000 openshift-0.9.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2019-09-04 19:31:35.000000 openshift-0.9.2/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      889 2019-09-04 19:32:07.000000 openshift-0.9.2/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-04 19:32:07.000000 openshift-0.9.2/openshift/
--rw-rw-r--   0 travis    (2000) travis    (2000)      741 2019-09-04 19:31:35.000000 openshift-0.9.2/openshift/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-04 19:32:07.000000 openshift-0.9.2/openshift/helper/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1404 2019-09-04 19:31:35.000000 openshift-0.9.2/openshift/helper/hashes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-09-04 19:31:35.000000 openshift-0.9.2/openshift/helper/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-04 19:32:07.000000 openshift-0.9.2/openshift/dynamic/
--rw-rw-r--   0 travis    (2000) travis    (2000)    41283 2019-09-04 19:31:35.000000 openshift-0.9.2/openshift/dynamic/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3256 2019-09-04 19:31:35.000000 openshift-0.9.2/openshift/dynamic/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       30 2019-09-04 19:31:35.000000 openshift-0.9.2/openshift/dynamic/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3812 2019-09-04 19:31:35.000000 openshift-0.9.2/openshift/dynamic/apply.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-04 19:32:07.000000 openshift-0.9.2/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1477 2019-09-04 19:31:35.000000 openshift-0.9.2/scripts/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-09-04 19:31:35.000000 openshift-0.9.2/scripts/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-28 21:59:57.000000 openshift-0.9.3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       82 2020-02-28 21:59:28.000000 openshift-0.9.3/requirements.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-28 21:59:57.000000 openshift-0.9.3/openshift/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-28 21:59:57.000000 openshift-0.9.3/openshift/helper/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1404 2020-02-28 21:59:28.000000 openshift-0.9.3/openshift/helper/hashes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-28 21:59:28.000000 openshift-0.9.3/openshift/helper/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-28 21:59:57.000000 openshift-0.9.3/openshift/dynamic/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3256 2020-02-28 21:59:28.000000 openshift-0.9.3/openshift/dynamic/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3812 2020-02-28 21:59:28.000000 openshift-0.9.3/openshift/dynamic/apply.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       30 2020-02-28 21:59:28.000000 openshift-0.9.3/openshift/dynamic/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41284 2020-02-28 21:59:28.000000 openshift-0.9.3/openshift/dynamic/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      741 2020-02-28 21:59:28.000000 openshift-0.9.3/openshift/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      889 2020-02-28 21:59:57.000000 openshift-0.9.3/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12939 2020-02-28 21:59:28.000000 openshift-0.9.3/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-28 21:59:57.000000 openshift-0.9.3/scripts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1477 2020-02-28 21:59:28.000000 openshift-0.9.3/scripts/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-28 21:59:28.000000 openshift-0.9.3/scripts/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      722 2020-02-28 21:59:57.000000 openshift-0.9.3/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-28 21:59:57.000000 openshift-0.9.3/openshift.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      889 2020-02-28 21:59:57.000000 openshift-0.9.3/openshift.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-28 21:59:57.000000 openshift-0.9.3/openshift.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       18 2020-02-28 21:59:57.000000 openshift-0.9.3/openshift.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      481 2020-02-28 21:59:57.000000 openshift-0.9.3/openshift.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       78 2020-02-28 21:59:57.000000 openshift-0.9.3/openshift.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       80 2020-02-28 21:59:57.000000 openshift-0.9.3/openshift.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2474 2020-02-28 21:59:28.000000 openshift-0.9.3/setup.py
```

### Comparing `openshift-0.9.2/README.md` & `openshift-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `openshift-0.9.2/setup.py` & `openshift-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 http://pypi.python.org/pypi/setuptools
 """
 
 from setuptools import find_packages, setup
 
 # Do not edit these constants. They will be updated automatically
 # by scripts/update-client.sh.
-CLIENT_VERSION = "0.9.2"
+CLIENT_VERSION = "0.9.3"
 PACKAGE_NAME = "openshift"
 DEVELOPMENT_STATUS = "3 - Alpha"
 
 
 def extract_requirements(filename):
     """
     Extracts requirements from a pip formatted requirements file.
```

### Comparing `openshift-0.9.2/openshift.egg-info/PKG-INFO` & `openshift-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openshift
-Version: 0.9.2
+Version: 0.9.3
 Summary: OpenShift python client
 Home-page: https://github.com/openshift/openshift-restclient-python
 Author: OpenShift
 Author-email: UNKNOWN
 License: Apache License Version 2.0
 Description: Python client for OpenShift http://openshift.redhat.com/
 Keywords: Swagger,OpenAPI,Kubernetes,OpenShift
```

### Comparing `openshift-0.9.2/setup.cfg` & `openshift-0.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `openshift-0.9.2/PKG-INFO` & `openshift-0.9.3/openshift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openshift
-Version: 0.9.2
+Version: 0.9.3
 Summary: OpenShift python client
 Home-page: https://github.com/openshift/openshift-restclient-python
 Author: OpenShift
 Author-email: UNKNOWN
 License: Apache License Version 2.0
 Description: Python client for OpenShift http://openshift.redhat.com/
 Keywords: Swagger,OpenAPI,Kubernetes,OpenShift
```

### Comparing `openshift-0.9.2/openshift/__init__.py` & `openshift-0.9.3/openshift/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Do not edit these constants. They will be updated automatically
 # by scripts/update-version.sh.
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 __k8s_client_version__ = "9.0.0"
```

### Comparing `openshift-0.9.2/openshift/helper/hashes.py` & `openshift-0.9.3/openshift/helper/hashes.py`

 * *Files identical despite different names*

### Comparing `openshift-0.9.2/openshift/dynamic/client.py` & `openshift-0.9.3/openshift/dynamic/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,15 +597,15 @@
         easy searching and retrieval of specific resources.
 
         Subclasses implement the abstract methods with different loading strategies.
     """
 
     def __init__(self, client, cache_file):
         self.client = client
-        default_cachefile_name = 'osrcp-{0}.json'.format(hashlib.md5(self.__get_default_cache_id()).hexdigest())
+        default_cachefile_name = 'osrcp-{0}.json'.format(hashlib.sha1(self.__get_default_cache_id()).hexdigest())
         self.__cache_file = cache_file or os.path.join(tempfile.gettempdir(), default_cachefile_name)
         self.__init_cache()
 
     def __get_default_cache_id(self):
         user = ""
         for func in [os.getlogin, os.getuid]:
             try:
```

### Comparing `openshift-0.9.2/openshift/dynamic/exceptions.py` & `openshift-0.9.3/openshift/dynamic/exceptions.py`

 * *Files identical despite different names*

### Comparing `openshift-0.9.2/openshift/dynamic/apply.py` & `openshift-0.9.3/openshift/dynamic/apply.py`

 * *Files identical despite different names*

### Comparing `openshift-0.9.2/scripts/constants.py` & `openshift-0.9.3/scripts/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Spec version will be set in downloaded spec and all
 # generated code will refer to it.
 SPEC_VERSION = "v3.9.0"
 
 # client version for packaging and releasing. It can
 # be different than SPEC_VERSION.
-CLIENT_VERSION = "0.9.2"
+CLIENT_VERSION = "0.9.3"
 KUBERNETES_CLIENT_VERSION = "9.0.0"
 
 # Name of the release package
 PACKAGE_NAME = "openshift"
 
 # Stage of development, mainly used in setup.py's classifiers.
 DEVELOPMENT_STATUS = "3 - Alpha"
```

