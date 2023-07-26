# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.942.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.943.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.942.tar", last modified: Tue Jul 25 04:18:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.943.tar", last modified: Wed Jul 26 00:37:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.942.tar` & `tencentcloud-sdk-python-ess-3.0.943.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    62111 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25058 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   438303 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:18:00.000000 tencentcloud-sdk-python-ess-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    62244 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25058 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   438395 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/README.rst
```

### Comparing `tencentcloud-sdk-python-ess-3.0.942/setup.py` & `tencentcloud-sdk-python-ess-3.0.943/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.942/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.943/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1029,15 +1029,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIntegrationMainOrganizationUser(self, request):
-        """通过子企业影子账号查询主企业员工账号
+        """集团企业统一使用主代子进行操作，无需根据子企业账号进行转化查询，该接口需要屏蔽下线
+
+        通过子企业影子账号查询主企业员工账号
 
         :param request: Request instance for DescribeIntegrationMainOrganizationUser.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeIntegrationMainOrganizationUserRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeIntegrationMainOrganizationUserResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.942/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         :type VerifyChannel: list of str
         :param _PreReadTime: 合同的强制预览时间：3~300s，未指定则按合同页数计算
         :type PreReadTime: int
         :param _UserId: 签署人userId，传此字段则不用传姓名、手机号
         :type UserId: str
         :param _ApproverSource: 签署人用户来源，企微侧用户请传入：WEWORKAPP
         :type ApproverSource: str
-        :param _CustomApproverTag: 客户自定义签署人标识，64位长度，保证唯一，非企微场景不使用此字段
+        :param _CustomApproverTag: 企业签署方或签标识，客户自定义，64位长度。用于发起含有或签签署人的合同。或签参与人必须有此字段。合同内不同或签参与人CustomApproverTag需要保证唯一。如果或签签署人为本方企微参与人，ApproverSource参数需要指定WEWORKAPP
         :type CustomApproverTag: str
         :param _ApproverOption: 签署人个性化能力值
         :type ApproverOption: :class:`tencentcloud.ess.v20201111.models.ApproverOption`
         :param _ApproverVerifyTypes: 签署人查看合同时认证方式, 
 1-实名查看 2-短信验证码查看(企业签署方不支持该方式)
 如果不传默认为1
 模板发起的时候,认证方式以模板配置为主
@@ -5310,15 +5310,17 @@
         r"""
         :param _Operator: 操作人信息
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _SealName: 电子印章名字
         :type SealName: str
         :param _Agent: 应用相关信息
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
-        :param _SealType: 电子印章类型，PERSONAL-个人私章,OFFICIAL-公章,SPECIAL_FINANCIAL-财务专用章,CONTRACT-合同专用章,LEGAL_REPRESENTATIVE-法定代表人章,SPECIAL_NATIONWIDE_INVOICE-发票专用章
+        :param _GenerateSource: 本接口支持上传图片印章及系统直接生成印章；如果要使用系统生成印章，此值传：SealGenerateSourceSystem；如果要使用图片上传请传字段 Image
+        :type GenerateSource: str
+        :param _SealType: 电子印章类型，OFFICIAL-公章,CONTRACT-合同专用章
         :type SealType: str
         :param _FileName: 电子印章图片文件名称
         :type FileName: str
         :param _Image: 电子印章图片base64编码
 参数Image,FileToken或GenerateSource=SealGenerateSourceSystem三选一。
         :type Image: str
         :param _Width: 电子印章宽度,单位px
@@ -5327,43 +5329,38 @@
         :param _Height: 电子印章高度,单位px
 参数不再启用，系统会设置印章大小为标准尺寸。
         :type Height: int
         :param _Color: 电子印章印章颜色(默认红色RED),RED-红色
 
 系统目前只支持红色印章创建。
         :type Color: str
-        :param _SealHorizontalText: 电子印章生成时的横向文字。
+        :param _SealHorizontalText: 暂时不支持横向文字设置
         :type SealHorizontalText: str
-        :param _SealChordText: 电子印章下弦文字
+        :param _SealChordText: 暂时不支持下弦文字设置
         :type SealChordText: str
-        :param _SealCentralType: 电子印章中心图案类型,STAR-圆形有五角星,NONE-圆形无五角星
-系统生成的印章只支持STAR
+        :param _SealCentralType: 系统生成的印章只支持STAR
         :type SealCentralType: str
         :param _FileToken: 通过文件上传时，服务端生成的电子印章上传图片的token
 
         :type FileToken: str
-        :param _GenerateSource: 印章生成来源方式
-取值：
-SealGenerateSourceSystem 表示系统生成企业印章
-        :type GenerateSource: str
         """
         self._Operator = None
         self._SealName = None
         self._Agent = None
+        self._GenerateSource = None
         self._SealType = None
         self._FileName = None
         self._Image = None
         self._Width = None
         self._Height = None
         self._Color = None
         self._SealHorizontalText = None
         self._SealChordText = None
         self._SealCentralType = None
         self._FileToken = None
-        self._GenerateSource = None
 
     @property
     def Operator(self):
         return self._Operator
 
     @Operator.setter
     def Operator(self, Operator):
@@ -5382,14 +5379,22 @@
         return self._Agent
 
     @Agent.setter
     def Agent(self, Agent):
         self._Agent = Agent
 
     @property
+    def GenerateSource(self):
+        return self._GenerateSource
+
+    @GenerateSource.setter
+    def GenerateSource(self, GenerateSource):
+        self._GenerateSource = GenerateSource
+
+    @property
     def SealType(self):
         return self._SealType
 
     @SealType.setter
     def SealType(self, SealType):
         self._SealType = SealType
 
@@ -5461,42 +5466,34 @@
     def FileToken(self):
         return self._FileToken
 
     @FileToken.setter
     def FileToken(self, FileToken):
         self._FileToken = FileToken
 
-    @property
-    def GenerateSource(self):
-        return self._GenerateSource
-
-    @GenerateSource.setter
-    def GenerateSource(self, GenerateSource):
-        self._GenerateSource = GenerateSource
-
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
         self._SealName = params.get("SealName")
         if params.get("Agent") is not None:
             self._Agent = Agent()
             self._Agent._deserialize(params.get("Agent"))
+        self._GenerateSource = params.get("GenerateSource")
         self._SealType = params.get("SealType")
         self._FileName = params.get("FileName")
         self._Image = params.get("Image")
         self._Width = params.get("Width")
         self._Height = params.get("Height")
         self._Color = params.get("Color")
         self._SealHorizontalText = params.get("SealHorizontalText")
         self._SealChordText = params.get("SealChordText")
         self._SealCentralType = params.get("SealCentralType")
         self._FileToken = params.get("FileToken")
-        self._GenerateSource = params.get("GenerateSource")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -9763,15 +9760,15 @@
         :type PreReadTime: int
         :param _UserId: 签署方经办人的用户ID,和签署方经办人姓名+手机号+证件必须有一个。
         :type UserId: str
         :param _Required: 当前只支持true，默认为true
         :type Required: bool
         :param _ApproverSource: 签署人用户来源,企微侧用户请传入：WEWORKAPP
         :type ApproverSource: str
-        :param _CustomApproverTag: 客户自定义签署人标识，64位长度，保证唯一。用于发起含有或签签署人的合同。或签参与人必须有此字段。不同或签参与人CustomApproverTag需要保证唯一。如果或签签署人为本方企微参与人，ApproverSource参数需要指定WEWORKAPP
+        :param _CustomApproverTag: 企业签署方或签标识，客户自定义，64位长度。用于发起含有或签签署人的合同。或签参与人必须有此字段。合同内不同或签参与人CustomApproverTag需要保证唯一。如果或签签署人为本方企微参与人，ApproverSource参数需要指定WEWORKAPP
         :type CustomApproverTag: str
         :param _RegisterInfo: 快速注册相关信息，目前暂未开放！
         :type RegisterInfo: :class:`tencentcloud.ess.v20201111.models.RegisterInfo`
         :param _ApproverOption: 签署人个性化能力值
         :type ApproverOption: :class:`tencentcloud.ess.v20201111.models.ApproverOption`
         :param _JumpUrl: 签署完前端跳转的url，暂未使用
         :type JumpUrl: str
```

### Comparing `tencentcloud-sdk-python-ess-3.0.942/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.943/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.942/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.943/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.942/README.rst` & `tencentcloud-sdk-python-ess-3.0.943/README.rst`

 * *Files identical despite different names*

