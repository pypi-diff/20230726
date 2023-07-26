# Comparing `tmp/tencentcloud-sdk-python-asr-3.0.942.tar.gz` & `tmp/tencentcloud-sdk-python-asr-3.0.943.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.942.tar", last modified: Tue Jul 25 04:10:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.943.tar", last modified: Wed Jul 26 00:30:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-asr-3.0.942.tar` & `tencentcloud-sdk-python-asr-3.0.943.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud_sdk_python_asr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud_sdk_python_asr.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/v20190614/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/v20190614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29417 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/v20190614/asr_client.py
--rw-r--r--   0 root         (0) root         (0)     7480 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/v20190614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   111930 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/v20190614/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:10:58.000000 tencentcloud-sdk-python-asr-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud_sdk_python_asr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud_sdk_python_asr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/v20190614/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/v20190614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29417 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/v20190614/asr_client.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/v20190614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   112062 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/v20190614/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/README.rst
```

### Comparing `tencentcloud-sdk-python-asr-3.0.942/setup.py` & `tencentcloud-sdk-python-asr-3.0.943/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.942/tencentcloud_sdk_python_asr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.943/tencentcloud_sdk_python_asr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/v20190614/asr_client.py` & `tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/v20190614/asr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/v20190614/errorcodes.py` & `tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/v20190614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.942/tencentcloud/asr/v20190614/models.py` & `tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/v20190614/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1750,16 +1750,18 @@
     """热词的词和权重
 
     """
 
     def __init__(self):
         r"""
         :param _Word: 热词
+注意：此字段可能返回 null，表示取不到有效值。
         :type Word: str
         :param _Weight: 权重
+注意：此字段可能返回 null，表示取不到有效值。
         :type Weight: int
         """
         self._Word = None
         self._Weight = None
 
     @property
     def Word(self):
```

### Comparing `tencentcloud-sdk-python-asr-3.0.942/tencentcloud/__init__.py` & `tencentcloud-sdk-python-asr-3.0.943/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-asr-3.0.942/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.943/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.942/README.rst` & `tencentcloud-sdk-python-asr-3.0.943/README.rst`

 * *Files identical despite different names*

