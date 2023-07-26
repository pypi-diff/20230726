# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.942.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.943.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.942.tar", last modified: Tue Jul 25 04:18:05 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.943.tar", last modified: Wed Jul 26 00:37:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.942.tar` & `tencentcloud-sdk-python-essbasic-3.0.943.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    55045 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   387357 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20210526/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    54057 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:18:05.000000 tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    55045 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   387540 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20210526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54057 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.942/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.943/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20210526/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4843,17 +4843,17 @@
     def __init__(self):
         r"""
         :param _ComponentId: 控件编号
 
 CreateFlowByTemplates发起合同时优先以ComponentId（不为空）填充；否则以ComponentName填充
 
 注：
-当GenerateMode=3时，通过"^"来决定是否使用关键字整词匹配能力。
+当GenerateMode=KEYWORD时，通过"^"来决定是否使用关键字整词匹配能力。
 例：
-当GenerateMode=3时，如果传入关键字"^甲方签署^"，则会在PDF文件中有且仅有"甲方签署"关键字的地方进行对应操作。
+当GenerateMode=KEYWORD时，如果传入关键字"^甲方签署^"，则会在PDF文件中有且仅有"甲方签署"关键字的地方进行对应操作。
 如传入的关键字为"甲方签署"，则PDF文件中每个出现关键字的位置都会执行相应操作。
 
 创建控件时，此值为空
 查询时返回完整结构
         :type ComponentId: str
         :param _ComponentType: 如果是Component控件类型，则可选的字段为：
 TEXT - 普通文本控件，输入文本字符串；
@@ -7800,17 +7800,17 @@
         :type ApproverType: str
         :param _RecipientId: 签署流程签署人在模板中对应的签署人Id；在非单方签署、以及非B2C签署的场景下必传，用于指定当前签署方在签署流程中的位置；
         :type RecipientId: str
         :param _Deadline: 签署截止时间戳，默认一年
         :type Deadline: int
         :param _CallbackUrl: 签署完回调url，最大长度1000个字符
         :type CallbackUrl: str
-        :param _SignComponents: 使用PDF文件直接发起合同时，签署人指定的签署控件
+        :param _SignComponents: 使用PDF文件直接发起合同时，签署人指定的签署控件；<br/>使用模板发起合同时，指定本企业印章签署控件的印章ID: <br/>通过ComponentId或ComponenetName指定签署控件，ComponentValue为印章ID。
         :type SignComponents: list of Component
-        :param _ComponentLimitType: 	签署方控件类型为 SIGN_SIGNATURE时，可以指定签署方签名方式
+        :param _ComponentLimitType: 签署方控件类型为 SIGN_SIGNATURE时，可以指定签署方签名方式
 	HANDWRITE – 手写签名
 	OCR_ESIGN -- AI智能识别手写签名
 	ESIGN -- 个人印章类型
 	SYSTEM_ESIGN -- 系统签名（该类型可以在用户签署时根据用户姓名一键生成一个签名来进行签署）
         :type ComponentLimitType: list of str
         :param _PreReadTime: 合同的强制预览时间：3~300s，未指定则按合同页数计算
         :type PreReadTime: int
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.942/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.943/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.942/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.943/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.942/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

