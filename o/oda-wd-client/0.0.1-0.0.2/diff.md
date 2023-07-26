# Comparing `tmp/oda_wd_client-0.0.1.tar.gz` & `tmp/oda_wd_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oda_wd_client-0.0.1.tar", max compression
+gzip compressed data, was "oda_wd_client-0.0.2.tar", max compression
```

## Comparing `oda_wd_client-0.0.1.tar` & `oda_wd_client-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0        0 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/__init__.py
--rw-r--r--   0        0        0      368 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/api.py
--rw-r--r--   0        0        0        0 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/base/__init__.py
--rw-r--r--   0        0        0     6120 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/base/api.py
--rw-r--r--   0        0        0      623 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/base/logging.py
--rw-r--r--   0        0        0      741 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/base/tools.py
--rw-r--r--   0        0        0     1065 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/base/types.py
--rw-r--r--   0        0        0      830 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/base/utils.py
--rw-r--r--   0        0        0        0 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/service/financial_management/__init__.py
--rw-r--r--   0        0        0     3416 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/service/financial_management/api.py
--rw-r--r--   0        0        0     1295 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/service/financial_management/types.py
--rw-r--r--   0        0        0     5745 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/service/financial_management/utils.py
--rw-r--r--   0        0        0        0 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/service/human_resources/__init__.py
--rw-r--r--   0        0        0     3062 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/service/human_resources/api.py
--rw-r--r--   0        0        0      221 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/service/human_resources/types.py
--rw-r--r--   0        0        0     2703 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/service/human_resources/utils.py
--rw-r--r--   0        0        0        0 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/service/resource_management/__init__.py
--rw-r--r--   0        0        0     1665 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/service/resource_management/api.py
--rw-r--r--   0        0        0     2622 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/service/resource_management/types.py
--rw-r--r--   0        0        0     6657 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/service/resource_management/utils.py
--rw-r--r--   0        0        0        0 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/service/staffing/__init__.py
--rw-r--r--   0        0        0     1407 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/service/staffing/api.py
--rw-r--r--   0        0        0     3329 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/service/staffing/types.py
--rw-r--r--   0        0        0      983 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/service/staffing/utils.py
--rw-r--r--   0        0        0      350 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/types/__init__.py
--rw-r--r--   0        0        0      211 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/types/financial_management.py
--rw-r--r--   0        0        0       85 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/types/human_resources.py
--rw-r--r--   0        0        0      283 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/types/resource_management.py
--rw-r--r--   0        0        0       82 2023-07-20 15:01:17.525458 oda_wd_client-0.0.1/oda_wd_client/types/staffing.py
--rw-r--r--   0        0        0      836 2023-07-20 15:01:17.529458 oda_wd_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 oda_wd_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/__init__.py
+-rw-r--r--   0        0        0      368 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/api.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/base/__init__.py
+-rw-r--r--   0        0        0     6120 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/base/api.py
+-rw-r--r--   0        0        0      623 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/base/logging.py
+-rw-r--r--   0        0        0      741 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/base/tools.py
+-rw-r--r--   0        0        0     1381 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/base/types.py
+-rw-r--r--   0        0        0      830 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/base/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/financial_management/__init__.py
+-rw-r--r--   0        0        0     3416 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/financial_management/api.py
+-rw-r--r--   0        0        0     1364 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/financial_management/types.py
+-rw-r--r--   0        0        0     5745 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/financial_management/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/human_resources/__init__.py
+-rw-r--r--   0        0        0     3062 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/human_resources/api.py
+-rw-r--r--   0        0        0      221 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/human_resources/types.py
+-rw-r--r--   0        0        0     2703 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/human_resources/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/resource_management/__init__.py
+-rw-r--r--   0        0        0     1665 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/resource_management/api.py
+-rw-r--r--   0        0        0     3841 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/resource_management/types.py
+-rw-r--r--   0        0        0     6985 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/resource_management/utils.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/staffing/__init__.py
+-rw-r--r--   0        0        0     1407 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/staffing/api.py
+-rw-r--r--   0        0        0     3329 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/staffing/types.py
+-rw-r--r--   0        0        0      983 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/service/staffing/utils.py
+-rw-r--r--   0        0        0      350 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/types/__init__.py
+-rw-r--r--   0        0        0      211 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/types/financial_management.py
+-rw-r--r--   0        0        0       85 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/types/human_resources.py
+-rw-r--r--   0        0        0      511 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/types/resource_management.py
+-rw-r--r--   0        0        0       82 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/oda_wd_client/types/staffing.py
+-rw-r--r--   0        0        0      836 2023-07-26 09:45:36.762193 oda_wd_client-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 oda_wd_client-0.0.2/PKG-INFO
```

### Comparing `oda_wd_client-0.0.1/oda_wd_client/base/api.py` & `oda_wd_client-0.0.2/oda_wd_client/base/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.1/oda_wd_client/base/logging.py` & `oda_wd_client-0.0.2/oda_wd_client/base/logging.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.1/oda_wd_client/base/tools.py` & `oda_wd_client-0.0.2/oda_wd_client/base/tools.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.1/oda_wd_client/base/types.py` & `oda_wd_client-0.0.2/oda_wd_client/base/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,19 +11,27 @@
     """
 
     workday_id: str
     workday_id_type: str
     workday_parent_id: str | None = None
     workday_parent_type: str | None = None
 
+    # This is the name of the class in Workday. Usually ends with "Object" (i.e. "SupplierObject")
+    _class_name: str | None = None
+
     def wd_object(
         self,
         client,
-        class_name: str,
+        class_name: str | None = None,
     ) -> sudsobject.Object:
+        class_name = class_name or self._class_name
+        assert (
+            class_name
+        ), "WD Class name must be supplied on class or call to wd_object"
+
         ref_obj = client.factory(f"ns0:{class_name}Type")
         id_obj = client.factory(f"ns0:{class_name}IDType")
         id_obj.value = self.workday_id
         id_obj._type = self.workday_id_type
         if self.workday_parent_id:
             id_obj._parent_id = self.workday_parent_id
             id_obj._parent_type = self.workday_parent_type
```

### Comparing `oda_wd_client-0.0.1/oda_wd_client/base/utils.py` & `oda_wd_client-0.0.2/oda_wd_client/base/utils.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.1/oda_wd_client/service/financial_management/api.py` & `oda_wd_client-0.0.2/oda_wd_client/service/financial_management/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.1/oda_wd_client/service/financial_management/types.py` & `oda_wd_client-0.0.2/oda_wd_client/service/financial_management/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,19 +29,21 @@
     workday_id: str
     text_id: str | None
     description: str
     is_default: bool = False
 
 
 class Currency(WorkdayReferenceBaseModel):
+    _class_name = "CurrencyObject"
     workday_id: str = Field(max_length=3, alias="currency_code")
     workday_id_type: Literal["Currency_ID"] = "Currency_ID"
     description: str | None = None
     retired: bool = False
 
 
 class Company(WorkdayReferenceBaseModel):
+    _class_name = "CompanyObject"
     workday_id: str
     workday_id_type: Literal["Company_Reference_ID"] = "Company_Reference_ID"
     name: str
     currency: Currency | None
     country_code: str | None = Field(max_length=2)
```

### Comparing `oda_wd_client-0.0.1/oda_wd_client/service/financial_management/utils.py` & `oda_wd_client-0.0.2/oda_wd_client/service/financial_management/utils.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.1/oda_wd_client/service/human_resources/api.py` & `oda_wd_client-0.0.2/oda_wd_client/service/human_resources/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.1/oda_wd_client/service/human_resources/utils.py` & `oda_wd_client-0.0.2/oda_wd_client/service/human_resources/utils.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.1/oda_wd_client/service/resource_management/api.py` & `oda_wd_client-0.0.2/oda_wd_client/service/resource_management/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.1/oda_wd_client/service/resource_management/utils.py` & `oda_wd_client-0.0.2/oda_wd_client/service/resource_management/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from oda_wd_client.base.api import WorkdayClient
 from oda_wd_client.base.utils import get_id_from_list
 from oda_wd_client.service.resource_management.types import (
     Supplier,
     SupplierInvoice,
     SupplierInvoiceLine,
-    TaxApplicability,
 )
 
 # Mapping the Workday tax ID types to canonical names used by our model
 # If the prefixes of this list were ISO 3166-compatible, we could just use those to match to country-specific fields,
 # but they're not (see Ireland), so we need a canonical mapping of our own.
 TAX_ID_SPEC = {
     "AUT-UID": "tax_id_au",
@@ -126,31 +125,43 @@
         else None,
         **contact_data,
         **account_data,
         **tax_id_data,
     )
 
 
-def _get_wd_invoice_lines_from_invoice(client, lines: list[SupplierInvoiceLine]):
+def _get_wd_invoice_lines_from_invoice(
+    client, lines: list[SupplierInvoiceLine]
+) -> list[sudsobject.Object]:
     returned_lines = []
 
     for line in lines:
         wd_line = client.factory("ns0:Supplier_Invoice_Line_Replacement_DataType")
-        # wd_tax = client.factory("ns0:Tax_Rate_Options_DataType")
         wd_line.Supplier_Invoice_Line_ID = line.order
         wd_line.Item_Description = line.description
         wd_line.Extended_Amount = line.amount
+        wd_line.Spend_Category_Reference = line.spend_category.wd_object(client)
 
-        # wd_line.Tax_Rate_Options_Data = wd_tax
-        test_applicability = TaxApplicability(
-            workday_id="NOR_Domestic_Purchase_of_Goods_and_Services"
-        )
-        wd_line.Tax_Applicability_Reference = test_applicability.wd_object(
-            client, "Tax_ApplicabilityObject"
+        # Tax options
+        wd_tax = client.factory("ns0:Tax_Rate_Options_DataType")
+        tax_opts = line.tax_rate_options_data
+        wd_tax.Tax_Rate_1_Reference = tax_opts.tax_rate.wd_object(client)
+        wd_tax.Tax_Recoverability_1_Reference = tax_opts.tax_recoverability.wd_object(
+            client
         )
+        wd_tax.Tax_Option_1_Reference = tax_opts.tax_option.wd_object(client)
+        wd_line.Tax_Rate_Options_Data = wd_tax
+
+        # Tax code
+        wd_line.Tax_Applicability_Reference = line.tax_applicability.wd_object(client)
+        wd_line.Tax_Code_Reference = line.tax_code.wd_object(client)
+
+        # Worktags
+        wd_line.Worktags_Reference.append(line.cost_center.wd_object(client))
+
         returned_lines.append(wd_line)
 
     return returned_lines
 
 
 def pydantic_supplier_invoice_to_workday(
     invoice: SupplierInvoice, client: WorkdayClient
@@ -163,27 +174,21 @@
     # Submit to business process rather than uploading invoice in draft mode
     invoice_data.Submit = True
 
     # Should not be edited inside Workday, only through API
     invoice_data.Locked_in_Workday = True
 
     invoice_data.Invoice_Number = invoice.invoice_number
-    invoice_data.Company_Reference = invoice.company.wd_object(client, "CompanyObject")
-    invoice_data.Currency_Reference = invoice.currency.wd_object(
-        client, "CurrencyObject"
-    )
-    invoice_data.Supplier_Reference = invoice.supplier.wd_object(
-        client, "SupplierObject"
-    )
-    invoice_data.Default_Tax_Option_Reference = invoice.tax_option.wd_object(
-        client, "Tax_OptionObject"
-    )
+    invoice_data.Company_Reference = invoice.company.wd_object(client)
+    invoice_data.Currency_Reference = invoice.currency.wd_object(client)
+    invoice_data.Supplier_Reference = invoice.supplier.wd_object(client)
+    invoice_data.Default_Tax_Option_Reference = invoice.tax_option.wd_object(client)
     invoice_data.Invoice_Date = str(invoice.invoice_date)
     invoice_data.Due_Date_Override = str(invoice.due_date)
     invoice_data.Control_Amount_Total = invoice.total_amount
-    invoice_data.Tax_Amount = invoice.tax_amount
+    # invoice_data.Tax_Amount = invoice.tax_amount
     # invoice_data.Attachment_Data = _get_wd_attachment_data_from_invoice(invoice)
     invoice_data.Invoice_Line_Replacement_Data = _get_wd_invoice_lines_from_invoice(
         client, invoice.lines
     )
 
     return invoice_data
```

### Comparing `oda_wd_client-0.0.1/oda_wd_client/service/staffing/api.py` & `oda_wd_client-0.0.2/oda_wd_client/service/staffing/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.1/oda_wd_client/service/staffing/types.py` & `oda_wd_client-0.0.2/oda_wd_client/service/staffing/types.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.1/oda_wd_client/service/staffing/utils.py` & `oda_wd_client-0.0.2/oda_wd_client/service/staffing/utils.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.0.1/pyproject.toml` & `oda_wd_client-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oda-wd-client"
-version = "0.0.1"
+version = "0.0.2"
 description = "A library for interacting with Workday from Python"
 authors = [
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

