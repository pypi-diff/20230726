# Comparing `tmp/tencentcloud-sdk-python-dnspod-3.0.942.tar.gz` & `tmp/tencentcloud-sdk-python-dnspod-3.0.943.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.942.tar", last modified: Tue Jul 25 04:16:48 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.943.tar", last modified: Wed Jul 26 00:36:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dnspod-3.0.942.tar` & `tencentcloud-sdk-python-dnspod-3.0.943.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud/dnspod/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud/dnspod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud/dnspod/v20210323/
--rw-r--r--   0 root         (0) root         (0)    60981 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud/dnspod/v20210323/dnspod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud/dnspod/v20210323/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24039 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud/dnspod/v20210323/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   340184 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud/dnspod/v20210323/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud_sdk_python_dnspod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-25 04:16:48.000000 tencentcloud-sdk-python-dnspod-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:36:11.000000 tencentcloud-sdk-python-dnspod-3.0.943/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-26 00:36:10.000000 tencentcloud-sdk-python-dnspod-3.0.943/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:36:11.000000 tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:36:10.000000 tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:36:11.000000 tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud/dnspod/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:36:10.000000 tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud/dnspod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:36:11.000000 tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud/dnspod/v20210323/
+-rw-r--r--   0 root         (0) root         (0)    61922 2023-07-26 00:36:10.000000 tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud/dnspod/v20210323/dnspod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:36:10.000000 tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud/dnspod/v20210323/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24132 2023-07-26 00:36:10.000000 tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud/dnspod/v20210323/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   351707 2023-07-26 00:36:10.000000 tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud/dnspod/v20210323/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:36:11.000000 tencentcloud-sdk-python-dnspod-3.0.943/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-26 00:36:11.000000 tencentcloud-sdk-python-dnspod-3.0.943/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:36:11.000000 tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud_sdk_python_dnspod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:36:11.000000 tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-26 00:36:11.000000 tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-26 00:36:11.000000 tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:36:11.000000 tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-26 00:36:10.000000 tencentcloud-sdk-python-dnspod-3.0.943/README.rst
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.942/setup.py` & `tencentcloud-sdk-python-dnspod-3.0.943/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud/dnspod/v20210323/dnspod_client.py` & `tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud/dnspod/v20210323/dnspod_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -804,14 +804,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeRecordFilterList(self, request):
+        """获取某个域名下的解析记录列表
+
+        :param request: Request instance for DescribeRecordFilterList.
+        :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeRecordFilterListRequest`
+        :rtype: :class:`tencentcloud.dnspod.v20210323.models.DescribeRecordFilterListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeRecordFilterList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeRecordFilterListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeRecordGroupList(self, request):
         """查询解析记录分组列表
 
         :param request: Request instance for DescribeRecordGroupList.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeRecordGroupListRequest`
         :rtype: :class:`tencentcloud.dnspod.v20210323.models.DescribeRecordGroupListResponse`
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud/dnspod/v20210323/errorcodes.py` & `tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud/dnspod/v20210323/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,14 +508,17 @@
 
 # 该域名使用的套餐不支持隐性URL转发或数量已达上限，如需要使用，请去商城购买。
 LIMITEXCEEDED_HIDDENURLEXCEEDED = 'LimitExceeded.HiddenUrlExceeded'
 
 # NS记录数量超出限制。
 LIMITEXCEEDED_NSCOUNTLIMIT = 'LimitExceeded.NsCountLimit'
 
+# 分页起始数量过大。
+LIMITEXCEEDED_OFFSETEXCEEDED = 'LimitExceeded.OffsetExceeded'
+
 # 记录的TTL值超出了限制。
 LIMITEXCEEDED_RECORDTTLLIMIT = 'LimitExceeded.RecordTtlLimit'
 
 # SRV记录数量超出限制。
 LIMITEXCEEDED_SRVCOUNTLIMIT = 'LimitExceeded.SrvCountLimit'
 
 # 子域名级数超出限制。
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud/dnspod/v20210323/models.py` & `tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud/dnspod/v20210323/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4784,14 +4784,390 @@
 
 
     def _deserialize(self, params):
         self._Exist = params.get("Exist")
         self._RequestId = params.get("RequestId")
 
 
+class DescribeRecordFilterListRequest(AbstractModel):
+    """DescribeRecordFilterList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Domain: 要获取的解析记录所属的域名。
+        :type Domain: str
+        :param _DomainId: 要获取的解析记录所属的域名 Id，如果传了 DomainId，系统将会忽略 Domain 参数。 可以通过接口 DescribeDomainList 查到所有的 Domain 以及 DomainId。
+        :type DomainId: int
+        :param _SubDomain: 根据解析记录的主机头获取解析记录。默认模糊匹配。可以通过设置 IsExactSubdomain 参数为 true 进行精确查找。
+        :type SubDomain: str
+        :param _RecordType: 获取某些类型的解析记录，如 A，CNAME，NS，AAAA，显性URL，隐性URL，CAA，SPF等。
+        :type RecordType: list of str
+        :param _RecordLine: 获取某些线路ID的解析记录。可以通过接口 DescribeRecordLineList 查看当前域名允许的线路信息。
+        :type RecordLine: list of str
+        :param _GroupId: 获取某些分组下的解析记录时，传这个分组 Id。可以通过接口 DescribeRecordGroupList 接口 GroupId 字段获取。
+        :type GroupId: list of int non-negative
+        :param _Keyword: 通过关键字搜索解析记录，当前支持搜索主机头和记录值
+        :type Keyword: str
+        :param _SortField: 排序字段，支持 NAME，LINE，TYPE，VALUE，WEIGHT，MX，TTL，UPDATED_ON 几个字段。
+NAME：解析记录的主机头
+LINE：解析记录线路
+TYPE：解析记录类型
+VALUE：解析记录值
+WEIGHT：权重
+MX：MX 优先级
+TTL：解析记录缓存时间
+UPDATED_ON：解析记录更新时间
+
+        :type SortField: str
+        :param _SortType: 排序方式，升序：ASC，降序：DESC。默认值为ASC。
+        :type SortType: str
+        :param _Offset: 偏移量，默认值为0。
+        :type Offset: int
+        :param _Limit: 限制数量，当前Limit最大支持3000。默认值为100。
+        :type Limit: int
+        :param _RecordValue: 根据解析记录的值获取解析记录
+        :type RecordValue: str
+        :param _RecordStatus: 根据解析记录的状态获取解析记录。可取值为 ENABLE，DISABLE。
+ENABLE：正常 
+DISABLE：暂停 
+        :type RecordStatus: list of str
+        :param _WeightBegin: 要获取解析记录权重查询区间起点。
+        :type WeightBegin: int
+        :param _WeightEnd: 要获取解析记录权重查询区间终点。
+        :type WeightEnd: int
+        :param _MXBegin: 要获取解析记录 MX 优先级查询区间起点。
+        :type MXBegin: int
+        :param _MXEnd: 要获取解析记录 MX 优先级查询区间终点。
+        :type MXEnd: int
+        :param _TTLBegin: 要获取解析记录 TTL 查询区间起点。
+        :type TTLBegin: int
+        :param _TTLEnd: 要获取解析记录 TTL 查询区间终点。
+        :type TTLEnd: int
+        :param _UpdatedAtBegin: 要获取解析记录更新时间查询区间起点。
+        :type UpdatedAtBegin: str
+        :param _UpdatedAtEnd: 要获取解析记录更新时间查询区间终点。
+        :type UpdatedAtEnd: str
+        :param _Remark: 根据解析记录的备注获取解析记录。
+        :type Remark: str
+        :param _IsExactSubDomain: 是否根据 Subdomain 参数进行精确查找。
+        :type IsExactSubDomain: bool
+        :param _ProjectId: 项目ID
+        :type ProjectId: int
+        """
+        self._Domain = None
+        self._DomainId = None
+        self._SubDomain = None
+        self._RecordType = None
+        self._RecordLine = None
+        self._GroupId = None
+        self._Keyword = None
+        self._SortField = None
+        self._SortType = None
+        self._Offset = None
+        self._Limit = None
+        self._RecordValue = None
+        self._RecordStatus = None
+        self._WeightBegin = None
+        self._WeightEnd = None
+        self._MXBegin = None
+        self._MXEnd = None
+        self._TTLBegin = None
+        self._TTLEnd = None
+        self._UpdatedAtBegin = None
+        self._UpdatedAtEnd = None
+        self._Remark = None
+        self._IsExactSubDomain = None
+        self._ProjectId = None
+
+    @property
+    def Domain(self):
+        return self._Domain
+
+    @Domain.setter
+    def Domain(self, Domain):
+        self._Domain = Domain
+
+    @property
+    def DomainId(self):
+        return self._DomainId
+
+    @DomainId.setter
+    def DomainId(self, DomainId):
+        self._DomainId = DomainId
+
+    @property
+    def SubDomain(self):
+        return self._SubDomain
+
+    @SubDomain.setter
+    def SubDomain(self, SubDomain):
+        self._SubDomain = SubDomain
+
+    @property
+    def RecordType(self):
+        return self._RecordType
+
+    @RecordType.setter
+    def RecordType(self, RecordType):
+        self._RecordType = RecordType
+
+    @property
+    def RecordLine(self):
+        return self._RecordLine
+
+    @RecordLine.setter
+    def RecordLine(self, RecordLine):
+        self._RecordLine = RecordLine
+
+    @property
+    def GroupId(self):
+        return self._GroupId
+
+    @GroupId.setter
+    def GroupId(self, GroupId):
+        self._GroupId = GroupId
+
+    @property
+    def Keyword(self):
+        return self._Keyword
+
+    @Keyword.setter
+    def Keyword(self, Keyword):
+        self._Keyword = Keyword
+
+    @property
+    def SortField(self):
+        return self._SortField
+
+    @SortField.setter
+    def SortField(self, SortField):
+        self._SortField = SortField
+
+    @property
+    def SortType(self):
+        return self._SortType
+
+    @SortType.setter
+    def SortType(self, SortType):
+        self._SortType = SortType
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
+    def RecordValue(self):
+        return self._RecordValue
+
+    @RecordValue.setter
+    def RecordValue(self, RecordValue):
+        self._RecordValue = RecordValue
+
+    @property
+    def RecordStatus(self):
+        return self._RecordStatus
+
+    @RecordStatus.setter
+    def RecordStatus(self, RecordStatus):
+        self._RecordStatus = RecordStatus
+
+    @property
+    def WeightBegin(self):
+        return self._WeightBegin
+
+    @WeightBegin.setter
+    def WeightBegin(self, WeightBegin):
+        self._WeightBegin = WeightBegin
+
+    @property
+    def WeightEnd(self):
+        return self._WeightEnd
+
+    @WeightEnd.setter
+    def WeightEnd(self, WeightEnd):
+        self._WeightEnd = WeightEnd
+
+    @property
+    def MXBegin(self):
+        return self._MXBegin
+
+    @MXBegin.setter
+    def MXBegin(self, MXBegin):
+        self._MXBegin = MXBegin
+
+    @property
+    def MXEnd(self):
+        return self._MXEnd
+
+    @MXEnd.setter
+    def MXEnd(self, MXEnd):
+        self._MXEnd = MXEnd
+
+    @property
+    def TTLBegin(self):
+        return self._TTLBegin
+
+    @TTLBegin.setter
+    def TTLBegin(self, TTLBegin):
+        self._TTLBegin = TTLBegin
+
+    @property
+    def TTLEnd(self):
+        return self._TTLEnd
+
+    @TTLEnd.setter
+    def TTLEnd(self, TTLEnd):
+        self._TTLEnd = TTLEnd
+
+    @property
+    def UpdatedAtBegin(self):
+        return self._UpdatedAtBegin
+
+    @UpdatedAtBegin.setter
+    def UpdatedAtBegin(self, UpdatedAtBegin):
+        self._UpdatedAtBegin = UpdatedAtBegin
+
+    @property
+    def UpdatedAtEnd(self):
+        return self._UpdatedAtEnd
+
+    @UpdatedAtEnd.setter
+    def UpdatedAtEnd(self, UpdatedAtEnd):
+        self._UpdatedAtEnd = UpdatedAtEnd
+
+    @property
+    def Remark(self):
+        return self._Remark
+
+    @Remark.setter
+    def Remark(self, Remark):
+        self._Remark = Remark
+
+    @property
+    def IsExactSubDomain(self):
+        return self._IsExactSubDomain
+
+    @IsExactSubDomain.setter
+    def IsExactSubDomain(self, IsExactSubDomain):
+        self._IsExactSubDomain = IsExactSubDomain
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+
+    def _deserialize(self, params):
+        self._Domain = params.get("Domain")
+        self._DomainId = params.get("DomainId")
+        self._SubDomain = params.get("SubDomain")
+        self._RecordType = params.get("RecordType")
+        self._RecordLine = params.get("RecordLine")
+        self._GroupId = params.get("GroupId")
+        self._Keyword = params.get("Keyword")
+        self._SortField = params.get("SortField")
+        self._SortType = params.get("SortType")
+        self._Offset = params.get("Offset")
+        self._Limit = params.get("Limit")
+        self._RecordValue = params.get("RecordValue")
+        self._RecordStatus = params.get("RecordStatus")
+        self._WeightBegin = params.get("WeightBegin")
+        self._WeightEnd = params.get("WeightEnd")
+        self._MXBegin = params.get("MXBegin")
+        self._MXEnd = params.get("MXEnd")
+        self._TTLBegin = params.get("TTLBegin")
+        self._TTLEnd = params.get("TTLEnd")
+        self._UpdatedAtBegin = params.get("UpdatedAtBegin")
+        self._UpdatedAtEnd = params.get("UpdatedAtEnd")
+        self._Remark = params.get("Remark")
+        self._IsExactSubDomain = params.get("IsExactSubDomain")
+        self._ProjectId = params.get("ProjectId")
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
+class DescribeRecordFilterListResponse(AbstractModel):
+    """DescribeRecordFilterList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RecordCountInfo: 记录的数量统计信息
+        :type RecordCountInfo: :class:`tencentcloud.dnspod.v20210323.models.RecordCountInfo`
+        :param _RecordList: 获取的记录列表
+        :type RecordList: list of RecordListItem
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RecordCountInfo = None
+        self._RecordList = None
+        self._RequestId = None
+
+    @property
+    def RecordCountInfo(self):
+        return self._RecordCountInfo
+
+    @RecordCountInfo.setter
+    def RecordCountInfo(self, RecordCountInfo):
+        self._RecordCountInfo = RecordCountInfo
+
+    @property
+    def RecordList(self):
+        return self._RecordList
+
+    @RecordList.setter
+    def RecordList(self, RecordList):
+        self._RecordList = RecordList
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
+        if params.get("RecordCountInfo") is not None:
+            self._RecordCountInfo = RecordCountInfo()
+            self._RecordCountInfo._deserialize(params.get("RecordCountInfo"))
+        if params.get("RecordList") is not None:
+            self._RecordList = []
+            for item in params.get("RecordList"):
+                obj = RecordListItem()
+                obj._deserialize(item)
+                self._RecordList.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeRecordGroupListRequest(AbstractModel):
     """DescribeRecordGroupList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.942/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.943/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.942/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.943/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.942/README.rst` & `tencentcloud-sdk-python-dnspod-3.0.943/README.rst`

 * *Files identical despite different names*

