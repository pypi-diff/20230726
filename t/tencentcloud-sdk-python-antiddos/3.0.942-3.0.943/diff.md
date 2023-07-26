# Comparing `tmp/tencentcloud-sdk-python-antiddos-3.0.942.tar.gz` & `tmp/tencentcloud-sdk-python-antiddos-3.0.943.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-antiddos-3.0.942.tar", last modified: Tue Jul 25 04:10:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-antiddos-3.0.943.tar", last modified: Wed Jul 26 00:16:56 2023, max compression
```

## Comparing `tencentcloud-sdk-python-antiddos-3.0.942.tar` & `tencentcloud-sdk-python-antiddos-3.0.943.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud/antiddos/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud/antiddos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud/antiddos/v20200309/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud/antiddos/v20200309/__init__.py
--rw-r--r--   0 root         (0) root         (0)    88539 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud/antiddos/v20200309/antiddos_client.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud/antiddos/v20200309/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   502349 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud/antiddos/v20200309/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud_sdk_python_antiddos.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud_sdk_python_antiddos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud_sdk_python_antiddos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud_sdk_python_antiddos.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-25 04:10:24.000000 tencentcloud-sdk-python-antiddos-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud/antiddos/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud/antiddos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud/antiddos/v20200309/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud/antiddos/v20200309/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89474 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud/antiddos/v20200309/antiddos_client.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud/antiddos/v20200309/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   506474 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud/antiddos/v20200309/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud_sdk_python_antiddos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud_sdk_python_antiddos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud_sdk_python_antiddos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud_sdk_python_antiddos.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-26 00:16:56.000000 tencentcloud-sdk-python-antiddos-3.0.943/README.rst
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.942/setup.py` & `tencentcloud-sdk-python-antiddos-3.0.943/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud/__init__.py` & `tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud/antiddos/v20200309/antiddos_client.py` & `tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud/antiddos/v20200309/antiddos_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -942,14 +942,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeBizMonitorTrend(self, request):
+        """获取高防IP业务监控流量曲线
+
+        :param request: Request instance for DescribeBizMonitorTrend.
+        :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeBizMonitorTrendRequest`
+        :rtype: :class:`tencentcloud.antiddos.v20200309.models.DescribeBizMonitorTrendResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeBizMonitorTrend", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeBizMonitorTrendResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeBizTrend(self, request):
         """获取业务流量曲线
 
         :param request: Request instance for DescribeBizTrend.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeBizTrendRequest`
         :rtype: :class:`tencentcloud.antiddos.v20200309.models.DescribeBizTrendResponse`
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud/antiddos/v20200309/errorcodes.py` & `tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud/antiddos/v20200309/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud/antiddos/v20200309/models.py` & `tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud/antiddos/v20200309/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6664,14 +6664,169 @@
     def _deserialize(self, params):
         if params.get("HttpStatusMap") is not None:
             self._HttpStatusMap = HttpStatusMap()
             self._HttpStatusMap._deserialize(params.get("HttpStatusMap"))
         self._RequestId = params.get("RequestId")
 
 
+class DescribeBizMonitorTrendRequest(AbstractModel):
+    """DescribeBizMonitorTrend请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Business: 大禹子产品代号（bgpip表示高防IP）
+        :type Business: str
+        :param _StartTime: 统计开始时间。 例：“2020-09-22 00:00:00”
+        :type StartTime: str
+        :param _EndTime: 统计结束时间。 例：“2020-09-22 00:00:00”
+        :type EndTime: str
+        :param _Id: 资源实例ID
+        :type Id: str
+        :param _MetricName: 统计纬度，可取值intraffic outtraffic inpkg outpkg
+        :type MetricName: str
+        :param _Period: 时间粒度 60 300 3600 21600 86400
+        :type Period: int
+        """
+        self._Business = None
+        self._StartTime = None
+        self._EndTime = None
+        self._Id = None
+        self._MetricName = None
+        self._Period = None
+
+    @property
+    def Business(self):
+        return self._Business
+
+    @Business.setter
+    def Business(self, Business):
+        self._Business = Business
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
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def MetricName(self):
+        return self._MetricName
+
+    @MetricName.setter
+    def MetricName(self, MetricName):
+        self._MetricName = MetricName
+
+    @property
+    def Period(self):
+        return self._Period
+
+    @Period.setter
+    def Period(self, Period):
+        self._Period = Period
+
+
+    def _deserialize(self, params):
+        self._Business = params.get("Business")
+        self._StartTime = params.get("StartTime")
+        self._EndTime = params.get("EndTime")
+        self._Id = params.get("Id")
+        self._MetricName = params.get("MetricName")
+        self._Period = params.get("Period")
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
+class DescribeBizMonitorTrendResponse(AbstractModel):
+    """DescribeBizMonitorTrend返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DataList: 曲线图各个时间点的值
+        :type DataList: list of float
+        :param _MetricName: 统计纬度
+        :type MetricName: str
+        :param _MaxData: 返回DataList中的最大值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MaxData: int
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._DataList = None
+        self._MetricName = None
+        self._MaxData = None
+        self._RequestId = None
+
+    @property
+    def DataList(self):
+        return self._DataList
+
+    @DataList.setter
+    def DataList(self, DataList):
+        self._DataList = DataList
+
+    @property
+    def MetricName(self):
+        return self._MetricName
+
+    @MetricName.setter
+    def MetricName(self, MetricName):
+        self._MetricName = MetricName
+
+    @property
+    def MaxData(self):
+        return self._MaxData
+
+    @MaxData.setter
+    def MaxData(self, MaxData):
+        self._MaxData = MaxData
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
+        self._DataList = params.get("DataList")
+        self._MetricName = params.get("MetricName")
+        self._MaxData = params.get("MaxData")
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeBizTrendRequest(AbstractModel):
     """DescribeBizTrend请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.942/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO` & `tencentcloud-sdk-python-antiddos-3.0.943/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-antiddos
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Antiddos SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.942/PKG-INFO` & `tencentcloud-sdk-python-antiddos-3.0.943/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-antiddos
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Antiddos SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.942/README.rst` & `tencentcloud-sdk-python-antiddos-3.0.943/README.rst`

 * *Files identical despite different names*

