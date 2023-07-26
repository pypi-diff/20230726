# Comparing `tmp/tencentcloud-sdk-python-iotvideo-3.0.942.tar.gz` & `tmp/tencentcloud-sdk-python-iotvideo-3.0.943.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iotvideo-3.0.942.tar", last modified: Tue Jul 25 04:20:10 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iotvideo-3.0.943.tar", last modified: Wed Jul 26 00:39:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iotvideo-3.0.942.tar` & `tencentcloud-sdk-python-iotvideo-3.0.943.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20211125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20211125/__init__.py
--rw-r--r--   0 root         (0) root         (0)    87393 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20211125/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)     2198 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20211125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   365162 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20211125/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20201215/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20201215/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72567 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20201215/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20201215/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   303767 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20201215/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20191126/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20191126/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64723 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20191126/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)     3098 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20191126/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   229605 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20191126/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud_sdk_python_iotvideo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud_sdk_python_iotvideo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      861 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:20:10.000000 tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud_sdk_python_iotvideo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20211125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20211125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89241 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20211125/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20211125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   373888 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20211125/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20201215/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20201215/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72567 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20201215/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20201215/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   303767 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20201215/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20191126/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20191126/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64723 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20191126/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20191126/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   229605 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20191126/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud_sdk_python_iotvideo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud_sdk_python_iotvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      861 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud_sdk_python_iotvideo.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.942/setup.py` & `tencentcloud-sdk-python-iotvideo-3.0.943/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20211125/iotvideo_client.py` & `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20211125/iotvideo_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,14 +436,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DeleteCloudStorageEvent(self, request):
+        """删除云存事件
+
+        :param request: Request instance for DeleteCloudStorageEvent.
+        :type request: :class:`tencentcloud.iotvideo.v20211125.models.DeleteCloudStorageEventRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20211125.models.DeleteCloudStorageEventResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteCloudStorageEvent", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteCloudStorageEventResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DeleteDevice(self, request):
         """删除设备
 
         :param request: Request instance for DeleteDevice.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DeleteDeviceRequest`
         :rtype: :class:`tencentcloud.iotvideo.v20211125.models.DeleteDeviceResponse`
 
@@ -1170,14 +1193,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeDevicePackages(self, request):
+        """根据设备信息拉取有效套餐列表
+
+        :param request: Request instance for DescribeDevicePackages.
+        :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeDevicePackagesRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20211125.models.DescribeDevicePackagesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDevicePackages", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDevicePackagesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceStatusLog(self, request):
         """获取设备上下线日志
 
         :param request: Request instance for DescribeDeviceStatusLog.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeDeviceStatusLogRequest`
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20211125/errorcodes.py` & `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20211125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20211125/models.py` & `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20211125/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -3107,14 +3107,132 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DeleteCloudStorageEventRequest(AbstractModel):
+    """DeleteCloudStorageEvent请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProductId: 产品ID
+        :type ProductId: str
+        :param _DeviceName: 设备名称
+        :type DeviceName: str
+        :param _EventId: 事件id
+        :type EventId: str
+        :param _StartTime: 开始时间，unix时间
+        :type StartTime: int
+        :param _EndTime: 结束时间，unix时间
+        :type EndTime: int
+        :param _UserId: 用户ID
+        :type UserId: str
+        """
+        self._ProductId = None
+        self._DeviceName = None
+        self._EventId = None
+        self._StartTime = None
+        self._EndTime = None
+        self._UserId = None
+
+    @property
+    def ProductId(self):
+        return self._ProductId
+
+    @ProductId.setter
+    def ProductId(self, ProductId):
+        self._ProductId = ProductId
+
+    @property
+    def DeviceName(self):
+        return self._DeviceName
+
+    @DeviceName.setter
+    def DeviceName(self, DeviceName):
+        self._DeviceName = DeviceName
+
+    @property
+    def EventId(self):
+        return self._EventId
+
+    @EventId.setter
+    def EventId(self, EventId):
+        self._EventId = EventId
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
+    def UserId(self):
+        return self._UserId
+
+    @UserId.setter
+    def UserId(self, UserId):
+        self._UserId = UserId
+
+
+    def _deserialize(self, params):
+        self._ProductId = params.get("ProductId")
+        self._DeviceName = params.get("DeviceName")
+        self._EventId = params.get("EventId")
+        self._StartTime = params.get("StartTime")
+        self._EndTime = params.get("EndTime")
+        self._UserId = params.get("UserId")
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
+class DeleteCloudStorageEventResponse(AbstractModel):
+    """DeleteCloudStorageEvent返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
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
+        self._RequestId = params.get("RequestId")
+
+
 class DeleteDeviceRequest(AbstractModel):
     """DeleteDevice请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5401,39 +5519,51 @@
 
     """
 
     def __init__(self):
         r"""
         :param _ThumbnailURL: 缩略图访问地址
         :type ThumbnailURL: str
+        :param _ExpireTime: 缩略图访问地址的过期时间
+        :type ExpireTime: int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._ThumbnailURL = None
+        self._ExpireTime = None
         self._RequestId = None
 
     @property
     def ThumbnailURL(self):
         return self._ThumbnailURL
 
     @ThumbnailURL.setter
     def ThumbnailURL(self, ThumbnailURL):
         self._ThumbnailURL = ThumbnailURL
 
     @property
+    def ExpireTime(self):
+        return self._ExpireTime
+
+    @ExpireTime.setter
+    def ExpireTime(self, ExpireTime):
+        self._ExpireTime = ExpireTime
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._ThumbnailURL = params.get("ThumbnailURL")
+        self._ExpireTime = params.get("ExpireTime")
         self._RequestId = params.get("RequestId")
 
 
 class DescribeCloudStorageTimeRequest(AbstractModel):
     """DescribeCloudStorageTime请求参数结构体
 
     """
@@ -6711,14 +6841,138 @@
             for item in params.get("EventHistory"):
                 obj = EventHistoryItem()
                 obj._deserialize(item)
                 self._EventHistory.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class DescribeDevicePackagesRequest(AbstractModel):
+    """DescribeDevicePackages请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProductId: 产品ID
+        :type ProductId: str
+        :param _DeviceName: 设备名称
+        :type DeviceName: str
+        :param _Limit: 分页拉取数量
+        :type Limit: int
+        :param _Offset: 分页拉取偏移
+        :type Offset: int
+        """
+        self._ProductId = None
+        self._DeviceName = None
+        self._Limit = None
+        self._Offset = None
+
+    @property
+    def ProductId(self):
+        return self._ProductId
+
+    @ProductId.setter
+    def ProductId(self, ProductId):
+        self._ProductId = ProductId
+
+    @property
+    def DeviceName(self):
+        return self._DeviceName
+
+    @DeviceName.setter
+    def DeviceName(self, DeviceName):
+        self._DeviceName = DeviceName
+
+    @property
+    def Limit(self):
+        return self._Limit
+
+    @Limit.setter
+    def Limit(self, Limit):
+        self._Limit = Limit
+
+    @property
+    def Offset(self):
+        return self._Offset
+
+    @Offset.setter
+    def Offset(self, Offset):
+        self._Offset = Offset
+
+
+    def _deserialize(self, params):
+        self._ProductId = params.get("ProductId")
+        self._DeviceName = params.get("DeviceName")
+        self._Limit = params.get("Limit")
+        self._Offset = params.get("Offset")
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
+class DescribeDevicePackagesResponse(AbstractModel):
+    """DescribeDevicePackages返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TotalCount: 有效云存套餐数量
+        :type TotalCount: int
+        :param _Packages: 有效云存套餐列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Packages: list of PackageInfo
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TotalCount = None
+        self._Packages = None
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
+    def Packages(self):
+        return self._Packages
+
+    @Packages.setter
+    def Packages(self, Packages):
+        self._Packages = Packages
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
+        if params.get("Packages") is not None:
+            self._Packages = []
+            for item in params.get("Packages"):
+                obj = PackageInfo()
+                obj._deserialize(item)
+                self._Packages.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeDeviceRequest(AbstractModel):
     """DescribeDevice请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -11855,14 +12109,84 @@
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
+class PackageInfo(AbstractModel):
+    """结构体（PackageInfo）记录了设备拥有的有效套餐信息，包括云存开启状态、云存类型、云存回看时长、云存套餐过期时间
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Status: 云存开启状态，0为未开启，2为正在生效，1为已过期
+注：这里只返回状态为0的数据
+        :type Status: int
+        :param _CSType: 云存类型，1为全时云存，2为事件云存
+        :type CSType: int
+        :param _CSShiftDuration: 云存回看时长
+        :type CSShiftDuration: int
+        :param _CSExpiredTime: 云存套餐过期时间
+        :type CSExpiredTime: int
+        """
+        self._Status = None
+        self._CSType = None
+        self._CSShiftDuration = None
+        self._CSExpiredTime = None
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def CSType(self):
+        return self._CSType
+
+    @CSType.setter
+    def CSType(self, CSType):
+        self._CSType = CSType
+
+    @property
+    def CSShiftDuration(self):
+        return self._CSShiftDuration
+
+    @CSShiftDuration.setter
+    def CSShiftDuration(self, CSShiftDuration):
+        self._CSShiftDuration = CSShiftDuration
+
+    @property
+    def CSExpiredTime(self):
+        return self._CSExpiredTime
+
+    @CSExpiredTime.setter
+    def CSExpiredTime(self, CSExpiredTime):
+        self._CSExpiredTime = CSExpiredTime
+
+
+    def _deserialize(self, params):
+        self._Status = params.get("Status")
+        self._CSType = params.get("CSType")
+        self._CSShiftDuration = params.get("CSShiftDuration")
+        self._CSExpiredTime = params.get("CSExpiredTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ProductModelDefinition(AbstractModel):
     """产品模型定义
 
     """
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20201215/iotvideo_client.py` & `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20201215/iotvideo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20201215/errorcodes.py` & `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20201215/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20201215/models.py` & `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20201215/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20191126/iotvideo_client.py` & `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20191126/iotvideo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20191126/errorcodes.py` & `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20191126/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/iotvideo/v20191126/models.py` & `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20191126/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.942/PKG-INFO` & `tencentcloud-sdk-python-iotvideo-3.0.943/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotvideo
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Iotvideo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.942/README.rst` & `tencentcloud-sdk-python-iotvideo-3.0.943/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.942/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotvideo
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Iotvideo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

