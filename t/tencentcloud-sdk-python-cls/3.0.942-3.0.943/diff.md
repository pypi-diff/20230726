# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.942.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.943.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.942.tar", last modified: Tue Jul 25 04:14:46 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.943.tar", last modified: Wed Jul 26 00:34:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.942.tar` & `tencentcloud-sdk-python-cls-3.0.943.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)    78273 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9048 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   468714 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/tencentcloud/cls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:14:46.000000 tencentcloud-sdk-python-cls-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)    81003 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9048 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   486508 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/tencentcloud/cls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-26 00:34:21.000000 tencentcloud-sdk-python-cls-3.0.943/README.rst
```

### Comparing `tencentcloud-sdk-python-cls-3.0.942/setup.py` & `tencentcloud-sdk-python-cls-3.0.943/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.942/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.943/tencentcloud/cls/v20201016/cls_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -758,14 +758,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DeleteScheduledSql(self, request):
+        """本接口用于删除ScheduledSql任务
+
+        :param request: Request instance for DeleteScheduledSql.
+        :type request: :class:`tencentcloud.cls.v20201016.models.DeleteScheduledSqlRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.DeleteScheduledSqlResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteScheduledSql", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteScheduledSqlResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DeleteShipper(self, request):
         """删除投递COS任务
 
         :param request: Request instance for DeleteShipper.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteShipperRequest`
         :rtype: :class:`tencentcloud.cls.v20201016.models.DeleteShipperResponse`
 
@@ -1241,14 +1264,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeScheduledSqlInfo(self, request):
+        """本接口用于获取ScheduledSql任务列表
+
+        :param request: Request instance for DescribeScheduledSqlInfo.
+        :type request: :class:`tencentcloud.cls.v20201016.models.DescribeScheduledSqlInfoRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.DescribeScheduledSqlInfoResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeScheduledSqlInfo", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeScheduledSqlInfoResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeShipperTasks(self, request):
         """获取投递任务列表
 
         :param request: Request instance for DescribeShipperTasks.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeShipperTasksRequest`
         :rtype: :class:`tencentcloud.cls.v20201016.models.DescribeShipperTasksResponse`
 
@@ -1607,14 +1653,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def ModifyScheduledSql(self, request):
+        """本接口用于修改ScheduledSql任务
+
+        :param request: Request instance for ModifyScheduledSql.
+        :type request: :class:`tencentcloud.cls.v20201016.models.ModifyScheduledSqlRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.ModifyScheduledSqlResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyScheduledSql", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyScheduledSqlResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyShipper(self, request):
         """修改现有的投递规则，客户如果使用此接口，需要自行处理CLS对指定bucket的写权限。
 
         :param request: Request instance for ModifyShipper.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyShipperRequest`
```

### Comparing `tencentcloud-sdk-python-cls-3.0.942/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.943/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.942/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.943/tencentcloud/cls/v20201016/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4541,25 +4541,25 @@
         r"""
         :param _SrcTopicId: 源日志主题
         :type SrcTopicId: str
         :param _Name: 任务名称
         :type Name: str
         :param _EnableFlag: 任务启动状态.  1正常开启,  2关闭
         :type EnableFlag: int
-        :param _DstResource: 加工任务目的topic_id以及别名
+        :param _DstResource: 定时SQL分析目标日志主题
         :type DstResource: :class:`tencentcloud.cls.v20201016.models.ScheduledSqlResouceInfo`
-        :param _ScheduledSqlContent: ScheduledSQL语句
+        :param _ScheduledSqlContent: 查询语句
         :type ScheduledSqlContent: str
         :param _ProcessStartTime: 调度开始时间,Unix时间戳，单位ms
         :type ProcessStartTime: int
         :param _ProcessType: 调度类型，1:持续运行 2:指定调度结束时间
         :type ProcessType: int
         :param _ProcessPeriod: 调度周期(分钟)
         :type ProcessPeriod: int
-        :param _ProcessTimeWindow: 调度时间窗口
+        :param _ProcessTimeWindow: 单次查询的时间窗口
         :type ProcessTimeWindow: str
         :param _ProcessDelay: 执行延迟(秒)
         :type ProcessDelay: int
         :param _SrcTopicRegion: 源topicId的地域信息
         :type SrcTopicRegion: str
         :param _ProcessEndTime: 调度结束时间，当ProcessType=2时为必传字段, Unix时间戳，单位ms
         :type ProcessEndTime: int
@@ -6265,14 +6265,84 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class DeleteScheduledSqlRequest(AbstractModel):
+    """DeleteScheduledSql请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskId: 任务ID
+        :type TaskId: str
+        :param _SrcTopicId: 源日志主题ID
+        :type SrcTopicId: str
+        """
+        self._TaskId = None
+        self._SrcTopicId = None
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+    @property
+    def SrcTopicId(self):
+        return self._SrcTopicId
+
+    @SrcTopicId.setter
+    def SrcTopicId(self, SrcTopicId):
+        self._SrcTopicId = SrcTopicId
+
+
+    def _deserialize(self, params):
+        self._TaskId = params.get("TaskId")
+        self._SrcTopicId = params.get("SrcTopicId")
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
+class DeleteScheduledSqlResponse(AbstractModel):
+    """DeleteScheduledSql返回参数结构体
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
 class DeleteShipperRequest(AbstractModel):
     """DeleteShipper请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8748,14 +8818,137 @@
             for item in params.get("Partitions"):
                 obj = PartitionInfo()
                 obj._deserialize(item)
                 self._Partitions.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class DescribeScheduledSqlInfoRequest(AbstractModel):
+    """DescribeScheduledSqlInfo请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Offset: 分页的偏移量，默认值为0。
+        :type Offset: int
+        :param _Limit: 分页单页限制数目，默认值为20，最大值100。
+        :type Limit: int
+        :param _Name: 任务名称
+        :type Name: str
+        :param _TaskId: 任务id
+        :type TaskId: str
+        """
+        self._Offset = None
+        self._Limit = None
+        self._Name = None
+        self._TaskId = None
+
+    @property
+    def Offset(self):
+        return self._Offset
+
+    @Offset.setter
+    def Offset(self, Offset):
+        self._Offset = Offset
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
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+
+    def _deserialize(self, params):
+        self._Offset = params.get("Offset")
+        self._Limit = params.get("Limit")
+        self._Name = params.get("Name")
+        self._TaskId = params.get("TaskId")
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
+class DescribeScheduledSqlInfoResponse(AbstractModel):
+    """DescribeScheduledSqlInfo返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ScheduledSqlTaskInfos: ScheduledSQL任务列表信息
+        :type ScheduledSqlTaskInfos: list of ScheduledSqlTaskInfo
+        :param _TotalCount: 任务总次数
+        :type TotalCount: int
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._ScheduledSqlTaskInfos = None
+        self._TotalCount = None
+        self._RequestId = None
+
+    @property
+    def ScheduledSqlTaskInfos(self):
+        return self._ScheduledSqlTaskInfos
+
+    @ScheduledSqlTaskInfos.setter
+    def ScheduledSqlTaskInfos(self, ScheduledSqlTaskInfos):
+        self._ScheduledSqlTaskInfos = ScheduledSqlTaskInfos
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
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("ScheduledSqlTaskInfos") is not None:
+            self._ScheduledSqlTaskInfos = []
+            for item in params.get("ScheduledSqlTaskInfos"):
+                obj = ScheduledSqlTaskInfo()
+                obj._deserialize(item)
+                self._ScheduledSqlTaskInfos.append(obj)
+        self._TotalCount = params.get("TotalCount")
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeShipperTasksRequest(AbstractModel):
     """DescribeShipperTasks请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -13493,14 +13686,194 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class ModifyScheduledSqlRequest(AbstractModel):
+    """ModifyScheduledSql请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskId: 任务ID
+        :type TaskId: str
+        :param _SrcTopicId: 源日志主题
+        :type SrcTopicId: str
+        :param _EnableFlag: 任务启动状态.   1正常开启,  2关闭
+        :type EnableFlag: int
+        :param _DstResource: 定时SQL分析的目标日志主题
+        :type DstResource: :class:`tencentcloud.cls.v20201016.models.ScheduledSqlResouceInfo`
+        :param _ScheduledSqlContent: 查询语句
+        :type ScheduledSqlContent: str
+        :param _ProcessPeriod: 调度周期(分钟)
+        :type ProcessPeriod: int
+        :param _ProcessTimeWindow: 单次查询的时间窗口. 例子中为近15分钟
+        :type ProcessTimeWindow: str
+        :param _ProcessDelay: 执行延迟(秒)
+        :type ProcessDelay: int
+        :param _SrcTopicRegion: 源topicId的地域信息
+        :type SrcTopicRegion: str
+        :param _Name: 任务名称
+        :type Name: str
+        :param _SyntaxRule: 语法规则。 默认值为0。 0：Lucene语法，1：CQL语法
+        :type SyntaxRule: int
+        """
+        self._TaskId = None
+        self._SrcTopicId = None
+        self._EnableFlag = None
+        self._DstResource = None
+        self._ScheduledSqlContent = None
+        self._ProcessPeriod = None
+        self._ProcessTimeWindow = None
+        self._ProcessDelay = None
+        self._SrcTopicRegion = None
+        self._Name = None
+        self._SyntaxRule = None
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+    @property
+    def SrcTopicId(self):
+        return self._SrcTopicId
+
+    @SrcTopicId.setter
+    def SrcTopicId(self, SrcTopicId):
+        self._SrcTopicId = SrcTopicId
+
+    @property
+    def EnableFlag(self):
+        return self._EnableFlag
+
+    @EnableFlag.setter
+    def EnableFlag(self, EnableFlag):
+        self._EnableFlag = EnableFlag
+
+    @property
+    def DstResource(self):
+        return self._DstResource
+
+    @DstResource.setter
+    def DstResource(self, DstResource):
+        self._DstResource = DstResource
+
+    @property
+    def ScheduledSqlContent(self):
+        return self._ScheduledSqlContent
+
+    @ScheduledSqlContent.setter
+    def ScheduledSqlContent(self, ScheduledSqlContent):
+        self._ScheduledSqlContent = ScheduledSqlContent
+
+    @property
+    def ProcessPeriod(self):
+        return self._ProcessPeriod
+
+    @ProcessPeriod.setter
+    def ProcessPeriod(self, ProcessPeriod):
+        self._ProcessPeriod = ProcessPeriod
+
+    @property
+    def ProcessTimeWindow(self):
+        return self._ProcessTimeWindow
+
+    @ProcessTimeWindow.setter
+    def ProcessTimeWindow(self, ProcessTimeWindow):
+        self._ProcessTimeWindow = ProcessTimeWindow
+
+    @property
+    def ProcessDelay(self):
+        return self._ProcessDelay
+
+    @ProcessDelay.setter
+    def ProcessDelay(self, ProcessDelay):
+        self._ProcessDelay = ProcessDelay
+
+    @property
+    def SrcTopicRegion(self):
+        return self._SrcTopicRegion
+
+    @SrcTopicRegion.setter
+    def SrcTopicRegion(self, SrcTopicRegion):
+        self._SrcTopicRegion = SrcTopicRegion
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def SyntaxRule(self):
+        return self._SyntaxRule
+
+    @SyntaxRule.setter
+    def SyntaxRule(self, SyntaxRule):
+        self._SyntaxRule = SyntaxRule
+
+
+    def _deserialize(self, params):
+        self._TaskId = params.get("TaskId")
+        self._SrcTopicId = params.get("SrcTopicId")
+        self._EnableFlag = params.get("EnableFlag")
+        if params.get("DstResource") is not None:
+            self._DstResource = ScheduledSqlResouceInfo()
+            self._DstResource._deserialize(params.get("DstResource"))
+        self._ScheduledSqlContent = params.get("ScheduledSqlContent")
+        self._ProcessPeriod = params.get("ProcessPeriod")
+        self._ProcessTimeWindow = params.get("ProcessTimeWindow")
+        self._ProcessDelay = params.get("ProcessDelay")
+        self._SrcTopicRegion = params.get("SrcTopicRegion")
+        self._Name = params.get("Name")
+        self._SyntaxRule = params.get("SyntaxRule")
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
+class ModifyScheduledSqlResponse(AbstractModel):
+    """ModifyScheduledSql返回参数结构体
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
 class ModifyShipperRequest(AbstractModel):
     """ModifyShipper请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -14926,14 +15299,256 @@
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
+class ScheduledSqlTaskInfo(AbstractModel):
+    """ScheduledSql任务详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskId: ScheduledSql任务id
+        :type TaskId: str
+        :param _Name: ScheduledSql任务名称
+        :type Name: str
+        :param _SrcTopicId: 源日志主题id
+        :type SrcTopicId: str
+        :param _SrcTopicName: 源日志主题名称
+        :type SrcTopicName: str
+        :param _DstResource: 定时SQL分析目标主题
+        :type DstResource: :class:`tencentcloud.cls.v20201016.models.ScheduledSqlResouceInfo`
+        :param _CreateTime: 任务创建时间
+        :type CreateTime: str
+        :param _UpdateTime: 任务更新时间
+        :type UpdateTime: str
+        :param _Status: 任务状态，1:运行 2:停止 3:异常-找不到源日志主题 4:异常-找不到目标主题
+
+5: 访问权限问题 6:内部故障 7:其他故障
+        :type Status: int
+        :param _EnableFlag: 任务启用状态，1开启,  2关闭
+        :type EnableFlag: int
+        :param _ScheduledSqlContent: 查询语句
+        :type ScheduledSqlContent: str
+        :param _ProcessStartTime: 调度开始时间
+        :type ProcessStartTime: str
+        :param _ProcessType: 调度类型，1:持续运行 2:指定调度结束时间
+        :type ProcessType: int
+        :param _ProcessEndTime: 调度结束时间，当process_type=2时为必传字段
+        :type ProcessEndTime: str
+        :param _ProcessPeriod: 调度周期(分钟)
+        :type ProcessPeriod: int
+        :param _ProcessTimeWindow: 查询的时间窗口. @m-15m, @m，意为近15分钟
+        :type ProcessTimeWindow: str
+        :param _ProcessDelay: 执行延迟(秒)
+        :type ProcessDelay: int
+        :param _SrcTopicRegion: 源topicId的地域信息
+        :type SrcTopicRegion: str
+        :param _SyntaxRule: 语法规则，0：Lucene语法，1：CQL语法
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SyntaxRule: int
+        """
+        self._TaskId = None
+        self._Name = None
+        self._SrcTopicId = None
+        self._SrcTopicName = None
+        self._DstResource = None
+        self._CreateTime = None
+        self._UpdateTime = None
+        self._Status = None
+        self._EnableFlag = None
+        self._ScheduledSqlContent = None
+        self._ProcessStartTime = None
+        self._ProcessType = None
+        self._ProcessEndTime = None
+        self._ProcessPeriod = None
+        self._ProcessTimeWindow = None
+        self._ProcessDelay = None
+        self._SrcTopicRegion = None
+        self._SyntaxRule = None
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def SrcTopicId(self):
+        return self._SrcTopicId
+
+    @SrcTopicId.setter
+    def SrcTopicId(self, SrcTopicId):
+        self._SrcTopicId = SrcTopicId
+
+    @property
+    def SrcTopicName(self):
+        return self._SrcTopicName
+
+    @SrcTopicName.setter
+    def SrcTopicName(self, SrcTopicName):
+        self._SrcTopicName = SrcTopicName
+
+    @property
+    def DstResource(self):
+        return self._DstResource
+
+    @DstResource.setter
+    def DstResource(self, DstResource):
+        self._DstResource = DstResource
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
+    def UpdateTime(self):
+        return self._UpdateTime
+
+    @UpdateTime.setter
+    def UpdateTime(self, UpdateTime):
+        self._UpdateTime = UpdateTime
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
+    def EnableFlag(self):
+        return self._EnableFlag
+
+    @EnableFlag.setter
+    def EnableFlag(self, EnableFlag):
+        self._EnableFlag = EnableFlag
+
+    @property
+    def ScheduledSqlContent(self):
+        return self._ScheduledSqlContent
+
+    @ScheduledSqlContent.setter
+    def ScheduledSqlContent(self, ScheduledSqlContent):
+        self._ScheduledSqlContent = ScheduledSqlContent
+
+    @property
+    def ProcessStartTime(self):
+        return self._ProcessStartTime
+
+    @ProcessStartTime.setter
+    def ProcessStartTime(self, ProcessStartTime):
+        self._ProcessStartTime = ProcessStartTime
+
+    @property
+    def ProcessType(self):
+        return self._ProcessType
+
+    @ProcessType.setter
+    def ProcessType(self, ProcessType):
+        self._ProcessType = ProcessType
+
+    @property
+    def ProcessEndTime(self):
+        return self._ProcessEndTime
+
+    @ProcessEndTime.setter
+    def ProcessEndTime(self, ProcessEndTime):
+        self._ProcessEndTime = ProcessEndTime
+
+    @property
+    def ProcessPeriod(self):
+        return self._ProcessPeriod
+
+    @ProcessPeriod.setter
+    def ProcessPeriod(self, ProcessPeriod):
+        self._ProcessPeriod = ProcessPeriod
+
+    @property
+    def ProcessTimeWindow(self):
+        return self._ProcessTimeWindow
+
+    @ProcessTimeWindow.setter
+    def ProcessTimeWindow(self, ProcessTimeWindow):
+        self._ProcessTimeWindow = ProcessTimeWindow
+
+    @property
+    def ProcessDelay(self):
+        return self._ProcessDelay
+
+    @ProcessDelay.setter
+    def ProcessDelay(self, ProcessDelay):
+        self._ProcessDelay = ProcessDelay
+
+    @property
+    def SrcTopicRegion(self):
+        return self._SrcTopicRegion
+
+    @SrcTopicRegion.setter
+    def SrcTopicRegion(self, SrcTopicRegion):
+        self._SrcTopicRegion = SrcTopicRegion
+
+    @property
+    def SyntaxRule(self):
+        return self._SyntaxRule
+
+    @SyntaxRule.setter
+    def SyntaxRule(self, SyntaxRule):
+        self._SyntaxRule = SyntaxRule
+
+
+    def _deserialize(self, params):
+        self._TaskId = params.get("TaskId")
+        self._Name = params.get("Name")
+        self._SrcTopicId = params.get("SrcTopicId")
+        self._SrcTopicName = params.get("SrcTopicName")
+        if params.get("DstResource") is not None:
+            self._DstResource = ScheduledSqlResouceInfo()
+            self._DstResource._deserialize(params.get("DstResource"))
+        self._CreateTime = params.get("CreateTime")
+        self._UpdateTime = params.get("UpdateTime")
+        self._Status = params.get("Status")
+        self._EnableFlag = params.get("EnableFlag")
+        self._ScheduledSqlContent = params.get("ScheduledSqlContent")
+        self._ProcessStartTime = params.get("ProcessStartTime")
+        self._ProcessType = params.get("ProcessType")
+        self._ProcessEndTime = params.get("ProcessEndTime")
+        self._ProcessPeriod = params.get("ProcessPeriod")
+        self._ProcessTimeWindow = params.get("ProcessTimeWindow")
+        self._ProcessDelay = params.get("ProcessDelay")
+        self._SrcTopicRegion = params.get("SrcTopicRegion")
+        self._SyntaxRule = params.get("SyntaxRule")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class SearchLogRequest(AbstractModel):
     """SearchLog请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-cls-3.0.942/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.943/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.942/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.943/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.942/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.943/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.942/README.rst` & `tencentcloud-sdk-python-cls-3.0.943/README.rst`

 * *Files identical despite different names*

