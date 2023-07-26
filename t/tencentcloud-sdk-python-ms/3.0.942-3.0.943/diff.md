# Comparing `tmp/tencentcloud-sdk-python-ms-3.0.942.tar.gz` & `tmp/tencentcloud-sdk-python-ms-3.0.943.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ms-3.0.942.tar", last modified: Tue Jul 25 04:22:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ms-3.0.943.tar", last modified: Wed Jul 26 00:41:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ms-3.0.942.tar` & `tencentcloud-sdk-python-ms-3.0.943.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/tencentcloud_sdk_python_ms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/tencentcloud_sdk_python_ms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/tencentcloud_sdk_python_ms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/tencentcloud_sdk_python_ms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/tencentcloud_sdk_python_ms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/tencentcloud/ms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/tencentcloud/ms/v20180408/
--rw-r--r--   0 root         (0) root         (0)    14764 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/tencentcloud/ms/v20180408/ms_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/tencentcloud/ms/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3469 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/tencentcloud/ms/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    90316 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/tencentcloud/ms/v20180408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/tencentcloud/ms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-25 04:22:04.000000 tencentcloud-sdk-python-ms-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/tencentcloud_sdk_python_ms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/tencentcloud_sdk_python_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/tencentcloud_sdk_python_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/tencentcloud_sdk_python_ms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/tencentcloud_sdk_python_ms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/tencentcloud/ms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/tencentcloud/ms/v20180408/
+-rw-r--r--   0 root         (0) root         (0)    21305 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/tencentcloud/ms/v20180408/ms_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/tencentcloud/ms/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5901 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/tencentcloud/ms/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   169826 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/tencentcloud/ms/v20180408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/tencentcloud/ms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-26 00:41:22.000000 tencentcloud-sdk-python-ms-3.0.943/README.rst
```

### Comparing `tencentcloud-sdk-python-ms-3.0.942/tencentcloud_sdk_python_ms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ms-3.0.943/tencentcloud_sdk_python_ms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ms
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Ms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ms-3.0.942/setup.py` & `tencentcloud-sdk-python-ms-3.0.943/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ms-3.0.942/tencentcloud/ms/v20180408/ms_client.py` & `tencentcloud-sdk-python-ms-3.0.943/tencentcloud/ms/v20180408/ms_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,14 +22,37 @@
 
 class MsClient(AbstractClient):
     _apiVersion = '2018-04-08'
     _endpoint = 'ms.tencentcloudapi.com'
     _service = 'ms'
 
 
+    def CancelEncryptTask(self, request):
+        """该接口供渠道合作应用加固使用，接口调用有白名单用户限制，取消渠道合作加固中的任务。
+
+        :param request: Request instance for CancelEncryptTask.
+        :type request: :class:`tencentcloud.ms.v20180408.models.CancelEncryptTaskRequest`
+        :rtype: :class:`tencentcloud.ms.v20180408.models.CancelEncryptTaskResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CancelEncryptTask", params, headers=headers)
+            response = json.loads(body)
+            model = models.CancelEncryptTaskResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def CreateBindInstance(self, request):
         """将应用和资源进行绑定。（注意：根据国家互联网用户实名制相关要求，使用该产品前，需先完成实名认证。）
 
         :param request: Request instance for CreateBindInstance.
         :type request: :class:`tencentcloud.ms.v20180408.models.CreateBindInstanceRequest`
         :rtype: :class:`tencentcloud.ms.v20180408.models.CreateBindInstanceResponse`
 
@@ -68,14 +91,62 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def CreateEncryptInstance(self, request):
+        """该接口供渠道合作应用加固使用，接口调用有白名单用户限制，用于创建加固任务。
+
+        :param request: Request instance for CreateEncryptInstance.
+        :type request: :class:`tencentcloud.ms.v20180408.models.CreateEncryptInstanceRequest`
+        :rtype: :class:`tencentcloud.ms.v20180408.models.CreateEncryptInstanceResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateEncryptInstance", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateEncryptInstanceResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def CreateOrderInstance(self, request):
+        """该接口供渠道合作应用加固使用，接口调用有白名单用户限制。
+        订单类型有：免费试用、按年收费、按次收费。
+        应用加固支持的平台类型有：android安卓加固 、ios源码混淆 、sdk加固、applet小程序加固。
+
+        :param request: Request instance for CreateOrderInstance.
+        :type request: :class:`tencentcloud.ms.v20180408.models.CreateOrderInstanceRequest`
+        :rtype: :class:`tencentcloud.ms.v20180408.models.CreateOrderInstanceResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateOrderInstance", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateOrderInstanceResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def CreateResourceInstances(self, request):
         """用户可以使用该接口自建资源，只支持白名单用户
 
         :param request: Request instance for CreateResourceInstances.
         :type request: :class:`tencentcloud.ms.v20180408.models.CreateResourceInstancesRequest`
         :rtype: :class:`tencentcloud.ms.v20180408.models.CreateResourceInstancesResponse`
 
@@ -181,14 +252,87 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeEncryptInstances(self, request):
+        """该接口供渠道合作应用加固使用，接口调用有白名单用户限制，用于查询加固任务，入参中的条件过滤字段均为精准匹配。支持功能点：1. 多任务分页查询  2.根据任务Id唯一值查询单记录
+
+        :param request: Request instance for DescribeEncryptInstances.
+        :type request: :class:`tencentcloud.ms.v20180408.models.DescribeEncryptInstancesRequest`
+        :rtype: :class:`tencentcloud.ms.v20180408.models.DescribeEncryptInstancesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeEncryptInstances", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeEncryptInstancesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeEncryptPlan(self, request):
+        """该接口供渠道合作应用加固使用，接口调用有白名单用户限制。入参中的条件过滤字段均为精准匹配。
+
+        :param request: Request instance for DescribeEncryptPlan.
+        :type request: :class:`tencentcloud.ms.v20180408.models.DescribeEncryptPlanRequest`
+        :rtype: :class:`tencentcloud.ms.v20180408.models.DescribeEncryptPlanResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeEncryptPlan", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeEncryptPlanResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeOrderInstances(self, request):
+        """该接口供渠道合作应用加固使用，接口调用有白名单用户限制。 接口返回的结果为：创建订单后，订单审批状态信息，以及与订单关联的资源状态等信息，入参中的条件过滤字段均为精准匹配。
+        接口功能点：
+        1.支持多订单分页查询；
+        2.支持唯一订单号精准匹配查询；
+        3.支持唯一资源号精准匹配查询；
+
+        :param request: Request instance for DescribeOrderInstances.
+        :type request: :class:`tencentcloud.ms.v20180408.models.DescribeOrderInstancesRequest`
+        :rtype: :class:`tencentcloud.ms.v20180408.models.DescribeOrderInstancesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeOrderInstances", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeOrderInstancesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceInstances(self, request):
         """获取某个用户的所有资源信息。（注意：根据国家互联网用户实名制相关要求，使用该产品前，需先完成实名认证。）
 
         :param request: Request instance for DescribeResourceInstances.
         :type request: :class:`tencentcloud.ms.v20180408.models.DescribeResourceInstancesRequest`
```

### Comparing `tencentcloud-sdk-python-ms-3.0.942/tencentcloud/ms/v20180408/models.py` & `tencentcloud-sdk-python-ms-3.0.943/tencentcloud/ms/v20180408/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,14 +14,714 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
+class AndroidAppInfo(AbstractModel):
+    """渠道合作安卓加固App信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _AppMd5: app文件的md5算法值，需要正确传递，在线加固必输。
+例如linux环境下执行算法命令md5sum ：
+#md5sum test.apk 
+d40cc11e4bddd643ecdf29cde729a12b
+        :type AppMd5: str
+        :param _AppSize: app的大小，非必输。
+        :type AppSize: int
+        :param _AppUrl: app下载链接，在线加固必输。
+        :type AppUrl: str
+        :param _AppName: app名称，非必输
+        :type AppName: str
+        :param _AppPkgName: app的包名，本次操作的包名。
+当安卓是按年收费、免费试用加固时，在线加固和输出工具要求该字段必输，且与AndroidPlan.AppPkgName值相等。
+        :type AppPkgName: str
+        :param _AppFileName: app的文件名，非必输。
+        :type AppFileName: str
+        :param _AppVersion: app版本号，非必输。
+        :type AppVersion: str
+        :param _AppType: 安卓app的文件类型，本次加固操作的应用类型 。
+安卓在线加固和输出工具加固必输，其值需等于“apk”或“aab”，且与AndroidAppInfo.AppType值相等。
+        :type AppType: str
+        """
+        self._AppMd5 = None
+        self._AppSize = None
+        self._AppUrl = None
+        self._AppName = None
+        self._AppPkgName = None
+        self._AppFileName = None
+        self._AppVersion = None
+        self._AppType = None
+
+    @property
+    def AppMd5(self):
+        return self._AppMd5
+
+    @AppMd5.setter
+    def AppMd5(self, AppMd5):
+        self._AppMd5 = AppMd5
+
+    @property
+    def AppSize(self):
+        return self._AppSize
+
+    @AppSize.setter
+    def AppSize(self, AppSize):
+        self._AppSize = AppSize
+
+    @property
+    def AppUrl(self):
+        return self._AppUrl
+
+    @AppUrl.setter
+    def AppUrl(self, AppUrl):
+        self._AppUrl = AppUrl
+
+    @property
+    def AppName(self):
+        return self._AppName
+
+    @AppName.setter
+    def AppName(self, AppName):
+        self._AppName = AppName
+
+    @property
+    def AppPkgName(self):
+        return self._AppPkgName
+
+    @AppPkgName.setter
+    def AppPkgName(self, AppPkgName):
+        self._AppPkgName = AppPkgName
+
+    @property
+    def AppFileName(self):
+        return self._AppFileName
+
+    @AppFileName.setter
+    def AppFileName(self, AppFileName):
+        self._AppFileName = AppFileName
+
+    @property
+    def AppVersion(self):
+        return self._AppVersion
+
+    @AppVersion.setter
+    def AppVersion(self, AppVersion):
+        self._AppVersion = AppVersion
+
+    @property
+    def AppType(self):
+        return self._AppType
+
+    @AppType.setter
+    def AppType(self, AppType):
+        self._AppType = AppType
+
+
+    def _deserialize(self, params):
+        self._AppMd5 = params.get("AppMd5")
+        self._AppSize = params.get("AppSize")
+        self._AppUrl = params.get("AppUrl")
+        self._AppName = params.get("AppName")
+        self._AppPkgName = params.get("AppPkgName")
+        self._AppFileName = params.get("AppFileName")
+        self._AppVersion = params.get("AppVersion")
+        self._AppType = params.get("AppType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AndroidPlan(AbstractModel):
+    """渠道合作安卓加固策略信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _PlanId: 非必输字段，PlanId 是指本次加固使用的配置策略Id，可通过载入上次配置接口获取。其值非0时，代表引用对应的策略。
+        :type PlanId: int
+        :param _AppPkgName: 本次操作的包名。
+当收费模式是安卓按年收费和安卓免费试用的在线加固和输出工具加固时，要求该字段必输，且与AndroidAppInfo.AppPkgName值相等。
+        :type AppPkgName: str
+        :param _AppType: 安卓app的文件类型，本次加固操作的应用类型 。 
+安卓在线加固和输出工具加固必输，其值需等于“apk”或“aab”，且与AndroidAppInfo.AppType值相等。
+
+        :type AppType: str
+        :param _EncryptParam: 安卓加固必输字段。
+加固策略，json格式字符串。
+字段说明（0-关闭，1-开启）：
+        "enable"=1 #DEX整体加固;
+        "antiprotect"=1 #反调试;
+        "antirepack"=1 #防重打包、防篡改;
+        "dexsig"=1       #签名校验;
+        "antimonitor"=1 #防模拟器运行保护;
+        "ptrace"=1 #防动态注入、动态调试;
+        "so"."enable" = 1 #文件加密;
+        "vmp"."enable" = 1 #VMP虚拟化保护;
+        "respro"."assets"."enable" = 1 #assets资源文件加密
+       "respro"."res"."enable" = 1 #res资源文件加密
+
+so文件加密：
+支持5种架构:
+apk 格式: /lib/armeabi/libxxx.so,/lib/arm64-v8a/libxxx.so,/lib/armeabi-v7a/libxxx.so,/lib/x86/libxxx.so,/lib/x86_64/libxxx.so
+aab格式: /base/lib/armeabi/libxxx.so,/base/lib/arm64-v8a/libxxx.so,/base/lib/armeabi-v7a/libxxx.so,/base/lib/x86/libxxx.so,/base/lib/x86_64/libxxx.so
+请列举 SO 库在 apk 文件解压后的完整有效路径，如:/lib/armeabi/libxxx.so；
+需要加固的 SO 库需确认为自研的 SO 库，不要加固第三方 SO 库，否则会增加 crash 风险
+
+res资源文件加密注意事项：
+请指定需要加密的文件全路径，如：res/layout/1.xml;
+res资源文件加密不能加密APP图标
+res目录文件，不能加密以下后缀规则的文件".wav", ".mp2", ".mp3", ".ogg", ".aac", ".mpg",".mpeg", ".mid", ".midi", ".smf", ".jet", ".rtttl", ".imy", ".xmf", ".mp4", ".m4a", ".m4v", ".3gp",".3gpp", ".3g2", ".3gpp2", ".amr", ".awb", ".wma", ".wmv"
+
+assets资源文件加密注意事项:
+请指定需要加密的文件全路径，如：assets/main.js；可以完整路径，也可以相对路径。
+如果有通配符需要完整路径 ":all"或者"*"代表所有文件
+assets资源文件加密不能加密APP图标
+assets目录文件，不能加密以下后缀规则的文件".wav", ".mp2", ".mp3", ".ogg", ".aac", ".mpg",".mpeg", ".mid", ".midi", ".smf", ".jet", ".rtttl", ".imy", ".xmf", ".mp4", ".m4a", ".m4v", ".3gp",".3gpp", ".3g2", ".3gpp2", ".amr", ".awb", ".wma", ".wmv"
+
+
+apk[dex+so+vmp+res+assets]加固参数示例：
+‘{
+    "dex": {
+        "enable": 1,
+        "antiprotect": 1,
+        "antirepack": 1,
+        "dexsig": 1,
+        "antimonitor": 1,
+        "ptrace": 1
+    },
+    "so": {
+        "enable": 1,
+        "ver": "1.3.3",
+        "file": [
+            "/lib/armeabi/libtest.so"
+        ]
+    },
+    "vmp": {
+        "enable": 1,
+        "ndkpath": "/xxx/android-ndk-r10e",
+        "profile": "/xxx/vmpprofile.txt",
+        "mapping": "/xxx/mapping.txt"
+    },
+    "respro": {
+        "assets": {
+            "enable": 1,
+            "file": [
+                "assets/1.js",
+                "assets/2.jpg"
+            ]
+        },
+        "res": {
+            "enable": 1,
+            "file": [
+                "res/layout/1.xml",
+                "res/layout/2.xml"
+            ]
+        }
+    }
+}’
+
+aab加固方案一 
+[dex+res+assets]加固json字符串：
+‘{
+    "dex": {
+        "enable": 1,
+        "antiprotect": 1,
+        "antimonitor": 1
+    },
+    "respro": {
+        "assets": {
+            "enable": 1,
+            "file": [
+                "assets/1.js",
+                "assets/2.jpg"
+            ]
+        },
+        "res": {
+            "enable": 1,
+            "file": [
+                "res/layout/1.xml",
+                "res/layout/2.xml"
+            ]
+        }
+    }
+}’
+
+aab加固方案二
+单独vmp加固：
+‘{
+    "vmp": {
+        "enable": 1,
+        "ndkpath": "/xxx/android-ndk-r10e",
+        "profile": "/xxx/vmpprofile.txt",
+        "mapping": "/xxx/mapping.txt",
+        "antiprotect": 1,
+        "antimonitor": 1
+    }
+}’
+        :type EncryptParam: str
+        """
+        self._PlanId = None
+        self._AppPkgName = None
+        self._AppType = None
+        self._EncryptParam = None
+
+    @property
+    def PlanId(self):
+        return self._PlanId
+
+    @PlanId.setter
+    def PlanId(self, PlanId):
+        self._PlanId = PlanId
+
+    @property
+    def AppPkgName(self):
+        return self._AppPkgName
+
+    @AppPkgName.setter
+    def AppPkgName(self, AppPkgName):
+        self._AppPkgName = AppPkgName
+
+    @property
+    def AppType(self):
+        return self._AppType
+
+    @AppType.setter
+    def AppType(self, AppType):
+        self._AppType = AppType
+
+    @property
+    def EncryptParam(self):
+        return self._EncryptParam
+
+    @EncryptParam.setter
+    def EncryptParam(self, EncryptParam):
+        self._EncryptParam = EncryptParam
+
+
+    def _deserialize(self, params):
+        self._PlanId = params.get("PlanId")
+        self._AppPkgName = params.get("AppPkgName")
+        self._AppType = params.get("AppType")
+        self._EncryptParam = params.get("EncryptParam")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AndroidResult(AbstractModel):
+    """安卓加固结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ResultId: 结果Id,用于查询加固结果
+        :type ResultId: str
+        :param _OrderId: 与当前任务关联的订单id
+        :type OrderId: str
+        :param _ResourceId: 与当前任务关联的资源Id
+        :type ResourceId: str
+        :param _OpUin: 本次任务发起者
+        :type OpUin: int
+        :param _AppType: 应用类型：安卓-apk; 安卓-aab;
+        :type AppType: str
+        :param _AppPkgName: 应用包名
+        :type AppPkgName: str
+        :param _BindAppPkgName: 后台资源绑定的包名
+        :type BindAppPkgName: str
+        :param _EncryptState: 加固结果
+        :type EncryptState: int
+        :param _EncryptStateDesc: 加固结果描述
+        :type EncryptStateDesc: str
+        :param _EncryptErrCode: 加固失败错误码
+        :type EncryptErrCode: int
+        :param _EncryptErrDesc: 加固失败原因
+        :type EncryptErrDesc: str
+        :param _EncryptErrRef: 加固失败解决方案
+        :type EncryptErrRef: str
+        :param _CreatTime: 任务创建时间
+        :type CreatTime: str
+        :param _StartTime: 任务开始处理时间
+        :type StartTime: str
+        :param _EndTime: 任务处理结束时间
+        :type EndTime: str
+        :param _CostTime: 加固耗时（秒单位）
+        :type CostTime: int
+        :param _AppUrl: 在线加固-安卓应用原包下载链接
+        :type AppUrl: str
+        :param _AppMd5: 在线加固-安卓应用文件MD5算法值
+        :type AppMd5: str
+        :param _AppName: 在线加固-安卓应用应用名称
+        :type AppName: str
+        :param _AppVersion: 在线加固-安卓应用版本；
+        :type AppVersion: str
+        :param _AppSize: 在线加固-安卓应用大小
+        :type AppSize: int
+        :param _OnlineToolVersion: 在线加固-安卓加固-腾讯云应用加固工具版本
+        :type OnlineToolVersion: str
+        :param _EncryptAppMd5: 在线加固-安卓加固，加固成功后文件md5算法值
+        :type EncryptAppMd5: str
+        :param _EncryptAppSize: 在线加固-安卓加固，加固成功后应用大小
+        :type EncryptAppSize: int
+        :param _EncryptPkgUrl: 在线加固-安卓加固，加固包下载链接。
+        :type EncryptPkgUrl: str
+        :param _OutputToolVersion: 输出工具-安卓加固-腾讯云输出工具版本
+        :type OutputToolVersion: str
+        :param _OutputToolSize: 输出工具-安卓加固-工具大小
+        :type OutputToolSize: int
+        :param _ToolOutputTime: 输出工具-安卓加固-工具输出时间
+        :type ToolOutputTime: str
+        :param _ToolExpireTime: 输出工具-安卓加固-工具到期时间
+        :type ToolExpireTime: str
+        :param _OutputToolUrl: 输出工具-安卓加固-输出工具下载链接
+        :type OutputToolUrl: str
+        :param _AndroidPlan: 本次安卓加固策略信息
+        :type AndroidPlan: :class:`tencentcloud.ms.v20180408.models.AndroidPlan`
+        """
+        self._ResultId = None
+        self._OrderId = None
+        self._ResourceId = None
+        self._OpUin = None
+        self._AppType = None
+        self._AppPkgName = None
+        self._BindAppPkgName = None
+        self._EncryptState = None
+        self._EncryptStateDesc = None
+        self._EncryptErrCode = None
+        self._EncryptErrDesc = None
+        self._EncryptErrRef = None
+        self._CreatTime = None
+        self._StartTime = None
+        self._EndTime = None
+        self._CostTime = None
+        self._AppUrl = None
+        self._AppMd5 = None
+        self._AppName = None
+        self._AppVersion = None
+        self._AppSize = None
+        self._OnlineToolVersion = None
+        self._EncryptAppMd5 = None
+        self._EncryptAppSize = None
+        self._EncryptPkgUrl = None
+        self._OutputToolVersion = None
+        self._OutputToolSize = None
+        self._ToolOutputTime = None
+        self._ToolExpireTime = None
+        self._OutputToolUrl = None
+        self._AndroidPlan = None
+
+    @property
+    def ResultId(self):
+        return self._ResultId
+
+    @ResultId.setter
+    def ResultId(self, ResultId):
+        self._ResultId = ResultId
+
+    @property
+    def OrderId(self):
+        return self._OrderId
+
+    @OrderId.setter
+    def OrderId(self, OrderId):
+        self._OrderId = OrderId
+
+    @property
+    def ResourceId(self):
+        return self._ResourceId
+
+    @ResourceId.setter
+    def ResourceId(self, ResourceId):
+        self._ResourceId = ResourceId
+
+    @property
+    def OpUin(self):
+        return self._OpUin
+
+    @OpUin.setter
+    def OpUin(self, OpUin):
+        self._OpUin = OpUin
+
+    @property
+    def AppType(self):
+        return self._AppType
+
+    @AppType.setter
+    def AppType(self, AppType):
+        self._AppType = AppType
+
+    @property
+    def AppPkgName(self):
+        return self._AppPkgName
+
+    @AppPkgName.setter
+    def AppPkgName(self, AppPkgName):
+        self._AppPkgName = AppPkgName
+
+    @property
+    def BindAppPkgName(self):
+        return self._BindAppPkgName
+
+    @BindAppPkgName.setter
+    def BindAppPkgName(self, BindAppPkgName):
+        self._BindAppPkgName = BindAppPkgName
+
+    @property
+    def EncryptState(self):
+        return self._EncryptState
+
+    @EncryptState.setter
+    def EncryptState(self, EncryptState):
+        self._EncryptState = EncryptState
+
+    @property
+    def EncryptStateDesc(self):
+        return self._EncryptStateDesc
+
+    @EncryptStateDesc.setter
+    def EncryptStateDesc(self, EncryptStateDesc):
+        self._EncryptStateDesc = EncryptStateDesc
+
+    @property
+    def EncryptErrCode(self):
+        return self._EncryptErrCode
+
+    @EncryptErrCode.setter
+    def EncryptErrCode(self, EncryptErrCode):
+        self._EncryptErrCode = EncryptErrCode
+
+    @property
+    def EncryptErrDesc(self):
+        return self._EncryptErrDesc
+
+    @EncryptErrDesc.setter
+    def EncryptErrDesc(self, EncryptErrDesc):
+        self._EncryptErrDesc = EncryptErrDesc
+
+    @property
+    def EncryptErrRef(self):
+        return self._EncryptErrRef
+
+    @EncryptErrRef.setter
+    def EncryptErrRef(self, EncryptErrRef):
+        self._EncryptErrRef = EncryptErrRef
+
+    @property
+    def CreatTime(self):
+        return self._CreatTime
+
+    @CreatTime.setter
+    def CreatTime(self, CreatTime):
+        self._CreatTime = CreatTime
+
+    @property
+    def StartTime(self):
+        return self._StartTime
+
+    @StartTime.setter
+    def StartTime(self, StartTime):
+        self._StartTime = StartTime
+
+    @property
+    def EndTime(self):
+        return self._EndTime
+
+    @EndTime.setter
+    def EndTime(self, EndTime):
+        self._EndTime = EndTime
+
+    @property
+    def CostTime(self):
+        return self._CostTime
+
+    @CostTime.setter
+    def CostTime(self, CostTime):
+        self._CostTime = CostTime
+
+    @property
+    def AppUrl(self):
+        return self._AppUrl
+
+    @AppUrl.setter
+    def AppUrl(self, AppUrl):
+        self._AppUrl = AppUrl
+
+    @property
+    def AppMd5(self):
+        return self._AppMd5
+
+    @AppMd5.setter
+    def AppMd5(self, AppMd5):
+        self._AppMd5 = AppMd5
+
+    @property
+    def AppName(self):
+        return self._AppName
+
+    @AppName.setter
+    def AppName(self, AppName):
+        self._AppName = AppName
+
+    @property
+    def AppVersion(self):
+        return self._AppVersion
+
+    @AppVersion.setter
+    def AppVersion(self, AppVersion):
+        self._AppVersion = AppVersion
+
+    @property
+    def AppSize(self):
+        return self._AppSize
+
+    @AppSize.setter
+    def AppSize(self, AppSize):
+        self._AppSize = AppSize
+
+    @property
+    def OnlineToolVersion(self):
+        return self._OnlineToolVersion
+
+    @OnlineToolVersion.setter
+    def OnlineToolVersion(self, OnlineToolVersion):
+        self._OnlineToolVersion = OnlineToolVersion
+
+    @property
+    def EncryptAppMd5(self):
+        return self._EncryptAppMd5
+
+    @EncryptAppMd5.setter
+    def EncryptAppMd5(self, EncryptAppMd5):
+        self._EncryptAppMd5 = EncryptAppMd5
+
+    @property
+    def EncryptAppSize(self):
+        return self._EncryptAppSize
+
+    @EncryptAppSize.setter
+    def EncryptAppSize(self, EncryptAppSize):
+        self._EncryptAppSize = EncryptAppSize
+
+    @property
+    def EncryptPkgUrl(self):
+        return self._EncryptPkgUrl
+
+    @EncryptPkgUrl.setter
+    def EncryptPkgUrl(self, EncryptPkgUrl):
+        self._EncryptPkgUrl = EncryptPkgUrl
+
+    @property
+    def OutputToolVersion(self):
+        return self._OutputToolVersion
+
+    @OutputToolVersion.setter
+    def OutputToolVersion(self, OutputToolVersion):
+        self._OutputToolVersion = OutputToolVersion
+
+    @property
+    def OutputToolSize(self):
+        return self._OutputToolSize
+
+    @OutputToolSize.setter
+    def OutputToolSize(self, OutputToolSize):
+        self._OutputToolSize = OutputToolSize
+
+    @property
+    def ToolOutputTime(self):
+        return self._ToolOutputTime
+
+    @ToolOutputTime.setter
+    def ToolOutputTime(self, ToolOutputTime):
+        self._ToolOutputTime = ToolOutputTime
+
+    @property
+    def ToolExpireTime(self):
+        return self._ToolExpireTime
+
+    @ToolExpireTime.setter
+    def ToolExpireTime(self, ToolExpireTime):
+        self._ToolExpireTime = ToolExpireTime
+
+    @property
+    def OutputToolUrl(self):
+        return self._OutputToolUrl
+
+    @OutputToolUrl.setter
+    def OutputToolUrl(self, OutputToolUrl):
+        self._OutputToolUrl = OutputToolUrl
+
+    @property
+    def AndroidPlan(self):
+        return self._AndroidPlan
+
+    @AndroidPlan.setter
+    def AndroidPlan(self, AndroidPlan):
+        self._AndroidPlan = AndroidPlan
+
+
+    def _deserialize(self, params):
+        self._ResultId = params.get("ResultId")
+        self._OrderId = params.get("OrderId")
+        self._ResourceId = params.get("ResourceId")
+        self._OpUin = params.get("OpUin")
+        self._AppType = params.get("AppType")
+        self._AppPkgName = params.get("AppPkgName")
+        self._BindAppPkgName = params.get("BindAppPkgName")
+        self._EncryptState = params.get("EncryptState")
+        self._EncryptStateDesc = params.get("EncryptStateDesc")
+        self._EncryptErrCode = params.get("EncryptErrCode")
+        self._EncryptErrDesc = params.get("EncryptErrDesc")
+        self._EncryptErrRef = params.get("EncryptErrRef")
+        self._CreatTime = params.get("CreatTime")
+        self._StartTime = params.get("StartTime")
+        self._EndTime = params.get("EndTime")
+        self._CostTime = params.get("CostTime")
+        self._AppUrl = params.get("AppUrl")
+        self._AppMd5 = params.get("AppMd5")
+        self._AppName = params.get("AppName")
+        self._AppVersion = params.get("AppVersion")
+        self._AppSize = params.get("AppSize")
+        self._OnlineToolVersion = params.get("OnlineToolVersion")
+        self._EncryptAppMd5 = params.get("EncryptAppMd5")
+        self._EncryptAppSize = params.get("EncryptAppSize")
+        self._EncryptPkgUrl = params.get("EncryptPkgUrl")
+        self._OutputToolVersion = params.get("OutputToolVersion")
+        self._OutputToolSize = params.get("OutputToolSize")
+        self._ToolOutputTime = params.get("ToolOutputTime")
+        self._ToolExpireTime = params.get("ToolExpireTime")
+        self._OutputToolUrl = params.get("OutputToolUrl")
+        if params.get("AndroidPlan") is not None:
+            self._AndroidPlan = AndroidPlan()
+            self._AndroidPlan._deserialize(params.get("AndroidPlan"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class AppDetailInfo(AbstractModel):
     """app的详细基础信息
 
     """
 
     def __init__(self):
         r"""
@@ -437,14 +1137,322 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class AppletInfo(AbstractModel):
+    """小程序加固信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _AppletJsUrl: 客户JS包
+        :type AppletJsUrl: str
+        :param _AppletLevel: 小程序加固等级配置
+1 - 开启代码混淆、代码压缩、代码反调试保护。 2 - 开启字符串编码和代码变换，代码膨胀，随机插入冗余代码，开启代码控制流平坦化，保证业务逻辑正常前提下，扁平化代码逻辑分支，破坏代码简单的线性结构。 3 - 开启代码加密，对字符串、函数、变量、属性、类、数组等结构进行加密保护，更多得代码控制流平坦化，扁平化逻辑分支。
+        :type AppletLevel: int
+        :param _Name: 本次加固输出产物名称，如”test.zip“,非空必须是 ”.zip“结尾
+        :type Name: str
+        """
+        self._AppletJsUrl = None
+        self._AppletLevel = None
+        self._Name = None
+
+    @property
+    def AppletJsUrl(self):
+        return self._AppletJsUrl
+
+    @AppletJsUrl.setter
+    def AppletJsUrl(self, AppletJsUrl):
+        self._AppletJsUrl = AppletJsUrl
+
+    @property
+    def AppletLevel(self):
+        return self._AppletLevel
+
+    @AppletLevel.setter
+    def AppletLevel(self, AppletLevel):
+        self._AppletLevel = AppletLevel
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+
+    def _deserialize(self, params):
+        self._AppletJsUrl = params.get("AppletJsUrl")
+        self._AppletLevel = params.get("AppletLevel")
+        self._Name = params.get("Name")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AppletPlan(AbstractModel):
+    """小程序加固配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _PlanId: 策略Id
+        :type PlanId: int
+        :param _AppletLevel: 1 - 开启代码混淆、代码压缩、代码反调试保护。
+2 - 开启字符串编码和代码变换，代码膨胀，随机插入冗余代码，开启代码控制流平坦化，保证业务逻辑正常前提下，扁平化代码逻辑分支，破坏代码简单的线性结构。
+3 - 开启代码加密，对字符串、函数、变量、属性、类、数组等结构进行加密保护，更多得代码控制流平坦化，扁平化逻辑分支。
+        :type AppletLevel: int
+        """
+        self._PlanId = None
+        self._AppletLevel = None
+
+    @property
+    def PlanId(self):
+        return self._PlanId
+
+    @PlanId.setter
+    def PlanId(self, PlanId):
+        self._PlanId = PlanId
+
+    @property
+    def AppletLevel(self):
+        return self._AppletLevel
+
+    @AppletLevel.setter
+    def AppletLevel(self, AppletLevel):
+        self._AppletLevel = AppletLevel
+
+
+    def _deserialize(self, params):
+        self._PlanId = params.get("PlanId")
+        self._AppletLevel = params.get("AppletLevel")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AppletResult(AbstractModel):
+    """渠道合作加固小程序加固结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ResultId: 加固任务结果id
+        :type ResultId: str
+        :param _ResourceId: 资源id
+        :type ResourceId: str
+        :param _OrderId: 订单id
+        :type OrderId: str
+        :param _OpUin: 操作账号
+        :type OpUin: int
+        :param _EncryptState: 加固结果
+        :type EncryptState: int
+        :param _EncryptStateDesc: 加固结果描述
+        :type EncryptStateDesc: str
+        :param _EncryptErrCode: 失败错误码
+        :type EncryptErrCode: int
+        :param _EncryptErrDesc: 失败原因
+        :type EncryptErrDesc: str
+        :param _EncryptErrRef: 解决方案
+        :type EncryptErrRef: str
+        :param _CreatTime: 任务创建时间
+        :type CreatTime: str
+        :param _StartTime: 任务开始处理时间
+        :type StartTime: str
+        :param _EndTime: 任务处理结束时间
+        :type EndTime: str
+        :param _CostTime: 加固耗时（秒单位）
+        :type CostTime: int
+        :param _EncryptPkgUrl: 在线加固成功下载包
+        :type EncryptPkgUrl: str
+        :param _AppletInfo: 本次加固配置
+        :type AppletInfo: :class:`tencentcloud.ms.v20180408.models.AppletInfo`
+        """
+        self._ResultId = None
+        self._ResourceId = None
+        self._OrderId = None
+        self._OpUin = None
+        self._EncryptState = None
+        self._EncryptStateDesc = None
+        self._EncryptErrCode = None
+        self._EncryptErrDesc = None
+        self._EncryptErrRef = None
+        self._CreatTime = None
+        self._StartTime = None
+        self._EndTime = None
+        self._CostTime = None
+        self._EncryptPkgUrl = None
+        self._AppletInfo = None
+
+    @property
+    def ResultId(self):
+        return self._ResultId
+
+    @ResultId.setter
+    def ResultId(self, ResultId):
+        self._ResultId = ResultId
+
+    @property
+    def ResourceId(self):
+        return self._ResourceId
+
+    @ResourceId.setter
+    def ResourceId(self, ResourceId):
+        self._ResourceId = ResourceId
+
+    @property
+    def OrderId(self):
+        return self._OrderId
+
+    @OrderId.setter
+    def OrderId(self, OrderId):
+        self._OrderId = OrderId
+
+    @property
+    def OpUin(self):
+        return self._OpUin
+
+    @OpUin.setter
+    def OpUin(self, OpUin):
+        self._OpUin = OpUin
+
+    @property
+    def EncryptState(self):
+        return self._EncryptState
+
+    @EncryptState.setter
+    def EncryptState(self, EncryptState):
+        self._EncryptState = EncryptState
+
+    @property
+    def EncryptStateDesc(self):
+        return self._EncryptStateDesc
+
+    @EncryptStateDesc.setter
+    def EncryptStateDesc(self, EncryptStateDesc):
+        self._EncryptStateDesc = EncryptStateDesc
+
+    @property
+    def EncryptErrCode(self):
+        return self._EncryptErrCode
+
+    @EncryptErrCode.setter
+    def EncryptErrCode(self, EncryptErrCode):
+        self._EncryptErrCode = EncryptErrCode
+
+    @property
+    def EncryptErrDesc(self):
+        return self._EncryptErrDesc
+
+    @EncryptErrDesc.setter
+    def EncryptErrDesc(self, EncryptErrDesc):
+        self._EncryptErrDesc = EncryptErrDesc
+
+    @property
+    def EncryptErrRef(self):
+        return self._EncryptErrRef
+
+    @EncryptErrRef.setter
+    def EncryptErrRef(self, EncryptErrRef):
+        self._EncryptErrRef = EncryptErrRef
+
+    @property
+    def CreatTime(self):
+        return self._CreatTime
+
+    @CreatTime.setter
+    def CreatTime(self, CreatTime):
+        self._CreatTime = CreatTime
+
+    @property
+    def StartTime(self):
+        return self._StartTime
+
+    @StartTime.setter
+    def StartTime(self, StartTime):
+        self._StartTime = StartTime
+
+    @property
+    def EndTime(self):
+        return self._EndTime
+
+    @EndTime.setter
+    def EndTime(self, EndTime):
+        self._EndTime = EndTime
+
+    @property
+    def CostTime(self):
+        return self._CostTime
+
+    @CostTime.setter
+    def CostTime(self, CostTime):
+        self._CostTime = CostTime
+
+    @property
+    def EncryptPkgUrl(self):
+        return self._EncryptPkgUrl
+
+    @EncryptPkgUrl.setter
+    def EncryptPkgUrl(self, EncryptPkgUrl):
+        self._EncryptPkgUrl = EncryptPkgUrl
+
+    @property
+    def AppletInfo(self):
+        return self._AppletInfo
+
+    @AppletInfo.setter
+    def AppletInfo(self, AppletInfo):
+        self._AppletInfo = AppletInfo
+
+
+    def _deserialize(self, params):
+        self._ResultId = params.get("ResultId")
+        self._ResourceId = params.get("ResourceId")
+        self._OrderId = params.get("OrderId")
+        self._OpUin = params.get("OpUin")
+        self._EncryptState = params.get("EncryptState")
+        self._EncryptStateDesc = params.get("EncryptStateDesc")
+        self._EncryptErrCode = params.get("EncryptErrCode")
+        self._EncryptErrDesc = params.get("EncryptErrDesc")
+        self._EncryptErrRef = params.get("EncryptErrRef")
+        self._CreatTime = params.get("CreatTime")
+        self._StartTime = params.get("StartTime")
+        self._EndTime = params.get("EndTime")
+        self._CostTime = params.get("CostTime")
+        self._EncryptPkgUrl = params.get("EncryptPkgUrl")
+        if params.get("AppletInfo") is not None:
+            self._AppletInfo = AppletInfo()
+            self._AppletInfo._deserialize(params.get("AppletInfo"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class BindInfo(AbstractModel):
     """用户绑定app的基本信息
 
     """
 
     def __init__(self):
         r"""
@@ -494,14 +1502,84 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class CancelEncryptTaskRequest(AbstractModel):
+    """CancelEncryptTask请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ResultId: 加固任务结果Id 
+        :type ResultId: str
+        """
+        self._ResultId = None
+
+    @property
+    def ResultId(self):
+        return self._ResultId
+
+    @ResultId.setter
+    def ResultId(self, ResultId):
+        self._ResultId = ResultId
+
+
+    def _deserialize(self, params):
+        self._ResultId = params.get("ResultId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CancelEncryptTaskResponse(AbstractModel):
+    """CancelEncryptTask返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _State: 1: 取消任务成功 ； -1 ：取消任务失败，原因为任务进程已结束，不能取消。
+        :type State: int
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._State = None
+        self._RequestId = None
+
+    @property
+    def State(self):
+        return self._State
+
+    @State.setter
+    def State(self, State):
+        self._State = State
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._State = params.get("State")
+        self._RequestId = params.get("RequestId")
+
+
 class CreateBindInstanceRequest(AbstractModel):
     """CreateBindInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -782,14 +1860,270 @@
         self._CosKey = params.get("CosKey")
         self._CosTocken = params.get("CosTocken")
         self._CosPrefix = params.get("CosPrefix")
         self._CosToken = params.get("CosToken")
         self._RequestId = params.get("RequestId")
 
 
+class CreateEncryptInstanceRequest(AbstractModel):
+    """CreateEncryptInstance请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _PlatformType: 平台类型  1.android安卓加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
+        :type PlatformType: int
+        :param _OrderType: 订单采购类型 1-免费试用 2-按年收费 3-按次收费
+        :type OrderType: int
+        :param _EncryptOpType: 1-在线加固、  2-输出工具加固
+        :type EncryptOpType: int
+        :param _ResourceId: 本次加固使用的资源id
+        :type ResourceId: str
+        :param _AndroidAppInfo: 渠道合作安卓加固App信息 
+        :type AndroidAppInfo: :class:`tencentcloud.ms.v20180408.models.AndroidAppInfo`
+        :param _AndroidPlan: 渠道合作安卓加固策略信息
+        :type AndroidPlan: :class:`tencentcloud.ms.v20180408.models.AndroidPlan`
+        :param _AppletInfo: 小程序加固信息
+        :type AppletInfo: :class:`tencentcloud.ms.v20180408.models.AppletInfo`
+        """
+        self._PlatformType = None
+        self._OrderType = None
+        self._EncryptOpType = None
+        self._ResourceId = None
+        self._AndroidAppInfo = None
+        self._AndroidPlan = None
+        self._AppletInfo = None
+
+    @property
+    def PlatformType(self):
+        return self._PlatformType
+
+    @PlatformType.setter
+    def PlatformType(self, PlatformType):
+        self._PlatformType = PlatformType
+
+    @property
+    def OrderType(self):
+        return self._OrderType
+
+    @OrderType.setter
+    def OrderType(self, OrderType):
+        self._OrderType = OrderType
+
+    @property
+    def EncryptOpType(self):
+        return self._EncryptOpType
+
+    @EncryptOpType.setter
+    def EncryptOpType(self, EncryptOpType):
+        self._EncryptOpType = EncryptOpType
+
+    @property
+    def ResourceId(self):
+        return self._ResourceId
+
+    @ResourceId.setter
+    def ResourceId(self, ResourceId):
+        self._ResourceId = ResourceId
+
+    @property
+    def AndroidAppInfo(self):
+        return self._AndroidAppInfo
+
+    @AndroidAppInfo.setter
+    def AndroidAppInfo(self, AndroidAppInfo):
+        self._AndroidAppInfo = AndroidAppInfo
+
+    @property
+    def AndroidPlan(self):
+        return self._AndroidPlan
+
+    @AndroidPlan.setter
+    def AndroidPlan(self, AndroidPlan):
+        self._AndroidPlan = AndroidPlan
+
+    @property
+    def AppletInfo(self):
+        return self._AppletInfo
+
+    @AppletInfo.setter
+    def AppletInfo(self, AppletInfo):
+        self._AppletInfo = AppletInfo
+
+
+    def _deserialize(self, params):
+        self._PlatformType = params.get("PlatformType")
+        self._OrderType = params.get("OrderType")
+        self._EncryptOpType = params.get("EncryptOpType")
+        self._ResourceId = params.get("ResourceId")
+        if params.get("AndroidAppInfo") is not None:
+            self._AndroidAppInfo = AndroidAppInfo()
+            self._AndroidAppInfo._deserialize(params.get("AndroidAppInfo"))
+        if params.get("AndroidPlan") is not None:
+            self._AndroidPlan = AndroidPlan()
+            self._AndroidPlan._deserialize(params.get("AndroidPlan"))
+        if params.get("AppletInfo") is not None:
+            self._AppletInfo = AppletInfo()
+            self._AppletInfo._deserialize(params.get("AppletInfo"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateEncryptInstanceResponse(AbstractModel):
+    """CreateEncryptInstance返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ResultId: 加固任务Id
+        :type ResultId: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._ResultId = None
+        self._RequestId = None
+
+    @property
+    def ResultId(self):
+        return self._ResultId
+
+    @ResultId.setter
+    def ResultId(self, ResultId):
+        self._ResultId = ResultId
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._ResultId = params.get("ResultId")
+        self._RequestId = params.get("RequestId")
+
+
+class CreateOrderInstanceRequest(AbstractModel):
+    """CreateOrderInstance请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _PlatformType: 平台类型枚举值：1-android安卓加固  ；2-ios源码混淆 ； 3-sdk加固 ； 4-applet小程序加固
+        :type PlatformType: int
+        :param _OrderType: 订单采购类型 1-免费试用 ；2-按年收费 ；3-按次收费
+        :type OrderType: int
+        :param _AppPkgNameList: 代表应用包名列表，值为单个包名（例如：“a.b.xxx”）或多个包名用逗号隔开(例如：“a.b.xxx,b.c.xxx”)。
+当安卓按年收费加固或安卓免费试用加固时，该字段要求非空，即PlatformType=1 并且 OrderType=2时，AppPkgNameList必传值。
+
+        :type AppPkgNameList: str
+        """
+        self._PlatformType = None
+        self._OrderType = None
+        self._AppPkgNameList = None
+
+    @property
+    def PlatformType(self):
+        return self._PlatformType
+
+    @PlatformType.setter
+    def PlatformType(self, PlatformType):
+        self._PlatformType = PlatformType
+
+    @property
+    def OrderType(self):
+        return self._OrderType
+
+    @OrderType.setter
+    def OrderType(self, OrderType):
+        self._OrderType = OrderType
+
+    @property
+    def AppPkgNameList(self):
+        return self._AppPkgNameList
+
+    @AppPkgNameList.setter
+    def AppPkgNameList(self, AppPkgNameList):
+        self._AppPkgNameList = AppPkgNameList
+
+
+    def _deserialize(self, params):
+        self._PlatformType = params.get("PlatformType")
+        self._OrderType = params.get("OrderType")
+        self._AppPkgNameList = params.get("AppPkgNameList")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateOrderInstanceResponse(AbstractModel):
+    """CreateOrderInstance返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _OrderId: 订单Id
+        :type OrderId: str
+        :param _ResourceId: 与订单关联的资源id
+        :type ResourceId: list of str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._OrderId = None
+        self._ResourceId = None
+        self._RequestId = None
+
+    @property
+    def OrderId(self):
+        return self._OrderId
+
+    @OrderId.setter
+    def OrderId(self, OrderId):
+        self._OrderId = OrderId
+
+    @property
+    def ResourceId(self):
+        return self._ResourceId
+
+    @ResourceId.setter
+    def ResourceId(self, ResourceId):
+        self._ResourceId = ResourceId
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._OrderId = params.get("OrderId")
+        self._ResourceId = params.get("ResourceId")
+        self._RequestId = params.get("RequestId")
+
+
 class CreateResourceInstancesRequest(AbstractModel):
     """CreateResourceInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1275,14 +2609,720 @@
             for item in params.get("ResultList"):
                 obj = ResultListItem()
                 obj._deserialize(item)
                 self._ResultList.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class DescribeEncryptInstancesRequest(AbstractModel):
+    """DescribeEncryptInstances请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _PageNumber: 多记录查询时使用，页码
+        :type PageNumber: int
+        :param _PageSize: 多记录每页展示数量
+        :type PageSize: int
+        :param _OrderField: 多记录查询时排序使用  仅支持CreateTime 任务创建时间排序
+        :type OrderField: str
+        :param _OrderDirection: 升序（asc）还是降序（desc），默认：desc。
+        :type OrderDirection: str
+        :param _PlatformType: (条件过滤字段) 平台类型  1.android安卓加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
+        :type PlatformType: int
+        :param _OrderType: (条件过滤字段) 订单采购类型 1-免费试用 2-按年收费 3-按次收费
+        :type OrderType: int
+        :param _EncryptOpType: (条件过滤字段) 1-在线加固 或 2-输出工具加固
+        :type EncryptOpType: int
+        :param _ResultId: (条件过滤字段) 单记录查询时使用，结果ID该字段非空时，结构会根据结果ID进行单记录查询，符合查询条件时，只返回一条记录。
+        :type ResultId: str
+        :param _OrderId: (条件过滤字段) 查询与订单Id关联的任务
+        :type OrderId: str
+        :param _ResourceId: (条件过滤字段) 查询与资源Id关联的任务
+        :type ResourceId: str
+        :param _AppType: (条件过滤字段) 安卓应用类型：安卓-apk; 安卓-aab;
+        :type AppType: str
+        :param _AppPkgName: （条件过滤字段）安卓应用的包名
+        :type AppPkgName: str
+        :param _EncryptState: 加固结果，
+0：正在排队；
+1：加固成功；
+2：加固中；
+3：加固失败；
+5：重试；
+多记录查询时，根据查询结果进行检索使用。
+        :type EncryptState: list of int
+        """
+        self._PageNumber = None
+        self._PageSize = None
+        self._OrderField = None
+        self._OrderDirection = None
+        self._PlatformType = None
+        self._OrderType = None
+        self._EncryptOpType = None
+        self._ResultId = None
+        self._OrderId = None
+        self._ResourceId = None
+        self._AppType = None
+        self._AppPkgName = None
+        self._EncryptState = None
+
+    @property
+    def PageNumber(self):
+        return self._PageNumber
+
+    @PageNumber.setter
+    def PageNumber(self, PageNumber):
+        self._PageNumber = PageNumber
+
+    @property
+    def PageSize(self):
+        return self._PageSize
+
+    @PageSize.setter
+    def PageSize(self, PageSize):
+        self._PageSize = PageSize
+
+    @property
+    def OrderField(self):
+        return self._OrderField
+
+    @OrderField.setter
+    def OrderField(self, OrderField):
+        self._OrderField = OrderField
+
+    @property
+    def OrderDirection(self):
+        return self._OrderDirection
+
+    @OrderDirection.setter
+    def OrderDirection(self, OrderDirection):
+        self._OrderDirection = OrderDirection
+
+    @property
+    def PlatformType(self):
+        return self._PlatformType
+
+    @PlatformType.setter
+    def PlatformType(self, PlatformType):
+        self._PlatformType = PlatformType
+
+    @property
+    def OrderType(self):
+        return self._OrderType
+
+    @OrderType.setter
+    def OrderType(self, OrderType):
+        self._OrderType = OrderType
+
+    @property
+    def EncryptOpType(self):
+        return self._EncryptOpType
+
+    @EncryptOpType.setter
+    def EncryptOpType(self, EncryptOpType):
+        self._EncryptOpType = EncryptOpType
+
+    @property
+    def ResultId(self):
+        return self._ResultId
+
+    @ResultId.setter
+    def ResultId(self, ResultId):
+        self._ResultId = ResultId
+
+    @property
+    def OrderId(self):
+        return self._OrderId
+
+    @OrderId.setter
+    def OrderId(self, OrderId):
+        self._OrderId = OrderId
+
+    @property
+    def ResourceId(self):
+        return self._ResourceId
+
+    @ResourceId.setter
+    def ResourceId(self, ResourceId):
+        self._ResourceId = ResourceId
+
+    @property
+    def AppType(self):
+        return self._AppType
+
+    @AppType.setter
+    def AppType(self, AppType):
+        self._AppType = AppType
+
+    @property
+    def AppPkgName(self):
+        return self._AppPkgName
+
+    @AppPkgName.setter
+    def AppPkgName(self, AppPkgName):
+        self._AppPkgName = AppPkgName
+
+    @property
+    def EncryptState(self):
+        return self._EncryptState
+
+    @EncryptState.setter
+    def EncryptState(self, EncryptState):
+        self._EncryptState = EncryptState
+
+
+    def _deserialize(self, params):
+        self._PageNumber = params.get("PageNumber")
+        self._PageSize = params.get("PageSize")
+        self._OrderField = params.get("OrderField")
+        self._OrderDirection = params.get("OrderDirection")
+        self._PlatformType = params.get("PlatformType")
+        self._OrderType = params.get("OrderType")
+        self._EncryptOpType = params.get("EncryptOpType")
+        self._ResultId = params.get("ResultId")
+        self._OrderId = params.get("OrderId")
+        self._ResourceId = params.get("ResourceId")
+        self._AppType = params.get("AppType")
+        self._AppPkgName = params.get("AppPkgName")
+        self._EncryptState = params.get("EncryptState")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeEncryptInstancesResponse(AbstractModel):
+    """DescribeEncryptInstances返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TotalCount: 总记录数
+        :type TotalCount: int
+        :param _EncryptResults: 渠道合作加固信息数组
+        :type EncryptResults: list of EncryptResults
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TotalCount = None
+        self._EncryptResults = None
+        self._RequestId = None
+
+    @property
+    def TotalCount(self):
+        return self._TotalCount
+
+    @TotalCount.setter
+    def TotalCount(self, TotalCount):
+        self._TotalCount = TotalCount
+
+    @property
+    def EncryptResults(self):
+        return self._EncryptResults
+
+    @EncryptResults.setter
+    def EncryptResults(self, EncryptResults):
+        self._EncryptResults = EncryptResults
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._TotalCount = params.get("TotalCount")
+        if params.get("EncryptResults") is not None:
+            self._EncryptResults = []
+            for item in params.get("EncryptResults"):
+                obj = EncryptResults()
+                obj._deserialize(item)
+                self._EncryptResults.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
+class DescribeEncryptPlanRequest(AbstractModel):
+    """DescribeEncryptPlan请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _PlatformType: 平台类型  1.android安卓加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
+        :type PlatformType: int
+        :param _OrderType: 订单采购类型 1-免费试用 2-按年收费 3-按次收费
+        :type OrderType: int
+        :param _EncryptOpType: 1-在线加固；2-输出工具
+        :type EncryptOpType: int
+        :param _ResourceId: 本次加固使用的资源id
+        :type ResourceId: str
+        :param _AppPkgName: （条件过滤字段）安卓加固查询时，根据包名查询
+        :type AppPkgName: str
+        :param _AppType: （条件过滤字段）安卓加固查询时，根据应用格式查询，枚举值：“apk”、“aab”
+        :type AppType: str
+        """
+        self._PlatformType = None
+        self._OrderType = None
+        self._EncryptOpType = None
+        self._ResourceId = None
+        self._AppPkgName = None
+        self._AppType = None
+
+    @property
+    def PlatformType(self):
+        return self._PlatformType
+
+    @PlatformType.setter
+    def PlatformType(self, PlatformType):
+        self._PlatformType = PlatformType
+
+    @property
+    def OrderType(self):
+        return self._OrderType
+
+    @OrderType.setter
+    def OrderType(self, OrderType):
+        self._OrderType = OrderType
+
+    @property
+    def EncryptOpType(self):
+        return self._EncryptOpType
+
+    @EncryptOpType.setter
+    def EncryptOpType(self, EncryptOpType):
+        self._EncryptOpType = EncryptOpType
+
+    @property
+    def ResourceId(self):
+        return self._ResourceId
+
+    @ResourceId.setter
+    def ResourceId(self, ResourceId):
+        self._ResourceId = ResourceId
+
+    @property
+    def AppPkgName(self):
+        return self._AppPkgName
+
+    @AppPkgName.setter
+    def AppPkgName(self, AppPkgName):
+        self._AppPkgName = AppPkgName
+
+    @property
+    def AppType(self):
+        return self._AppType
+
+    @AppType.setter
+    def AppType(self, AppType):
+        self._AppType = AppType
+
+
+    def _deserialize(self, params):
+        self._PlatformType = params.get("PlatformType")
+        self._OrderType = params.get("OrderType")
+        self._EncryptOpType = params.get("EncryptOpType")
+        self._ResourceId = params.get("ResourceId")
+        self._AppPkgName = params.get("AppPkgName")
+        self._AppType = params.get("AppType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeEncryptPlanResponse(AbstractModel):
+    """DescribeEncryptPlan返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _PlatformType: 平台类型整型值  
+        :type PlatformType: int
+        :param _PlatformTypeDesc: 平台类型描述 1.android安卓加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
+        :type PlatformTypeDesc: str
+        :param _EncryptOpType: 1- 在线加固 2-输出工具加固
+        :type EncryptOpType: int
+        :param _EncryptOpTypeDesc: 1- 在线加固 2-输出工具加固
+        :type EncryptOpTypeDesc: str
+        :param _OrderType: 订单收费类型枚举值
+        :type OrderType: int
+        :param _OrderTypeDesc: 订单收费类型描述
+        :type OrderTypeDesc: str
+        :param _ResourceId: 资源id
+        :type ResourceId: str
+        :param _AndroidPlan: 上次安卓加固策略
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AndroidPlan: :class:`tencentcloud.ms.v20180408.models.AndroidPlan`
+        :param _AppletPlan: 上次小程序加固策略
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AppletPlan: :class:`tencentcloud.ms.v20180408.models.AppletPlan`
+        :param _IOSPlan: 上次ios源码混淆加固配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IOSPlan: :class:`tencentcloud.ms.v20180408.models.IOSPlan`
+        :param _SDKPlan: 上次sdk加固配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SDKPlan: :class:`tencentcloud.ms.v20180408.models.SDKPlan`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._PlatformType = None
+        self._PlatformTypeDesc = None
+        self._EncryptOpType = None
+        self._EncryptOpTypeDesc = None
+        self._OrderType = None
+        self._OrderTypeDesc = None
+        self._ResourceId = None
+        self._AndroidPlan = None
+        self._AppletPlan = None
+        self._IOSPlan = None
+        self._SDKPlan = None
+        self._RequestId = None
+
+    @property
+    def PlatformType(self):
+        return self._PlatformType
+
+    @PlatformType.setter
+    def PlatformType(self, PlatformType):
+        self._PlatformType = PlatformType
+
+    @property
+    def PlatformTypeDesc(self):
+        return self._PlatformTypeDesc
+
+    @PlatformTypeDesc.setter
+    def PlatformTypeDesc(self, PlatformTypeDesc):
+        self._PlatformTypeDesc = PlatformTypeDesc
+
+    @property
+    def EncryptOpType(self):
+        return self._EncryptOpType
+
+    @EncryptOpType.setter
+    def EncryptOpType(self, EncryptOpType):
+        self._EncryptOpType = EncryptOpType
+
+    @property
+    def EncryptOpTypeDesc(self):
+        return self._EncryptOpTypeDesc
+
+    @EncryptOpTypeDesc.setter
+    def EncryptOpTypeDesc(self, EncryptOpTypeDesc):
+        self._EncryptOpTypeDesc = EncryptOpTypeDesc
+
+    @property
+    def OrderType(self):
+        return self._OrderType
+
+    @OrderType.setter
+    def OrderType(self, OrderType):
+        self._OrderType = OrderType
+
+    @property
+    def OrderTypeDesc(self):
+        return self._OrderTypeDesc
+
+    @OrderTypeDesc.setter
+    def OrderTypeDesc(self, OrderTypeDesc):
+        self._OrderTypeDesc = OrderTypeDesc
+
+    @property
+    def ResourceId(self):
+        return self._ResourceId
+
+    @ResourceId.setter
+    def ResourceId(self, ResourceId):
+        self._ResourceId = ResourceId
+
+    @property
+    def AndroidPlan(self):
+        return self._AndroidPlan
+
+    @AndroidPlan.setter
+    def AndroidPlan(self, AndroidPlan):
+        self._AndroidPlan = AndroidPlan
+
+    @property
+    def AppletPlan(self):
+        return self._AppletPlan
+
+    @AppletPlan.setter
+    def AppletPlan(self, AppletPlan):
+        self._AppletPlan = AppletPlan
+
+    @property
+    def IOSPlan(self):
+        return self._IOSPlan
+
+    @IOSPlan.setter
+    def IOSPlan(self, IOSPlan):
+        self._IOSPlan = IOSPlan
+
+    @property
+    def SDKPlan(self):
+        return self._SDKPlan
+
+    @SDKPlan.setter
+    def SDKPlan(self, SDKPlan):
+        self._SDKPlan = SDKPlan
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._PlatformType = params.get("PlatformType")
+        self._PlatformTypeDesc = params.get("PlatformTypeDesc")
+        self._EncryptOpType = params.get("EncryptOpType")
+        self._EncryptOpTypeDesc = params.get("EncryptOpTypeDesc")
+        self._OrderType = params.get("OrderType")
+        self._OrderTypeDesc = params.get("OrderTypeDesc")
+        self._ResourceId = params.get("ResourceId")
+        if params.get("AndroidPlan") is not None:
+            self._AndroidPlan = AndroidPlan()
+            self._AndroidPlan._deserialize(params.get("AndroidPlan"))
+        if params.get("AppletPlan") is not None:
+            self._AppletPlan = AppletPlan()
+            self._AppletPlan._deserialize(params.get("AppletPlan"))
+        if params.get("IOSPlan") is not None:
+            self._IOSPlan = IOSPlan()
+            self._IOSPlan._deserialize(params.get("IOSPlan"))
+        if params.get("SDKPlan") is not None:
+            self._SDKPlan = SDKPlan()
+            self._SDKPlan._deserialize(params.get("SDKPlan"))
+        self._RequestId = params.get("RequestId")
+
+
+class DescribeOrderInstancesRequest(AbstractModel):
+    """DescribeOrderInstances请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _PageNumber: 页码
+        :type PageNumber: int
+        :param _PageSize: 每页展示数量
+        :type PageSize: int
+        :param _OrderField: 按某个字段排序，目前仅支持CreateTime排序。
+        :type OrderField: str
+        :param _OrderDirection: 升序（asc）还是降序（desc），默认：desc。
+        :type OrderDirection: str
+        :param _PlatformType: （条件过滤字段）平台类型  1.android安卓加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
+        :type PlatformType: int
+        :param _OrderType: （条件过滤字段）订单采购类型 1-免费试用 2-按年收费 3-按次收费
+        :type OrderType: int
+        :param _ApprovalStatus: （条件过滤字段）订单审批状态：
+        :type ApprovalStatus: int
+        :param _ResourceStatus: （条件过滤字段）资源状态：
+        :type ResourceStatus: int
+        :param _OrderId: （条件过滤字段）订单ID
+        :type OrderId: str
+        :param _ResourceId: （条件过滤字段）资源ID
+        :type ResourceId: str
+        :param _AppPkgName: （条件过滤字段）安卓包名，查询android安卓加固订单时使用
+        :type AppPkgName: str
+        """
+        self._PageNumber = None
+        self._PageSize = None
+        self._OrderField = None
+        self._OrderDirection = None
+        self._PlatformType = None
+        self._OrderType = None
+        self._ApprovalStatus = None
+        self._ResourceStatus = None
+        self._OrderId = None
+        self._ResourceId = None
+        self._AppPkgName = None
+
+    @property
+    def PageNumber(self):
+        return self._PageNumber
+
+    @PageNumber.setter
+    def PageNumber(self, PageNumber):
+        self._PageNumber = PageNumber
+
+    @property
+    def PageSize(self):
+        return self._PageSize
+
+    @PageSize.setter
+    def PageSize(self, PageSize):
+        self._PageSize = PageSize
+
+    @property
+    def OrderField(self):
+        return self._OrderField
+
+    @OrderField.setter
+    def OrderField(self, OrderField):
+        self._OrderField = OrderField
+
+    @property
+    def OrderDirection(self):
+        return self._OrderDirection
+
+    @OrderDirection.setter
+    def OrderDirection(self, OrderDirection):
+        self._OrderDirection = OrderDirection
+
+    @property
+    def PlatformType(self):
+        return self._PlatformType
+
+    @PlatformType.setter
+    def PlatformType(self, PlatformType):
+        self._PlatformType = PlatformType
+
+    @property
+    def OrderType(self):
+        return self._OrderType
+
+    @OrderType.setter
+    def OrderType(self, OrderType):
+        self._OrderType = OrderType
+
+    @property
+    def ApprovalStatus(self):
+        return self._ApprovalStatus
+
+    @ApprovalStatus.setter
+    def ApprovalStatus(self, ApprovalStatus):
+        self._ApprovalStatus = ApprovalStatus
+
+    @property
+    def ResourceStatus(self):
+        return self._ResourceStatus
+
+    @ResourceStatus.setter
+    def ResourceStatus(self, ResourceStatus):
+        self._ResourceStatus = ResourceStatus
+
+    @property
+    def OrderId(self):
+        return self._OrderId
+
+    @OrderId.setter
+    def OrderId(self, OrderId):
+        self._OrderId = OrderId
+
+    @property
+    def ResourceId(self):
+        return self._ResourceId
+
+    @ResourceId.setter
+    def ResourceId(self, ResourceId):
+        self._ResourceId = ResourceId
+
+    @property
+    def AppPkgName(self):
+        return self._AppPkgName
+
+    @AppPkgName.setter
+    def AppPkgName(self, AppPkgName):
+        self._AppPkgName = AppPkgName
+
+
+    def _deserialize(self, params):
+        self._PageNumber = params.get("PageNumber")
+        self._PageSize = params.get("PageSize")
+        self._OrderField = params.get("OrderField")
+        self._OrderDirection = params.get("OrderDirection")
+        self._PlatformType = params.get("PlatformType")
+        self._OrderType = params.get("OrderType")
+        self._ApprovalStatus = params.get("ApprovalStatus")
+        self._ResourceStatus = params.get("ResourceStatus")
+        self._OrderId = params.get("OrderId")
+        self._ResourceId = params.get("ResourceId")
+        self._AppPkgName = params.get("AppPkgName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeOrderInstancesResponse(AbstractModel):
+    """DescribeOrderInstances返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TotalCount: 总记录数
+        :type TotalCount: int
+        :param _Orders: 订单信息
+        :type Orders: list of Orders
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TotalCount = None
+        self._Orders = None
+        self._RequestId = None
+
+    @property
+    def TotalCount(self):
+        return self._TotalCount
+
+    @TotalCount.setter
+    def TotalCount(self, TotalCount):
+        self._TotalCount = TotalCount
+
+    @property
+    def Orders(self):
+        return self._Orders
+
+    @Orders.setter
+    def Orders(self, Orders):
+        self._Orders = Orders
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._TotalCount = params.get("TotalCount")
+        if params.get("Orders") is not None:
+            self._Orders = []
+            for item in params.get("Orders"):
+                obj = Orders()
+                obj._deserialize(item)
+                self._Orders.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeResourceInstancesRequest(AbstractModel):
     """DescribeResourceInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2107,14 +4147,191 @@
     def _deserialize(self, params):
         self._UserUin = params.get("UserUin")
         self._UserAppid = params.get("UserAppid")
         self._TimeStamp = params.get("TimeStamp")
         self._RequestId = params.get("RequestId")
 
 
+class EncryptResults(AbstractModel):
+    """渠道合作加固结果信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _PlatformType: 平台类型枚举值  1-android安卓加固   2-ios源码混淆  3-sdk加固  4-applet小程序加固
+        :type PlatformType: int
+        :param _PlatformDesc: 平台类型描述  1-android安卓加固   2-ios源码混淆  3-sdk加固  4-applet小程序加固
+        :type PlatformDesc: str
+        :param _OrderType: 订单采购类型枚举值， 1-免费试用 2-按年收费 3-按次收费
+        :type OrderType: int
+        :param _OrderTypeDesc: 订单采购类型 描述：1-免费试用 2-按年收费 3-按次收费
+        :type OrderTypeDesc: str
+        :param _EncryptOpType: 枚举值：1-在线加固 或 2-输出工具加固
+        :type EncryptOpType: int
+        :param _EncryptOpTypeDesc: 描述：1-在线加固 或 2-输出工具加固
+        :type EncryptOpTypeDesc: str
+        :param _ResourceId: 与当前任务关联的资源Id
+        :type ResourceId: str
+        :param _OrderId: 与当前任务关联的订单Id
+        :type OrderId: str
+        :param _AndroidResult: 对应PlatformType平台类型值   1-android安卓加固结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AndroidResult: :class:`tencentcloud.ms.v20180408.models.AndroidResult`
+        :param _IOSResult: 对应PlatformType平台类型值   2-ios源码混淆加固结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IOSResult: :class:`tencentcloud.ms.v20180408.models.IOSResult`
+        :param _SDKResult: 对应PlatformType平台类型值   3-sdk加固结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SDKResult: :class:`tencentcloud.ms.v20180408.models.SDKResult`
+        :param _AppletResult: 对应PlatformType平台类型值   4-applet小程序加固结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AppletResult: :class:`tencentcloud.ms.v20180408.models.AppletResult`
+        """
+        self._PlatformType = None
+        self._PlatformDesc = None
+        self._OrderType = None
+        self._OrderTypeDesc = None
+        self._EncryptOpType = None
+        self._EncryptOpTypeDesc = None
+        self._ResourceId = None
+        self._OrderId = None
+        self._AndroidResult = None
+        self._IOSResult = None
+        self._SDKResult = None
+        self._AppletResult = None
+
+    @property
+    def PlatformType(self):
+        return self._PlatformType
+
+    @PlatformType.setter
+    def PlatformType(self, PlatformType):
+        self._PlatformType = PlatformType
+
+    @property
+    def PlatformDesc(self):
+        return self._PlatformDesc
+
+    @PlatformDesc.setter
+    def PlatformDesc(self, PlatformDesc):
+        self._PlatformDesc = PlatformDesc
+
+    @property
+    def OrderType(self):
+        return self._OrderType
+
+    @OrderType.setter
+    def OrderType(self, OrderType):
+        self._OrderType = OrderType
+
+    @property
+    def OrderTypeDesc(self):
+        return self._OrderTypeDesc
+
+    @OrderTypeDesc.setter
+    def OrderTypeDesc(self, OrderTypeDesc):
+        self._OrderTypeDesc = OrderTypeDesc
+
+    @property
+    def EncryptOpType(self):
+        return self._EncryptOpType
+
+    @EncryptOpType.setter
+    def EncryptOpType(self, EncryptOpType):
+        self._EncryptOpType = EncryptOpType
+
+    @property
+    def EncryptOpTypeDesc(self):
+        return self._EncryptOpTypeDesc
+
+    @EncryptOpTypeDesc.setter
+    def EncryptOpTypeDesc(self, EncryptOpTypeDesc):
+        self._EncryptOpTypeDesc = EncryptOpTypeDesc
+
+    @property
+    def ResourceId(self):
+        return self._ResourceId
+
+    @ResourceId.setter
+    def ResourceId(self, ResourceId):
+        self._ResourceId = ResourceId
+
+    @property
+    def OrderId(self):
+        return self._OrderId
+
+    @OrderId.setter
+    def OrderId(self, OrderId):
+        self._OrderId = OrderId
+
+    @property
+    def AndroidResult(self):
+        return self._AndroidResult
+
+    @AndroidResult.setter
+    def AndroidResult(self, AndroidResult):
+        self._AndroidResult = AndroidResult
+
+    @property
+    def IOSResult(self):
+        return self._IOSResult
+
+    @IOSResult.setter
+    def IOSResult(self, IOSResult):
+        self._IOSResult = IOSResult
+
+    @property
+    def SDKResult(self):
+        return self._SDKResult
+
+    @SDKResult.setter
+    def SDKResult(self, SDKResult):
+        self._SDKResult = SDKResult
+
+    @property
+    def AppletResult(self):
+        return self._AppletResult
+
+    @AppletResult.setter
+    def AppletResult(self, AppletResult):
+        self._AppletResult = AppletResult
+
+
+    def _deserialize(self, params):
+        self._PlatformType = params.get("PlatformType")
+        self._PlatformDesc = params.get("PlatformDesc")
+        self._OrderType = params.get("OrderType")
+        self._OrderTypeDesc = params.get("OrderTypeDesc")
+        self._EncryptOpType = params.get("EncryptOpType")
+        self._EncryptOpTypeDesc = params.get("EncryptOpTypeDesc")
+        self._ResourceId = params.get("ResourceId")
+        self._OrderId = params.get("OrderId")
+        if params.get("AndroidResult") is not None:
+            self._AndroidResult = AndroidResult()
+            self._AndroidResult._deserialize(params.get("AndroidResult"))
+        if params.get("IOSResult") is not None:
+            self._IOSResult = IOSResult()
+            self._IOSResult._deserialize(params.get("IOSResult"))
+        if params.get("SDKResult") is not None:
+            self._SDKResult = SDKResult()
+            self._SDKResult._deserialize(params.get("SDKResult"))
+        if params.get("AppletResult") is not None:
+            self._AppletResult = AppletResult()
+            self._AppletResult._deserialize(params.get("AppletResult"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class Filter(AbstractModel):
     """筛选数据结构
 
     """
 
     def __init__(self):
         r"""
@@ -2152,14 +4369,80 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class IOSPlan(AbstractModel):
+    """渠道合作IOS源码混淆配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _PlanId: 策略id
+        :type PlanId: int
+        """
+        self._PlanId = None
+
+    @property
+    def PlanId(self):
+        return self._PlanId
+
+    @PlanId.setter
+    def PlanId(self, PlanId):
+        self._PlanId = PlanId
+
+
+    def _deserialize(self, params):
+        self._PlanId = params.get("PlanId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class IOSResult(AbstractModel):
+    """渠道合作ios源码混淆加固结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ResultId: 加固任务结果Id
+        :type ResultId: str
+        """
+        self._ResultId = None
+
+    @property
+    def ResultId(self):
+        return self._ResultId
+
+    @ResultId.setter
+    def ResultId(self, ResultId):
+        self._ResultId = ResultId
+
+
+    def _deserialize(self, params):
+        self._ResultId = params.get("ResultId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class OptPluginListItem(AbstractModel):
     """APK检测服务：非广告插件结果列表(SDK、风险插件等)
 
     """
 
     def __init__(self):
         r"""
@@ -2209,14 +4492,276 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class Orders(AbstractModel):
+    """渠道合作加固订单资源信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _OrderId: 订单号
+        :type OrderId: str
+        :param _PlatformType: 平台类型整型值 
+        :type PlatformType: int
+        :param _PlatformTypeDesc: 平台类型描述：  1.android安卓加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
+        :type PlatformTypeDesc: str
+        :param _OrderType: 订单采购类型整型值
+        :type OrderType: int
+        :param _OrderTypeDesc: 订单采购类型描述： 1-免费试用 2-按年收费 3-按次收费
+        :type OrderTypeDesc: str
+        :param _AppPkgName: 安卓包年收费加固的包名
+        :type AppPkgName: str
+        :param _ResourceId: 资源号
+        :type ResourceId: str
+        :param _ResourceStatus: 资源状态整型值
+        :type ResourceStatus: int
+        :param _ResourceStatusDesc: 资源状态描述
+0-未生效、1-生效中、2-已失效。
+        :type ResourceStatusDesc: str
+        :param _TestTimes: 订单类型为免费试用时的免费加固次数。
+        :type TestTimes: int
+        :param _ValidTime: 资源生效时间
+        :type ValidTime: str
+        :param _ExpireTime: 资源过期时间
+        :type ExpireTime: str
+        :param _CreateTime: 资源创建时间
+        :type CreateTime: str
+        :param _Approver: 订单审批人
+        :type Approver: str
+        :param _ApprovalStatus: 订单审批状态整型值
+        :type ApprovalStatus: int
+        :param _ApprovalStatusDesc: 订单审批状态整型值描述：0-未审批、1-审批通过、2-驳回。
+        :type ApprovalStatusDesc: str
+        :param _ApprovalTime: 订单审批时间
+        :type ApprovalTime: str
+        :param _TimesTaskTotalCount: 按次收费加固资源，其关联的总任务数
+        :type TimesTaskTotalCount: int
+        :param _TimesTaskSuccessCount: 按次收费加固资源，其关联的任务成功数
+        :type TimesTaskSuccessCount: int
+        :param _TimesTaskFailCount: 按次收费加固资源，其关联的任务失败数
+        :type TimesTaskFailCount: int
+        """
+        self._OrderId = None
+        self._PlatformType = None
+        self._PlatformTypeDesc = None
+        self._OrderType = None
+        self._OrderTypeDesc = None
+        self._AppPkgName = None
+        self._ResourceId = None
+        self._ResourceStatus = None
+        self._ResourceStatusDesc = None
+        self._TestTimes = None
+        self._ValidTime = None
+        self._ExpireTime = None
+        self._CreateTime = None
+        self._Approver = None
+        self._ApprovalStatus = None
+        self._ApprovalStatusDesc = None
+        self._ApprovalTime = None
+        self._TimesTaskTotalCount = None
+        self._TimesTaskSuccessCount = None
+        self._TimesTaskFailCount = None
+
+    @property
+    def OrderId(self):
+        return self._OrderId
+
+    @OrderId.setter
+    def OrderId(self, OrderId):
+        self._OrderId = OrderId
+
+    @property
+    def PlatformType(self):
+        return self._PlatformType
+
+    @PlatformType.setter
+    def PlatformType(self, PlatformType):
+        self._PlatformType = PlatformType
+
+    @property
+    def PlatformTypeDesc(self):
+        return self._PlatformTypeDesc
+
+    @PlatformTypeDesc.setter
+    def PlatformTypeDesc(self, PlatformTypeDesc):
+        self._PlatformTypeDesc = PlatformTypeDesc
+
+    @property
+    def OrderType(self):
+        return self._OrderType
+
+    @OrderType.setter
+    def OrderType(self, OrderType):
+        self._OrderType = OrderType
+
+    @property
+    def OrderTypeDesc(self):
+        return self._OrderTypeDesc
+
+    @OrderTypeDesc.setter
+    def OrderTypeDesc(self, OrderTypeDesc):
+        self._OrderTypeDesc = OrderTypeDesc
+
+    @property
+    def AppPkgName(self):
+        return self._AppPkgName
+
+    @AppPkgName.setter
+    def AppPkgName(self, AppPkgName):
+        self._AppPkgName = AppPkgName
+
+    @property
+    def ResourceId(self):
+        return self._ResourceId
+
+    @ResourceId.setter
+    def ResourceId(self, ResourceId):
+        self._ResourceId = ResourceId
+
+    @property
+    def ResourceStatus(self):
+        return self._ResourceStatus
+
+    @ResourceStatus.setter
+    def ResourceStatus(self, ResourceStatus):
+        self._ResourceStatus = ResourceStatus
+
+    @property
+    def ResourceStatusDesc(self):
+        return self._ResourceStatusDesc
+
+    @ResourceStatusDesc.setter
+    def ResourceStatusDesc(self, ResourceStatusDesc):
+        self._ResourceStatusDesc = ResourceStatusDesc
+
+    @property
+    def TestTimes(self):
+        return self._TestTimes
+
+    @TestTimes.setter
+    def TestTimes(self, TestTimes):
+        self._TestTimes = TestTimes
+
+    @property
+    def ValidTime(self):
+        return self._ValidTime
+
+    @ValidTime.setter
+    def ValidTime(self, ValidTime):
+        self._ValidTime = ValidTime
+
+    @property
+    def ExpireTime(self):
+        return self._ExpireTime
+
+    @ExpireTime.setter
+    def ExpireTime(self, ExpireTime):
+        self._ExpireTime = ExpireTime
+
+    @property
+    def CreateTime(self):
+        return self._CreateTime
+
+    @CreateTime.setter
+    def CreateTime(self, CreateTime):
+        self._CreateTime = CreateTime
+
+    @property
+    def Approver(self):
+        return self._Approver
+
+    @Approver.setter
+    def Approver(self, Approver):
+        self._Approver = Approver
+
+    @property
+    def ApprovalStatus(self):
+        return self._ApprovalStatus
+
+    @ApprovalStatus.setter
+    def ApprovalStatus(self, ApprovalStatus):
+        self._ApprovalStatus = ApprovalStatus
+
+    @property
+    def ApprovalStatusDesc(self):
+        return self._ApprovalStatusDesc
+
+    @ApprovalStatusDesc.setter
+    def ApprovalStatusDesc(self, ApprovalStatusDesc):
+        self._ApprovalStatusDesc = ApprovalStatusDesc
+
+    @property
+    def ApprovalTime(self):
+        return self._ApprovalTime
+
+    @ApprovalTime.setter
+    def ApprovalTime(self, ApprovalTime):
+        self._ApprovalTime = ApprovalTime
+
+    @property
+    def TimesTaskTotalCount(self):
+        return self._TimesTaskTotalCount
+
+    @TimesTaskTotalCount.setter
+    def TimesTaskTotalCount(self, TimesTaskTotalCount):
+        self._TimesTaskTotalCount = TimesTaskTotalCount
+
+    @property
+    def TimesTaskSuccessCount(self):
+        return self._TimesTaskSuccessCount
+
+    @TimesTaskSuccessCount.setter
+    def TimesTaskSuccessCount(self, TimesTaskSuccessCount):
+        self._TimesTaskSuccessCount = TimesTaskSuccessCount
+
+    @property
+    def TimesTaskFailCount(self):
+        return self._TimesTaskFailCount
+
+    @TimesTaskFailCount.setter
+    def TimesTaskFailCount(self, TimesTaskFailCount):
+        self._TimesTaskFailCount = TimesTaskFailCount
+
+
+    def _deserialize(self, params):
+        self._OrderId = params.get("OrderId")
+        self._PlatformType = params.get("PlatformType")
+        self._PlatformTypeDesc = params.get("PlatformTypeDesc")
+        self._OrderType = params.get("OrderType")
+        self._OrderTypeDesc = params.get("OrderTypeDesc")
+        self._AppPkgName = params.get("AppPkgName")
+        self._ResourceId = params.get("ResourceId")
+        self._ResourceStatus = params.get("ResourceStatus")
+        self._ResourceStatusDesc = params.get("ResourceStatusDesc")
+        self._TestTimes = params.get("TestTimes")
+        self._ValidTime = params.get("ValidTime")
+        self._ExpireTime = params.get("ExpireTime")
+        self._CreateTime = params.get("CreateTime")
+        self._Approver = params.get("Approver")
+        self._ApprovalStatus = params.get("ApprovalStatus")
+        self._ApprovalStatusDesc = params.get("ApprovalStatusDesc")
+        self._ApprovalTime = params.get("ApprovalTime")
+        self._TimesTaskTotalCount = params.get("TimesTaskTotalCount")
+        self._TimesTaskSuccessCount = params.get("TimesTaskSuccessCount")
+        self._TimesTaskFailCount = params.get("TimesTaskFailCount")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class PlanDetailInfo(AbstractModel):
     """加固策略具体信息
 
     """
 
     def __init__(self):
         r"""
@@ -2982,14 +5527,80 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SDKPlan(AbstractModel):
+    """渠道合作sdk加固策略配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _PlanId: 策略id
+        :type PlanId: int
+        """
+        self._PlanId = None
+
+    @property
+    def PlanId(self):
+        return self._PlanId
+
+    @PlanId.setter
+    def PlanId(self, PlanId):
+        self._PlanId = PlanId
+
+
+    def _deserialize(self, params):
+        self._PlanId = params.get("PlanId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SDKResult(AbstractModel):
+    """渠道合作加固sdk加固结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ResultId: 加固任务结果Id
+        :type ResultId: str
+        """
+        self._ResultId = None
+
+    @property
+    def ResultId(self):
+        return self._ResultId
+
+    @ResultId.setter
+    def ResultId(self, ResultId):
+        self._ResultId = ResultId
+
+
+    def _deserialize(self, params):
+        self._ResultId = params.get("ResultId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ServiceInfo(AbstractModel):
     """提交app加固的服务信息
 
     """
```

### Comparing `tencentcloud-sdk-python-ms-3.0.942/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ms-3.0.943/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ms-3.0.942/PKG-INFO` & `tencentcloud-sdk-python-ms-3.0.943/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ms
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Ms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ms-3.0.942/README.rst` & `tencentcloud-sdk-python-ms-3.0.943/README.rst`

 * *Files identical despite different names*

