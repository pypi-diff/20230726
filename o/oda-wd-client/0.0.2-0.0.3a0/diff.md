# Comparing `tmp/oda_wd_client-0.0.2.tar.gz` & `tmp/oda_wd_client-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oda_wd_client-0.0.2.tar", max compression
+gzip compressed data, was "oda_wd_client-0.0.3a0.tar", max compression
```

## Comparing `oda_wd_client-0.0.2.tar` & `oda_wd_client-0.0.3a0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0        0 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/__init__.py
--rw-r--r--   0        0        0      368 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/api.py
--rw-r--r--   0        0        0        0 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/base/__init__.py
--rw-r--r--   0        0        0     6120 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/base/api.py
--rw-r--r--   0        0        0      623 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/base/logging.py
--rw-r--r--   0        0        0      741 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/base/tools.py
--rw-r--r--   0        0        0     1381 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/base/types.py
--rw-r--r--   0        0        0      830 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/base/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/financial_management/__init__.py
--rw-r--r--   0        0        0     3416 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/financial_management/api.py
--rw-r--r--   0        0        0     1364 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/financial_management/types.py
--rw-r--r--   0        0        0     5745 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/financial_management/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/human_resources/__init__.py
--rw-r--r--   0        0        0     3062 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/human_resources/api.py
--rw-r--r--   0        0        0      221 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/human_resources/types.py
--rw-r--r--   0        0        0     2703 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/human_resources/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/resource_management/__init__.py
--rw-r--r--   0        0        0     1665 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/resource_management/api.py
--rw-r--r--   0        0        0     3841 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/resource_management/types.py
--rw-r--r--   0        0        0     6985 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/resource_management/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/staffing/__init__.py
--rw-r--r--   0        0        0     1407 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/staffing/api.py
--rw-r--r--   0        0        0     3329 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/staffing/types.py
--rw-r--r--   0        0        0      983 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/staffing/utils.py
--rw-r--r--   0        0        0      350 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/types/__init__.py
--rw-r--r--   0        0        0      211 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/types/financial_management.py
--rw-r--r--   0        0        0       85 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/types/human_resources.py
--rw-r--r--   0        0        0      511 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/types/resource_management.py
--rw-r--r--   0        0        0       82 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/types/staffing.py
--rw-r--r--   0        0        0      836 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 oda_wd_client-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 12:58:45.595819 oda_wd_client-0.0.3a0/oda_wd_client/__init__.py
+-rw-r--r--   0        0        0      368 2023-07-26 12:58:45.595819 oda_wd_client-0.0.3a0/oda_wd_client/api.py
+-rw-r--r--   0        0        0        0 2023-07-26 12:58:45.595819 oda_wd_client-0.0.3a0/oda_wd_client/base/__init__.py
+-rw-r--r--   0        0        0     6120 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/base/api.py
+-rw-r--r--   0        0        0      623 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/base/logging.py
+-rw-r--r--   0        0        0      741 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/base/tools.py
+-rw-r--r--   0        0        0     1381 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/base/types.py
+-rw-r--r--   0        0        0      830 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/base/utils.py
+-rw-r--r--   0        0        0       19 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/financial_management/__init__.py
+-rw-r--r--   0        0        0     3796 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/financial_management/api.py
+-rw-r--r--   0        0        0     3708 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/financial_management/types.py
+-rw-r--r--   0        0        0     7865 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/financial_management/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/human_resources/__init__.py
+-rw-r--r--   0        0        0     3062 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/human_resources/api.py
+-rw-r--r--   0        0        0      321 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/human_resources/types.py
+-rw-r--r--   0        0        0     2703 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/human_resources/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/resource_management/__init__.py
+-rw-r--r--   0        0        0     1665 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/resource_management/api.py
+-rw-r--r--   0        0        0     3652 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/resource_management/types.py
+-rw-r--r--   0        0        0     6985 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/resource_management/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/staffing/__init__.py
+-rw-r--r--   0        0        0     1407 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/staffing/api.py
+-rw-r--r--   0        0        0     3422 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/staffing/types.py
+-rw-r--r--   0        0        0      983 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/service/staffing/utils.py
+-rw-r--r--   0        0        0      350 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/types/__init__.py
+-rw-r--r--   0        0        0      528 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/types/financial_management.py
+-rw-r--r--   0        0        0       85 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/types/human_resources.py
+-rw-r--r--   0        0        0      511 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/types/resource_management.py
+-rw-r--r--   0        0        0       82 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/oda_wd_client/types/staffing.py
+-rw-r--r--   0        0        0      838 2023-07-26 12:58:45.599819 oda_wd_client-0.0.3a0/pyproject.toml
+-rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 oda_wd_client-0.0.3a0/PKG-INFO
```

### Comparing `oda_wd_client-0.0.2/oda_wd_client/base/api.py` & `oda_wd_client-0.0.3a0/oda_wd_client/base/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.2/oda_wd_client/base/logging.py` & `oda_wd_client-0.0.3a0/oda_wd_client/base/logging.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.2/oda_wd_client/base/tools.py` & `oda_wd_client-0.0.3a0/oda_wd_client/base/tools.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.2/oda_wd_client/base/types.py` & `oda_wd_client-0.0.3a0/oda_wd_client/base/types.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.2/oda_wd_client/base/utils.py` & `oda_wd_client-0.0.3a0/oda_wd_client/base/utils.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.2/oda_wd_client/service/financial_management/api.py` & `oda_wd_client-0.0.3a0/oda_wd_client/service/financial_management/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import Iterator
 
 from suds import sudsobject
 
 from oda_wd_client.base.api import WorkdayClient
 from oda_wd_client.base.tools import suds_to_dict
 from oda_wd_client.service.financial_management.types import (
+    AccountingJournalData,
     Company,
     ConversionRate,
     ConversionRateType,
     Currency,
 )
 from oda_wd_client.service.financial_management.utils import (
+    pydantic_accounting_journal_to_workday,
     pydantic_conversion_rate_to_workday,
     workday_company_to_pydantic,
     workday_conversion_rate_to_pydantic,
     workday_conversion_rate_type_to_pydantic,
     workday_currency_to_pydantic,
     workday_tax_applicability_to_pydantic,
 )
@@ -86,7 +88,15 @@
         for tax_applicability in results:
             if return_suds_object:
                 yield tax_applicability
             else:
                 yield workday_tax_applicability_to_pydantic(
                     suds_to_dict(tax_applicability)
                 )
+
+    def submit_accounting_journal(
+        self, journal: AccountingJournalData
+    ) -> sudsobject.Object:
+        data_object = pydantic_accounting_journal_to_workday(journal, client=self)
+        return self._request(
+            "Submit_Accounting_Journal", Accounting_Journal_Data=data_object
+        )
```

### Comparing `oda_wd_client-0.0.2/oda_wd_client/service/human_resources/api.py` & `oda_wd_client-0.0.3a0/oda_wd_client/service/human_resources/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.2/oda_wd_client/service/human_resources/utils.py` & `oda_wd_client-0.0.3a0/oda_wd_client/service/human_resources/utils.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.2/oda_wd_client/service/resource_management/api.py` & `oda_wd_client-0.0.3a0/oda_wd_client/service/resource_management/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.2/oda_wd_client/service/resource_management/types.py` & `oda_wd_client-0.0.3a0/oda_wd_client/service/resource_management/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,23 @@
 from decimal import Decimal
 from typing import Literal
 
 from pydantic import BaseModel, Field, validator
 
 from oda_wd_client.base.types import WorkdayReferenceBaseModel
 from oda_wd_client.base.utils import parse_workday_date
-from oda_wd_client.service.financial_management.types import Company, Currency
+from oda_wd_client.service.financial_management.types import (
+    Company,
+    CostCenter,
+    Currency,
+    SpendCategory,
+)
+
+# All public imports should be done through oda_wd_client.types.resource_management
+__all__: list = []
 
 
 class TaxApplicability(WorkdayReferenceBaseModel):
     _class_name = "Tax_ApplicabilityObject"
     workday_id: str
     workday_id_type: Literal["Tax_Applicability_ID"] = "Tax_Applicability_ID"
     # Code is human-readable text but not critical, so we default to empty string
@@ -80,32 +88,22 @@
 class TaxRecoverability(WorkdayReferenceBaseModel):
     _class_name = "Tax_RecoverabilityObject"
     workday_id_type: Literal[
         "Tax_Recoverability_Object_ID"
     ] = "Tax_Recoverability_Object_ID"
 
 
-class SpendCategory(WorkdayReferenceBaseModel):
-    _class_name = "Spend_CategoryObject"
-    workday_id_type: Literal["Spend_Category_ID"] = "Spend_Category_ID"
-
-
 class TaxRateOptionsData(BaseModel):
     tax_rate: TaxRate
     tax_recoverability: TaxRecoverability = TaxRecoverability(
         workday_id="Fully_Recoverable"
     )
     tax_option: TaxOption = TaxOption(workday_id="CALC_TAX_DUE")
 
 
-class CostCenter(WorkdayReferenceBaseModel):
-    _class_name = "Accounting_WorktagObject"
-    workday_id_type: Literal["Cost_Center_Reference_ID"] = "Cost_Center_Reference_ID"
-
-
 class SupplierInvoiceLine(BaseModel):
     order: int | None
     description: str | None
     tax_rate_options_data: TaxRateOptionsData
     tax_applicability: TaxApplicability
     tax_code: TaxCode
     spend_category: SpendCategory
```

### Comparing `oda_wd_client-0.0.2/oda_wd_client/service/resource_management/utils.py` & `oda_wd_client-0.0.3a0/oda_wd_client/service/resource_management/utils.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.2/oda_wd_client/service/staffing/api.py` & `oda_wd_client-0.0.3a0/oda_wd_client/service/staffing/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.2/oda_wd_client/service/staffing/types.py` & `oda_wd_client-0.0.3a0/oda_wd_client/service/staffing/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from enum import Enum
 
 from pydantic import BaseModel
 
+# All public imports should be done through oda_wd_client.types.staffing
+__all__: list = []
+
 
 class Document(BaseModel):
     class WorkdayCategory(str, Enum):
         employee_contract = "EMPLOYEE_CONTRACT"
         student_collections = "STUDENT_COLLECTIONS"
         prospect_resume_cover_letter = "PROSPECT_RESUME_AND_COVER_LETTER"
         candidate_resume_cover_letter = "CANDIDATE_RESUME_AND_COVER_LETTER"
```

### Comparing `oda_wd_client-0.0.2/oda_wd_client/service/staffing/utils.py` & `oda_wd_client-0.0.3a0/oda_wd_client/service/staffing/utils.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.2/pyproject.toml` & `oda_wd_client-0.0.3a0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oda-wd-client"
-version = "0.0.2"
+version = "0.0.3a0"
 description = "A library for interacting with Workday from Python"
 authors = [
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

