# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.942.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.943.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.942.tar", last modified: Tue Jul 25 04:26:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.943.tar", last modified: Wed Jul 26 00:45:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.942.tar` & `tencentcloud-sdk-python-tdmq-3.0.943.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94553 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)    10019 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   591001 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-25 04:26:51.000000 tencentcloud-sdk-python-tdmq-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94553 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)    10019 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   591304 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-26 00:45:40.000000 tencentcloud-sdk-python-tdmq-3.0.943/README.rst
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.942/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.943/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud/tdmq/v20200217/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -14963,14 +14963,17 @@
         :param _CreateTime: 创建时间，毫秒为单位
         :type CreateTime: int
         :param _Remark: 集群说明信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type Remark: str
         :param _Vpcs: VPC及网络信息
         :type Vpcs: list of VpcEndpointInfo
+        :param _ZoneIds: 可用区信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ZoneIds: list of int
         :param _VirtualHostNumber: 虚拟主机数量
         :type VirtualHostNumber: int
         :param _QueueNumber: 队列数量
         :type QueueNumber: int
         :param _MessagePublishRate: 每秒生产消息数 单位：条/秒
         :type MessagePublishRate: float
         :param _MessageStackNumber: 堆积消息数 单位：条
@@ -14985,23 +14988,23 @@
         :type ConsumerNumber: int
         :param _ExchangeNumber: Exchang数量
         :type ExchangeNumber: int
         :param _ExceptionInformation: 集群异常。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ExceptionInformation: str
         :param _ClusterStatus: 实例状态，0表示创建中，1表示正常，2表示隔离中，3表示已销毁，4 - 异常, 5 - 发货失败
-注意：此字段可能返回 null，表示取不到有效值。
         :type ClusterStatus: int
         """
         self._ClusterId = None
         self._ClusterName = None
         self._Region = None
         self._CreateTime = None
         self._Remark = None
         self._Vpcs = None
+        self._ZoneIds = None
         self._VirtualHostNumber = None
         self._QueueNumber = None
         self._MessagePublishRate = None
         self._MessageStackNumber = None
         self._ExpireTime = None
         self._ChannelNumber = None
         self._ConnectionNumber = None
@@ -15055,14 +15058,22 @@
         return self._Vpcs
 
     @Vpcs.setter
     def Vpcs(self, Vpcs):
         self._Vpcs = Vpcs
 
     @property
+    def ZoneIds(self):
+        return self._ZoneIds
+
+    @ZoneIds.setter
+    def ZoneIds(self, ZoneIds):
+        self._ZoneIds = ZoneIds
+
+    @property
     def VirtualHostNumber(self):
         return self._VirtualHostNumber
 
     @VirtualHostNumber.setter
     def VirtualHostNumber(self, VirtualHostNumber):
         self._VirtualHostNumber = VirtualHostNumber
 
@@ -15155,14 +15166,15 @@
         self._Remark = params.get("Remark")
         if params.get("Vpcs") is not None:
             self._Vpcs = []
             for item in params.get("Vpcs"):
                 obj = VpcEndpointInfo()
                 obj._deserialize(item)
                 self._Vpcs.append(obj)
+        self._ZoneIds = params.get("ZoneIds")
         self._VirtualHostNumber = params.get("VirtualHostNumber")
         self._QueueNumber = params.get("QueueNumber")
         self._MessagePublishRate = params.get("MessagePublishRate")
         self._MessageStackNumber = params.get("MessageStackNumber")
         self._ExpireTime = params.get("ExpireTime")
         self._ChannelNumber = params.get("ChannelNumber")
         self._ConnectionNumber = params.get("ConnectionNumber")
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.942/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.943/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdmq-3.0.942/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.943/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.942/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.943/README.rst`

 * *Files identical despite different names*

