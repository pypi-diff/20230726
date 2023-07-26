# Comparing `tmp/efpy-0.1.3.tar.gz` & `tmp/efpy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efpy-0.1.3.tar", last modified: Wed Jul 26 14:01:03 2023, max compression
+gzip compressed data, was "efpy-0.1.4.tar", last modified: Wed Jul 26 14:11:53 2023, max compression
```

## Comparing `efpy-0.1.3.tar` & `efpy-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 14:01:03.425197 efpy-0.1.3/
--rw-rw-rw-   0        0        0      255 2023-07-26 14:01:03.425197 efpy-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 14:01:03.425197 efpy-0.1.3/efpy/
--rw-rw-rw-   0        0        0     1082 2023-07-26 14:00:22.000000 efpy-0.1.3/efpy/__init__.py
--rw-rw-rw-   0        0        0     1447 2021-06-24 08:59:48.000000 efpy-0.1.3/efpy/env.py
--rw-rw-rw-   0        0        0     2723 2023-07-26 13:58:57.000000 efpy-0.1.3/efpy/expHelper.py
-drwxrwxrwx   0        0        0        0 2023-07-26 14:01:03.425197 efpy-0.1.3/efpy.egg-info/
--rw-rw-rw-   0        0        0      255 2023-07-26 14:01:03.000000 efpy-0.1.3/efpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-07-26 14:01:03.000000 efpy-0.1.3/efpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 14:01:03.000000 efpy-0.1.3/efpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-26 14:01:03.000000 efpy-0.1.3/efpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-26 14:01:03.000000 efpy-0.1.3/efpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 14:01:03.425197 efpy-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      752 2023-07-26 13:58:19.000000 efpy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:11:53.704205 efpy-0.1.4/
+-rw-rw-rw-   0        0        0      255 2023-07-26 14:11:53.704205 efpy-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 14:11:53.704205 efpy-0.1.4/efpy/
+-rw-rw-rw-   0        0        0     1106 2023-07-26 14:10:32.000000 efpy-0.1.4/efpy/__init__.py
+-rw-rw-rw-   0        0        0     1447 2021-06-24 08:59:48.000000 efpy-0.1.4/efpy/env.py
+-rw-rw-rw-   0        0        0     2723 2023-07-26 13:58:57.000000 efpy-0.1.4/efpy/expHelper.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:11:53.704205 efpy-0.1.4/efpy.egg-info/
+-rw-rw-rw-   0        0        0      255 2023-07-26 14:11:53.000000 efpy-0.1.4/efpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-07-26 14:11:53.000000 efpy-0.1.4/efpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 14:11:53.000000 efpy-0.1.4/efpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 14:11:53.000000 efpy-0.1.4/efpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-26 14:11:53.000000 efpy-0.1.4/efpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 14:11:53.704205 efpy-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-07-26 14:11:45.000000 efpy-0.1.4/setup.py
```

### Comparing `efpy-0.1.3/efpy/__init__.py` & `efpy-0.1.4/efpy/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ##########################################################################
 from efpy.env import printResult
 from efpy.env import getParams
 from efpy.env import isExpEnv
 
-from .expHelper import getYamlConfName
-from .expHelper import getSubExpId
-from .expHelper import unpackAggrParam
-from .expHelper import convParam2Setting
-from .expHelper import loadSettingFromYaml
-from .expHelper import removeNoneSetting
+from efpy.expHelper import getYamlConfName
+from efpy.expHelper import getSubExpId
+from efpy.expHelper import unpackAggrParam
+from efpy.expHelper import convParam2Setting
+from efpy.expHelper import loadSettingFromYaml
+from efpy.expHelper import removeNoneSetting
```

### Comparing `efpy-0.1.3/efpy/env.py` & `efpy-0.1.4/efpy/env.py`

 * *Files identical despite different names*

### Comparing `efpy-0.1.3/efpy/expHelper.py` & `efpy-0.1.4/efpy/expHelper.py`

 * *Files identical despite different names*

### Comparing `efpy-0.1.3/setup.py` & `efpy-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 #############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
     name = "efpy",
-    version = "0.1.3",
+    version = "0.1.4",
     keywords = ("experience","environment"),
     description = "experience",
     long_description = "experience",
     license = "MIT Licence",
 
     url = "https://github.com/imcjp/efpy",
     author = "Cai Jianping",
     author_email = "jpingcai@163.com",
 
     packages = find_packages(),
     include_package_data = True,
     platforms = "any",
-    install_requires = ['yaml','re']
+    install_requires = ['PyYAML']
 )
```

