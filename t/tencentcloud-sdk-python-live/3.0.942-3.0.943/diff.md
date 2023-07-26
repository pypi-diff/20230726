# Comparing `tmp/tencentcloud-sdk-python-live-3.0.942.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.943.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.942.tar", last modified: Tue Jul 25 04:20:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.943.tar", last modified: Wed Jul 26 00:40:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.942.tar` & `tencentcloud-sdk-python-live-3.0.943.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:52.000000 tencentcloud-sdk-python-live-3.0.942/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-25 04:20:51.000000 tencentcloud-sdk-python-live-3.0.942/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:52.000000 tencentcloud-sdk-python-live-3.0.942/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:52.000000 tencentcloud-sdk-python-live-3.0.942/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:52.000000 tencentcloud-sdk-python-live-3.0.942/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:20:51.000000 tencentcloud-sdk-python-live-3.0.942/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20054 2023-07-25 04:20:51.000000 tencentcloud-sdk-python-live-3.0.942/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   154723 2023-07-25 04:20:51.000000 tencentcloud-sdk-python-live-3.0.942/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)   756652 2023-07-25 04:20:51.000000 tencentcloud-sdk-python-live-3.0.942/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:20:51.000000 tencentcloud-sdk-python-live-3.0.942/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:20:51.000000 tencentcloud-sdk-python-live-3.0.942/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:20:52.000000 tencentcloud-sdk-python-live-3.0.942/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:52.000000 tencentcloud-sdk-python-live-3.0.942/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:20:52.000000 tencentcloud-sdk-python-live-3.0.942/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-25 04:20:52.000000 tencentcloud-sdk-python-live-3.0.942/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-25 04:20:52.000000 tencentcloud-sdk-python-live-3.0.942/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:20:52.000000 tencentcloud-sdk-python-live-3.0.942/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-25 04:20:52.000000 tencentcloud-sdk-python-live-3.0.942/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-25 04:20:51.000000 tencentcloud-sdk-python-live-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:40:14.000000 tencentcloud-sdk-python-live-3.0.943/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-26 00:40:13.000000 tencentcloud-sdk-python-live-3.0.943/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:40:14.000000 tencentcloud-sdk-python-live-3.0.943/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:40:14.000000 tencentcloud-sdk-python-live-3.0.943/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:40:14.000000 tencentcloud-sdk-python-live-3.0.943/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:40:13.000000 tencentcloud-sdk-python-live-3.0.943/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20054 2023-07-26 00:40:13.000000 tencentcloud-sdk-python-live-3.0.943/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   154723 2023-07-26 00:40:13.000000 tencentcloud-sdk-python-live-3.0.943/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)   756776 2023-07-26 00:40:13.000000 tencentcloud-sdk-python-live-3.0.943/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:40:13.000000 tencentcloud-sdk-python-live-3.0.943/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:40:13.000000 tencentcloud-sdk-python-live-3.0.943/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:40:14.000000 tencentcloud-sdk-python-live-3.0.943/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:40:14.000000 tencentcloud-sdk-python-live-3.0.943/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:40:14.000000 tencentcloud-sdk-python-live-3.0.943/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-26 00:40:14.000000 tencentcloud-sdk-python-live-3.0.943/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-26 00:40:14.000000 tencentcloud-sdk-python-live-3.0.943/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:40:14.000000 tencentcloud-sdk-python-live-3.0.943/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-26 00:40:14.000000 tencentcloud-sdk-python-live-3.0.943/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-26 00:40:13.000000 tencentcloud-sdk-python-live-3.0.943/README.rst
```

### Comparing `tencentcloud-sdk-python-live-3.0.942/setup.py` & `tencentcloud-sdk-python-live-3.0.943/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.942/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.943/tencentcloud/live/v20180801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.942/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.943/tencentcloud/live/v20180801/live_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.942/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.943/tencentcloud/live/v20180801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2713,14 +2713,15 @@
 注意：
 1. 建议优先使用 flv 文件，对于 mp4 未交织好的文件轮播推流易产生卡顿，可通过点播转码进行重新交织后再轮播。
 2. 拒绝内网域名等攻击性拉流地址，如有使用，则做账号封禁处理。
 3. 源文件请保持时间戳正常交织递增，避免因源文件异常影响推流及播放。
 4. 视频编码格式仅支持: H264, H265。
 5. 音频编码格式仅支持: AAC。
 6. 点播源请使用小文件，尽量时长保持在1小时内，较大文件打开和续播耗时较久，耗时超过15秒会有无法正常转推风险。
+7. 避免使用低频存储的文件，该类文件因低频存储，拉取时容易出现慢速，影响拉转推质量。
         :type SourceUrls: list of str
         :param _DomainName: 推流域名。
 将拉取过来的流推到该域名。
 注意：如果目标地址为非云直播，且样式不同于云直播，请使用 ToUrl 传入完整推流地址，详细用法请参考 ToUrl 参数说明。
         :type DomainName: str
         :param _AppName: 推流路径。
 将拉取过来的流推到该路径。
```

### Comparing `tencentcloud-sdk-python-live-3.0.942/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.943/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-live-3.0.942/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.943/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.942/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.943/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.942/README.rst` & `tencentcloud-sdk-python-live-3.0.943/README.rst`

 * *Files identical despite different names*

