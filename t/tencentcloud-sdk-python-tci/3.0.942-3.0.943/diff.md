# Comparing `tmp/tencentcloud-sdk-python-tci-3.0.942.tar.gz` & `tmp/tencentcloud-sdk-python-tci-3.0.943.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tci-3.0.942.tar", last modified: Tue Jul 25 04:26:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tci-3.0.943.tar", last modified: Wed Jul 26 00:45:09 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tci-3.0.942.tar` & `tencentcloud-sdk-python-tci-3.0.943.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/tencentcloud/tci/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/tencentcloud/tci/v20190318/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/tencentcloud/tci/v20190318/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44187 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/tencentcloud/tci/v20190318/tci_client.py
--rw-r--r--   0 root         (0) root         (0)     8913 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/tencentcloud/tci/v20190318/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   285108 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/tencentcloud/tci/v20190318/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/tencentcloud/tci/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/tencentcloud_sdk_python_tci.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/tencentcloud_sdk_python_tci.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/tencentcloud_sdk_python_tci.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/tencentcloud_sdk_python_tci.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/tencentcloud_sdk_python_tci.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:26:20.000000 tencentcloud-sdk-python-tci-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/tencentcloud/tci/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/tencentcloud/tci/v20190318/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/tencentcloud/tci/v20190318/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44187 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/tencentcloud/tci/v20190318/tci_client.py
+-rw-r--r--   0 root         (0) root         (0)     8913 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/tencentcloud/tci/v20190318/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   285108 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/tencentcloud/tci/v20190318/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/tencentcloud/tci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/tencentcloud_sdk_python_tci.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/tencentcloud_sdk_python_tci.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/tencentcloud_sdk_python_tci.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/tencentcloud_sdk_python_tci.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/tencentcloud_sdk_python_tci.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-26 00:45:09.000000 tencentcloud-sdk-python-tci-3.0.943/README.rst
```

### Comparing `tencentcloud-sdk-python-tci-3.0.942/setup.py` & `tencentcloud-sdk-python-tci-3.0.943/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tci-3.0.942/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tci-3.0.943/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.942'
+__version__ = '3.0.943'
```

### Comparing `tencentcloud-sdk-python-tci-3.0.942/tencentcloud/tci/v20190318/tci_client.py` & `tencentcloud-sdk-python-tci-3.0.943/tencentcloud/tci/v20190318/tci_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tci-3.0.942/tencentcloud/tci/v20190318/errorcodes.py` & `tencentcloud-sdk-python-tci-3.0.943/tencentcloud/tci/v20190318/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tci-3.0.942/tencentcloud/tci/v20190318/models.py` & `tencentcloud-sdk-python-tci-3.0.943/tencentcloud/tci/v20190318/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tci-3.0.942/tencentcloud_sdk_python_tci.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tci-3.0.943/tencentcloud_sdk_python_tci.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tci
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Tci SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tci-3.0.942/PKG-INFO` & `tencentcloud-sdk-python-tci-3.0.943/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tci
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Tci SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tci-3.0.942/README.rst` & `tencentcloud-sdk-python-tci-3.0.943/README.rst`

 * *Files identical despite different names*

