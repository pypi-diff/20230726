# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.942.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.943.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.942.tar", last modified: Tue Jul 25 04:22:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.943.tar", last modified: Wed Jul 26 00:41:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.942.tar` & `tencentcloud-sdk-python-ocr-3.0.943.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/tencentcloud/ocr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/tencentcloud/ocr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5894 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   115781 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)   817590 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/tencentcloud/ocr/v20181119/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-25 04:22:32.000000 tencentcloud-sdk-python-ocr-3.0.942/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   115946 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)   820213 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/v20181119/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/README.rst
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.942/setup.py` & `tencentcloud-sdk-python-ocr-3.0.943/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.942/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.942/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.942/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -837,15 +837,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetTaskState(self, request):
-        """支持查询智能表单录入任务的状态。本产品免费公测中，您可以点击demo（超连接：https://ocr.smartform.cloud.tencent.com/）试用，如需购买请与商务团队联系。
+        """支持查询智能表单录入任务的状态。本产品免费公测中，您可以点击demo（超链接：https://ocr.smartform.cloud.tencent.com/）试用，如需购买请与商务团队联系。
 
         :param request: Request instance for GetTaskState.
         :type request: :class:`tencentcloud.ocr.v20181119.models.GetTaskStateRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.GetTaskStateResponse`
 
         """
         try:
@@ -1476,14 +1476,19 @@
                 </tr>
                 <tr>
                   <td> VatElectronicInvoiceToll</td>
                   <td> 增值税电子普通发票(通行费)</td>
                   <td> 3 </td>
                 </tr>
                 <tr>
+                  <td> VatSalesList</td>
+                  <td> 增值税销货清单</td>
+                  <td> 3 </td>
+                </tr>
+                <tr>
                   <td> VatElectronicSpecialInvoiceFull</td>
                   <td> 电子发票(专用发票)</td>
                   <td> 16 </td>
                 </tr>
                 <tr>
                   <td> VatElectronicInvoiceFull</td>
                   <td> 电子发票(普通发票) </td>
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.942/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/v20181119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10686,19 +10686,22 @@
         :type Title: str
         :param _Total: 金额
         :type Total: str
         :param _OtherInvoiceListItems: 列表
         :type OtherInvoiceListItems: list of OtherInvoiceItem
         :param _OtherInvoiceTableItems: 表格
         :type OtherInvoiceTableItems: list of OtherInvoiceList
+        :param _Date: 发票日期
+        :type Date: str
         """
         self._Title = None
         self._Total = None
         self._OtherInvoiceListItems = None
         self._OtherInvoiceTableItems = None
+        self._Date = None
 
     @property
     def Title(self):
         return self._Title
 
     @Title.setter
     def Title(self, Title):
@@ -10724,14 +10727,22 @@
     def OtherInvoiceTableItems(self):
         return self._OtherInvoiceTableItems
 
     @OtherInvoiceTableItems.setter
     def OtherInvoiceTableItems(self, OtherInvoiceTableItems):
         self._OtherInvoiceTableItems = OtherInvoiceTableItems
 
+    @property
+    def Date(self):
+        return self._Date
+
+    @Date.setter
+    def Date(self, Date):
+        self._Date = Date
+
 
     def _deserialize(self, params):
         self._Title = params.get("Title")
         self._Total = params.get("Total")
         if params.get("OtherInvoiceListItems") is not None:
             self._OtherInvoiceListItems = []
             for item in params.get("OtherInvoiceListItems"):
@@ -10740,14 +10751,15 @@
                 self._OtherInvoiceListItems.append(obj)
         if params.get("OtherInvoiceTableItems") is not None:
             self._OtherInvoiceTableItems = []
             for item in params.get("OtherInvoiceTableItems"):
                 obj = OtherInvoiceList()
                 obj._deserialize(item)
                 self._OtherInvoiceTableItems.append(obj)
+        self._Date = params.get("Date")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -16988,14 +17000,17 @@
         :type TrainTicket: :class:`tencentcloud.ocr.v20181119.models.TrainTicket`
         :param _MedicalOutpatientInvoice: 医疗门诊收费票据（电子）
 注意：此字段可能返回 null，表示取不到有效值。
         :type MedicalOutpatientInvoice: :class:`tencentcloud.ocr.v20181119.models.MedicalInvoice`
         :param _MedicalHospitalizedInvoice: 医疗住院收费票据（电子）
 注意：此字段可能返回 null，表示取不到有效值。
         :type MedicalHospitalizedInvoice: :class:`tencentcloud.ocr.v20181119.models.MedicalInvoice`
+        :param _VatSalesList: 增值税销货清单
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VatSalesList: :class:`tencentcloud.ocr.v20181119.models.VatInvoiceInfo`
         """
         self._VatSpecialInvoice = None
         self._VatCommonInvoice = None
         self._VatElectronicCommonInvoice = None
         self._VatElectronicSpecialInvoice = None
         self._VatElectronicInvoiceBlockchain = None
         self._VatElectronicInvoiceToll = None
@@ -17013,14 +17028,15 @@
         self._QuotaInvoice = None
         self._AirTransport = None
         self._NonTaxIncomeGeneralBill = None
         self._NonTaxIncomeElectronicBill = None
         self._TrainTicket = None
         self._MedicalOutpatientInvoice = None
         self._MedicalHospitalizedInvoice = None
+        self._VatSalesList = None
 
     @property
     def VatSpecialInvoice(self):
         return self._VatSpecialInvoice
 
     @VatSpecialInvoice.setter
     def VatSpecialInvoice(self, VatSpecialInvoice):
@@ -17206,14 +17222,22 @@
     def MedicalHospitalizedInvoice(self):
         return self._MedicalHospitalizedInvoice
 
     @MedicalHospitalizedInvoice.setter
     def MedicalHospitalizedInvoice(self, MedicalHospitalizedInvoice):
         self._MedicalHospitalizedInvoice = MedicalHospitalizedInvoice
 
+    @property
+    def VatSalesList(self):
+        return self._VatSalesList
+
+    @VatSalesList.setter
+    def VatSalesList(self, VatSalesList):
+        self._VatSalesList = VatSalesList
+
 
     def _deserialize(self, params):
         if params.get("VatSpecialInvoice") is not None:
             self._VatSpecialInvoice = VatInvoiceInfo()
             self._VatSpecialInvoice._deserialize(params.get("VatSpecialInvoice"))
         if params.get("VatCommonInvoice") is not None:
             self._VatCommonInvoice = VatInvoiceInfo()
@@ -17280,14 +17304,17 @@
             self._TrainTicket._deserialize(params.get("TrainTicket"))
         if params.get("MedicalOutpatientInvoice") is not None:
             self._MedicalOutpatientInvoice = MedicalInvoice()
             self._MedicalOutpatientInvoice._deserialize(params.get("MedicalOutpatientInvoice"))
         if params.get("MedicalHospitalizedInvoice") is not None:
             self._MedicalHospitalizedInvoice = MedicalInvoice()
             self._MedicalHospitalizedInvoice._deserialize(params.get("MedicalHospitalizedInvoice"))
+        if params.get("VatSalesList") is not None:
+            self._VatSalesList = VatInvoiceInfo()
+            self._VatSalesList._deserialize(params.get("VatSalesList"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -22943,14 +22970,22 @@
         :type Receiptor: str
         :param _ElectronicFullMark: 是否有全电纸质票（0：没有，1：有）
         :type ElectronicFullMark: int
         :param _ElectronicFullNumber: 全电号码
         :type ElectronicFullNumber: str
         :param _FormName: 发票联名
         :type FormName: str
+        :param _BlockChainMark: 是否有区块链标记（0：没有，1：有）	
+        :type BlockChainMark: int
+        :param _AcquisitionMark: 是否有收购标记（0：没有，1：有）	
+        :type AcquisitionMark: int
+        :param _SubTotal: 小计金额
+        :type SubTotal: str
+        :param _SubTax: 小计税额
+        :type SubTax: str
         """
         self._CheckCode = None
         self._FormType = None
         self._TravelTax = None
         self._BuyerAddrTel = None
         self._BuyerBankAccount = None
         self._CompanySealContent = None
@@ -22986,14 +23021,18 @@
         self._Province = None
         self._VatInvoiceItemInfos = None
         self._CodeConfirm = None
         self._Receiptor = None
         self._ElectronicFullMark = None
         self._ElectronicFullNumber = None
         self._FormName = None
+        self._BlockChainMark = None
+        self._AcquisitionMark = None
+        self._SubTotal = None
+        self._SubTax = None
 
     @property
     def CheckCode(self):
         return self._CheckCode
 
     @CheckCode.setter
     def CheckCode(self, CheckCode):
@@ -23323,14 +23362,46 @@
     def FormName(self):
         return self._FormName
 
     @FormName.setter
     def FormName(self, FormName):
         self._FormName = FormName
 
+    @property
+    def BlockChainMark(self):
+        return self._BlockChainMark
+
+    @BlockChainMark.setter
+    def BlockChainMark(self, BlockChainMark):
+        self._BlockChainMark = BlockChainMark
+
+    @property
+    def AcquisitionMark(self):
+        return self._AcquisitionMark
+
+    @AcquisitionMark.setter
+    def AcquisitionMark(self, AcquisitionMark):
+        self._AcquisitionMark = AcquisitionMark
+
+    @property
+    def SubTotal(self):
+        return self._SubTotal
+
+    @SubTotal.setter
+    def SubTotal(self, SubTotal):
+        self._SubTotal = SubTotal
+
+    @property
+    def SubTax(self):
+        return self._SubTax
+
+    @SubTax.setter
+    def SubTax(self, SubTax):
+        self._SubTax = SubTax
+
 
     def _deserialize(self, params):
         self._CheckCode = params.get("CheckCode")
         self._FormType = params.get("FormType")
         self._TravelTax = params.get("TravelTax")
         self._BuyerAddrTel = params.get("BuyerAddrTel")
         self._BuyerBankAccount = params.get("BuyerBankAccount")
@@ -23372,14 +23443,18 @@
                 obj._deserialize(item)
                 self._VatInvoiceItemInfos.append(obj)
         self._CodeConfirm = params.get("CodeConfirm")
         self._Receiptor = params.get("Receiptor")
         self._ElectronicFullMark = params.get("ElectronicFullMark")
         self._ElectronicFullNumber = params.get("ElectronicFullNumber")
         self._FormName = params.get("FormName")
+        self._BlockChainMark = params.get("BlockChainMark")
+        self._AcquisitionMark = params.get("AcquisitionMark")
+        self._SubTotal = params.get("SubTotal")
+        self._SubTax = params.get("SubTax")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -23638,27 +23713,30 @@
         :type DateStart: str
         :param _DateEnd: 通行日期止
         :type DateEnd: str
         :param _LicensePlate: 车牌号
         :type LicensePlate: str
         :param _VehicleType: 车辆类型
         :type VehicleType: str
+        :param _SerialNumber: 序号
+        :type SerialNumber: str
         """
         self._Name = None
         self._Specification = None
         self._Unit = None
         self._Quantity = None
         self._Price = None
         self._Total = None
         self._TaxRate = None
         self._Tax = None
         self._DateStart = None
         self._DateEnd = None
         self._LicensePlate = None
         self._VehicleType = None
+        self._SerialNumber = None
 
     @property
     def Name(self):
         return self._Name
 
     @Name.setter
     def Name(self, Name):
@@ -23748,28 +23826,37 @@
     def VehicleType(self):
         return self._VehicleType
 
     @VehicleType.setter
     def VehicleType(self, VehicleType):
         self._VehicleType = VehicleType
 
+    @property
+    def SerialNumber(self):
+        return self._SerialNumber
+
+    @SerialNumber.setter
+    def SerialNumber(self, SerialNumber):
+        self._SerialNumber = SerialNumber
+
 
     def _deserialize(self, params):
         self._Name = params.get("Name")
         self._Specification = params.get("Specification")
         self._Unit = params.get("Unit")
         self._Quantity = params.get("Quantity")
         self._Price = params.get("Price")
         self._Total = params.get("Total")
         self._TaxRate = params.get("TaxRate")
         self._Tax = params.get("Tax")
         self._DateStart = params.get("DateStart")
         self._DateEnd = params.get("DateEnd")
         self._LicensePlate = params.get("LicensePlate")
         self._VehicleType = params.get("VehicleType")
+        self._SerialNumber = params.get("SerialNumber")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.942/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.943/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.942/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.943/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.942
+Version: 3.0.943
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.942/README.rst` & `tencentcloud-sdk-python-ocr-3.0.943/README.rst`

 * *Files identical despite different names*

