# Comparing `tmp/delta-sharing-0.7.1.tar.gz` & `tmp/delta-sharing-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delta-sharing-0.7.1.tar", last modified: Mon Jul 17 23:20:46 2023, max compression
+gzip compressed data, was "delta-sharing-0.7.2.tar", last modified: Tue Jul 25 21:40:14 2023, max compression
```

## Comparing `delta-sharing-0.7.1.tar` & `delta-sharing-0.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-07-17 23:20:46.788423 delta-sharing-0.7.1/
--rw-r--r--   0 lin.zhou   (502) staff       (20)      534 2023-07-17 23:08:22.000000 delta-sharing-0.7.1/NOTICE.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2282 2023-07-17 23:20:46.788240 delta-sharing-0.7.1/PKG-INFO
--rw-r--r--   0 lin.zhou   (502) staff       (20)     1201 2023-07-10 07:05:33.000000 delta-sharing-0.7.1/README.md
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-07-17 23:20:46.786462 delta-sharing-0.7.1/delta_sharing/
--rw-r--r--   0 lin.zhou   (502) staff       (20)     1274 2023-07-17 23:08:22.000000 delta-sharing-0.7.1/delta_sharing/__init__.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)      855 2023-07-10 07:05:33.000000 delta-sharing-0.7.1/delta_sharing/_yarl_patch.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)     5066 2023-07-10 07:05:33.000000 delta-sharing-0.7.1/delta_sharing/converter.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)    12923 2023-07-17 23:08:22.000000 delta-sharing-0.7.1/delta_sharing/delta_sharing.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)    10304 2023-07-17 23:08:22.000000 delta-sharing-0.7.1/delta_sharing/protocol.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)     7912 2023-07-17 23:08:22.000000 delta-sharing-0.7.1/delta_sharing/reader.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)    16644 2023-07-17 23:08:22.000000 delta-sharing-0.7.1/delta_sharing/rest_client.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)      626 2023-07-17 23:19:50.000000 delta-sharing-0.7.1/delta_sharing/version.py
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-07-17 23:20:46.787952 delta-sharing-0.7.1/delta_sharing.egg-info/
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2282 2023-07-17 23:20:46.000000 delta-sharing-0.7.1/delta_sharing.egg-info/PKG-INFO
--rw-r--r--   0 lin.zhou   (502) staff       (20)      430 2023-07-17 23:20:46.000000 delta-sharing-0.7.1/delta_sharing.egg-info/SOURCES.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)        1 2023-07-17 23:20:46.000000 delta-sharing-0.7.1/delta_sharing.egg-info/dependency_links.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)      167 2023-07-17 23:20:46.000000 delta-sharing-0.7.1/delta_sharing.egg-info/requires.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)       14 2023-07-17 23:20:46.000000 delta-sharing-0.7.1/delta_sharing.egg-info/top_level.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)       38 2023-07-17 23:20:46.788538 delta-sharing-0.7.1/setup.cfg
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2600 2023-07-10 07:05:33.000000 delta-sharing-0.7.1/setup.py
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-07-25 21:40:14.879483 delta-sharing-0.7.2/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      534 2023-07-21 00:01:06.000000 delta-sharing-0.7.2/NOTICE.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2282 2023-07-25 21:40:14.879310 delta-sharing-0.7.2/PKG-INFO
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     1201 2023-07-10 07:05:33.000000 delta-sharing-0.7.2/README.md
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-07-25 21:40:14.877788 delta-sharing-0.7.2/delta_sharing/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     1274 2023-07-21 00:01:06.000000 delta-sharing-0.7.2/delta_sharing/__init__.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      855 2023-07-10 07:05:33.000000 delta-sharing-0.7.2/delta_sharing/_yarl_patch.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     5066 2023-07-10 07:05:33.000000 delta-sharing-0.7.2/delta_sharing/converter.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)    12923 2023-07-21 00:01:06.000000 delta-sharing-0.7.2/delta_sharing/delta_sharing.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)    10304 2023-07-21 00:01:06.000000 delta-sharing-0.7.2/delta_sharing/protocol.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     7912 2023-07-21 00:01:06.000000 delta-sharing-0.7.2/delta_sharing/reader.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)    16644 2023-07-21 00:01:06.000000 delta-sharing-0.7.2/delta_sharing/rest_client.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      626 2023-07-25 21:37:48.000000 delta-sharing-0.7.2/delta_sharing/version.py
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-07-25 21:40:14.878995 delta-sharing-0.7.2/delta_sharing.egg-info/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2282 2023-07-25 21:40:14.000000 delta-sharing-0.7.2/delta_sharing.egg-info/PKG-INFO
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      430 2023-07-25 21:40:14.000000 delta-sharing-0.7.2/delta_sharing.egg-info/SOURCES.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)        1 2023-07-25 21:40:14.000000 delta-sharing-0.7.2/delta_sharing.egg-info/dependency_links.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      167 2023-07-25 21:40:14.000000 delta-sharing-0.7.2/delta_sharing.egg-info/requires.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)       14 2023-07-25 21:40:14.000000 delta-sharing-0.7.2/delta_sharing.egg-info/top_level.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)       38 2023-07-25 21:40:14.879582 delta-sharing-0.7.2/setup.cfg
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2600 2023-07-10 07:05:33.000000 delta-sharing-0.7.2/setup.py
```

### Comparing `delta-sharing-0.7.1/NOTICE.txt` & `delta-sharing-0.7.2/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.1/PKG-INFO` & `delta-sharing-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delta-sharing
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python Connector for Delta Sharing
 Home-page: https://github.com/delta-io/delta-sharing/
 Author: The Delta Lake Project Authors
 Author-email: delta-users@googlegroups.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/delta-io/delta-sharing
 Project-URL: Documentation, https://github.com/delta-io/delta-sharing
```

### Comparing `delta-sharing-0.7.1/README.md` & `delta-sharing-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.1/delta_sharing/__init__.py` & `delta-sharing-0.7.2/delta_sharing/__init__.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.1/delta_sharing/_yarl_patch.py` & `delta-sharing-0.7.2/delta_sharing/_yarl_patch.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.1/delta_sharing/converter.py` & `delta-sharing-0.7.2/delta_sharing/converter.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.1/delta_sharing/delta_sharing.py` & `delta-sharing-0.7.2/delta_sharing/delta_sharing.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.1/delta_sharing/protocol.py` & `delta-sharing-0.7.2/delta_sharing/protocol.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.1/delta_sharing/reader.py` & `delta-sharing-0.7.2/delta_sharing/reader.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.1/delta_sharing/rest_client.py` & `delta-sharing-0.7.2/delta_sharing/rest_client.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.1/delta_sharing/version.py` & `delta-sharing-0.7.2/delta_sharing/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.7.1"
+__version__ = "0.7.2"
```

### Comparing `delta-sharing-0.7.1/delta_sharing.egg-info/PKG-INFO` & `delta-sharing-0.7.2/delta_sharing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delta-sharing
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python Connector for Delta Sharing
 Home-page: https://github.com/delta-io/delta-sharing/
 Author: The Delta Lake Project Authors
 Author-email: delta-users@googlegroups.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/delta-io/delta-sharing
 Project-URL: Documentation, https://github.com/delta-io/delta-sharing
```

### Comparing `delta-sharing-0.7.1/setup.py` & `delta-sharing-0.7.2/setup.py`

 * *Files identical despite different names*

