# Comparing `tmp/tencentcloud-sdk-python-vm-3.0.942.tar.gz` & `tmp/tencentcloud-sdk-python-vm-3.0.943.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vm-3.0.942.tar", last modified: Tue Jul 25 04:29:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vm-3.0.943.tar", last modified: Wed Jul 26 00:48:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vm-3.0.942.tar` & `tencentcloud-sdk-python-vm-3.0.943.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:27.000000 tencentcloud-sdk-python-vm-3.0.942/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-25 04:29:26.000000 tencentcloud-sdk-python-vm-3.0.942/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:27.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud_sdk_python_vm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:29:27.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud_sdk_python_vm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      741 2023-07-25 04:29:27.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud_sdk_python_vm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-25 04:29:27.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud_sdk_python_vm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:29:27.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud_sdk_python_vm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:27.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:29:26.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:27.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:27.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20200709/
--rw-r--r--   0 root         (0) root         (0)     5863 2023-07-25 04:29:26.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20200709/vm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:29:26.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20200709/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-07-25 04:29:26.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20200709/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    76744 2023-07-25 04:29:26.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20200709/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:27.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20201229/
--rw-r--r--   0 root         (0) root         (0)     9114 2023-07-25 04:29:26.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20201229/vm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:29:26.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20201229/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-07-25 04:29:26.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20201229/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    95095 2023-07-25 04:29:26.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20201229/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:29:26.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:27.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20210922/
--rw-r--r--   0 root         (0) root         (0)     5305 2023-07-25 04:29:26.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20210922/vm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:29:26.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20210922/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-07-25 04:29:26.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20210922/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    84771 2023-07-25 04:29:26.000000 tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20210922/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:29:27.000000 tencentcloud-sdk-python-vm-3.0.942/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-25 04:29:27.000000 tencentcloud-sdk-python-vm-3.0.942/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-25 04:29:26.000000 tencentcloud-sdk-python-vm-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud_sdk_python_vm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud_sdk_python_vm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      741 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud_sdk_python_vm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud_sdk_python_vm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud_sdk_python_vm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20200709/
+-rw-r--r--   0 root         (0) root         (0)     5863 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20200709/vm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20200709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20200709/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    76744 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20200709/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20201229/
+-rw-r--r--   0 root         (0) root         (0)     9114 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20201229/vm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20201229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20201229/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    95095 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20201229/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20210922/
+-rw-r--r--   0 root         (0) root         (0)     5305 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20210922/vm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20210922/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20210922/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    84771 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20210922/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-26 00:48:00.000000 tencentcloud-sdk-python-vm-3.0.943/README.rst
```

### Comparing `tencentcloud-sdk-python-vm-3.0.942/setup.py` & `tencentcloud-sdk-python-vm-3.0.943/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.942/tencentcloud_sdk_python_vm.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-vm-3.0.943/tencentcloud_sdk_python_vm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.942/tencentcloud_sdk_python_vm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vm-3.0.943/tencentcloud_sdk_python_vm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vm
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Vm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vm-3.0.942/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vm-3.0.943/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20200709/vm_client.py` & `tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20200709/vm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20200709/errorcodes.py` & `tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20200709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20200709/models.py` & `tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20200709/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20201229/vm_client.py` & `tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20201229/vm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20201229/errorcodes.py` & `tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20201229/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20201229/models.py` & `tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20201229/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20210922/vm_client.py` & `tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20210922/vm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20210922/errorcodes.py` & `tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20210922/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.942/tencentcloud/vm/v20210922/models.py` & `tencentcloud-sdk-python-vm-3.0.943/tencentcloud/vm/v20210922/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vm-3.0.942/PKG-INFO` & `tencentcloud-sdk-python-vm-3.0.943/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vm
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Vm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vm-3.0.942/README.rst` & `tencentcloud-sdk-python-vm-3.0.943/README.rst`

 * *Files identical despite different names*

