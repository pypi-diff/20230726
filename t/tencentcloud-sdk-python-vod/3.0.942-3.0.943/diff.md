# Comparing `tmp/tencentcloud-sdk-python-vod-3.0.942.tar.gz` & `tmp/tencentcloud-sdk-python-vod-3.0.943.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.942.tar", last modified: Tue Jul 25 04:29:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.943.tar", last modified: Wed Jul 26 00:48:10 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vod-3.0.942.tar` & `tencentcloud-sdk-python-vod-3.0.943.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/tencentcloud/vod/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/tencentcloud/vod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/tencentcloud/vod/v20180717/
--rw-r--r--   0 root         (0) root         (0)   183379 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/tencentcloud/vod/v20180717/vod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/tencentcloud/vod/v20180717/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25211 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/tencentcloud/vod/v20180717/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1854207 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/tencentcloud/vod/v20180717/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/tencentcloud_sdk_python_vod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:29:35.000000 tencentcloud-sdk-python-vod-3.0.942/tencentcloud_sdk_python_vod.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/tencentcloud/vod/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/tencentcloud/vod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/tencentcloud/vod/v20180717/
+-rw-r--r--   0 root         (0) root         (0)   183379 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/tencentcloud/vod/v20180717/vod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/tencentcloud/vod/v20180717/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25211 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/tencentcloud/vod/v20180717/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1854302 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/tencentcloud/vod/v20180717/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/tencentcloud_sdk_python_vod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:48:10.000000 tencentcloud-sdk-python-vod-3.0.943/tencentcloud_sdk_python_vod.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-vod-3.0.942/setup.py` & `tencentcloud-sdk-python-vod-3.0.943/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.942/tencentcloud/vod/v20180717/vod_client.py` & `tencentcloud-sdk-python-vod-3.0.943/tencentcloud/vod/v20180717/vod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.942/tencentcloud/vod/v20180717/errorcodes.py` & `tencentcloud-sdk-python-vod-3.0.943/tencentcloud/vod/v20180717/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.942/tencentcloud/vod/v20180717/models.py` & `tencentcloud-sdk-python-vod-3.0.943/tencentcloud/vod/v20180717/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -34423,14 +34423,15 @@
     """
 
     def __init__(self):
         r"""
         :param _Url: 转码后的视频文件地址。
         :type Url: str
         :param _Definition: 转码规格 ID，参见[转码参数模板](https://cloud.tencent.com/document/product/266/33476)。
+<font color=red>注意：取值 0 表示原始文件。</font> 
         :type Definition: int
         :param _Bitrate: 视频流码率平均值与音频流码率平均值之和， 单位：bps。
         :type Bitrate: int
         :param _Height: 视频流高度的最大值，单位：px。
         :type Height: int
         :param _Width: 视频流宽度的最大值，单位：px。
         :type Width: int
@@ -47716,17 +47717,17 @@
 class RestoreMediaRequest(AbstractModel):
     """RestoreMedia请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _FileIds: 媒体文件唯一标识列表。
+        :param _FileIds: 媒体文件唯一标识列表，最大长度：100。
         :type FileIds: list of str
-        :param _RestoreDay: 解冻出的临时媒体文件的可访问持续时长，单位为“天”。
+        :param _RestoreDay: 解冻出的临时媒体文件的可访问持续时长，必须大于0，单位为“天”。
         :type RestoreDay: int
         :param _RestoreTier: 解冻模式。当媒体文件当前的存储类型为归档存储时，有以下取值：
 <li>极速模式：Expedited，解冻任务在5分钟后完成。</li>
 <li>标准模式：Standard，解冻任务在5小时后完成 。</li>
 <li>批量模式：Bulk，，解冻任务在12小时后完成。</li>
 当媒体文件的存储类型为深度归档存储时，有以下取值：
 <li>标准模式：Standard，解冻任务在24小时后完成。</li>
@@ -49240,15 +49241,15 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class RoundPlayListItemInfo(AbstractModel):
-    """加权轮播媒体文件信息
+    """轮播媒体文件信息
 
     """
 
     def __init__(self):
         r"""
         :param _FileId: 媒体文件标识。
         :type FileId: str
```

### Comparing `tencentcloud-sdk-python-vod-3.0.942/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vod-3.0.943/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vod-3.0.942/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.943/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.942/README.rst` & `tencentcloud-sdk-python-vod-3.0.943/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.942/tencentcloud_sdk_python_vod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.943/tencentcloud_sdk_python_vod.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

