# Comparing `tmp/mergepythonclient-0.1.1.tar.gz` & `tmp/mergepythonclient-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergepythonclient-0.1.1.tar", max compression
+gzip compressed data, was "mergepythonclient-0.1.2.tar", max compression
```

## Comparing `mergepythonclient-0.1.1.tar` & `mergepythonclient-0.1.2.tar`

### file list

```diff
@@ -1,1114 +1,1114 @@
--rw-r--r--   0        0        0     3274 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     4897 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/README.md
--rw-r--r--   0        0        0      535 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      249 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/__init__.py
--rw-r--r--   0        0        0     2459 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/client.py
--rw-r--r--   0        0        0      519 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/core/api_error.py
--rw-r--r--   0        0        0     1113 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      201 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/environment.py
--rw-r--r--   0        0        0        0 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/py.typed
--rw-r--r--   0        0        0      178 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/__init__.py
--rw-r--r--   0        0        0    12630 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/__init__.py
--rw-r--r--   0        0        0    12026 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/client.py
--rw-r--r--   0        0        0     1410 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2394 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2634 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/accounts/__init__.py
--rw-r--r--   0        0        0    18106 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/addresses/__init__.py
--rw-r--r--   0        0        0     4472 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/addresses/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/attachments/__init__.py
--rw-r--r--   0        0        0    14525 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/attachments/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2472 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.034730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/balance_sheets/__init__.py
--rw-r--r--   0        0        0    10863 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/balance_sheets/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/cash_flow_statements/__init__.py
--rw-r--r--   0        0        0    10991 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/cash_flow_statements/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/company_info/__init__.py
--rw-r--r--   0        0        0    10522 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/company_info/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/contacts/__init__.py
--rw-r--r--   0        0        0    17812 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/contacts/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/credit_notes/__init__.py
--rw-r--r--   0        0        0    14782 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/credit_notes/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2137 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/expenses/__init__.py
--rw-r--r--   0        0        0    16471 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/expenses/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     3050 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2819 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/income_statements/__init__.py
--rw-r--r--   0        0        0    10937 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/income_statements/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/invoices/__init__.py
--rw-r--r--   0        0        0    20058 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/invoices/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/issues/__init__.py
--rw-r--r--   0        0        0    10522 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/items/__init__.py
--rw-r--r--   0        0        0    13083 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/items/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/journal_entries/__init__.py
--rw-r--r--   0        0        0    16787 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/journal_entries/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/link_token/__init__.py
--rw-r--r--   0        0        0     8898 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0    10663 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     7356 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/payments/__init__.py
--rw-r--r--   0        0        0    17271 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/payments/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/phone_numbers/__init__.py
--rw-r--r--   0        0        0     3281 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/phone_numbers/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/purchase_orders/__init__.py
--rw-r--r--   0        0        0    19114 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/purchase_orders/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2829 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     8228 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     3372 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/tax_rates/__init__.py
--rw-r--r--   0        0        0    10743 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/tax_rates/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/tracking_categories/__init__.py
--rw-r--r--   0        0        0    13333 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/tracking_categories/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/transactions/__init__.py
--rw-r--r--   0        0        0    12010 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/transactions/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/vendor_credits/__init__.py
--rw-r--r--   0        0        0    12034 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/vendor_credits/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     5199 2023-07-24 18:15:26.038730 mergepythonclient-0.1.1/src/merge/resources/accounting/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    17717 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/__init__.py
--rw-r--r--   0        0        0    17393 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account.py
--rw-r--r--   0        0        0      195 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_classification.py
--rw-r--r--   0        0        0      171 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_currency.py
--rw-r--r--   0        0        0     1483 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_integration.py
--rw-r--r--   0        0        0    16986 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_request.py
--rw-r--r--   0        0        0      202 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_request_classification.py
--rw-r--r--   0        0        0      178 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_request_currency.py
--rw-r--r--   0        0        0      192 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_request_status.py
--rw-r--r--   0        0        0     1105 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_response.py
--rw-r--r--   0        0        0      185 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_status.py
--rw-r--r--   0        0        0      758 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_status_enum.py
--rw-r--r--   0        0        0      845 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_token.py
--rw-r--r--   0        0        0     1935 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_attachment.py
--rw-r--r--   0        0        0     1462 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_attachment_request.py
--rw-r--r--   0        0        0     1158 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_attachment_response.py
--rw-r--r--   0        0        0     1344 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_phone_number.py
--rw-r--r--   0        0        0     1346 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_phone_number_request.py
--rw-r--r--   0        0        0      819 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounts_list_request_remote_fields.py
--rw-r--r--   0        0        0      831 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounts_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      835 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounts_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      847 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounts_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0    11090 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/address.py
--rw-r--r--   0        0        0      167 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/address_country.py
--rw-r--r--   0        0        0      177 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/address_type.py
--rw-r--r--   0        0        0      555 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/address_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/available_actions.py
--rw-r--r--   0        0        0    16903 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/balance_sheet.py
--rw-r--r--   0        0        0      176 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/balance_sheet_currency.py
--rw-r--r--   0        0        0    17216 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/cash_flow_statement.py
--rw-r--r--   0        0        0      181 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/cash_flow_statement_currency.py
--rw-r--r--   0        0        0     1391 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/category_enum.py
--rw-r--r--   0        0        0      560 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/category_type_enum.py
--rw-r--r--   0        0        0     1103 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/classification_enum.py
--rw-r--r--   0        0        0      997 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0    16863 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/company_info.py
--rw-r--r--   0        0        0      175 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/company_info_currency.py
--rw-r--r--   0        0        0      827 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/company_info_list_request_expand.py
--rw-r--r--   0        0        0      843 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/company_info_retrieve_request_expand.py
--rw-r--r--   0        0        0     2324 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/condition_type_enum.py
--rw-r--r--   0        0        0     3027 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/contact.py
--rw-r--r--   0        0        0     2478 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/contact_request.py
--rw-r--r--   0        0        0      182 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/contact_request_status.py
--rw-r--r--   0        0        0     1105 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/contact_response.py
--rw-r--r--   0        0        0      175 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/contact_status.py
--rw-r--r--   0        0        0     1675 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/contacts_list_request_expand.py
--rw-r--r--   0        0        0     1707 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/contacts_retrieve_request_expand.py
--rw-r--r--   0        0        0    35178 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/country_enum.py
--rw-r--r--   0        0        0    17747 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_note.py
--rw-r--r--   0        0        0      174 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_note_currency.py
--rw-r--r--   0        0        0     2275 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_note_line_item.py
--rw-r--r--   0        0        0      198 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_note_status.py
--rw-r--r--   0        0        0      784 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_note_status_enum.py
--rw-r--r--   0        0        0     1859 2023-07-24 18:15:26.042730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_list_request_expand.py
--rw-r--r--   0        0        0      731 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_list_request_remote_fields.py
--rw-r--r--   0        0        0      743 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     1891 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_expand.py
--rw-r--r--   0        0        0      747 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      759 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0    47961 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/currency_enum.py
--rw-r--r--   0        0        0      870 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/debug_model_log_summary.py
--rw-r--r--   0        0        0      522 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/error_validation_problem.py
--rw-r--r--   0        0        0    16980 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense.py
--rw-r--r--   0        0        0      171 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_currency.py
--rw-r--r--   0        0        0     2074 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_line.py
--rw-r--r--   0        0        0     2076 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_line_request.py
--rw-r--r--   0        0        0    16445 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_request.py
--rw-r--r--   0        0        0      178 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_request_currency.py
--rw-r--r--   0        0        0     1105 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_response.py
--rw-r--r--   0        0        0     3715 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expenses_list_request_expand.py
--rw-r--r--   0        0        0     3779 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/expenses_retrieve_request_expand.py
--rw-r--r--   0        0        0    17240 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/income_statement.py
--rw-r--r--   0        0        0      179 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/income_statement_currency.py
--rw-r--r--   0        0        0    18003 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice.py
--rw-r--r--   0        0        0      171 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_currency.py
--rw-r--r--   0        0        0    16460 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_line_item.py
--rw-r--r--   0        0        0      179 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_line_item_currency.py
--rw-r--r--   0        0        0    16389 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_line_item_request.py
--rw-r--r--   0        0        0      186 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_line_item_request_currency.py
--rw-r--r--   0        0        0    17620 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_request.py
--rw-r--r--   0        0        0      178 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_request_currency.py
--rw-r--r--   0        0        0      184 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_request_type.py
--rw-r--r--   0        0        0     1105 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_response.py
--rw-r--r--   0        0        0      177 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_type.py
--rw-r--r--   0        0        0      709 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_type_enum.py
--rw-r--r--   0        0        0     8275 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoices_list_request_expand.py
--rw-r--r--   0        0        0      622 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoices_list_request_type.py
--rw-r--r--   0        0        0     8403 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoices_retrieve_request_expand.py
--rw-r--r--   0        0        0     1323 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/issues_list_request_status.py
--rw-r--r--   0        0        0     2624 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/item.py
--rw-r--r--   0        0        0      172 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/item_status.py
--rw-r--r--   0        0        0     1791 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/items_list_request_expand.py
--rw-r--r--   0        0        0     1823 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/items_retrieve_request_expand.py
--rw-r--r--   0        0        0     3771 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entries_list_request_expand.py
--rw-r--r--   0        0        0     3835 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entries_retrieve_request_expand.py
--rw-r--r--   0        0        0    17164 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry.py
--rw-r--r--   0        0        0      176 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry_currency.py
--rw-r--r--   0        0        0      197 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry_posting_status.py
--rw-r--r--   0        0        0    16526 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry_request.py
--rw-r--r--   0        0        0      183 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry_request_currency.py
--rw-r--r--   0        0        0      204 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry_request_posting_status.py
--rw-r--r--   0        0        0     1126 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry_response.py
--rw-r--r--   0        0        0     1790 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_line.py
--rw-r--r--   0        0        0     1792 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_line_request.py
--rw-r--r--   0        0        0      835 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-24 18:15:26.046730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0      993 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/operator_schema.py
--rw-r--r--   0        0        0      959 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      888 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_account_list.py
--rw-r--r--   0        0        0      941 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_accounting_attachment_list.py
--rw-r--r--   0        0        0      909 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_balance_sheet_list.py
--rw-r--r--   0        0        0      930 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_cash_flow_statement_list.py
--rw-r--r--   0        0        0      905 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_company_info_list.py
--rw-r--r--   0        0        0      921 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      888 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_contact_list.py
--rw-r--r--   0        0        0      901 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_credit_note_list.py
--rw-r--r--   0        0        0      888 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_expense_list.py
--rw-r--r--   0        0        0      921 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_income_statement_list.py
--rw-r--r--   0        0        0      888 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_invoice_list.py
--rw-r--r--   0        0        0      880 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_issue_list.py
--rw-r--r--   0        0        0      876 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_item_list.py
--rw-r--r--   0        0        0      909 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_journal_entry_list.py
--rw-r--r--   0        0        0      888 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_payment_list.py
--rw-r--r--   0        0        0      913 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_purchase_order_list.py
--rw-r--r--   0        0        0      901 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      889 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_tax_rate_list.py
--rw-r--r--   0        0        0      925 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_tracking_category_list.py
--rw-r--r--   0        0        0      904 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_transaction_list.py
--rw-r--r--   0        0        0      909 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_vendor_credit_list.py
--rw-r--r--   0        0        0    16832 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/payment.py
--rw-r--r--   0        0        0      171 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/payment_currency.py
--rw-r--r--   0        0        0    16241 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/payment_request.py
--rw-r--r--   0        0        0      178 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/payment_request_currency.py
--rw-r--r--   0        0        0     1105 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/payment_response.py
--rw-r--r--   0        0        0     3715 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/payments_list_request_expand.py
--rw-r--r--   0        0        0     3779 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/payments_retrieve_request_expand.py
--rw-r--r--   0        0        0      554 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/posting_status_enum.py
--rw-r--r--   0        0        0    17816 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order.py
--rw-r--r--   0        0        0      177 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_currency.py
--rw-r--r--   0        0        0    16830 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_line_item.py
--rw-r--r--   0        0        0      185 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_line_item_currency.py
--rw-r--r--   0        0        0    16854 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_line_item_request.py
--rw-r--r--   0        0        0      192 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_line_item_request_currency.py
--rw-r--r--   0        0        0    17041 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_request.py
--rw-r--r--   0        0        0      184 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_request_currency.py
--rw-r--r--   0        0        0      217 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_request_status.py
--rw-r--r--   0        0        0     1130 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_response.py
--rw-r--r--   0        0        0      210 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_status.py
--rw-r--r--   0        0        0     1154 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_status_enum.py
--rw-r--r--   0        0        0     9043 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_orders_list_request_expand.py
--rw-r--r--   0        0        0     9171 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_orders_retrieve_request_expand.py
--rw-r--r--   0        0        0      802 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/remote_key.py
--rw-r--r--   0        0        0     1299 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/remote_response.py
--rw-r--r--   0        0        0     1649 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/report_item.py
--rw-r--r--   0        0        0      723 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/response_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0      542 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/status_7_d_1_enum.py
--rw-r--r--   0        0        0     1411 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     2002 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/tax_rate.py
--rw-r--r--   0        0        0     2481 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/tracking_category.py
--rw-r--r--   0        0        0      197 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/tracking_category_category_type.py
--rw-r--r--   0        0        0      184 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/tracking_category_status.py
--rw-r--r--   0        0        0    17229 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/transaction.py
--rw-r--r--   0        0        0      175 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/transaction_currency.py
--rw-r--r--   0        0        0    16685 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/transaction_line_item.py
--rw-r--r--   0        0        0      183 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/transaction_line_item_currency.py
--rw-r--r--   0        0        0     3899 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/transactions_list_request_expand.py
--rw-r--r--   0        0        0     3963 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/transactions_retrieve_request_expand.py
--rw-r--r--   0        0        0      762 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/validation_problem_source.py
--rw-r--r--   0        0        0    16901 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credit.py
--rw-r--r--   0        0        0      176 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credit_currency.py
--rw-r--r--   0        0        0     1999 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credit_line.py
--rw-r--r--   0        0        0     3675 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credits_list_request_expand.py
--rw-r--r--   0        0        0     3739 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credits_retrieve_request_expand.py
--rw-r--r--   0        0        0      915 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/accounting/types/webhook_receiver.py
--rw-r--r--   0        0        0     9656 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/ats/__init__.py
--rw-r--r--   0        0        0    10018 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/ats/client.py
--rw-r--r--   0        0        0     1144 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2416 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2656 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.050730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/activities/__init__.py
--rw-r--r--   0        0        0    18450 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/activities/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/applications/__init__.py
--rw-r--r--   0        0        0    22753 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/applications/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/attachments/__init__.py
--rw-r--r--   0        0        0    18326 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/attachments/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2494 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/candidates/__init__.py
--rw-r--r--   0        0        0    25052 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/candidates/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2159 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/departments/__init__.py
--rw-r--r--   0        0        0     9128 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/departments/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/eeocs/__init__.py
--rw-r--r--   0        0        0    13425 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/eeocs/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     3072 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2841 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/interviews/__init__.py
--rw-r--r--   0        0        0    19472 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/interviews/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/issues/__init__.py
--rw-r--r--   0        0        0    10566 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/job_interview_stages/__init__.py
--rw-r--r--   0        0        0    10955 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/job_interview_stages/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/jobs/__init__.py
--rw-r--r--   0        0        0    14939 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/jobs/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/link_token/__init__.py
--rw-r--r--   0        0        0     8920 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0    10685 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/offers/__init__.py
--rw-r--r--   0        0        0    13609 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/offers/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/offices/__init__.py
--rw-r--r--   0        0        0     9042 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/offices/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     7378 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2851 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/reject_reasons/__init__.py
--rw-r--r--   0        0        0     9178 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/reject_reasons/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/scorecards/__init__.py
--rw-r--r--   0        0        0    14473 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/scorecards/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     8294 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     3394 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/tags/__init__.py
--rw-r--r--   0        0        0     6731 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/tags/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/users/__init__.py
--rw-r--r--   0        0        0    11995 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/users/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     5243 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    13447 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/__init__.py
--rw-r--r--   0        0        0     1240 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/access_role_enum.py
--rw-r--r--   0        0        0     1483 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/account_token.py
--rw-r--r--   0        0        0      857 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activities_list_request_remote_fields.py
--rw-r--r--   0        0        0      869 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      873 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      885 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     2705 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activity.py
--rw-r--r--   0        0        0      189 2023-07-24 18:15:26.054730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_activity_type.py
--rw-r--r--   0        0        0     2155 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_request.py
--rw-r--r--   0        0        0      196 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_request_activity_type.py
--rw-r--r--   0        0        0      187 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_request_visibility.py
--rw-r--r--   0        0        0     1109 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_response.py
--rw-r--r--   0        0        0      705 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_type_enum.py
--rw-r--r--   0        0        0      180 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_visibility.py
--rw-r--r--   0        0        0     2473 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/application.py
--rw-r--r--   0        0        0     2269 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/application_request.py
--rw-r--r--   0        0        0     1121 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/application_response.py
--rw-r--r--   0        0        0     8243 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/applications_list_request_expand.py
--rw-r--r--   0        0        0     8371 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/applications_retrieve_request_expand.py
--rw-r--r--   0        0        0     2146 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment.py
--rw-r--r--   0        0        0      199 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment_attachment_type.py
--rw-r--r--   0        0        0     1820 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment_request.py
--rw-r--r--   0        0        0      206 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment_request_attachment_type.py
--rw-r--r--   0        0        0     1117 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment_response.py
--rw-r--r--   0        0        0      985 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/available_actions.py
--rw-r--r--   0        0        0     3471 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/candidate.py
--rw-r--r--   0        0        0     3061 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/candidate_request.py
--rw-r--r--   0        0        0     1113 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/candidate_response.py
--rw-r--r--   0        0        0      833 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/candidates_list_request_expand.py
--rw-r--r--   0        0        0      849 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/candidates_retrieve_request_expand.py
--rw-r--r--   0        0        0     1391 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     2324 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/condition_type_enum.py
--rw-r--r--   0        0        0      870 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/debug_model_log_summary.py
--rw-r--r--   0        0        0     1698 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/department.py
--rw-r--r--   0        0        0     1337 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/disability_status_enum.py
--rw-r--r--   0        0        0     4088 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeoc.py
--rw-r--r--   0        0        0      201 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeoc_disability_status.py
--rw-r--r--   0        0        0      160 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeoc_gender.py
--rw-r--r--   0        0        0      152 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeoc_race.py
--rw-r--r--   0        0        0      189 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeoc_veteran_status.py
--rw-r--r--   0        0        0     3803 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py
--rw-r--r--   0        0        0     3851 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     3867 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     3915 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1529 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/email_address.py
--rw-r--r--   0        0        0      210 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/email_address_email_address_type.py
--rw-r--r--   0        0        0     1553 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/email_address_request.py
--rw-r--r--   0        0        0      217 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/email_address_request_email_address_type.py
--rw-r--r--   0        0        0      742 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/email_address_type_enum.py
--rw-r--r--   0        0        0      522 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/error_validation_problem.py
--rw-r--r--   0        0        0     1160 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/gender_enum.py
--rw-r--r--   0        0        0     4187 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/interviews_list_request_expand.py
--rw-r--r--   0        0        0     4251 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/interviews_retrieve_request_expand.py
--rw-r--r--   0        0        0     1323 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/issues_list_request_status.py
--rw-r--r--   0        0        0     3428 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/job.py
--rw-r--r--   0        0        0     2387 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/job_interview_stage.py
--rw-r--r--   0        0        0      169 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/job_status.py
--rw-r--r--   0        0        0     1045 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/job_status_enum.py
--rw-r--r--   0        0        0     3771 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/jobs_list_request_expand.py
--rw-r--r--   0        0        0      956 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/jobs_list_request_status.py
--rw-r--r--   0        0        0     3835 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/jobs_retrieve_request_expand.py
--rw-r--r--   0        0        0      835 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0     2786 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/offer.py
--rw-r--r--   0        0        0      177 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/offer_status.py
--rw-r--r--   0        0        0     1832 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/offer_status_enum.py
--rw-r--r--   0        0        0      767 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/offers_list_request_expand.py
--rw-r--r--   0        0        0      783 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/offers_retrieve_request_expand.py
--rw-r--r--   0        0        0     1817 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/office.py
--rw-r--r--   0        0        0      993 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/operator_schema.py
--rw-r--r--   0        0        0     1180 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/overall_recommendation_enum.py
--rw-r--r--   0        0        0      959 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      892 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_activity_list.py
--rw-r--r--   0        0        0      904 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_application_list.py
--rw-r--r--   0        0        0      900 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_attachment_list.py
--rw-r--r--   0        0        0      896 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_candidate_list.py
--rw-r--r--   0        0        0      921 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      900 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_department_list.py
--rw-r--r--   0        0        0      876 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_eeoc_list.py
--rw-r--r--   0        0        0      880 2023-07-24 18:15:26.058730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_issue_list.py
--rw-r--r--   0        0        0      930 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_job_interview_stage_list.py
--rw-r--r--   0        0        0      872 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_job_list.py
--rw-r--r--   0        0        0      880 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_offer_list.py
--rw-r--r--   0        0        0      884 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_office_list.py
--rw-r--r--   0        0        0      909 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_reject_reason_list.py
--rw-r--r--   0        0        0      901 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_remote_user_list.py
--rw-r--r--   0        0        0      933 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_scheduled_interview_list.py
--rw-r--r--   0        0        0      896 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_scorecard_list.py
--rw-r--r--   0        0        0      901 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      872 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_tag_list.py
--rw-r--r--   0        0        0     3068 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/patched_candidate_request.py
--rw-r--r--   0        0        0     1624 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/phone_number.py
--rw-r--r--   0        0        0      205 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/phone_number_phone_number_type.py
--rw-r--r--   0        0        0     1648 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/phone_number_request.py
--rw-r--r--   0        0        0      212 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/phone_number_request_phone_number_type.py
--rw-r--r--   0        0        0     1039 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/phone_number_type_enum.py
--rw-r--r--   0        0        0     2326 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/race_enum.py
--rw-r--r--   0        0        0      814 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/reason_enum.py
--rw-r--r--   0        0        0     1775 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/reject_reason.py
--rw-r--r--   0        0        0      802 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_key.py
--rw-r--r--   0        0        0     1330 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_response.py
--rw-r--r--   0        0        0      195 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_response_response_type.py
--rw-r--r--   0        0        0     2562 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_user.py
--rw-r--r--   0        0        0      183 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_user_access_role.py
--rw-r--r--   0        0        0      723 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/response_type_enum.py
--rw-r--r--   0        0        0     3187 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview.py
--rw-r--r--   0        0        0     2464 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview_request.py
--rw-r--r--   0        0        0      237 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview_request_status.py
--rw-r--r--   0        0        0     1150 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview_response.py
--rw-r--r--   0        0        0      230 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview_status.py
--rw-r--r--   0        0        0      893 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview_status_enum.py
--rw-r--r--   0        0        0     2692 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scorecard.py
--rw-r--r--   0        0        0      226 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scorecard_overall_recommendation.py
--rw-r--r--   0        0        0     1731 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scorecards_list_request_expand.py
--rw-r--r--   0        0        0     1763 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py
--rw-r--r--   0        0        0      695 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1623 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/tag.py
--rw-r--r--   0        0        0     1659 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/url.py
--rw-r--r--   0        0        0     1683 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/url_request.py
--rw-r--r--   0        0        0      171 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/url_request_url_type.py
--rw-r--r--   0        0        0     1451 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/url_type_enum.py
--rw-r--r--   0        0        0      164 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/url_url_type.py
--rw-r--r--   0        0        0      762 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/validation_problem_source.py
--rw-r--r--   0        0        0     1467 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/veteran_status_enum.py
--rw-r--r--   0        0        0      760 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/visibility_enum.py
--rw-r--r--   0        0        0      915 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/ats/types/webhook_receiver.py
--rw-r--r--   0        0        0     9538 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/__init__.py
--rw-r--r--   0        0        0     9931 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/client.py
--rw-r--r--   0        0        0     1144 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2394 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2634 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/accounts/__init__.py
--rw-r--r--   0        0        0    25839 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/association_types/__init__.py
--rw-r--r--   0        0        0    17150 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/association_types/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/associations/__init__.py
--rw-r--r--   0        0        0    12433 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/associations/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2472 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/contacts/__init__.py
--rw-r--r--   0        0        0    28151 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/contacts/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/custom_object_classes/__init__.py
--rw-r--r--   0        0        0    13261 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/custom_object_classes/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/custom_objects/__init__.py
--rw-r--r--   0        0        0    22340 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/custom_objects/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2137 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/engagement_types/__init__.py
--rw-r--r--   0        0        0    14939 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/engagement_types/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.062730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/engagements/__init__.py
--rw-r--r--   0        0        0    25713 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/engagements/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     3050 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2819 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/issues/__init__.py
--rw-r--r--   0        0        0    10522 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/leads/__init__.py
--rw-r--r--   0        0        0    22008 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/leads/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/link_token/__init__.py
--rw-r--r--   0        0        0     8898 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0    10663 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/notes/__init__.py
--rw-r--r--   0        0        0    22286 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/notes/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/opportunities/__init__.py
--rw-r--r--   0        0        0    30390 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/opportunities/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     7356 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2829 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     8228 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/stages/__init__.py
--rw-r--r--   0        0        0    14713 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/stages/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     3372 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/tasks/__init__.py
--rw-r--r--   0        0        0    25263 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/tasks/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/users/__init__.py
--rw-r--r--   0        0        0    17118 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/users/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     5199 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    13264 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/__init__.py
--rw-r--r--   0        0        0     2708 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/account.py
--rw-r--r--   0        0        0     1483 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/account_integration.py
--rw-r--r--   0        0        0     1916 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/account_request.py
--rw-r--r--   0        0        0      845 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/account_token.py
--rw-r--r--   0        0        0      719 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/activity_type_enum.py
--rw-r--r--   0        0        0    10978 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/address.py
--rw-r--r--   0        0        0      184 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/address_address_type.py
--rw-r--r--   0        0        0      167 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/address_country.py
--rw-r--r--   0        0        0    11024 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/address_request.py
--rw-r--r--   0        0        0      191 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/address_request_address_type.py
--rw-r--r--   0        0        0      174 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/address_request_country.py
--rw-r--r--   0        0        0      555 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/address_type_enum.py
--rw-r--r--   0        0        0     1226 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/association.py
--rw-r--r--   0        0        0      955 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/association_sub_type.py
--rw-r--r--   0        0        0     1663 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/association_type.py
--rw-r--r--   0        0        0      191 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/association_type_cardinality.py
--rw-r--r--   0        0        0     1335 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/association_type_request_request.py
--rw-r--r--   0        0        0     1245 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/available_actions.py
--rw-r--r--   0        0        0     1033 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/cardinality_enum.py
--rw-r--r--   0        0        0     1391 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     2324 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/condition_type_enum.py
--rw-r--r--   0        0        0     2324 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/contact.py
--rw-r--r--   0        0        0     1944 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/contact_request.py
--rw-r--r--   0        0        0    35178 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/country_enum.py
--rw-r--r--   0        0        0     1108 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/crm_account_response.py
--rw-r--r--   0        0        0     1141 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/crm_association_type_response.py
--rw-r--r--   0        0        0     1108 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/crm_contact_response.py
--rw-r--r--   0        0        0     1129 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/crm_custom_object_response.py
--rw-r--r--   0        0        0     1399 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/custom_object.py
--rw-r--r--   0        0        0     1520 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/custom_object_class.py
--rw-r--r--   0        0        0      782 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/custom_object_request.py
--rw-r--r--   0        0        0      870 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/debug_model_log_summary.py
--rw-r--r--   0        0        0      549 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/direction_enum.py
--rw-r--r--   0        0        0     1317 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/email_address.py
--rw-r--r--   0        0        0     1319 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/email_address_request.py
--rw-r--r--   0        0        0      522 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/encoding_enum.py
--rw-r--r--   0        0        0     2645 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement.py
--rw-r--r--   0        0        0      178 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_direction.py
--rw-r--r--   0        0        0     2216 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_request.py
--rw-r--r--   0        0        0      185 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_request_direction.py
--rw-r--r--   0        0        0     1117 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_response.py
--rw-r--r--   0        0        0     1866 2023-07-24 18:15:26.066730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_type.py
--rw-r--r--   0        0        0      195 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_type_activity_type.py
--rw-r--r--   0        0        0     3563 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagements_list_request_expand.py
--rw-r--r--   0        0        0     3627 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/engagements_retrieve_request_expand.py
--rw-r--r--   0        0        0      913 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/error_validation_problem.py
--rw-r--r--   0        0        0     1193 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/field_format_enum.py
--rw-r--r--   0        0        0     1179 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/field_type_enum.py
--rw-r--r--   0        0        0      999 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/ignore_common_model_request.py
--rw-r--r--   0        0        0     1323 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/issues_list_request_status.py
--rw-r--r--   0        0        0     1186 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/item_format_enum.py
--rw-r--r--   0        0        0      964 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/item_schema.py
--rw-r--r--   0        0        0     1172 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/item_type_enum.py
--rw-r--r--   0        0        0     2863 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/lead.py
--rw-r--r--   0        0        0     2369 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/lead_request.py
--rw-r--r--   0        0        0     1093 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/lead_response.py
--rw-r--r--   0        0        0     1851 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/leads_list_request_expand.py
--rw-r--r--   0        0        0     1883 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/leads_retrieve_request_expand.py
--rw-r--r--   0        0        0      835 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0     2150 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/note.py
--rw-r--r--   0        0        0     1590 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/note_request.py
--rw-r--r--   0        0        0     1093 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/note_response.py
--rw-r--r--   0        0        0     3267 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/notes_list_request_expand.py
--rw-r--r--   0        0        0     3331 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/notes_retrieve_request_expand.py
--rw-r--r--   0        0        0      925 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/object_class_description_request.py
--rw-r--r--   0        0        0      993 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/operator_schema.py
--rw-r--r--   0        0        0     1475 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunities_list_request_expand.py
--rw-r--r--   0        0        0      665 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunities_list_request_status.py
--rw-r--r--   0        0        0     1507 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunities_retrieve_request_expand.py
--rw-r--r--   0        0        0     2685 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity.py
--rw-r--r--   0        0        0     2243 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity_request.py
--rw-r--r--   0        0        0      208 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity_request_status.py
--rw-r--r--   0        0        0     1121 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity_response.py
--rw-r--r--   0        0        0      201 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity_status.py
--rw-r--r--   0        0        0      704 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity_status_enum.py
--rw-r--r--   0        0        0      893 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/origin_type_enum.py
--rw-r--r--   0        0        0      959 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      888 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_account_list.py
--rw-r--r--   0        0        0      904 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_association_list.py
--rw-r--r--   0        0        0      921 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_association_type_list.py
--rw-r--r--   0        0        0      921 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      888 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_contact_list.py
--rw-r--r--   0        0        0      930 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_custom_object_class_list.py
--rw-r--r--   0        0        0      909 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_custom_object_list.py
--rw-r--r--   0        0        0      900 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_engagement_list.py
--rw-r--r--   0        0        0      917 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_engagement_type_list.py
--rw-r--r--   0        0        0      880 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_issue_list.py
--rw-r--r--   0        0        0      876 2023-07-24 18:15:26.070730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_lead_list.py
--rw-r--r--   0        0        0      876 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_note_list.py
--rw-r--r--   0        0        0      904 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_opportunity_list.py
--rw-r--r--   0        0        0      926 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_remote_field_class_list.py
--rw-r--r--   0        0        0      880 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_stage_list.py
--rw-r--r--   0        0        0      901 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      876 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_task_list.py
--rw-r--r--   0        0        0      876 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_user_list.py
--rw-r--r--   0        0        0     1923 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_account_request.py
--rw-r--r--   0        0        0     1951 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_contact_request.py
--rw-r--r--   0        0        0     2245 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_engagement_request.py
--rw-r--r--   0        0        0      192 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_engagement_request_direction.py
--rw-r--r--   0        0        0     2272 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_opportunity_request.py
--rw-r--r--   0        0        0      215 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_opportunity_request_status.py
--rw-r--r--   0        0        0     2029 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_task_request.py
--rw-r--r--   0        0        0      187 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_task_request_status.py
--rw-r--r--   0        0        0     1307 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/phone_number.py
--rw-r--r--   0        0        0     1309 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/phone_number_request.py
--rw-r--r--   0        0        0      814 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/reason_enum.py
--rw-r--r--   0        0        0      802 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_data.py
--rw-r--r--   0        0        0      880 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field.py
--rw-r--r--   0        0        0     1284 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_class.py
--rw-r--r--   0        0        0     1722 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class.py
--rw-r--r--   0        0        0      213 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_field_format.py
--rw-r--r--   0        0        0      205 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_field_type.py
--rw-r--r--   0        0        0      911 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_item_schema.py
--rw-r--r--   0        0        0      825 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_request.py
--rw-r--r--   0        0        0      986 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_key.py
--rw-r--r--   0        0        0     1299 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_response.py
--rw-r--r--   0        0        0      723 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/response_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1694 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/stage.py
--rw-r--r--   0        0        0     1411 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     2429 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/task.py
--rw-r--r--   0        0        0     2000 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/task_request.py
--rw-r--r--   0        0        0      180 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/task_request_status.py
--rw-r--r--   0        0        0     1093 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/task_response.py
--rw-r--r--   0        0        0      173 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/task_status.py
--rw-r--r--   0        0        0      517 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/task_status_enum.py
--rw-r--r--   0        0        0     1531 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/tasks_list_request_expand.py
--rw-r--r--   0        0        0     1563 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/tasks_retrieve_request_expand.py
--rw-r--r--   0        0        0     1894 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/user.py
--rw-r--r--   0        0        0      762 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/validation_problem_source.py
--rw-r--r--   0        0        0      915 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/crm/types/webhook_receiver.py
--rw-r--r--   0        0        0    10290 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/__init__.py
--rw-r--r--   0        0        0     9511 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/client.py
--rw-r--r--   0        0        0     1106 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2418 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2658 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2496 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/bank_info/__init__.py
--rw-r--r--   0        0        0    15339 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/bank_info/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/benefits/__init__.py
--rw-r--r--   0        0        0    10821 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/benefits/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/companies/__init__.py
--rw-r--r--   0        0        0     9072 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/companies/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2161 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/employee_payroll_runs/__init__.py
--rw-r--r--   0        0        0    13612 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/employee_payroll_runs/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/employees/__init__.py
--rw-r--r--   0        0        0    30137 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/employees/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/employments/__init__.py
--rw-r--r--   0        0        0    14343 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/employments/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     3074 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2843 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/groups/__init__.py
--rw-r--r--   0        0        0    11861 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/groups/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/issues/__init__.py
--rw-r--r--   0        0        0    10570 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/link_token/__init__.py
--rw-r--r--   0        0        0     8922 2023-07-24 18:15:26.074730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0    10687 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/locations/__init__.py
--rw-r--r--   0        0        0    11629 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/locations/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     7380 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/pay_groups/__init__.py
--rw-r--r--   0        0        0     9094 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/pay_groups/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/payroll_runs/__init__.py
--rw-r--r--   0        0        0    15544 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/payroll_runs/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2853 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     8300 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     3396 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/teams/__init__.py
--rw-r--r--   0        0        0    10785 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/teams/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/time_off/__init__.py
--rw-r--r--   0        0        0    22208 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/time_off/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/time_off_balances/__init__.py
--rw-r--r--   0        0        0    15538 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/time_off_balances/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     5247 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    14549 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/__init__.py
--rw-r--r--   0        0        0     1483 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/account_token.py
--rw-r--r--   0        0        0      555 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/account_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/available_actions.py
--rw-r--r--   0        0        0     2399 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/bank_info.py
--rw-r--r--   0        0        0      185 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/bank_info_account_type.py
--rw-r--r--   0        0        0      529 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/bank_info_list_request_account_type.py
--rw-r--r--   0        0        0      728 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/bank_info_list_request_order_by.py
--rw-r--r--   0        0        0     2342 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/benefit.py
--rw-r--r--   0        0        0     1391 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     1962 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/company.py
--rw-r--r--   0        0        0     2324 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/condition_type_enum.py
--rw-r--r--   0        0        0    35178 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/country_enum.py
--rw-r--r--   0        0        0      870 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/debug_model_log_summary.py
--rw-r--r--   0        0        0     2140 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/deduction.py
--rw-r--r--   0        0        0     2143 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/earning.py
--rw-r--r--   0        0        0      177 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/earning_type.py
--rw-r--r--   0        0        0      949 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/earning_type_enum.py
--rw-r--r--   0        0        0     6788 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee.py
--rw-r--r--   0        0        0      205 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_employment_status.py
--rw-r--r--   0        0        0      176 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_ethnicity.py
--rw-r--r--   0        0        0      164 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_gender.py
--rw-r--r--   0        0        0      193 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_marital_status.py
--rw-r--r--   0        0        0     2796 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_payroll_run.py
--rw-r--r--   0        0        0      829 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py
--rw-r--r--   0        0        0      845 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py
--rw-r--r--   0        0        0     6252 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_request.py
--rw-r--r--   0        0        0      212 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_request_employment_status.py
--rw-r--r--   0        0        0      183 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_request_ethnicity.py
--rw-r--r--   0        0        0      171 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_request_gender.py
--rw-r--r--   0        0        0      200 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_request_marital_status.py
--rw-r--r--   0        0        0     1109 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_response.py
--rw-r--r--   0        0        0      739 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_list_request_employment_status.py
--rw-r--r--   0        0        0    80247 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_list_request_expand.py
--rw-r--r--   0        0        0     4067 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_list_request_remote_fields.py
--rw-r--r--   0        0        0     4115 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py
--rw-r--r--   0        0        0    81343 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_retrieve_request_expand.py
--rw-r--r--   0        0        0     4131 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     4179 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0    18682 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employment.py
--rw-r--r--   0        0        0      199 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_employment_type.py
--rw-r--r--   0        0        0      183 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_flsa_status.py
--rw-r--r--   0        0        0      187 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_pay_currency.py
--rw-r--r--   0        0        0      191 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_pay_frequency.py
--rw-r--r--   0        0        0      179 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_pay_period.py
--rw-r--r--   0        0        0      770 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_status_enum.py
--rw-r--r--   0        0        0     1166 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_type_enum.py
--rw-r--r--   0        0        0      777 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_list_request_expand.py
--rw-r--r--   0        0        0      707 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_list_request_order_by.py
--rw-r--r--   0        0        0     4219 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_list_request_remote_fields.py
--rw-r--r--   0        0        0     4267 2023-07-24 18:15:26.078730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      793 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_retrieve_request_expand.py
--rw-r--r--   0        0        0     4283 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     4331 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0      522 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/error_validation_problem.py
--rw-r--r--   0        0        0     2511 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/ethnicity_enum.py
--rw-r--r--   0        0        0      986 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/flsa_status_enum.py
--rw-r--r--   0        0        0     1146 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/gender_enum.py
--rw-r--r--   0        0        0     2225 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/group.py
--rw-r--r--   0        0        0      169 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/group_type.py
--rw-r--r--   0        0        0     1136 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/group_type_enum.py
--rw-r--r--   0        0        0      180 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/ignore_common_model_request_reason.py
--rw-r--r--   0        0        0     1323 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/issues_list_request_status.py
--rw-r--r--   0        0        0      835 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0    11870 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/location.py
--rw-r--r--   0        0        0      168 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/location_country.py
--rw-r--r--   0        0        0      189 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/location_location_type.py
--rw-r--r--   0        0        0      509 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/location_type_enum.py
--rw-r--r--   0        0        0     1685 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/marital_status_enum.py
--rw-r--r--   0        0        0     1037 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0      993 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/operator_schema.py
--rw-r--r--   0        0        0      959 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      893 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_bank_info_list.py
--rw-r--r--   0        0        0      888 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_benefit_list.py
--rw-r--r--   0        0        0      888 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_company_list.py
--rw-r--r--   0        0        0      921 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      892 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_employee_list.py
--rw-r--r--   0        0        0      934 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py
--rw-r--r--   0        0        0      900 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_employment_list.py
--rw-r--r--   0        0        0      880 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_group_list.py
--rw-r--r--   0        0        0      880 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_issue_list.py
--rw-r--r--   0        0        0      892 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_location_list.py
--rw-r--r--   0        0        0      893 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_pay_group_list.py
--rw-r--r--   0        0        0      901 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_payroll_run_list.py
--rw-r--r--   0        0        0      901 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      876 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_team_list.py
--rw-r--r--   0        0        0      918 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_time_off_balance_list.py
--rw-r--r--   0        0        0      889 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_time_off_list.py
--rw-r--r--   0        0        0    48882 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/pay_currency_enum.py
--rw-r--r--   0        0        0     1940 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/pay_frequency_enum.py
--rw-r--r--   0        0        0     1754 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/pay_group.py
--rw-r--r--   0        0        0     1798 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/pay_period_enum.py
--rw-r--r--   0        0        0     2811 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_run.py
--rw-r--r--   0        0        0      175 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_run_run_state.py
--rw-r--r--   0        0        0      171 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_run_run_type.py
--rw-r--r--   0        0        0      801 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py
--rw-r--r--   0        0        0     1104 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py
--rw-r--r--   0        0        0      813 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      817 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      829 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1305 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/policy_type_enum.py
--rw-r--r--   0        0        0      814 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/reason_enum.py
--rw-r--r--   0        0        0      802 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/remote_key.py
--rw-r--r--   0        0        0     1330 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/remote_response.py
--rw-r--r--   0        0        0      195 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/remote_response_response_type.py
--rw-r--r--   0        0        0      723 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/request_format_enum.py
--rw-r--r--   0        0        0     1312 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/request_type_enum.py
--rw-r--r--   0        0        0      562 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/response_type_enum.py
--rw-r--r--   0        0        0     1032 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/run_state_enum.py
--rw-r--r--   0        0        0     1173 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/run_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1975 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/tax.py
--rw-r--r--   0        0        0     1953 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/team.py
--rw-r--r--   0        0        0     3481 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off.py
--rw-r--r--   0        0        0     2517 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_balance.py
--rw-r--r--   0        0        0      187 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_balance_policy_type.py
--rw-r--r--   0        0        0     1272 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py
--rw-r--r--   0        0        0      751 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_expand.py
--rw-r--r--   0        0        0     1595 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_remote_fields.py
--rw-r--r--   0        0        0     1223 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_request_type.py
--rw-r--r--   0        0        0     1619 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     1029 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_status.py
--rw-r--r--   0        0        0     3199 2023-07-24 18:15:26.082730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_request.py
--rw-r--r--   0        0        0      191 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_request_request_type.py
--rw-r--r--   0        0        0      193 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_request_status.py
--rw-r--r--   0        0        0      184 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_request_type.py
--rw-r--r--   0        0        0      166 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_request_units.py
--rw-r--r--   0        0        0     1106 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_response.py
--rw-r--r--   0        0        0      767 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_retrieve_request_expand.py
--rw-r--r--   0        0        0     1627 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     1651 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0      186 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_status.py
--rw-r--r--   0        0        0     1146 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_status_enum.py
--rw-r--r--   0        0        0      159 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_units.py
--rw-r--r--   0        0        0      495 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/units_enum.py
--rw-r--r--   0        0        0      762 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/validation_problem_source.py
--rw-r--r--   0        0        0      915 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/hris/types/webhook_receiver.py
--rw-r--r--   0        0        0     7030 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/__init__.py
--rw-r--r--   0        0        0     8338 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/client.py
--rw-r--r--   0        0        0      946 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2394 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2634 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/accounts/__init__.py
--rw-r--r--   0        0        0     9020 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/attachments/__init__.py
--rw-r--r--   0        0        0    17085 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/attachments/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2472 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/collections/__init__.py
--rw-r--r--   0        0        0    19110 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/collections/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/comments/__init__.py
--rw-r--r--   0        0        0    15411 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/comments/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/contacts/__init__.py
--rw-r--r--   0        0        0    10333 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/contacts/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2137 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     3050 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2819 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/issues/__init__.py
--rw-r--r--   0        0        0    10522 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/link_token/__init__.py
--rw-r--r--   0        0        0     8898 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0    10663 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     7356 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/projects/__init__.py
--rw-r--r--   0        0        0    13470 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/projects/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2829 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     8228 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     3372 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/tags/__init__.py
--rw-r--r--   0        0        0     8930 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/tags/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/teams/__init__.py
--rw-r--r--   0        0        0     8952 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/teams/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/tickets/__init__.py
--rw-r--r--   0        0        0    41949 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/tickets/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/users/__init__.py
--rw-r--r--   0        0        0    10782 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/users/client.py
--rw-r--r--   0        0        0       65 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     5199 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0     9623 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/__init__.py
--rw-r--r--   0        0        0      743 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/access_level_enum.py
--rw-r--r--   0        0        0     1879 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account.py
--rw-r--r--   0        0        0     1483 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_token.py
--rw-r--r--   0        0        0     2201 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/attachment.py
--rw-r--r--   0        0        0     1716 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/attachment_request.py
--rw-r--r--   0        0        0     1245 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/available_actions.py
--rw-r--r--   0        0        0     1391 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/category_enum.py
--rw-r--r--   0        0        0     2535 2023-07-24 18:15:26.086730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collection.py
--rw-r--r--   0        0        0      187 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collection_access_level.py
--rw-r--r--   0        0        0      199 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collection_collection_type.py
--rw-r--r--   0        0        0      536 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collection_type_enum.py
--rw-r--r--   0        0        0      527 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collections_list_request_collection_type.py
--rw-r--r--   0        0        0      727 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collections_users_list_request_expand.py
--rw-r--r--   0        0        0     2161 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comment.py
--rw-r--r--   0        0        0     1693 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comment_request.py
--rw-r--r--   0        0        0     1105 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comment_response.py
--rw-r--r--   0        0        0     1435 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comments_list_request_expand.py
--rw-r--r--   0        0        0     1467 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comments_retrieve_request_expand.py
--rw-r--r--   0        0        0      997 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     2324 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/condition_type_enum.py
--rw-r--r--   0        0        0     2024 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/contact.py
--rw-r--r--   0        0        0      870 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/debug_model_log_summary.py
--rw-r--r--   0        0        0      522 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/error_validation_problem.py
--rw-r--r--   0        0        0     1193 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/field_format_enum.py
--rw-r--r--   0        0        0     1179 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/field_type_enum.py
--rw-r--r--   0        0        0     1323 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/issues_list_request_status.py
--rw-r--r--   0        0        0     1186 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/item_format_enum.py
--rw-r--r--   0        0        0      964 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/item_schema.py
--rw-r--r--   0        0        0     1172 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/item_type_enum.py
--rw-r--r--   0        0        0      835 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0      993 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/operator_schema.py
--rw-r--r--   0        0        0      959 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      888 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_account_list.py
--rw-r--r--   0        0        0      900 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_attachment_list.py
--rw-r--r--   0        0        0      900 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_collection_list.py
--rw-r--r--   0        0        0      888 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_comment_list.py
--rw-r--r--   0        0        0      921 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      888 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_contact_list.py
--rw-r--r--   0        0        0      880 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_issue_list.py
--rw-r--r--   0        0        0      888 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_project_list.py
--rw-r--r--   0        0        0      926 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_remote_field_class_list.py
--rw-r--r--   0        0        0      901 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      872 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_tag_list.py
--rw-r--r--   0        0        0      876 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_team_list.py
--rw-r--r--   0        0        0      884 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_ticket_list.py
--rw-r--r--   0        0        0      876 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_user_list.py
--rw-r--r--   0        0        0     3241 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/patched_ticket_request.py
--rw-r--r--   0        0        0      184 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/patched_ticket_request_priority.py
--rw-r--r--   0        0        0      195 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/patched_ticket_request_status.py
--rw-r--r--   0        0        0      843 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/priority_enum.py
--rw-r--r--   0        0        0     1704 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/project.py
--rw-r--r--   0        0        0      715 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/projects_users_list_request_expand.py
--rw-r--r--   0        0        0      802 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_data.py
--rw-r--r--   0        0        0      880 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_field.py
--rw-r--r--   0        0        0     1284 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_field_class.py
--rw-r--r--   0        0        0      825 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_field_request.py
--rw-r--r--   0        0        0      986 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_key.py
--rw-r--r--   0        0        0     1299 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_response.py
--rw-r--r--   0        0        0      723 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/response_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1559 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tag.py
--rw-r--r--   0        0        0     1705 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/team.py
--rw-r--r--   0        0        0     3778 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket.py
--rw-r--r--   0        0        0      170 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_priority.py
--rw-r--r--   0        0        0     3258 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_request.py
--rw-r--r--   0        0        0      177 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_request_priority.py
--rw-r--r--   0        0        0      188 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_request_status.py
--rw-r--r--   0        0        0     1101 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_response.py
--rw-r--r--   0        0        0      181 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_status.py
--rw-r--r--   0        0        0      926 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_status_enum.py
--rw-r--r--   0        0        0     1126 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticketing_attachment_response.py
--rw-r--r--   0        0        0      743 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_collaborators_list_request_expand.py
--rw-r--r--   0        0        0    37875 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_expand.py
--rw-r--r--   0        0        0      810 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_priority.py
--rw-r--r--   0        0        0     1635 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_remote_fields.py
--rw-r--r--   0        0        0     1659 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      845 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_status.py
--rw-r--r--   0        0        0    38387 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_retrieve_request_expand.py
--rw-r--r--   0        0        0     1667 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     1691 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1949 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/user.py
--rw-r--r--   0        0        0      683 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/users_list_request_expand.py
--rw-r--r--   0        0        0      699 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/users_retrieve_request_expand.py
--rw-r--r--   0        0        0      762 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/validation_problem_source.py
--rw-r--r--   0        0        0      915 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-24 18:15:26.090730 mergepythonclient-0.1.1/src/merge/resources/ticketing/types/webhook_receiver.py
--rw-r--r--   0        0        0     5686 1970-01-01 00:00:00.000000 mergepythonclient-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3275 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     4884 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/README.md
+-rw-r--r--   0        0        0      534 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      249 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/__init__.py
+-rw-r--r--   0        0        0     2459 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/client.py
+-rw-r--r--   0        0        0      519 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/core/api_error.py
+-rw-r--r--   0        0        0     1113 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      201 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/environment.py
+-rw-r--r--   0        0        0        0 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/py.typed
+-rw-r--r--   0        0        0      178 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/__init__.py
+-rw-r--r--   0        0        0    12630 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/__init__.py
+-rw-r--r--   0        0        0    12026 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/client.py
+-rw-r--r--   0        0        0     1410 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2430 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2670 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/accounts/__init__.py
+-rw-r--r--   0        0        0    18250 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/addresses/__init__.py
+-rw-r--r--   0        0        0     4508 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/addresses/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/attachments/__init__.py
+-rw-r--r--   0        0        0    14669 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/attachments/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2508 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/balance_sheets/__init__.py
+-rw-r--r--   0        0        0    10935 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/balance_sheets/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/cash_flow_statements/__init__.py
+-rw-r--r--   0        0        0    11063 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/cash_flow_statements/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/company_info/__init__.py
+-rw-r--r--   0        0        0    10594 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/company_info/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/contacts/__init__.py
+-rw-r--r--   0        0        0    17956 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/contacts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/credit_notes/__init__.py
+-rw-r--r--   0        0        0    14854 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/credit_notes/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2173 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/expenses/__init__.py
+-rw-r--r--   0        0        0    16615 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/expenses/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     3086 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2855 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/income_statements/__init__.py
+-rw-r--r--   0        0        0    11009 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/income_statements/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/invoices/__init__.py
+-rw-r--r--   0        0        0    20202 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/invoices/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/issues/__init__.py
+-rw-r--r--   0        0        0    10594 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/items/__init__.py
+-rw-r--r--   0        0        0    13155 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/items/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/journal_entries/__init__.py
+-rw-r--r--   0        0        0    16931 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/journal_entries/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     8934 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0    10699 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     7392 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/payments/__init__.py
+-rw-r--r--   0        0        0    17415 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/payments/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.118764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/phone_numbers/__init__.py
+-rw-r--r--   0        0        0     3317 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/phone_numbers/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/purchase_orders/__init__.py
+-rw-r--r--   0        0        0    19258 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/purchase_orders/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2865 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     8336 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     3408 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/tax_rates/__init__.py
+-rw-r--r--   0        0        0    10815 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/tax_rates/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/tracking_categories/__init__.py
+-rw-r--r--   0        0        0    13405 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/tracking_categories/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/transactions/__init__.py
+-rw-r--r--   0        0        0    12082 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/transactions/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/vendor_credits/__init__.py
+-rw-r--r--   0        0        0    12106 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/vendor_credits/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     5271 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    17717 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/__init__.py
+-rw-r--r--   0        0        0    17393 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/account.py
+-rw-r--r--   0        0        0      195 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_classification.py
+-rw-r--r--   0        0        0      171 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_currency.py
+-rw-r--r--   0        0        0     1483 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_integration.py
+-rw-r--r--   0        0        0    16986 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_request.py
+-rw-r--r--   0        0        0      202 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_request_classification.py
+-rw-r--r--   0        0        0      178 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_request_currency.py
+-rw-r--r--   0        0        0      192 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_request_status.py
+-rw-r--r--   0        0        0     1105 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_response.py
+-rw-r--r--   0        0        0      185 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_status.py
+-rw-r--r--   0        0        0      758 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_status_enum.py
+-rw-r--r--   0        0        0      845 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_token.py
+-rw-r--r--   0        0        0     1935 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounting_attachment.py
+-rw-r--r--   0        0        0     1462 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounting_attachment_request.py
+-rw-r--r--   0        0        0     1158 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounting_attachment_response.py
+-rw-r--r--   0        0        0     1344 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounting_phone_number.py
+-rw-r--r--   0        0        0     1346 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounting_phone_number_request.py
+-rw-r--r--   0        0        0      819 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounts_list_request_remote_fields.py
+-rw-r--r--   0        0        0      831 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounts_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      835 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounts_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      847 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounts_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0    11090 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/address.py
+-rw-r--r--   0        0        0      167 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/address_country.py
+-rw-r--r--   0        0        0      177 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/address_type.py
+-rw-r--r--   0        0        0      555 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/address_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/available_actions.py
+-rw-r--r--   0        0        0    16903 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/balance_sheet.py
+-rw-r--r--   0        0        0      176 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/balance_sheet_currency.py
+-rw-r--r--   0        0        0    17216 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/cash_flow_statement.py
+-rw-r--r--   0        0        0      181 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/cash_flow_statement_currency.py
+-rw-r--r--   0        0        0     1391 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/category_enum.py
+-rw-r--r--   0        0        0      560 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/category_type_enum.py
+-rw-r--r--   0        0        0     1103 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/classification_enum.py
+-rw-r--r--   0        0        0      997 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0    16863 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/company_info.py
+-rw-r--r--   0        0        0      175 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/company_info_currency.py
+-rw-r--r--   0        0        0      827 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/company_info_list_request_expand.py
+-rw-r--r--   0        0        0      843 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/company_info_retrieve_request_expand.py
+-rw-r--r--   0        0        0     2324 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/condition_type_enum.py
+-rw-r--r--   0        0        0     3027 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/contact.py
+-rw-r--r--   0        0        0     2478 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/contact_request.py
+-rw-r--r--   0        0        0      182 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/contact_request_status.py
+-rw-r--r--   0        0        0     1105 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/contact_response.py
+-rw-r--r--   0        0        0      175 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/contact_status.py
+-rw-r--r--   0        0        0     1675 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/contacts_list_request_expand.py
+-rw-r--r--   0        0        0     1707 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/contacts_retrieve_request_expand.py
+-rw-r--r--   0        0        0    35178 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/country_enum.py
+-rw-r--r--   0        0        0    17747 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_note.py
+-rw-r--r--   0        0        0      174 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_note_currency.py
+-rw-r--r--   0        0        0     2275 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_note_line_item.py
+-rw-r--r--   0        0        0      198 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_note_status.py
+-rw-r--r--   0        0        0      784 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_note_status_enum.py
+-rw-r--r--   0        0        0     1859 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_notes_list_request_expand.py
+-rw-r--r--   0        0        0      731 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_notes_list_request_remote_fields.py
+-rw-r--r--   0        0        0      743 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_notes_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1891 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_notes_retrieve_request_expand.py
+-rw-r--r--   0        0        0      747 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_notes_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      759 2023-07-26 18:26:59.122764 mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_notes_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0    47961 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/currency_enum.py
+-rw-r--r--   0        0        0      870 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0      522 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/error_validation_problem.py
+-rw-r--r--   0        0        0    16980 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/expense.py
+-rw-r--r--   0        0        0      171 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/expense_currency.py
+-rw-r--r--   0        0        0     2074 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/expense_line.py
+-rw-r--r--   0        0        0     2076 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/expense_line_request.py
+-rw-r--r--   0        0        0    16445 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/expense_request.py
+-rw-r--r--   0        0        0      178 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/expense_request_currency.py
+-rw-r--r--   0        0        0     1105 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/expense_response.py
+-rw-r--r--   0        0        0     3715 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/expenses_list_request_expand.py
+-rw-r--r--   0        0        0     3779 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/expenses_retrieve_request_expand.py
+-rw-r--r--   0        0        0    17240 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/income_statement.py
+-rw-r--r--   0        0        0      179 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/income_statement_currency.py
+-rw-r--r--   0        0        0    18003 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice.py
+-rw-r--r--   0        0        0      171 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice_currency.py
+-rw-r--r--   0        0        0    16460 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice_line_item.py
+-rw-r--r--   0        0        0      179 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice_line_item_currency.py
+-rw-r--r--   0        0        0    16389 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice_line_item_request.py
+-rw-r--r--   0        0        0      186 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice_line_item_request_currency.py
+-rw-r--r--   0        0        0    17620 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice_request.py
+-rw-r--r--   0        0        0      178 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice_request_currency.py
+-rw-r--r--   0        0        0      184 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice_request_type.py
+-rw-r--r--   0        0        0     1105 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice_response.py
+-rw-r--r--   0        0        0      177 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice_type.py
+-rw-r--r--   0        0        0      709 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice_type_enum.py
+-rw-r--r--   0        0        0     8275 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoices_list_request_expand.py
+-rw-r--r--   0        0        0      622 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoices_list_request_type.py
+-rw-r--r--   0        0        0     8403 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoices_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1323 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/issues_list_request_status.py
+-rw-r--r--   0        0        0     2624 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/item.py
+-rw-r--r--   0        0        0      172 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/item_status.py
+-rw-r--r--   0        0        0     1791 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/items_list_request_expand.py
+-rw-r--r--   0        0        0     1823 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/items_retrieve_request_expand.py
+-rw-r--r--   0        0        0     3771 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_entries_list_request_expand.py
+-rw-r--r--   0        0        0     3835 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_entries_retrieve_request_expand.py
+-rw-r--r--   0        0        0    17164 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_entry.py
+-rw-r--r--   0        0        0      176 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_entry_currency.py
+-rw-r--r--   0        0        0      197 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_entry_posting_status.py
+-rw-r--r--   0        0        0    16526 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_entry_request.py
+-rw-r--r--   0        0        0      183 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_entry_request_currency.py
+-rw-r--r--   0        0        0      204 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_entry_request_posting_status.py
+-rw-r--r--   0        0        0     1126 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_entry_response.py
+-rw-r--r--   0        0        0     1790 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_line.py
+-rw-r--r--   0        0        0     1792 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_line_request.py
+-rw-r--r--   0        0        0      835 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0      993 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/operator_schema.py
+-rw-r--r--   0        0        0      959 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_account_list.py
+-rw-r--r--   0        0        0      941 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_accounting_attachment_list.py
+-rw-r--r--   0        0        0      909 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_balance_sheet_list.py
+-rw-r--r--   0        0        0      930 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_cash_flow_statement_list.py
+-rw-r--r--   0        0        0      905 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_company_info_list.py
+-rw-r--r--   0        0        0      921 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_contact_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_credit_note_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_expense_list.py
+-rw-r--r--   0        0        0      921 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_income_statement_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_invoice_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_item_list.py
+-rw-r--r--   0        0        0      909 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_journal_entry_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_payment_list.py
+-rw-r--r--   0        0        0      913 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_purchase_order_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      889 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_tax_rate_list.py
+-rw-r--r--   0        0        0      925 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_tracking_category_list.py
+-rw-r--r--   0        0        0      904 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_transaction_list.py
+-rw-r--r--   0        0        0      909 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_vendor_credit_list.py
+-rw-r--r--   0        0        0    16832 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/payment.py
+-rw-r--r--   0        0        0      171 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/payment_currency.py
+-rw-r--r--   0        0        0    16241 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/payment_request.py
+-rw-r--r--   0        0        0      178 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/payment_request_currency.py
+-rw-r--r--   0        0        0     1105 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/payment_response.py
+-rw-r--r--   0        0        0     3715 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/payments_list_request_expand.py
+-rw-r--r--   0        0        0     3779 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/payments_retrieve_request_expand.py
+-rw-r--r--   0        0        0      554 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/posting_status_enum.py
+-rw-r--r--   0        0        0    17816 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order.py
+-rw-r--r--   0        0        0      177 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order_currency.py
+-rw-r--r--   0        0        0    16830 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order_line_item.py
+-rw-r--r--   0        0        0      185 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order_line_item_currency.py
+-rw-r--r--   0        0        0    16854 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order_line_item_request.py
+-rw-r--r--   0        0        0      192 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order_line_item_request_currency.py
+-rw-r--r--   0        0        0    17041 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order_request.py
+-rw-r--r--   0        0        0      184 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order_request_currency.py
+-rw-r--r--   0        0        0      217 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order_request_status.py
+-rw-r--r--   0        0        0     1130 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order_response.py
+-rw-r--r--   0        0        0      210 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order_status.py
+-rw-r--r--   0        0        0     1154 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order_status_enum.py
+-rw-r--r--   0        0        0     9043 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_orders_list_request_expand.py
+-rw-r--r--   0        0        0     9171 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_orders_retrieve_request_expand.py
+-rw-r--r--   0        0        0      802 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/remote_key.py
+-rw-r--r--   0        0        0     1299 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/remote_response.py
+-rw-r--r--   0        0        0     1649 2023-07-26 18:26:59.126765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/report_item.py
+-rw-r--r--   0        0        0      723 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/response_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0      542 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/status_7_d_1_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     2002 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/tax_rate.py
+-rw-r--r--   0        0        0     2481 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/tracking_category.py
+-rw-r--r--   0        0        0      197 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/tracking_category_category_type.py
+-rw-r--r--   0        0        0      184 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/tracking_category_status.py
+-rw-r--r--   0        0        0    17229 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/transaction.py
+-rw-r--r--   0        0        0      175 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/transaction_currency.py
+-rw-r--r--   0        0        0    16685 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/transaction_line_item.py
+-rw-r--r--   0        0        0      183 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/transaction_line_item_currency.py
+-rw-r--r--   0        0        0     3899 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/transactions_list_request_expand.py
+-rw-r--r--   0        0        0     3963 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/transactions_retrieve_request_expand.py
+-rw-r--r--   0        0        0      762 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/validation_problem_source.py
+-rw-r--r--   0        0        0    16901 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/vendor_credit.py
+-rw-r--r--   0        0        0      176 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/vendor_credit_currency.py
+-rw-r--r--   0        0        0     1999 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/vendor_credit_line.py
+-rw-r--r--   0        0        0     3675 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/vendor_credits_list_request_expand.py
+-rw-r--r--   0        0        0     3739 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/vendor_credits_retrieve_request_expand.py
+-rw-r--r--   0        0        0      915 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/accounting/types/webhook_receiver.py
+-rw-r--r--   0        0        0     9656 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/__init__.py
+-rw-r--r--   0        0        0    10018 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/client.py
+-rw-r--r--   0        0        0     1144 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2416 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2656 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/activities/__init__.py
+-rw-r--r--   0        0        0    18450 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/activities/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/applications/__init__.py
+-rw-r--r--   0        0        0    22753 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/applications/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/attachments/__init__.py
+-rw-r--r--   0        0        0    18326 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/attachments/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2494 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/candidates/__init__.py
+-rw-r--r--   0        0        0    25052 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/candidates/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2159 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/departments/__init__.py
+-rw-r--r--   0        0        0     9128 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/departments/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/eeocs/__init__.py
+-rw-r--r--   0        0        0    13425 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/eeocs/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     3072 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2841 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/interviews/__init__.py
+-rw-r--r--   0        0        0    19472 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/interviews/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/issues/__init__.py
+-rw-r--r--   0        0        0    10566 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/job_interview_stages/__init__.py
+-rw-r--r--   0        0        0    10955 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/job_interview_stages/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/jobs/__init__.py
+-rw-r--r--   0        0        0    14939 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/jobs/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     8920 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0    10685 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/offers/__init__.py
+-rw-r--r--   0        0        0    13609 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/offers/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/offices/__init__.py
+-rw-r--r--   0        0        0     9042 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/offices/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     7378 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2851 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/reject_reasons/__init__.py
+-rw-r--r--   0        0        0     9178 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/reject_reasons/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/scorecards/__init__.py
+-rw-r--r--   0        0        0    14473 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/scorecards/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     8294 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     3394 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/tags/__init__.py
+-rw-r--r--   0        0        0     6731 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/tags/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/users/__init__.py
+-rw-r--r--   0        0        0    11995 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/users/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     5243 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    13447 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/types/__init__.py
+-rw-r--r--   0        0        0     1240 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/types/access_role_enum.py
+-rw-r--r--   0        0        0     1483 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/types/account_token.py
+-rw-r--r--   0        0        0      857 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/types/activities_list_request_remote_fields.py
+-rw-r--r--   0        0        0      869 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      873 2023-07-26 18:26:59.130765 mergepythonclient-0.1.2/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      885 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     2705 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/activity.py
+-rw-r--r--   0        0        0      189 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/activity_activity_type.py
+-rw-r--r--   0        0        0     2155 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/activity_request.py
+-rw-r--r--   0        0        0      196 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/activity_request_activity_type.py
+-rw-r--r--   0        0        0      187 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/activity_request_visibility.py
+-rw-r--r--   0        0        0     1109 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/activity_response.py
+-rw-r--r--   0        0        0      705 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/activity_type_enum.py
+-rw-r--r--   0        0        0      180 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/activity_visibility.py
+-rw-r--r--   0        0        0     2473 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/application.py
+-rw-r--r--   0        0        0     2269 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/application_request.py
+-rw-r--r--   0        0        0     1121 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/application_response.py
+-rw-r--r--   0        0        0     8243 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/applications_list_request_expand.py
+-rw-r--r--   0        0        0     8371 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/applications_retrieve_request_expand.py
+-rw-r--r--   0        0        0     2146 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/attachment.py
+-rw-r--r--   0        0        0      199 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/attachment_attachment_type.py
+-rw-r--r--   0        0        0     1820 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/attachment_request.py
+-rw-r--r--   0        0        0      206 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/attachment_request_attachment_type.py
+-rw-r--r--   0        0        0     1117 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/attachment_response.py
+-rw-r--r--   0        0        0      985 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/attachment_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/available_actions.py
+-rw-r--r--   0        0        0     3471 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/candidate.py
+-rw-r--r--   0        0        0     3061 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/candidate_request.py
+-rw-r--r--   0        0        0     1113 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/candidate_response.py
+-rw-r--r--   0        0        0      833 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/candidates_list_request_expand.py
+-rw-r--r--   0        0        0      849 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/candidates_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1391 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     2324 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/condition_type_enum.py
+-rw-r--r--   0        0        0      870 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0     1698 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/department.py
+-rw-r--r--   0        0        0     1337 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/disability_status_enum.py
+-rw-r--r--   0        0        0     4088 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/eeoc.py
+-rw-r--r--   0        0        0      201 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/eeoc_disability_status.py
+-rw-r--r--   0        0        0      160 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/eeoc_gender.py
+-rw-r--r--   0        0        0      152 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/eeoc_race.py
+-rw-r--r--   0        0        0      189 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/eeoc_veteran_status.py
+-rw-r--r--   0        0        0     3803 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py
+-rw-r--r--   0        0        0     3851 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     3867 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     3915 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1529 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/email_address.py
+-rw-r--r--   0        0        0      210 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/email_address_email_address_type.py
+-rw-r--r--   0        0        0     1553 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/email_address_request.py
+-rw-r--r--   0        0        0      217 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/email_address_request_email_address_type.py
+-rw-r--r--   0        0        0      742 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/email_address_type_enum.py
+-rw-r--r--   0        0        0      522 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/error_validation_problem.py
+-rw-r--r--   0        0        0     1160 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/gender_enum.py
+-rw-r--r--   0        0        0     4187 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/interviews_list_request_expand.py
+-rw-r--r--   0        0        0     4251 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/interviews_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1323 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/issues_list_request_status.py
+-rw-r--r--   0        0        0     3428 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/job.py
+-rw-r--r--   0        0        0     2387 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/job_interview_stage.py
+-rw-r--r--   0        0        0      169 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/job_status.py
+-rw-r--r--   0        0        0     1045 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/job_status_enum.py
+-rw-r--r--   0        0        0     3771 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/jobs_list_request_expand.py
+-rw-r--r--   0        0        0      956 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/jobs_list_request_status.py
+-rw-r--r--   0        0        0     3835 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/jobs_retrieve_request_expand.py
+-rw-r--r--   0        0        0      835 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0     2786 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/offer.py
+-rw-r--r--   0        0        0      177 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/offer_status.py
+-rw-r--r--   0        0        0     1832 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/offer_status_enum.py
+-rw-r--r--   0        0        0      767 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/offers_list_request_expand.py
+-rw-r--r--   0        0        0      783 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/offers_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1817 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/office.py
+-rw-r--r--   0        0        0      993 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/operator_schema.py
+-rw-r--r--   0        0        0     1180 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/overall_recommendation_enum.py
+-rw-r--r--   0        0        0      959 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      892 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_activity_list.py
+-rw-r--r--   0        0        0      904 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_application_list.py
+-rw-r--r--   0        0        0      900 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_attachment_list.py
+-rw-r--r--   0        0        0      896 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_candidate_list.py
+-rw-r--r--   0        0        0      921 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      900 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_department_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_eeoc_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      930 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_job_interview_stage_list.py
+-rw-r--r--   0        0        0      872 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_job_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_offer_list.py
+-rw-r--r--   0        0        0      884 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_office_list.py
+-rw-r--r--   0        0        0      909 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_reject_reason_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_remote_user_list.py
+-rw-r--r--   0        0        0      933 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_scheduled_interview_list.py
+-rw-r--r--   0        0        0      896 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_scorecard_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      872 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_tag_list.py
+-rw-r--r--   0        0        0     3068 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/patched_candidate_request.py
+-rw-r--r--   0        0        0     1624 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/phone_number.py
+-rw-r--r--   0        0        0      205 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/phone_number_phone_number_type.py
+-rw-r--r--   0        0        0     1648 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/phone_number_request.py
+-rw-r--r--   0        0        0      212 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/phone_number_request_phone_number_type.py
+-rw-r--r--   0        0        0     1039 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/phone_number_type_enum.py
+-rw-r--r--   0        0        0     2326 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/race_enum.py
+-rw-r--r--   0        0        0      814 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/reason_enum.py
+-rw-r--r--   0        0        0     1775 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/reject_reason.py
+-rw-r--r--   0        0        0      802 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/remote_key.py
+-rw-r--r--   0        0        0     1330 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/remote_response.py
+-rw-r--r--   0        0        0      195 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/remote_response_response_type.py
+-rw-r--r--   0        0        0     2562 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/remote_user.py
+-rw-r--r--   0        0        0      183 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/remote_user_access_role.py
+-rw-r--r--   0        0        0      723 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/response_type_enum.py
+-rw-r--r--   0        0        0     3187 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/scheduled_interview.py
+-rw-r--r--   0        0        0     2464 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/scheduled_interview_request.py
+-rw-r--r--   0        0        0      237 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/scheduled_interview_request_status.py
+-rw-r--r--   0        0        0     1150 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/scheduled_interview_response.py
+-rw-r--r--   0        0        0      230 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/scheduled_interview_status.py
+-rw-r--r--   0        0        0      893 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/scheduled_interview_status_enum.py
+-rw-r--r--   0        0        0     2692 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/scorecard.py
+-rw-r--r--   0        0        0      226 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/scorecard_overall_recommendation.py
+-rw-r--r--   0        0        0     1731 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/scorecards_list_request_expand.py
+-rw-r--r--   0        0        0     1763 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py
+-rw-r--r--   0        0        0      695 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1623 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/tag.py
+-rw-r--r--   0        0        0     1659 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/url.py
+-rw-r--r--   0        0        0     1683 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/url_request.py
+-rw-r--r--   0        0        0      171 2023-07-26 18:26:59.134765 mergepythonclient-0.1.2/src/merge/resources/ats/types/url_request_url_type.py
+-rw-r--r--   0        0        0     1451 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/ats/types/url_type_enum.py
+-rw-r--r--   0        0        0      164 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/ats/types/url_url_type.py
+-rw-r--r--   0        0        0      762 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/ats/types/validation_problem_source.py
+-rw-r--r--   0        0        0     1467 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/ats/types/veteran_status_enum.py
+-rw-r--r--   0        0        0      760 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/ats/types/visibility_enum.py
+-rw-r--r--   0        0        0      915 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/ats/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/ats/types/webhook_receiver.py
+-rw-r--r--   0        0        0     9538 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/__init__.py
+-rw-r--r--   0        0        0     9931 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/client.py
+-rw-r--r--   0        0        0     1144 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2416 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2656 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/accounts/__init__.py
+-rw-r--r--   0        0        0    25993 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/association_types/__init__.py
+-rw-r--r--   0        0        0    17340 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/association_types/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/associations/__init__.py
+-rw-r--r--   0        0        0    12477 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/associations/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2494 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/contacts/__init__.py
+-rw-r--r--   0        0        0    28327 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/contacts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/custom_object_classes/__init__.py
+-rw-r--r--   0        0        0    13387 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/custom_object_classes/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/custom_objects/__init__.py
+-rw-r--r--   0        0        0    22608 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/custom_objects/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2159 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/engagement_types/__init__.py
+-rw-r--r--   0        0        0    15005 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/engagement_types/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/engagements/__init__.py
+-rw-r--r--   0        0        0    25867 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/engagements/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     3072 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2841 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/issues/__init__.py
+-rw-r--r--   0        0        0    10566 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/leads/__init__.py
+-rw-r--r--   0        0        0    22118 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/leads/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     8920 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0    10685 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/notes/__init__.py
+-rw-r--r--   0        0        0    22396 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/notes/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/opportunities/__init__.py
+-rw-r--r--   0        0        0    30544 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/opportunities/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     7378 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2851 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     8294 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/stages/__init__.py
+-rw-r--r--   0        0        0    14779 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/stages/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     3394 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/tasks/__init__.py
+-rw-r--r--   0        0        0    25417 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/tasks/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/users/__init__.py
+-rw-r--r--   0        0        0    17206 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/users/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     5243 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    13264 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/__init__.py
+-rw-r--r--   0        0        0     2708 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/account.py
+-rw-r--r--   0        0        0     1483 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/account_integration.py
+-rw-r--r--   0        0        0     1916 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/account_request.py
+-rw-r--r--   0        0        0      845 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/account_token.py
+-rw-r--r--   0        0        0      719 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/activity_type_enum.py
+-rw-r--r--   0        0        0    10978 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/address.py
+-rw-r--r--   0        0        0      184 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/address_address_type.py
+-rw-r--r--   0        0        0      167 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/address_country.py
+-rw-r--r--   0        0        0    11024 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/address_request.py
+-rw-r--r--   0        0        0      191 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/address_request_address_type.py
+-rw-r--r--   0        0        0      174 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/address_request_country.py
+-rw-r--r--   0        0        0      555 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/address_type_enum.py
+-rw-r--r--   0        0        0     1226 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/association.py
+-rw-r--r--   0        0        0      955 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/association_sub_type.py
+-rw-r--r--   0        0        0     1663 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/association_type.py
+-rw-r--r--   0        0        0      191 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/association_type_cardinality.py
+-rw-r--r--   0        0        0     1335 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/association_type_request_request.py
+-rw-r--r--   0        0        0     1245 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/available_actions.py
+-rw-r--r--   0        0        0     1033 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/cardinality_enum.py
+-rw-r--r--   0        0        0     1391 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     2324 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/condition_type_enum.py
+-rw-r--r--   0        0        0     2324 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/contact.py
+-rw-r--r--   0        0        0     1944 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/contact_request.py
+-rw-r--r--   0        0        0    35178 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/country_enum.py
+-rw-r--r--   0        0        0     1108 2023-07-26 18:26:59.138765 mergepythonclient-0.1.2/src/merge/resources/crm/types/crm_account_response.py
+-rw-r--r--   0        0        0     1141 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/crm_association_type_response.py
+-rw-r--r--   0        0        0     1108 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/crm_contact_response.py
+-rw-r--r--   0        0        0     1129 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/crm_custom_object_response.py
+-rw-r--r--   0        0        0     1399 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/custom_object.py
+-rw-r--r--   0        0        0     1520 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/custom_object_class.py
+-rw-r--r--   0        0        0      782 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/custom_object_request.py
+-rw-r--r--   0        0        0      870 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0      549 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/direction_enum.py
+-rw-r--r--   0        0        0     1317 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/email_address.py
+-rw-r--r--   0        0        0     1319 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/email_address_request.py
+-rw-r--r--   0        0        0      522 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/encoding_enum.py
+-rw-r--r--   0        0        0     2645 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/engagement.py
+-rw-r--r--   0        0        0      178 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/engagement_direction.py
+-rw-r--r--   0        0        0     2216 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/engagement_request.py
+-rw-r--r--   0        0        0      185 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/engagement_request_direction.py
+-rw-r--r--   0        0        0     1117 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/engagement_response.py
+-rw-r--r--   0        0        0     1866 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/engagement_type.py
+-rw-r--r--   0        0        0      195 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/engagement_type_activity_type.py
+-rw-r--r--   0        0        0     3563 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/engagements_list_request_expand.py
+-rw-r--r--   0        0        0     3627 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/engagements_retrieve_request_expand.py
+-rw-r--r--   0        0        0      913 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/error_validation_problem.py
+-rw-r--r--   0        0        0     1193 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/field_format_enum.py
+-rw-r--r--   0        0        0     1179 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/field_type_enum.py
+-rw-r--r--   0        0        0      999 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/ignore_common_model_request.py
+-rw-r--r--   0        0        0     1323 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/issues_list_request_status.py
+-rw-r--r--   0        0        0     1186 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/item_format_enum.py
+-rw-r--r--   0        0        0      964 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/item_schema.py
+-rw-r--r--   0        0        0     1172 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/item_type_enum.py
+-rw-r--r--   0        0        0     2863 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/lead.py
+-rw-r--r--   0        0        0     2369 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/lead_request.py
+-rw-r--r--   0        0        0     1093 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/lead_response.py
+-rw-r--r--   0        0        0     1851 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/leads_list_request_expand.py
+-rw-r--r--   0        0        0     1883 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/leads_retrieve_request_expand.py
+-rw-r--r--   0        0        0      835 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0     2150 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/note.py
+-rw-r--r--   0        0        0     1590 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/note_request.py
+-rw-r--r--   0        0        0     1093 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/note_response.py
+-rw-r--r--   0        0        0     3267 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/notes_list_request_expand.py
+-rw-r--r--   0        0        0     3331 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/notes_retrieve_request_expand.py
+-rw-r--r--   0        0        0      925 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/object_class_description_request.py
+-rw-r--r--   0        0        0      993 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/operator_schema.py
+-rw-r--r--   0        0        0     1475 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/opportunities_list_request_expand.py
+-rw-r--r--   0        0        0      665 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/opportunities_list_request_status.py
+-rw-r--r--   0        0        0     1507 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/opportunities_retrieve_request_expand.py
+-rw-r--r--   0        0        0     2685 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/opportunity.py
+-rw-r--r--   0        0        0     2243 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/opportunity_request.py
+-rw-r--r--   0        0        0      208 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/opportunity_request_status.py
+-rw-r--r--   0        0        0     1121 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/opportunity_response.py
+-rw-r--r--   0        0        0      201 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/opportunity_status.py
+-rw-r--r--   0        0        0      704 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/opportunity_status_enum.py
+-rw-r--r--   0        0        0      893 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/origin_type_enum.py
+-rw-r--r--   0        0        0      959 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_account_list.py
+-rw-r--r--   0        0        0      904 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_association_list.py
+-rw-r--r--   0        0        0      921 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_association_type_list.py
+-rw-r--r--   0        0        0      921 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_contact_list.py
+-rw-r--r--   0        0        0      930 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_custom_object_class_list.py
+-rw-r--r--   0        0        0      909 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_custom_object_list.py
+-rw-r--r--   0        0        0      900 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_engagement_list.py
+-rw-r--r--   0        0        0      917 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_engagement_type_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_lead_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_note_list.py
+-rw-r--r--   0        0        0      904 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_opportunity_list.py
+-rw-r--r--   0        0        0      926 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_remote_field_class_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_stage_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_task_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_user_list.py
+-rw-r--r--   0        0        0     1923 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/patched_account_request.py
+-rw-r--r--   0        0        0     1951 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/patched_contact_request.py
+-rw-r--r--   0        0        0     2245 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/patched_engagement_request.py
+-rw-r--r--   0        0        0      192 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/patched_engagement_request_direction.py
+-rw-r--r--   0        0        0     2272 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/patched_opportunity_request.py
+-rw-r--r--   0        0        0      215 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/patched_opportunity_request_status.py
+-rw-r--r--   0        0        0     2029 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/patched_task_request.py
+-rw-r--r--   0        0        0      187 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/patched_task_request_status.py
+-rw-r--r--   0        0        0     1307 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/phone_number.py
+-rw-r--r--   0        0        0     1309 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/phone_number_request.py
+-rw-r--r--   0        0        0      814 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/reason_enum.py
+-rw-r--r--   0        0        0      802 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_data.py
+-rw-r--r--   0        0        0      880 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_field.py
+-rw-r--r--   0        0        0     1284 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_field_class.py
+-rw-r--r--   0        0        0     1722 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_field_class_for_custom_object_class.py
+-rw-r--r--   0        0        0      213 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_field_format.py
+-rw-r--r--   0        0        0      205 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_field_type.py
+-rw-r--r--   0        0        0      911 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_item_schema.py
+-rw-r--r--   0        0        0      825 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_field_request.py
+-rw-r--r--   0        0        0      986 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_key.py
+-rw-r--r--   0        0        0     1299 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_response.py
+-rw-r--r--   0        0        0      723 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/response_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1694 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/stage.py
+-rw-r--r--   0        0        0     1411 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     2429 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/task.py
+-rw-r--r--   0        0        0     2000 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/task_request.py
+-rw-r--r--   0        0        0      180 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/task_request_status.py
+-rw-r--r--   0        0        0     1093 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/task_response.py
+-rw-r--r--   0        0        0      173 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/task_status.py
+-rw-r--r--   0        0        0      517 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/task_status_enum.py
+-rw-r--r--   0        0        0     1531 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/tasks_list_request_expand.py
+-rw-r--r--   0        0        0     1563 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/tasks_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1894 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/user.py
+-rw-r--r--   0        0        0      762 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/validation_problem_source.py
+-rw-r--r--   0        0        0      915 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/crm/types/webhook_receiver.py
+-rw-r--r--   0        0        0    10290 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/hris/__init__.py
+-rw-r--r--   0        0        0     9511 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/hris/client.py
+-rw-r--r--   0        0        0     1106 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2418 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2658 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2496 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.142765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/bank_info/__init__.py
+-rw-r--r--   0        0        0    15339 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/bank_info/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/benefits/__init__.py
+-rw-r--r--   0        0        0    10821 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/benefits/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/companies/__init__.py
+-rw-r--r--   0        0        0     9072 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/companies/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2161 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/employee_payroll_runs/__init__.py
+-rw-r--r--   0        0        0    13612 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/employee_payroll_runs/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/employees/__init__.py
+-rw-r--r--   0        0        0    30137 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/employees/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/employments/__init__.py
+-rw-r--r--   0        0        0    14343 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/employments/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     3074 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2843 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/groups/__init__.py
+-rw-r--r--   0        0        0    11861 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/groups/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/issues/__init__.py
+-rw-r--r--   0        0        0    10570 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     8922 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0    10687 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/locations/__init__.py
+-rw-r--r--   0        0        0    11629 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/locations/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     7380 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/pay_groups/__init__.py
+-rw-r--r--   0        0        0     9094 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/pay_groups/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/payroll_runs/__init__.py
+-rw-r--r--   0        0        0    15544 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/payroll_runs/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2853 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     8300 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     3396 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/teams/__init__.py
+-rw-r--r--   0        0        0    10785 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/teams/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/time_off/__init__.py
+-rw-r--r--   0        0        0    22208 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/time_off/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/time_off_balances/__init__.py
+-rw-r--r--   0        0        0    15538 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/time_off_balances/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     5247 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    14549 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/account_token.py
+-rw-r--r--   0        0        0      555 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/account_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/available_actions.py
+-rw-r--r--   0        0        0     2399 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/bank_info.py
+-rw-r--r--   0        0        0      185 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/bank_info_account_type.py
+-rw-r--r--   0        0        0      529 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/bank_info_list_request_account_type.py
+-rw-r--r--   0        0        0      728 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/bank_info_list_request_order_by.py
+-rw-r--r--   0        0        0     2342 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/benefit.py
+-rw-r--r--   0        0        0     1391 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     1962 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/company.py
+-rw-r--r--   0        0        0     2324 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/condition_type_enum.py
+-rw-r--r--   0        0        0    35178 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/country_enum.py
+-rw-r--r--   0        0        0      870 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0     2140 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/deduction.py
+-rw-r--r--   0        0        0     2143 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/earning.py
+-rw-r--r--   0        0        0      177 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/earning_type.py
+-rw-r--r--   0        0        0      949 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/earning_type_enum.py
+-rw-r--r--   0        0        0     6788 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employee.py
+-rw-r--r--   0        0        0      205 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_employment_status.py
+-rw-r--r--   0        0        0      176 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_ethnicity.py
+-rw-r--r--   0        0        0      164 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_gender.py
+-rw-r--r--   0        0        0      193 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_marital_status.py
+-rw-r--r--   0        0        0     2796 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_payroll_run.py
+-rw-r--r--   0        0        0      829 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py
+-rw-r--r--   0        0        0      845 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py
+-rw-r--r--   0        0        0     6252 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_request.py
+-rw-r--r--   0        0        0      212 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_request_employment_status.py
+-rw-r--r--   0        0        0      183 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_request_ethnicity.py
+-rw-r--r--   0        0        0      171 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_request_gender.py
+-rw-r--r--   0        0        0      200 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_request_marital_status.py
+-rw-r--r--   0        0        0     1109 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_response.py
+-rw-r--r--   0        0        0      739 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employees_list_request_employment_status.py
+-rw-r--r--   0        0        0    80247 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employees_list_request_expand.py
+-rw-r--r--   0        0        0     4067 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employees_list_request_remote_fields.py
+-rw-r--r--   0        0        0     4115 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0    81343 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employees_retrieve_request_expand.py
+-rw-r--r--   0        0        0     4131 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     4179 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0    18682 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employment.py
+-rw-r--r--   0        0        0      199 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employment_employment_type.py
+-rw-r--r--   0        0        0      183 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employment_flsa_status.py
+-rw-r--r--   0        0        0      187 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employment_pay_currency.py
+-rw-r--r--   0        0        0      191 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employment_pay_frequency.py
+-rw-r--r--   0        0        0      179 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employment_pay_period.py
+-rw-r--r--   0        0        0      770 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employment_status_enum.py
+-rw-r--r--   0        0        0     1166 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employment_type_enum.py
+-rw-r--r--   0        0        0      777 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employments_list_request_expand.py
+-rw-r--r--   0        0        0      707 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employments_list_request_order_by.py
+-rw-r--r--   0        0        0     4219 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employments_list_request_remote_fields.py
+-rw-r--r--   0        0        0     4267 2023-07-26 18:26:59.146765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      793 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employments_retrieve_request_expand.py
+-rw-r--r--   0        0        0     4283 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     4331 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0      522 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/error_validation_problem.py
+-rw-r--r--   0        0        0     2511 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/ethnicity_enum.py
+-rw-r--r--   0        0        0      986 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/flsa_status_enum.py
+-rw-r--r--   0        0        0     1146 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/gender_enum.py
+-rw-r--r--   0        0        0     2225 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/group.py
+-rw-r--r--   0        0        0      169 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/group_type.py
+-rw-r--r--   0        0        0     1136 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/group_type_enum.py
+-rw-r--r--   0        0        0      180 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/ignore_common_model_request_reason.py
+-rw-r--r--   0        0        0     1323 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/issues_list_request_status.py
+-rw-r--r--   0        0        0      835 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0    11870 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/location.py
+-rw-r--r--   0        0        0      168 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/location_country.py
+-rw-r--r--   0        0        0      189 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/location_location_type.py
+-rw-r--r--   0        0        0      509 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/location_type_enum.py
+-rw-r--r--   0        0        0     1685 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/marital_status_enum.py
+-rw-r--r--   0        0        0     1037 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0      993 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/operator_schema.py
+-rw-r--r--   0        0        0      959 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      893 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_bank_info_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_benefit_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_company_list.py
+-rw-r--r--   0        0        0      921 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      892 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_employee_list.py
+-rw-r--r--   0        0        0      934 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py
+-rw-r--r--   0        0        0      900 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_employment_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_group_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      892 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_location_list.py
+-rw-r--r--   0        0        0      893 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_pay_group_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_payroll_run_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_team_list.py
+-rw-r--r--   0        0        0      918 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_time_off_balance_list.py
+-rw-r--r--   0        0        0      889 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_time_off_list.py
+-rw-r--r--   0        0        0    48882 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/pay_currency_enum.py
+-rw-r--r--   0        0        0     1940 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/pay_frequency_enum.py
+-rw-r--r--   0        0        0     1754 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/pay_group.py
+-rw-r--r--   0        0        0     1798 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/pay_period_enum.py
+-rw-r--r--   0        0        0     2811 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/payroll_run.py
+-rw-r--r--   0        0        0      175 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/payroll_run_run_state.py
+-rw-r--r--   0        0        0      171 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/payroll_run_run_type.py
+-rw-r--r--   0        0        0      801 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1104 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py
+-rw-r--r--   0        0        0      813 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      817 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      829 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1305 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/policy_type_enum.py
+-rw-r--r--   0        0        0      814 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/reason_enum.py
+-rw-r--r--   0        0        0      802 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/remote_key.py
+-rw-r--r--   0        0        0     1330 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/remote_response.py
+-rw-r--r--   0        0        0      195 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/remote_response_response_type.py
+-rw-r--r--   0        0        0      723 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/request_format_enum.py
+-rw-r--r--   0        0        0     1312 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/request_type_enum.py
+-rw-r--r--   0        0        0      562 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/response_type_enum.py
+-rw-r--r--   0        0        0     1032 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/run_state_enum.py
+-rw-r--r--   0        0        0     1173 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/run_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1975 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/tax.py
+-rw-r--r--   0        0        0     1953 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/team.py
+-rw-r--r--   0        0        0     3481 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off.py
+-rw-r--r--   0        0        0     2517 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_balance.py
+-rw-r--r--   0        0        0      187 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_balance_policy_type.py
+-rw-r--r--   0        0        0     1272 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py
+-rw-r--r--   0        0        0      751 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_list_request_expand.py
+-rw-r--r--   0        0        0     1595 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1223 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_list_request_request_type.py
+-rw-r--r--   0        0        0     1619 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1029 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_list_request_status.py
+-rw-r--r--   0        0        0     3199 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_request.py
+-rw-r--r--   0        0        0      191 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_request_request_type.py
+-rw-r--r--   0        0        0      193 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_request_status.py
+-rw-r--r--   0        0        0      184 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_request_type.py
+-rw-r--r--   0        0        0      166 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_request_units.py
+-rw-r--r--   0        0        0     1106 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_response.py
+-rw-r--r--   0        0        0      767 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1627 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     1651 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0      186 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_status.py
+-rw-r--r--   0        0        0     1146 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_status_enum.py
+-rw-r--r--   0        0        0      159 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_units.py
+-rw-r--r--   0        0        0      495 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/units_enum.py
+-rw-r--r--   0        0        0      762 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/validation_problem_source.py
+-rw-r--r--   0        0        0      915 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/hris/types/webhook_receiver.py
+-rw-r--r--   0        0        0     7030 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/__init__.py
+-rw-r--r--   0        0        0     8338 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/client.py
+-rw-r--r--   0        0        0      946 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2428 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2668 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/accounts/__init__.py
+-rw-r--r--   0        0        0     9088 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/attachments/__init__.py
+-rw-r--r--   0        0        0    17255 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/attachments/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2506 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/collections/__init__.py
+-rw-r--r--   0        0        0    19212 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/collections/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/comments/__init__.py
+-rw-r--r--   0        0        0    15547 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/comments/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/contacts/__init__.py
+-rw-r--r--   0        0        0    10401 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/contacts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2171 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     3084 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2853 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.150765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/issues/__init__.py
+-rw-r--r--   0        0        0    10590 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     8932 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0    10697 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     7390 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/projects/__init__.py
+-rw-r--r--   0        0        0    13572 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/projects/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2863 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     8330 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     3406 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/tags/__init__.py
+-rw-r--r--   0        0        0     8998 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/tags/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/teams/__init__.py
+-rw-r--r--   0        0        0     9020 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/teams/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/tickets/__init__.py
+-rw-r--r--   0        0        0    42221 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/tickets/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/users/__init__.py
+-rw-r--r--   0        0        0    10850 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/users/client.py
+-rw-r--r--   0        0        0       65 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     5267 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0     9623 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/__init__.py
+-rw-r--r--   0        0        0      743 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/access_level_enum.py
+-rw-r--r--   0        0        0     1879 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/account.py
+-rw-r--r--   0        0        0     1483 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/account_token.py
+-rw-r--r--   0        0        0     2201 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/attachment.py
+-rw-r--r--   0        0        0     1716 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/attachment_request.py
+-rw-r--r--   0        0        0     1245 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/available_actions.py
+-rw-r--r--   0        0        0     1391 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/category_enum.py
+-rw-r--r--   0        0        0     2535 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/collection.py
+-rw-r--r--   0        0        0      187 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/collection_access_level.py
+-rw-r--r--   0        0        0      199 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/collection_collection_type.py
+-rw-r--r--   0        0        0      536 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/collection_type_enum.py
+-rw-r--r--   0        0        0      527 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/collections_list_request_collection_type.py
+-rw-r--r--   0        0        0      727 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/collections_users_list_request_expand.py
+-rw-r--r--   0        0        0     2161 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/comment.py
+-rw-r--r--   0        0        0     1693 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/comment_request.py
+-rw-r--r--   0        0        0     1105 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/comment_response.py
+-rw-r--r--   0        0        0     1435 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/comments_list_request_expand.py
+-rw-r--r--   0        0        0     1467 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/comments_retrieve_request_expand.py
+-rw-r--r--   0        0        0      997 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     2324 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/condition_type_enum.py
+-rw-r--r--   0        0        0     2024 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/contact.py
+-rw-r--r--   0        0        0      870 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0      522 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/error_validation_problem.py
+-rw-r--r--   0        0        0     1193 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/field_format_enum.py
+-rw-r--r--   0        0        0     1179 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/field_type_enum.py
+-rw-r--r--   0        0        0     1323 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/issues_list_request_status.py
+-rw-r--r--   0        0        0     1186 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/item_format_enum.py
+-rw-r--r--   0        0        0      964 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/item_schema.py
+-rw-r--r--   0        0        0     1172 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/item_type_enum.py
+-rw-r--r--   0        0        0      835 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0      993 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/operator_schema.py
+-rw-r--r--   0        0        0      959 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_account_list.py
+-rw-r--r--   0        0        0      900 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_attachment_list.py
+-rw-r--r--   0        0        0      900 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_collection_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_comment_list.py
+-rw-r--r--   0        0        0      921 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_contact_list.py
+-rw-r--r--   0        0        0      880 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      888 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_project_list.py
+-rw-r--r--   0        0        0      926 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_remote_field_class_list.py
+-rw-r--r--   0        0        0      901 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      872 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_tag_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_team_list.py
+-rw-r--r--   0        0        0      884 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_ticket_list.py
+-rw-r--r--   0        0        0      876 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_user_list.py
+-rw-r--r--   0        0        0     3241 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/patched_ticket_request.py
+-rw-r--r--   0        0        0      184 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/patched_ticket_request_priority.py
+-rw-r--r--   0        0        0      195 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/patched_ticket_request_status.py
+-rw-r--r--   0        0        0      843 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/priority_enum.py
+-rw-r--r--   0        0        0     1704 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/project.py
+-rw-r--r--   0        0        0      715 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/projects_users_list_request_expand.py
+-rw-r--r--   0        0        0      802 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/remote_data.py
+-rw-r--r--   0        0        0      880 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/remote_field.py
+-rw-r--r--   0        0        0     1284 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/remote_field_class.py
+-rw-r--r--   0        0        0      825 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/remote_field_request.py
+-rw-r--r--   0        0        0      986 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/remote_key.py
+-rw-r--r--   0        0        0     1299 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/remote_response.py
+-rw-r--r--   0        0        0      723 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/response_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1559 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tag.py
+-rw-r--r--   0        0        0     1705 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/team.py
+-rw-r--r--   0        0        0     3778 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/ticket.py
+-rw-r--r--   0        0        0      170 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/ticket_priority.py
+-rw-r--r--   0        0        0     3258 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/ticket_request.py
+-rw-r--r--   0        0        0      177 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/ticket_request_priority.py
+-rw-r--r--   0        0        0      188 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/ticket_request_status.py
+-rw-r--r--   0        0        0     1101 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/ticket_response.py
+-rw-r--r--   0        0        0      181 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/ticket_status.py
+-rw-r--r--   0        0        0      926 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/ticket_status_enum.py
+-rw-r--r--   0        0        0     1126 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/ticketing_attachment_response.py
+-rw-r--r--   0        0        0      743 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_collaborators_list_request_expand.py
+-rw-r--r--   0        0        0    37875 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_list_request_expand.py
+-rw-r--r--   0        0        0      810 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_list_request_priority.py
+-rw-r--r--   0        0        0     1635 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1659 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      845 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_list_request_status.py
+-rw-r--r--   0        0        0    38387 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1667 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     1691 2023-07-26 18:26:59.154765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1949 2023-07-26 18:26:59.158765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/user.py
+-rw-r--r--   0        0        0      683 2023-07-26 18:26:59.158765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/users_list_request_expand.py
+-rw-r--r--   0        0        0      699 2023-07-26 18:26:59.158765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/users_retrieve_request_expand.py
+-rw-r--r--   0        0        0      762 2023-07-26 18:26:59.158765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/validation_problem_source.py
+-rw-r--r--   0        0        0      915 2023-07-26 18:26:59.158765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-26 18:26:59.158765 mergepythonclient-0.1.2/src/merge/resources/ticketing/types/webhook_receiver.py
+-rw-r--r--   0        0        0     5673 1970-01-01 00:00:00.000000 mergepythonclient-0.1.2/PKG-INFO
```

### Comparing `mergepythonclient-0.1.1/LICENSE.md` & `mergepythonclient-0.1.2/LICENSE.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 &quot;**MSA**&quot; for the purpose of this License means: (a) for Merge &quot;Launch&quot; Customers, the Subscriber Agreement (available at: [https://merge.dev/subscriber-agreement](https://merge.dev/subscriber-agreement)); and (b) for Merge &quot;Growth&quot; and/or &quot;Expand&quot; Customers, Merge&#39;s Master Services Agreement (available at [https://merge.dev/msa](https://merge.dev/msa)), unless Merge and Customer have entered into a separate written agreement governing the Customer&#39;s use of the Service. Customer&#39;s use of any Merge Asset will be governed by the applicable MSA as well as the additional terms of this License. Capitalized terms used but not defined herein shall have the meaning as set forth in the MSA. In the event of any inconsistency between the terms of the MSA and this License, the terms of the MSA will prevail.
 
 Merge reserves the right to modify or update this License in its sole discretion, the effective date of such updates and/or modifications will be the earlier of: (i) 30 days from the date of such update or modification; or (ii) Customer&#39;s continued use of any Merge Asset.
 
 1. **SDK and Snippets License**. Customer&#39;s right to access and use the Service under Section 1 of the MSA is extended to include use of the Merge Assets but solely during the Term and subject to the terms of the MSA.
 2. **Use with the Service Only**. Customer may use the Merge Assets but only in connections with the Service and Merge Integrations. Any other use of the Merge Assets requires Merge&#39;s prior written consent.
 3. **Limitations**. Customer&#39;s use of the Merge Assets may be subject to bandwidth limitations that Merge may impose from time to time during the Subscription. Merge will make commercially reasonable efforts to notify Customer of such limitations in advance via the location where Customer gained access to the applicable Merge Asset(s).
-4. **Merge Assets &amp; Intellectual Property Rights**. Any modifications or derivatives (together, &quot;**Asset Derivatives**&quot;) made by Customer to the Merge Assets are deemed &quot;works made for hire&quot; as that term is defined in the United States Copyright Act and are the sole property of Merge. To the extent that ownership of any Asset Derivative does not by operation of law vest in Merge, Customer hereby assigns to Merge all right, title and interest in and to the Asset Derivative, including all related intellectual property rights. Asset Derivatives will be governed by the terms of this License.
+4. **Merge Assets &amp; Intellectual Property Rights**. Any modifications or derivatives (together, &quot;**Asset Derivatives**&quot;) made by Customer to the Merge Assets are deemed &quot;works made for hire&quot; as that term is defined in the United States Copyright Act and are the sole property of Merge. To the extent that ownership of any Asset Derivative does not by operation of law vest in Merge, Customer hereby assigns to Merge all right, title and interest in and to the Asset Derivative, including all related intellectual property rights. Asset Derivatives will be governed by the terms of this License.
```

### Comparing `mergepythonclient-0.1.1/README.md` & `mergepythonclient-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 
 ## Instantiation
 
 ```python
 import merge
 from merge.client import Merge
 
-client = Merge(api_key="Bearer YOUR_API_KEY", account_token="YOUR_ACCOUNT_TOKEN")
+client = Merge(api_key="YOUR_API_KEY", account_token="YOUR_ACCOUNT_TOKEN")
 ```
 
 ## Categories
 
 This SDK contains both the ATS, HRIS, CRM, Ticketing, and Accounting categories. Even if you do not plan on using more than one Merge API category right now, the SDK provides upgrade-flexibility in case you find new Merge API categories useful in the future.
 
 Each category is namespaced:
 
 ```python
-client = Merge(api_key="Bearer YOUR_API_KEY")
+client = Merge(api_key="YOUR_API_KEY")
 
 client.ats. # APIs specific to the ATS Category
 
 client.hris. # APIs specific to the HRIS Category
 ```
 
 ## Usage
@@ -81,15 +81,15 @@
 import merge
 from merge.client import Merge
 
 merge_client = Merge(
     api_key="<YOUR_API_KEY>", 
     account_token="<YOUR_ACCOUNT_TOKEN>")
 
-candidate = merge_client.ats.candiates.retrieve(
+candidate = merge_client.ats.candidates.retrieve(
     id="521b18c2-4d01-4297-b451-19858d07c133")
 ```
 
 ## Filter Candidate
 
 ```python
 import merge
```

### Comparing `mergepythonclient-0.1.1/pyproject.toml` & `mergepythonclient-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MergePythonClient"
-version = "0.1.1"
+version = "0.1.2"
 description = "Client library for the merge API"
 readme = "README.md"
 authors = ["Merge <hello@merge.dev>"]
 license = "custom"
 repository = "https://github.com/merge-api/merge-python-client"
 packages = [
     { include = "merge", from = "src"}
@@ -17,8 +17,8 @@
 
 [tool.poetry.dev-dependencies]
 mypy = "0.971"
 pytest = "^7.4.0"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `mergepythonclient-0.1.1/src/merge/client.py` & `mergepythonclient-0.1.2/src/merge/client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,19 +22,19 @@
         api_key: str,
         timeout: typing.Optional[float] = 60
     ):
         self._environment = environment
         self._client_wrapper = SyncClientWrapper(
             account_token=account_token, api_key=api_key, httpx_client=httpx.Client(timeout=timeout)
         )
-        self.ats = AtsClient(environment=environment, client_wrapper=self._client_wrapper)
-        self.crm = CrmClient(environment=environment, client_wrapper=self._client_wrapper)
         self.hris = HrisClient(environment=environment, client_wrapper=self._client_wrapper)
+        self.ats = AtsClient(environment=environment, client_wrapper=self._client_wrapper)
         self.ticketing = TicketingClient(environment=environment, client_wrapper=self._client_wrapper)
         self.accounting = AccountingClient(environment=environment, client_wrapper=self._client_wrapper)
+        self.crm = CrmClient(environment=environment, client_wrapper=self._client_wrapper)
 
 
 class AsyncMerge:
     def __init__(
         self,
         *,
         environment: MergeEnvironment = MergeEnvironment.PRODUCTION,
@@ -42,12 +42,12 @@
         api_key: str,
         timeout: typing.Optional[float] = 60
     ):
         self._environment = environment
         self._client_wrapper = AsyncClientWrapper(
             account_token=account_token, api_key=api_key, httpx_client=httpx.AsyncClient(timeout=timeout)
         )
-        self.ats = AsyncAtsClient(environment=environment, client_wrapper=self._client_wrapper)
-        self.crm = AsyncCrmClient(environment=environment, client_wrapper=self._client_wrapper)
         self.hris = AsyncHrisClient(environment=environment, client_wrapper=self._client_wrapper)
+        self.ats = AsyncAtsClient(environment=environment, client_wrapper=self._client_wrapper)
         self.ticketing = AsyncTicketingClient(environment=environment, client_wrapper=self._client_wrapper)
         self.accounting = AsyncAccountingClient(environment=environment, client_wrapper=self._client_wrapper)
+        self.crm = AsyncCrmClient(environment=environment, client_wrapper=self._client_wrapper)
```

### Comparing `mergepythonclient-0.1.1/src/merge/core/__init__.py` & `mergepythonclient-0.1.2/src/merge/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/core/client_wrapper.py` & `mergepythonclient-0.1.2/src/merge/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/core/datetime_utils.py` & `mergepythonclient-0.1.2/src/merge/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/core/jsonable_encoder.py` & `mergepythonclient-0.1.2/src/merge/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/__init__.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/__init__.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/account_details/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/account_details/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def retrieve(self) -> AccountDetails:
         """
         Get details for a linked account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "account-details"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/account-details"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountDetails, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -46,15 +46,15 @@
 
     async def retrieve(self) -> AccountDetails:
         """
         Get details for a linked account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "account-details"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/account-details"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountDetails, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/account_token/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/account_token/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         Returns the account token for the end user with the provided public token.
 
         Parameters:
             - public_token: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"account-token/{public_token}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/account-token/{public_token}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -52,15 +52,15 @@
         Returns the account token for the end user with the provided public token.
 
         Parameters:
             - public_token: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"account-token/{public_token}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/account-token/{public_token}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/accounts/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/accounts/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
 
             - show_enum_origins: typing.Optional[AccountsListRequestShowEnumOrigins]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/accounts"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -126,15 +126,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: AccountRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/accounts"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountResponse, _response.json())  # type: ignore
@@ -165,15 +165,15 @@
 
             - remote_fields: typing.Optional[AccountsRetrieveRequestRemoteFields]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[AccountsRetrieveRequestShowEnumOrigins]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/accounts/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
@@ -191,15 +191,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Account` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/accounts/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -260,15 +260,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
 
             - show_enum_origins: typing.Optional[AccountsListRequestShowEnumOrigins]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/accounts"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -308,15 +308,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: AccountRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/accounts"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountResponse, _response.json())  # type: ignore
@@ -347,15 +347,15 @@
 
             - remote_fields: typing.Optional[AccountsRetrieveRequestRemoteFields]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[AccountsRetrieveRequestShowEnumOrigins]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/accounts/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
@@ -373,15 +373,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Account` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/accounts/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/addresses/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/addresses/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
             - remote_fields: typing.Optional[typing_extensions.Literal["type"]]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["type"]]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"addresses/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/addresses/{id}"),
             params=remove_none_from_dict(
                 {
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
             ),
@@ -88,15 +88,15 @@
 
             - remote_fields: typing.Optional[typing_extensions.Literal["type"]]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["type"]]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"addresses/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/addresses/{id}"),
             params=remove_none_from_dict(
                 {
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
             ),
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/attachments/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/attachments/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "attachments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/attachments"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
@@ -109,15 +109,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: AccountingAttachmentRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "attachments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/attachments"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountingAttachmentResponse, _response.json())  # type: ignore
@@ -134,15 +134,15 @@
         Parameters:
             - id: str.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"attachments/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/attachments/{id}"),
             params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountingAttachment, _response.json())  # type: ignore
         try:
@@ -153,15 +153,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `AccountingAttachment` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "attachments/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/attachments/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -213,15 +213,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "attachments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/attachments"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
@@ -258,15 +258,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: AccountingAttachmentRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "attachments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/attachments"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountingAttachmentResponse, _response.json())  # type: ignore
@@ -283,15 +283,15 @@
         Parameters:
             - id: str.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"attachments/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/attachments/{id}"),
             params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountingAttachment, _response.json())  # type: ignore
         try:
@@ -302,15 +302,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `AccountingAttachment` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "attachments/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/attachments/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/available_actions/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/available_actions/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def retrieve(self) -> AvailableActions:
         """
         Returns a list of models and actions available for an account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "available-actions"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/available-actions"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AvailableActions, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -46,15 +46,15 @@
 
     async def retrieve(self) -> AvailableActions:
         """
         Returns a list of models and actions available for an account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "available-actions"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/available-actions"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AvailableActions, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/balance_sheets/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/balance_sheets/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "balance-sheets"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/balance-sheets"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -107,15 +107,15 @@
 
             - expand: typing.Optional[typing_extensions.Literal["company"]]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"balance-sheets/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/balance-sheets/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BalanceSheet, _response.json())  # type: ignore
         try:
@@ -171,15 +171,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "balance-sheets"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/balance-sheets"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -217,15 +217,15 @@
 
             - expand: typing.Optional[typing_extensions.Literal["company"]]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"balance-sheets/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/balance-sheets/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BalanceSheet, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/cash_flow_statements/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/cash_flow_statements/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "cash-flow-statements"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/cash-flow-statements"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -107,15 +107,15 @@
 
             - expand: typing.Optional[typing_extensions.Literal["company"]]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"cash-flow-statements/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/cash-flow-statements/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CashFlowStatement, _response.json())  # type: ignore
         try:
@@ -171,15 +171,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "cash-flow-statements"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/cash-flow-statements"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -217,15 +217,15 @@
 
             - expand: typing.Optional[typing_extensions.Literal["company"]]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"cash-flow-statements/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/cash-flow-statements/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CashFlowStatement, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/company_info/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/company_info/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "company-info"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/company-info"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
@@ -104,15 +104,15 @@
 
             - expand: typing.Optional[CompanyInfoRetrieveRequestExpand]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"company-info/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/company-info/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CompanyInfo, _response.json())  # type: ignore
         try:
@@ -165,15 +165,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "company-info"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/company-info"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
@@ -210,15 +210,15 @@
 
             - expand: typing.Optional[CompanyInfoRetrieveRequestExpand]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"company-info/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/company-info/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CompanyInfo, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/contacts/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/contacts/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "contacts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/contacts"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -124,15 +124,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: ContactRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "contacts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/contacts"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ContactResponse, _response.json())  # type: ignore
@@ -163,15 +163,15 @@
 
             - remote_fields: typing.Optional[typing_extensions.Literal["status"]]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"contacts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/contacts/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
@@ -189,15 +189,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Contact` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "contacts/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/contacts/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -258,15 +258,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "contacts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/contacts"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -306,15 +306,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: ContactRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "contacts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/contacts"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ContactResponse, _response.json())  # type: ignore
@@ -345,15 +345,15 @@
 
             - remote_fields: typing.Optional[typing_extensions.Literal["status"]]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"contacts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/contacts/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
@@ -371,15 +371,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Contact` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "contacts/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/contacts/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/credit_notes/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/credit_notes/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
             - transaction_date_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - transaction_date_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "credit-notes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/credit-notes"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -134,15 +134,15 @@
 
             - remote_fields: typing.Optional[CreditNotesRetrieveRequestRemoteFields]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[CreditNotesRetrieveRequestShowEnumOrigins]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"credit-notes/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/credit-notes/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
@@ -217,15 +217,15 @@
 
             - transaction_date_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - transaction_date_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "credit-notes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/credit-notes"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -273,15 +273,15 @@
 
             - remote_fields: typing.Optional[CreditNotesRetrieveRequestRemoteFields]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[CreditNotesRetrieveRequestShowEnumOrigins]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"credit-notes/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/credit-notes/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/delete_account/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/delete_account/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     def create(self) -> None:
         """
         Delete a linked account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "delete-account"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/delete-account"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
@@ -43,15 +43,15 @@
 
     async def create(self) -> None:
         """
         Delete a linked account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "delete-account"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/delete-account"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/expenses/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/expenses/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
             - transaction_date_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - transaction_date_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "expenses"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/expenses"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -123,15 +123,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: ExpenseRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "expenses"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/expenses"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ExpenseResponse, _response.json())  # type: ignore
@@ -156,15 +156,15 @@
 
             - expand: typing.Optional[ExpensesRetrieveRequestExpand]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"expenses/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/expenses/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Expense, _response.json())  # type: ignore
         try:
@@ -175,15 +175,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Expense` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "expenses/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/expenses/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -244,15 +244,15 @@
 
             - transaction_date_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - transaction_date_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "expenses"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/expenses"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -292,15 +292,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: ExpenseRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "expenses"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/expenses"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ExpenseResponse, _response.json())  # type: ignore
@@ -325,15 +325,15 @@
 
             - expand: typing.Optional[ExpensesRetrieveRequestExpand]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"expenses/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/expenses/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Expense, _response.json())  # type: ignore
         try:
@@ -344,15 +344,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Expense` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "expenses/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/expenses/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/force_resync/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/force_resync/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     def sync_status_resync_create(self) -> typing.List[SyncStatus]:
         """
         Force re-sync of all models. This is available for all organizations via the dashboard. Force re-sync is also available programmatically via API for monthly, quarterly, and highest sync frequency customers on the Core, Professional, or Enterprise plans. Doing so will consume a sync credit for the relevant linked account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "sync-status/resync"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/sync-status/resync"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[SyncStatus], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -47,15 +47,15 @@
 
     async def sync_status_resync_create(self) -> typing.List[SyncStatus]:
         """
         Force re-sync of all models. This is available for all organizations via the dashboard. Force re-sync is also available programmatically via API for monthly, quarterly, and highest sync frequency customers on the Core, Professional, or Enterprise plans. Doing so will consume a sync credit for the relevant linked account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "sync-status/resync"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/sync-status/resync"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[SyncStatus], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/generate_key/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/generate_key/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         Create a remote key.
 
         Parameters:
             - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "generate-key"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/generate-key"),
             json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
@@ -58,15 +58,15 @@
         Create a remote key.
 
         Parameters:
             - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "generate-key"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/generate-key"),
             json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/income_statements/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/income_statements/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "income-statements"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/income-statements"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -107,15 +107,15 @@
 
             - expand: typing.Optional[typing_extensions.Literal["company"]]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"income-statements/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/income-statements/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(IncomeStatement, _response.json())  # type: ignore
         try:
@@ -171,15 +171,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "income-statements"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/income-statements"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -217,15 +217,15 @@
 
             - expand: typing.Optional[typing_extensions.Literal["company"]]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"income-statements/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/income-statements/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(IncomeStatement, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/invoices/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/invoices/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             - type: typing.Optional[InvoicesListRequestType]. If provided, will only return Invoices with this type
 
                                                               * `ACCOUNTS_RECEIVABLE` - ACCOUNTS_RECEIVABLE
                                                               * `ACCOUNTS_PAYABLE` - ACCOUNTS_PAYABLE
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "invoices"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/invoices"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "contact_id": contact_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
@@ -144,15 +144,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: InvoiceRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "invoices"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/invoices"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(InvoiceResponse, _response.json())  # type: ignore
@@ -183,15 +183,15 @@
 
             - remote_fields: typing.Optional[typing_extensions.Literal["type"]]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["type"]]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoices/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/invoices/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
@@ -209,15 +209,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Invoice` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "invoices/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/invoices/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -293,15 +293,15 @@
             - type: typing.Optional[InvoicesListRequestType]. If provided, will only return Invoices with this type
 
                                                               * `ACCOUNTS_RECEIVABLE` - ACCOUNTS_RECEIVABLE
                                                               * `ACCOUNTS_PAYABLE` - ACCOUNTS_PAYABLE
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "invoices"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/invoices"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "contact_id": contact_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
@@ -345,15 +345,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: InvoiceRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "invoices"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/invoices"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(InvoiceResponse, _response.json())  # type: ignore
@@ -384,15 +384,15 @@
 
             - remote_fields: typing.Optional[typing_extensions.Literal["type"]]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["type"]]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoices/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/invoices/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
@@ -410,15 +410,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Invoice` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "invoices/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/invoices/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/issues/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/issues/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             - status: typing.Optional[IssuesListRequestStatus]. Status of the issue. Options: ('ONGOING', 'RESOLVED')
 
                                                                 * `ONGOING` - ONGOING
                                                                 * `RESOLVED` - RESOLVED
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "issues"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/issues"),
             params=remove_none_from_dict(
                 {
                     "account_token": account_token,
                     "cursor": cursor,
                     "end_date": end_date,
                     "end_user_organization_name": end_user_organization_name,
                     "first_incident_time_after": first_incident_time_after,
@@ -108,15 +108,15 @@
         Get a specific issue.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"issues/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/issues/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Issue, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -180,15 +180,15 @@
             - status: typing.Optional[IssuesListRequestStatus]. Status of the issue. Options: ('ONGOING', 'RESOLVED')
 
                                                                 * `ONGOING` - ONGOING
                                                                 * `RESOLVED` - RESOLVED
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "issues"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/issues"),
             params=remove_none_from_dict(
                 {
                     "account_token": account_token,
                     "cursor": cursor,
                     "end_date": end_date,
                     "end_user_organization_name": end_user_organization_name,
                     "first_incident_time_after": first_incident_time_after,
@@ -218,15 +218,15 @@
         Get a specific issue.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"issues/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/issues/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Issue, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/items/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/items/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "items"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/items"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -123,15 +123,15 @@
 
             - remote_fields: typing.Optional[typing_extensions.Literal["status"]]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"items/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/items/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
@@ -200,15 +200,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "items"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/items"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -254,15 +254,15 @@
 
             - remote_fields: typing.Optional[typing_extensions.Literal["status"]]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"items/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/items/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/journal_entries/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/journal_entries/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
             - transaction_date_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - transaction_date_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "journal-entries"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/journal-entries"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -123,15 +123,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: JournalEntryRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "journal-entries"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/journal-entries"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(JournalEntryResponse, _response.json())  # type: ignore
@@ -156,15 +156,15 @@
 
             - expand: typing.Optional[JournalEntriesRetrieveRequestExpand]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"journal-entries/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/journal-entries/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(JournalEntry, _response.json())  # type: ignore
         try:
@@ -175,15 +175,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `JournalEntry` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "journal-entries/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/journal-entries/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -244,15 +244,15 @@
 
             - transaction_date_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - transaction_date_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "journal-entries"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/journal-entries"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -292,15 +292,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: JournalEntryRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "journal-entries"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/journal-entries"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(JournalEntryResponse, _response.json())  # type: ignore
@@ -325,15 +325,15 @@
 
             - expand: typing.Optional[JournalEntriesRetrieveRequestExpand]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"journal-entries/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/journal-entries/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(JournalEntry, _response.json())  # type: ignore
         try:
@@ -344,15 +344,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `JournalEntry` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "journal-entries/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/journal-entries/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/link_token/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/link_token/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             _request["link_expiry_mins"] = link_expiry_mins
         if should_create_magic_link_url is not OMIT:
             _request["should_create_magic_link_url"] = should_create_magic_link_url
         if common_models is not OMIT:
             _request["common_models"] = common_models
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "link-token"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/link-token"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(LinkToken, _response.json())  # type: ignore
         try:
@@ -138,15 +138,15 @@
             _request["link_expiry_mins"] = link_expiry_mins
         if should_create_magic_link_url is not OMIT:
             _request["should_create_magic_link_url"] = should_create_magic_link_url
         if common_models is not OMIT:
             _request["common_models"] = common_models
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "link-token"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/link-token"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(LinkToken, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/linked_accounts/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/linked_accounts/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - status: typing.Optional[str]. Filter by status. Options: `COMPLETE`, `INCOMPLETE`, `RELINK_NEEDED`
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "linked-accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/linked-accounts"),
             params=remove_none_from_dict(
                 {
                     "category": category,
                     "cursor": cursor,
                     "end_user_email_address": end_user_email_address,
                     "end_user_organization_name": end_user_organization_name,
                     "end_user_origin_id": end_user_origin_id,
@@ -166,15 +166,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - status: typing.Optional[str]. Filter by status. Options: `COMPLETE`, `INCOMPLETE`, `RELINK_NEEDED`
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "linked-accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/linked-accounts"),
             params=remove_none_from_dict(
                 {
                     "category": category,
                     "cursor": cursor,
                     "end_user_email_address": end_user_email_address,
                     "end_user_organization_name": end_user_organization_name,
                     "end_user_origin_id": end_user_origin_id,
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/passthrough/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/passthrough/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             _request["headers"] = headers
         if request_format is not OMIT:
             _request["request_format"] = request_format
         if normalize_response is not OMIT:
             _request["normalize_response"] = normalize_response
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "passthrough"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/passthrough"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteResponse, _response.json())  # type: ignore
         try:
@@ -137,15 +137,15 @@
             _request["headers"] = headers
         if request_format is not OMIT:
             _request["request_format"] = request_format
         if normalize_response is not OMIT:
             _request["normalize_response"] = normalize_response
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "passthrough"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/passthrough"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteResponse, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/payments/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/payments/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
             - transaction_date_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - transaction_date_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "payments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/payments"),
             params=remove_none_from_dict(
                 {
                     "account_id": account_id,
                     "company_id": company_id,
                     "contact_id": contact_id,
                     "created_after": created_after,
                     "created_before": created_before,
@@ -131,15 +131,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: PaymentRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "payments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/payments"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaymentResponse, _response.json())  # type: ignore
@@ -164,15 +164,15 @@
 
             - expand: typing.Optional[PaymentsRetrieveRequestExpand]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"payments/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/payments/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Payment, _response.json())  # type: ignore
         try:
@@ -183,15 +183,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Payment` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "payments/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/payments/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -258,15 +258,15 @@
 
             - transaction_date_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - transaction_date_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "payments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/payments"),
             params=remove_none_from_dict(
                 {
                     "account_id": account_id,
                     "company_id": company_id,
                     "contact_id": contact_id,
                     "created_after": created_after,
                     "created_before": created_before,
@@ -308,15 +308,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: PaymentRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "payments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/payments"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaymentResponse, _response.json())  # type: ignore
@@ -341,15 +341,15 @@
 
             - expand: typing.Optional[PaymentsRetrieveRequestExpand]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"payments/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/payments/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Payment, _response.json())  # type: ignore
         try:
@@ -360,15 +360,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Payment` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "payments/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/payments/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/phone_numbers/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/phone_numbers/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         Parameters:
             - id: str.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"phone-numbers/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/phone-numbers/{id}"),
             params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountingPhoneNumber, _response.json())  # type: ignore
         try:
@@ -59,15 +59,15 @@
         Parameters:
             - id: str.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"phone-numbers/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/phone-numbers/{id}"),
             params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountingPhoneNumber, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/purchase_orders/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/purchase_orders/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "purchase-orders"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/purchase-orders"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -132,15 +132,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: PurchaseOrderRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "purchase-orders"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/purchase-orders"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PurchaseOrderResponse, _response.json())  # type: ignore
@@ -171,15 +171,15 @@
 
             - remote_fields: typing.Optional[typing_extensions.Literal["status"]]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"purchase-orders/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/purchase-orders/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
@@ -197,15 +197,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `PurchaseOrder` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "purchase-orders/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/purchase-orders/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -272,15 +272,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "purchase-orders"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/purchase-orders"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -322,15 +322,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: PurchaseOrderRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "purchase-orders"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/purchase-orders"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PurchaseOrderResponse, _response.json())  # type: ignore
@@ -361,15 +361,15 @@
 
             - remote_fields: typing.Optional[typing_extensions.Literal["status"]]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"purchase-orders/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/purchase-orders/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
@@ -387,15 +387,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `PurchaseOrder` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "purchase-orders/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/purchase-orders/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/regenerate_key/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/generate_key/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,61 +12,61 @@
 from .....environment import MergeEnvironment
 from ...types.remote_key import RemoteKey
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class RegenerateKeyClient:
+class GenerateKeyClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def create(self, *, name: str) -> RemoteKey:
         """
-        Exchange remote keys.
+        Create a remote key.
 
         Parameters:
             - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "regenerate-key"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/generate-key"),
             json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncRegenerateKeyClient:
+class AsyncGenerateKeyClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def create(self, *, name: str) -> RemoteKey:
         """
-        Exchange remote keys.
+        Create a remote key.
 
         Parameters:
             - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "regenerate-key"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/generate-key"),
             json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/selective_sync/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/selective_sync/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     def configurations_list(self) -> typing.List[LinkedAccountSelectiveSyncConfiguration]:
         """
         Get a linked account's selective syncs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/selective-sync/configurations"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -51,15 +51,15 @@
         Replace a linked account's selective syncs.
 
         Parameters:
             - sync_configurations: typing.List[LinkedAccountSelectiveSyncConfigurationRequest]. The selective syncs associated with a linked account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/selective-sync/configurations"),
             json=jsonable_encoder({"sync_configurations": sync_configurations}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
@@ -83,15 +83,15 @@
 
             - cursor: typing.Optional[str]. The pagination cursor value.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/meta"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/selective-sync/meta"),
             params=remove_none_from_dict({"common_model": common_model, "cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedConditionSchemaList, _response.json())  # type: ignore
         try:
@@ -110,15 +110,15 @@
 
     async def configurations_list(self) -> typing.List[LinkedAccountSelectiveSyncConfiguration]:
         """
         Get a linked account's selective syncs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/selective-sync/configurations"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -133,15 +133,15 @@
         Replace a linked account's selective syncs.
 
         Parameters:
             - sync_configurations: typing.List[LinkedAccountSelectiveSyncConfigurationRequest]. The selective syncs associated with a linked account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/selective-sync/configurations"),
             json=jsonable_encoder({"sync_configurations": sync_configurations}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
@@ -165,15 +165,15 @@
 
             - cursor: typing.Optional[str]. The pagination cursor value.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/meta"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/selective-sync/meta"),
             params=remove_none_from_dict({"common_model": common_model, "cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedConditionSchemaList, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/sync_status/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/sync_status/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         Parameters:
             - cursor: typing.Optional[str]. The pagination cursor value.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "sync-status"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/sync-status"),
             params=remove_none_from_dict({"cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedSyncStatusList, _response.json())  # type: ignore
         try:
@@ -63,15 +63,15 @@
         Parameters:
             - cursor: typing.Optional[str]. The pagination cursor value.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "sync-status"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/sync-status"),
             params=remove_none_from_dict({"cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedSyncStatusList, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/tax_rates/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/tax_rates/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tax-rates"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/tax-rates"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -107,15 +107,15 @@
 
             - expand: typing.Optional[typing_extensions.Literal["company"]]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tax-rates/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/tax-rates/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TaxRate, _response.json())  # type: ignore
         try:
@@ -171,15 +171,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tax-rates"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/tax-rates"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -217,15 +217,15 @@
 
             - expand: typing.Optional[typing_extensions.Literal["company"]]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tax-rates/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/tax-rates/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TaxRate, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/tracking_categories/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/tracking_categories/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tracking-categories"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/tracking-categories"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -121,15 +121,15 @@
 
             - remote_fields: typing.Optional[typing_extensions.Literal["status"]]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tracking-categories/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/tracking-categories/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
@@ -198,15 +198,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tracking-categories"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/tracking-categories"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -252,15 +252,15 @@
 
             - remote_fields: typing.Optional[typing_extensions.Literal["status"]]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tracking-categories/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/tracking-categories/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/transactions/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/transactions/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
             - transaction_date_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - transaction_date_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "transactions"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/transactions"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -116,15 +116,15 @@
 
             - expand: typing.Optional[TransactionsRetrieveRequestExpand]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"transactions/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/transactions/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Transaction, _response.json())  # type: ignore
         try:
@@ -186,15 +186,15 @@
 
             - transaction_date_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - transaction_date_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "transactions"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/transactions"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -234,15 +234,15 @@
 
             - expand: typing.Optional[TransactionsRetrieveRequestExpand]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"transactions/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/transactions/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Transaction, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/vendor_credits/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/vendor_credits/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
             - transaction_date_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - transaction_date_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "vendor-credits"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/vendor-credits"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -116,15 +116,15 @@
 
             - expand: typing.Optional[VendorCreditsRetrieveRequestExpand]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"vendor-credits/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/vendor-credits/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(VendorCredit, _response.json())  # type: ignore
         try:
@@ -186,15 +186,15 @@
 
             - transaction_date_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - transaction_date_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "vendor-credits"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/vendor-credits"),
             params=remove_none_from_dict(
                 {
                     "company_id": company_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -234,15 +234,15 @@
 
             - expand: typing.Optional[VendorCreditsRetrieveRequestExpand]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"vendor-credits/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/vendor-credits/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(VendorCredit, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/resources/webhook_receivers/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/webhook_receivers/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def list(self) -> typing.List[WebhookReceiver]:
         """
         Returns a list of `WebhookReceiver` objects.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "webhook-receivers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/webhook-receivers"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[WebhookReceiver], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -53,15 +53,15 @@
             - key: typing.Optional[str]. <span style="white-space: nowrap">`non-empty`</span>
         """
         _request: typing.Dict[str, typing.Any] = {"event": event, "is_active": is_active}
         if key is not OMIT:
             _request["key"] = key
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "webhook-receivers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/webhook-receivers"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(WebhookReceiver, _response.json())  # type: ignore
         try:
@@ -80,15 +80,15 @@
 
     async def list(self) -> typing.List[WebhookReceiver]:
         """
         Returns a list of `WebhookReceiver` objects.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "webhook-receivers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/webhook-receivers"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[WebhookReceiver], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -108,15 +108,15 @@
             - key: typing.Optional[str]. <span style="white-space: nowrap">`non-empty`</span>
         """
         _request: typing.Dict[str, typing.Any] = {"event": event, "is_active": is_active}
         if key is not OMIT:
             _request["key"] = key
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "webhook-receivers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/webhook-receivers"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(WebhookReceiver, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/__init__.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/account.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_details.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_details.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_details_and_actions.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_details_and_actions_integration.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_details_and_actions_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_integration.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_response.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/account_token.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/account_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_attachment.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounting_attachment.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_attachment_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounting_attachment_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_attachment_response.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounting_attachment_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_phone_number.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounting_phone_number.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounting_phone_number_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounting_phone_number_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounts_list_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounts_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounts_list_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounts_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounts_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounts_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/accounts_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/accounts_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/address.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/address.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/address_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/address_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/available_actions.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/balance_sheet.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/cash_flow_statement.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/cash_flow_statement.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/categories_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/category_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/category_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/category_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/classification_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/classification_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/common_model_scopes_body_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/company_info.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/company_info.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/company_info_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/company_info_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/company_info_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/company_info_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/condition_schema.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/condition_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/contact.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/contact.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/contact_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/contact_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/contact_response.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/contact_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/contacts_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/contacts_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/contacts_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/contacts_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/country_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/country_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_note.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_note.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_note_line_item.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_note_line_item.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_note_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_note_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_notes_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_list_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_notes_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_list_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_notes_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_notes_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_notes_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/credit_notes_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/credit_notes_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/currency_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/currency_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/debug_mode_log.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/debug_model_log_summary.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/enabled_actions_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/encoding_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/error_validation_problem.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/expense.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_line.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/expense_line.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_line_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/expense_line_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/expense_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/expense_response.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/expense_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/expenses_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/expenses_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/expenses_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/expenses_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/income_statement.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/income_statement.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_line_item.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice_line_item.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_line_item_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice_line_item_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_response.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoice_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoice_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoices_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoices_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoices_list_request_type.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoices_list_request_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/invoices_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/invoices_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/issue.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/issue.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/issue_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/item.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/item.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/items_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/items_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/items_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/items_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entries_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_entries_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entries_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_entries_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_entry.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_entry_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_entry_response.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_entry_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_line.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_line.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/journal_line_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/journal_line_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/link_token.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/link_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_condition.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_condition_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_selective_sync_configuration.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_selective_sync_configuration_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_account_status.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/linked_accounts_list_request_category.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/meta_response.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/method_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/model_operation.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/multipart_form_field_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/operator_schema.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_account_details_and_actions_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_account_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_account_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_accounting_attachment_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_accounting_attachment_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_balance_sheet_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_balance_sheet_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_cash_flow_statement_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_cash_flow_statement_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_company_info_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_company_info_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_condition_schema_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_contact_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_contact_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_credit_note_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_credit_note_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_expense_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_expense_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_income_statement_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_income_statement_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_invoice_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_invoice_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_issue_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_item_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_item_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_journal_entry_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_journal_entry_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_payment_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_payment_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_purchase_order_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_purchase_order_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_sync_status_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_tax_rate_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_tax_rate_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_tracking_category_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_tracking_category_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_transaction_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_transaction_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/paginated_vendor_credit_list.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/paginated_vendor_credit_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/payment.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/payment.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/payment_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/payment_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/payment_response.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/payment_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/payments_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/payments_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/payments_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/payments_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/posting_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/posting_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_line_item.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order_line_item.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_line_item_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order_line_item_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_request.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_response.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_order_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_order_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_orders_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_orders_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/purchase_orders_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/purchase_orders_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/remote_data.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/remote_key.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/remote_response.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/report_item.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/report_item.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/request_format_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/response_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/selective_sync_configurations_usage_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/status_7_d_1_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/status_7_d_1_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/sync_status.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/sync_status_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/tax_rate.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/tax_rate.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/tracking_category.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/tracking_category.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/transaction.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/transaction.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/transaction_line_item.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/transaction_line_item.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/transactions_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/transactions_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/transactions_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/transactions_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/validation_problem_source.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credit.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/vendor_credit.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credit_line.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/vendor_credit_line.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credits_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/vendor_credits_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/vendor_credits_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/vendor_credits_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/warning_validation_problem.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/accounting/types/webhook_receiver.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/__init__.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/__init__.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/account_details/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/account_details/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def retrieve(self) -> AccountDetails:
         """
         Get details for a linked account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/account-details"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/account-details"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountDetails, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -46,15 +46,15 @@
 
     async def retrieve(self) -> AccountDetails:
         """
         Get details for a linked account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/account-details"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/account-details"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountDetails, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/account_token/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/activities/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/activities/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/applications/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/applications/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/attachments/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/attachments/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/available_actions/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/available_actions/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def retrieve(self) -> AvailableActions:
         """
         Returns a list of models and actions available for an account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/available-actions"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/available-actions"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AvailableActions, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -46,15 +46,15 @@
 
     async def retrieve(self) -> AvailableActions:
         """
         Returns a list of models and actions available for an account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/available-actions"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/available-actions"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AvailableActions, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/candidates/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/candidates/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/delete_account/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/departments/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/departments/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/eeocs/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/eeocs/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/force_resync/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/generate_key/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/generate_key/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         Create a remote key.
 
         Parameters:
             - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/generate-key"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/generate-key"),
             json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
@@ -58,15 +58,15 @@
         Create a remote key.
 
         Parameters:
             - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/generate-key"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/generate-key"),
             json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/interviews/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/interviews/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/issues/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/job_interview_stages/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/job_interview_stages/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/jobs/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/jobs/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/link_token/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/linked_accounts/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/linked_accounts/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - status: typing.Optional[str]. Filter by status. Options: `COMPLETE`, `INCOMPLETE`, `RELINK_NEEDED`
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/linked-accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/linked-accounts"),
             params=remove_none_from_dict(
                 {
                     "category": category,
                     "cursor": cursor,
                     "end_user_email_address": end_user_email_address,
                     "end_user_organization_name": end_user_organization_name,
                     "end_user_origin_id": end_user_origin_id,
@@ -166,15 +166,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - status: typing.Optional[str]. Filter by status. Options: `COMPLETE`, `INCOMPLETE`, `RELINK_NEEDED`
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/linked-accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/linked-accounts"),
             params=remove_none_from_dict(
                 {
                     "category": category,
                     "cursor": cursor,
                     "end_user_email_address": end_user_email_address,
                     "end_user_organization_name": end_user_organization_name,
                     "end_user_origin_id": end_user_origin_id,
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/offers/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/offers/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/offices/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/offices/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/passthrough/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/passthrough/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             _request["headers"] = headers
         if request_format is not OMIT:
             _request["request_format"] = request_format
         if normalize_response is not OMIT:
             _request["normalize_response"] = normalize_response
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/passthrough"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/passthrough"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteResponse, _response.json())  # type: ignore
         try:
@@ -137,15 +137,15 @@
             _request["headers"] = headers
         if request_format is not OMIT:
             _request["request_format"] = request_format
         if normalize_response is not OMIT:
             _request["normalize_response"] = normalize_response
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/passthrough"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/passthrough"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteResponse, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/regenerate_key/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/reject_reasons/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/reject_reasons/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/scorecards/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/scorecards/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/selective_sync/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/sync_status/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/sync_status/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         Parameters:
             - cursor: typing.Optional[str]. The pagination cursor value.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/sync-status"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/sync-status"),
             params=remove_none_from_dict({"cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedSyncStatusList, _response.json())  # type: ignore
         try:
@@ -63,15 +63,15 @@
         Parameters:
             - cursor: typing.Optional[str]. The pagination cursor value.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/sync-status"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/sync-status"),
             params=remove_none_from_dict({"cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedSyncStatusList, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/tags/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/tags/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/users/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/resources/webhook_receivers/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/__init__.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/access_role_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/access_role_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/account_details.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/account_details.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/account_details_and_actions.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/account_details_and_actions_integration.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/account_details_and_actions_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/account_integration.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/account_token.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/account_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/activities_list_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/activities_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/activity.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/activity.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/activity_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_response.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/activity_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/activity_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/activity_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/application.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/application.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/application_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/application_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/application_response.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/application_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/applications_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/applications_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/applications_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/applications_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/attachment.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/attachment_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment_response.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/attachment_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/attachment_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/attachment_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/available_actions.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/candidate.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/candidate.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/candidate_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/candidate_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/candidate_response.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/candidate_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/candidates_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/candidates_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/candidates_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/candidates_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/categories_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/category_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/common_model_scopes_body_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/condition_schema.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/condition_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/debug_mode_log.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/debug_model_log_summary.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/department.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/department.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/disability_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/disability_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/eeoc.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/eeoc.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/email_address.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/email_address.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/email_address_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/email_address_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/email_address_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/email_address_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/enabled_actions_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/encoding_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/error_validation_problem.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/gender_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/gender_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/interviews_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/interviews_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/interviews_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/interviews_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/issue.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/issue.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/issue_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/job.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/job.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/job_interview_stage.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/job_interview_stage.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/job_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/job_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/jobs_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/jobs_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/jobs_list_request_status.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/jobs_list_request_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/jobs_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/jobs_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/link_token.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/link_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_condition.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_condition_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_account_status.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/linked_accounts_list_request_category.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/meta_response.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/method_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/model_operation.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/multipart_form_field_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/offer.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/offer.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/offer_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/offer_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/offers_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/offers_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/offers_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/offers_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/office.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/office.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/operator_schema.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/overall_recommendation_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/overall_recommendation_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_activity_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_activity_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_application_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_application_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_attachment_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_attachment_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_candidate_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_candidate_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_condition_schema_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_department_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_department_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_eeoc_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_eeoc_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_issue_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_job_interview_stage_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_job_interview_stage_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_job_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_job_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_offer_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_offer_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_office_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_office_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_reject_reason_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_reject_reason_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_remote_user_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_remote_user_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_scheduled_interview_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_scheduled_interview_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_scorecard_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_scorecard_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_sync_status_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/paginated_tag_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/paginated_tag_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/patched_candidate_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/patched_candidate_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/phone_number.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/phone_number_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/phone_number_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/phone_number_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/phone_number_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/race_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/race_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/reason_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/reject_reason.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/reject_reason.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_data.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_key.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_response.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/remote_user.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/remote_user.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/request_format_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/response_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/scheduled_interview.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/scheduled_interview_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview_response.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/scheduled_interview_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/scheduled_interview_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/scheduled_interview_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/scorecard.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/scorecard.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/scorecards_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/scorecards_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/sync_status.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/sync_status_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/tag.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/tag.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/url.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/url.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/url_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/url_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/url_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/url_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/validation_problem_source.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/veteran_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/veteran_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/visibility_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/visibility_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/warning_validation_problem.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ats/types/webhook_receiver.py` & `mergepythonclient-0.1.2/src/merge/resources/ats/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/__init__.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/__init__.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/account_details/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/account_details/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def retrieve(self) -> AccountDetails:
         """
         Get details for a linked account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "account-details"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/account-details"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountDetails, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -46,15 +46,15 @@
 
     async def retrieve(self) -> AccountDetails:
         """
         Get details for a linked account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "account-details"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/account-details"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountDetails, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/account_token/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/account_token/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         Returns the account token for the end user with the provided public token.
 
         Parameters:
             - public_token: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"account-token/{public_token}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/account-token/{public_token}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -52,15 +52,15 @@
         Returns the account token for the end user with the provided public token.
 
         Parameters:
             - public_token: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"account-token/{public_token}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/account-token/{public_token}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/accounts/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/accounts/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/accounts"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
@@ -120,15 +120,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: AccountRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/accounts"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CrmAccountResponse, _response.json())  # type: ignore
@@ -156,15 +156,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/accounts/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                 }
             ),
@@ -197,15 +197,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: PatchedAccountRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/accounts/{id}"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CrmAccountResponse, _response.json())  # type: ignore
@@ -220,15 +220,15 @@
         Returns metadata for `CRMAccount` PATCHs.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/meta/patch/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/accounts/meta/patch/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -238,15 +238,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `CRMAccount` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/accounts/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -275,15 +275,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/accounts/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
@@ -350,15 +350,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/accounts"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
@@ -397,15 +397,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: AccountRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/accounts"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CrmAccountResponse, _response.json())  # type: ignore
@@ -433,15 +433,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/accounts/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                 }
             ),
@@ -474,15 +474,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: PatchedAccountRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/accounts/{id}"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CrmAccountResponse, _response.json())  # type: ignore
@@ -497,15 +497,15 @@
         Returns metadata for `CRMAccount` PATCHs.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/meta/patch/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/accounts/meta/patch/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -515,15 +515,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `CRMAccount` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/accounts/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -552,15 +552,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/accounts/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/association_types/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/association_types/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,16 @@
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"custom-object-classes/{custom_object_class_id}/association-types"
+                f"{self._environment.value}/",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/association-types",
             ),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -119,15 +120,16 @@
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: AssociationTypeRequestRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"custom-object-classes/{custom_object_class_id}/association-types"
+                f"{self._environment.value}/",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/association-types",
             ),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -157,15 +159,16 @@
             - expand: typing.Optional[typing_extensions.Literal["target_object_classes"]]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"custom-object-classes/{custom_object_class_id}/association-types/{id}"
+                f"{self._environment.value}/",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/association-types/{id}",
             ),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AssociationType, _response.json())  # type: ignore
@@ -182,15 +185,15 @@
         Parameters:
             - custom_object_class_id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._environment.value}/",
-                f"custom-object-classes/{custom_object_class_id}/association-types/meta/post",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/association-types/meta/post",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
@@ -247,15 +250,16 @@
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"custom-object-classes/{custom_object_class_id}/association-types"
+                f"{self._environment.value}/",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/association-types",
             ),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -297,15 +301,16 @@
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: AssociationTypeRequestRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"custom-object-classes/{custom_object_class_id}/association-types"
+                f"{self._environment.value}/",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/association-types",
             ),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -335,15 +340,16 @@
             - expand: typing.Optional[typing_extensions.Literal["target_object_classes"]]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"custom-object-classes/{custom_object_class_id}/association-types/{id}"
+                f"{self._environment.value}/",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/association-types/{id}",
             ),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AssociationType, _response.json())  # type: ignore
@@ -362,15 +368,15 @@
         Parameters:
             - custom_object_class_id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._environment.value}/",
-                f"custom-object-classes/{custom_object_class_id}/association-types/meta/post",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/association-types/meta/post",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/associations/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/associations/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._environment.value}/",
-                f"custom-object-classes/{custom_object_class_id}/custom-objects/{object_id}/associations",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/custom-objects/{object_id}/associations",
             ),
             params=remove_none_from_dict(
                 {
                     "association_type_id": association_type_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
@@ -130,15 +130,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._environment.value}/",
-                f"custom-object-classes/{source_class_id}/custom-objects/{source_object_id}/associations/{target_class_id}/{target_object_id}/{association_type_id}",
+                f"api/crm/v1/custom-object-classes/{source_class_id}/custom-objects/{source_object_id}/associations/{target_class_id}/{target_object_id}/{association_type_id}",
             ),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Association, _response.json())  # type: ignore
@@ -203,15 +203,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._environment.value}/",
-                f"custom-object-classes/{custom_object_class_id}/custom-objects/{object_id}/associations",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/custom-objects/{object_id}/associations",
             ),
             params=remove_none_from_dict(
                 {
                     "association_type_id": association_type_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
@@ -264,15 +264,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._environment.value}/",
-                f"custom-object-classes/{source_class_id}/custom-objects/{source_object_id}/associations/{target_class_id}/{target_object_id}/{association_type_id}",
+                f"api/crm/v1/custom-object-classes/{source_class_id}/custom-objects/{source_object_id}/associations/{target_class_id}/{target_object_id}/{association_type_id}",
             ),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Association, _response.json())  # type: ignore
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/available_actions/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/available_actions/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def retrieve(self) -> AvailableActions:
         """
         Returns a list of models and actions available for an account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "available-actions"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/available-actions"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AvailableActions, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -46,15 +46,15 @@
 
     async def retrieve(self) -> AvailableActions:
         """
         Returns a list of models and actions available for an account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "available-actions"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/available-actions"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AvailableActions, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/contacts/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/contacts/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "contacts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/contacts"),
             params=remove_none_from_dict(
                 {
                     "account_id": account_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -121,15 +121,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: ContactRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "contacts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/contacts"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CrmContactResponse, _response.json())  # type: ignore
@@ -157,15 +157,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"contacts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/contacts/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                 }
             ),
@@ -198,15 +198,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: PatchedContactRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"contacts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/contacts/{id}"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CrmContactResponse, _response.json())  # type: ignore
@@ -223,15 +223,15 @@
         Parameters:
             - model_id: str.
 
             - request: IgnoreCommonModelRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"contacts/ignore/{model_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/contacts/ignore/{model_id}"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
@@ -245,15 +245,15 @@
         Returns metadata for `CRMContact` PATCHs.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"contacts/meta/patch/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/contacts/meta/patch/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -263,15 +263,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `CRMContact` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "contacts/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/contacts/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -300,15 +300,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "contacts/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/contacts/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
@@ -375,15 +375,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "contacts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/contacts"),
             params=remove_none_from_dict(
                 {
                     "account_id": account_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -422,15 +422,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: ContactRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "contacts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/contacts"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CrmContactResponse, _response.json())  # type: ignore
@@ -458,15 +458,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"contacts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/contacts/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                 }
             ),
@@ -499,15 +499,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: PatchedContactRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"contacts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/contacts/{id}"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CrmContactResponse, _response.json())  # type: ignore
@@ -524,15 +524,15 @@
         Parameters:
             - model_id: str.
 
             - request: IgnoreCommonModelRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"contacts/ignore/{model_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/contacts/ignore/{model_id}"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
@@ -546,15 +546,15 @@
         Returns metadata for `CRMContact` PATCHs.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"contacts/meta/patch/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/contacts/meta/patch/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -564,15 +564,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `CRMContact` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "contacts/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/contacts/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -601,15 +601,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "contacts/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/contacts/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/custom_object_classes/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/custom_object_classes/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "custom-object-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/custom-object-classes"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
@@ -103,15 +103,15 @@
 
             - expand: typing.Optional[typing_extensions.Literal["fields"]]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"custom-object-classes/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/custom-object-classes/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CustomObjectClass, _response.json())  # type: ignore
         try:
@@ -131,15 +131,17 @@
 
             - is_debug_mode: typing.Optional[bool]. Whether to include debug fields (such as log file links) in the response.
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"custom-object-classes/generator/{generator_id}"),
+            urllib.parse.urljoin(
+                f"{self._environment.value}/", f"api/crm/v1/custom-object-classes/generator/{generator_id}"
+            ),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CustomObjectClass, _response.json())  # type: ignore
         try:
@@ -192,15 +194,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "custom-object-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/custom-object-classes"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
@@ -237,15 +239,15 @@
 
             - expand: typing.Optional[typing_extensions.Literal["fields"]]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"custom-object-classes/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/custom-object-classes/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CustomObjectClass, _response.json())  # type: ignore
         try:
@@ -265,15 +267,17 @@
 
             - is_debug_mode: typing.Optional[bool]. Whether to include debug fields (such as log file links) in the response.
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"custom-object-classes/generator/{generator_id}"),
+            urllib.parse.urljoin(
+                f"{self._environment.value}/", f"api/crm/v1/custom-object-classes/generator/{generator_id}"
+            ),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CustomObjectClass, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/custom_objects/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/custom_objects/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,16 @@
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"custom-object-classes/{custom_object_class_id}/custom-objects"
+                f"{self._environment.value}/",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/custom-objects",
             ),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
@@ -118,15 +119,16 @@
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: CustomObjectRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"custom-object-classes/{custom_object_class_id}/custom-objects"
+                f"{self._environment.value}/",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/custom-objects",
             ),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -156,15 +158,16 @@
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"custom-object-classes/{custom_object_class_id}/custom-objects/{id}"
+                f"{self._environment.value}/",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/custom-objects/{id}",
             ),
             params=remove_none_from_dict(
                 {"include_remote_data": include_remote_data, "include_remote_fields": include_remote_fields}
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -198,15 +201,16 @@
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: CustomObjectRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"custom-object-classes/{custom_object_class_id}/custom-objects/{id}"
+                f"{self._environment.value}/",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/custom-objects/{id}",
             ),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -228,15 +232,15 @@
 
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._environment.value}/",
-                f"custom-object-classes/{custom_object_class_id}/custom-objects/meta/patch/{id}",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/custom-objects/meta/patch/{id}",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
@@ -252,15 +256,15 @@
         Parameters:
             - custom_object_class_id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._environment.value}/",
-                f"custom-object-classes/{custom_object_class_id}/custom-objects/meta/post",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/custom-objects/meta/post",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
@@ -317,15 +321,16 @@
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"custom-object-classes/{custom_object_class_id}/custom-objects"
+                f"{self._environment.value}/",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/custom-objects",
             ),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
@@ -367,15 +372,16 @@
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: CustomObjectRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"custom-object-classes/{custom_object_class_id}/custom-objects"
+                f"{self._environment.value}/",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/custom-objects",
             ),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -405,15 +411,16 @@
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"custom-object-classes/{custom_object_class_id}/custom-objects/{id}"
+                f"{self._environment.value}/",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/custom-objects/{id}",
             ),
             params=remove_none_from_dict(
                 {"include_remote_data": include_remote_data, "include_remote_fields": include_remote_fields}
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -447,15 +454,16 @@
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: CustomObjectRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"custom-object-classes/{custom_object_class_id}/custom-objects/{id}"
+                f"{self._environment.value}/",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/custom-objects/{id}",
             ),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -477,15 +485,15 @@
 
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._environment.value}/",
-                f"custom-object-classes/{custom_object_class_id}/custom-objects/meta/patch/{id}",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/custom-objects/meta/patch/{id}",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
@@ -503,15 +511,15 @@
         Parameters:
             - custom_object_class_id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._environment.value}/",
-                f"custom-object-classes/{custom_object_class_id}/custom-objects/meta/post",
+                f"api/crm/v1/custom-object-classes/{custom_object_class_id}/custom-objects/meta/post",
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/delete_account/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/delete_account/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     def create(self) -> None:
         """
         Delete a linked account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "delete-account"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/delete-account"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
@@ -43,15 +43,15 @@
 
     async def create(self) -> None:
         """
         Delete a linked account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "delete-account"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/delete-account"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/engagement_types/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/engagement_types/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "engagement-types"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/engagement-types"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
@@ -103,15 +103,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"engagement-types/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/engagement-types/{id}"),
             params=remove_none_from_dict(
                 {"include_remote_data": include_remote_data, "include_remote_fields": include_remote_fields}
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -143,15 +143,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "engagement-types/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/engagement-types/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
@@ -212,15 +212,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "engagement-types"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/engagement-types"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
@@ -257,15 +257,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"engagement-types/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/engagement-types/{id}"),
             params=remove_none_from_dict(
                 {"include_remote_data": include_remote_data, "include_remote_fields": include_remote_fields}
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -297,15 +297,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "engagement-types/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/engagement-types/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/engagements/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/engagements/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "engagements"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/engagements"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
@@ -117,15 +117,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: EngagementRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "engagements"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/engagements"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EngagementResponse, _response.json())  # type: ignore
@@ -153,15 +153,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"engagements/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/engagements/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                 }
             ),
@@ -194,15 +194,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: PatchedEngagementRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"engagements/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/engagements/{id}"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EngagementResponse, _response.json())  # type: ignore
@@ -217,15 +217,15 @@
         Returns metadata for `Engagement` PATCHs.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"engagements/meta/patch/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/engagements/meta/patch/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -235,15 +235,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Engagement` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "engagements/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/engagements/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -272,15 +272,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "engagements/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/engagements/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
@@ -344,15 +344,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "engagements"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/engagements"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
@@ -390,15 +390,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: EngagementRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "engagements"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/engagements"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EngagementResponse, _response.json())  # type: ignore
@@ -426,15 +426,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"engagements/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/engagements/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                 }
             ),
@@ -467,15 +467,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: PatchedEngagementRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"engagements/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/engagements/{id}"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EngagementResponse, _response.json())  # type: ignore
@@ -490,15 +490,15 @@
         Returns metadata for `Engagement` PATCHs.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"engagements/meta/patch/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/engagements/meta/patch/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -508,15 +508,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Engagement` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "engagements/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/engagements/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -545,15 +545,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "engagements/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/engagements/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/force_resync/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/force_resync/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     def sync_status_resync_create(self) -> typing.List[SyncStatus]:
         """
         Force re-sync of all models. This is available for all organizations via the dashboard. Force re-sync is also available programmatically via API for monthly, quarterly, and highest sync frequency customers on the Core, Professional, or Enterprise plans. Doing so will consume a sync credit for the relevant linked account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "sync-status/resync"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/sync-status/resync"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[SyncStatus], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -47,15 +47,15 @@
 
     async def sync_status_resync_create(self) -> typing.List[SyncStatus]:
         """
         Force re-sync of all models. This is available for all organizations via the dashboard. Force re-sync is also available programmatically via API for monthly, quarterly, and highest sync frequency customers on the Core, Professional, or Enterprise plans. Doing so will consume a sync credit for the relevant linked account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "sync-status/resync"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/sync-status/resync"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[SyncStatus], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/generate_key/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/regenerate_key/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,61 +12,61 @@
 from .....environment import MergeEnvironment
 from ...types.remote_key import RemoteKey
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class GenerateKeyClient:
+class RegenerateKeyClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def create(self, *, name: str) -> RemoteKey:
         """
-        Create a remote key.
+        Exchange remote keys.
 
         Parameters:
             - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "generate-key"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/regenerate-key"),
             json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncGenerateKeyClient:
+class AsyncRegenerateKeyClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def create(self, *, name: str) -> RemoteKey:
         """
-        Create a remote key.
+        Exchange remote keys.
 
         Parameters:
             - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "generate-key"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/regenerate-key"),
             json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/issues/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/issues/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             - status: typing.Optional[IssuesListRequestStatus]. Status of the issue. Options: ('ONGOING', 'RESOLVED')
 
                                                                 * `ONGOING` - ONGOING
                                                                 * `RESOLVED` - RESOLVED
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "issues"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/issues"),
             params=remove_none_from_dict(
                 {
                     "account_token": account_token,
                     "cursor": cursor,
                     "end_date": end_date,
                     "end_user_organization_name": end_user_organization_name,
                     "first_incident_time_after": first_incident_time_after,
@@ -108,15 +108,15 @@
         Get a specific issue.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"issues/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/issues/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Issue, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -180,15 +180,15 @@
             - status: typing.Optional[IssuesListRequestStatus]. Status of the issue. Options: ('ONGOING', 'RESOLVED')
 
                                                                 * `ONGOING` - ONGOING
                                                                 * `RESOLVED` - RESOLVED
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "issues"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/issues"),
             params=remove_none_from_dict(
                 {
                     "account_token": account_token,
                     "cursor": cursor,
                     "end_date": end_date,
                     "end_user_organization_name": end_user_organization_name,
                     "first_incident_time_after": first_incident_time_after,
@@ -218,15 +218,15 @@
         Get a specific issue.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"issues/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounting/v1/issues/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Issue, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/leads/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/leads/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "leads"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/leads"),
             params=remove_none_from_dict(
                 {
                     "converted_account_id": converted_account_id,
                     "converted_contact_id": converted_contact_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
@@ -128,15 +128,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: LeadRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "leads"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/leads"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(LeadResponse, _response.json())  # type: ignore
@@ -164,15 +164,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"leads/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/leads/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                 }
             ),
@@ -189,15 +189,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Lead` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "leads/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/leads/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -226,15 +226,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "leads/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/leads/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
@@ -307,15 +307,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "leads"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/leads"),
             params=remove_none_from_dict(
                 {
                     "converted_account_id": converted_account_id,
                     "converted_contact_id": converted_contact_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
@@ -356,15 +356,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: LeadRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "leads"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/leads"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(LeadResponse, _response.json())  # type: ignore
@@ -392,15 +392,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"leads/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/leads/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                 }
             ),
@@ -417,15 +417,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Lead` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "leads/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/leads/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -454,15 +454,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "leads/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/leads/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/link_token/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/link_token/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             _request["link_expiry_mins"] = link_expiry_mins
         if should_create_magic_link_url is not OMIT:
             _request["should_create_magic_link_url"] = should_create_magic_link_url
         if common_models is not OMIT:
             _request["common_models"] = common_models
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "link-token"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/link-token"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(LinkToken, _response.json())  # type: ignore
         try:
@@ -138,15 +138,15 @@
             _request["link_expiry_mins"] = link_expiry_mins
         if should_create_magic_link_url is not OMIT:
             _request["should_create_magic_link_url"] = should_create_magic_link_url
         if common_models is not OMIT:
             _request["common_models"] = common_models
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "link-token"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/link-token"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(LinkToken, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/linked_accounts/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/linked_accounts/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - status: typing.Optional[str]. Filter by status. Options: `COMPLETE`, `INCOMPLETE`, `RELINK_NEEDED`
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "linked-accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/linked-accounts"),
             params=remove_none_from_dict(
                 {
                     "category": category,
                     "cursor": cursor,
                     "end_user_email_address": end_user_email_address,
                     "end_user_organization_name": end_user_organization_name,
                     "end_user_origin_id": end_user_origin_id,
@@ -166,15 +166,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - status: typing.Optional[str]. Filter by status. Options: `COMPLETE`, `INCOMPLETE`, `RELINK_NEEDED`
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "linked-accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/linked-accounts"),
             params=remove_none_from_dict(
                 {
                     "category": category,
                     "cursor": cursor,
                     "end_user_email_address": end_user_email_address,
                     "end_user_organization_name": end_user_organization_name,
                     "end_user_origin_id": end_user_origin_id,
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/notes/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/notes/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "notes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/notes"),
             params=remove_none_from_dict(
                 {
                     "account_id": account_id,
                     "contact_id": contact_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
@@ -132,15 +132,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: NoteRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "notes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/notes"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(NoteResponse, _response.json())  # type: ignore
@@ -168,15 +168,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"notes/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/notes/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                 }
             ),
@@ -193,15 +193,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Note` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "notes/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/notes/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -230,15 +230,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "notes/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/notes/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
@@ -314,15 +314,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "notes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/notes"),
             params=remove_none_from_dict(
                 {
                     "account_id": account_id,
                     "contact_id": contact_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
@@ -364,15 +364,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: NoteRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "notes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/notes"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(NoteResponse, _response.json())  # type: ignore
@@ -400,15 +400,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"notes/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/notes/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                 }
             ),
@@ -425,15 +425,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Note` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "notes/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/notes/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -462,15 +462,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "notes/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/notes/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/opportunities/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/opportunities/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
                                                                        * `OPEN` - OPEN
                                                                        * `WON` - WON
                                                                        * `LOST` - LOST
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "opportunities"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/opportunities"),
             params=remove_none_from_dict(
                 {
                     "account_id": account_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -147,15 +147,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: OpportunityRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "opportunities"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/opportunities"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(OpportunityResponse, _response.json())  # type: ignore
@@ -189,15 +189,15 @@
 
             - remote_fields: typing.Optional[typing_extensions.Literal["status"]]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"opportunities/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/opportunities/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
@@ -232,15 +232,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: PatchedOpportunityRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"opportunities/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/opportunities/{id}"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(OpportunityResponse, _response.json())  # type: ignore
@@ -255,15 +255,15 @@
         Returns metadata for `Opportunity` PATCHs.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"opportunities/meta/patch/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/opportunities/meta/patch/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -273,15 +273,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Opportunity` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "opportunities/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/opportunities/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -310,15 +310,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "opportunities/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/opportunities/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
@@ -404,15 +404,15 @@
 
                                                                        * `OPEN` - OPEN
                                                                        * `WON` - WON
                                                                        * `LOST` - LOST
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "opportunities"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/opportunities"),
             params=remove_none_from_dict(
                 {
                     "account_id": account_id,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -456,15 +456,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: OpportunityRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "opportunities"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/opportunities"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(OpportunityResponse, _response.json())  # type: ignore
@@ -498,15 +498,15 @@
 
             - remote_fields: typing.Optional[typing_extensions.Literal["status"]]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["status"]]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"opportunities/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/opportunities/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
@@ -541,15 +541,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: PatchedOpportunityRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"opportunities/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/opportunities/{id}"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(OpportunityResponse, _response.json())  # type: ignore
@@ -564,15 +564,15 @@
         Returns metadata for `Opportunity` PATCHs.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"opportunities/meta/patch/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/opportunities/meta/patch/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -582,15 +582,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Opportunity` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "opportunities/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/opportunities/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -619,15 +619,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "opportunities/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/opportunities/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/passthrough/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/passthrough/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             _request["headers"] = headers
         if request_format is not OMIT:
             _request["request_format"] = request_format
         if normalize_response is not OMIT:
             _request["normalize_response"] = normalize_response
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "passthrough"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/passthrough"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteResponse, _response.json())  # type: ignore
         try:
@@ -137,15 +137,15 @@
             _request["headers"] = headers
         if request_format is not OMIT:
             _request["request_format"] = request_format
         if normalize_response is not OMIT:
             _request["normalize_response"] = normalize_response
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "passthrough"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/passthrough"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteResponse, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/regenerate_key/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/regenerate_key/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         Exchange remote keys.
 
         Parameters:
             - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "regenerate-key"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/regenerate-key"),
             json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
@@ -58,15 +58,15 @@
         Exchange remote keys.
 
         Parameters:
             - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "regenerate-key"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/regenerate-key"),
             json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/selective_sync/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/selective_sync/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     def configurations_list(self) -> typing.List[LinkedAccountSelectiveSyncConfiguration]:
         """
         Get a linked account's selective syncs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/selective-sync/configurations"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -51,15 +51,15 @@
         Replace a linked account's selective syncs.
 
         Parameters:
             - sync_configurations: typing.List[LinkedAccountSelectiveSyncConfigurationRequest]. The selective syncs associated with a linked account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/selective-sync/configurations"),
             json=jsonable_encoder({"sync_configurations": sync_configurations}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
@@ -83,15 +83,15 @@
 
             - cursor: typing.Optional[str]. The pagination cursor value.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/meta"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/selective-sync/meta"),
             params=remove_none_from_dict({"common_model": common_model, "cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedConditionSchemaList, _response.json())  # type: ignore
         try:
@@ -110,15 +110,15 @@
 
     async def configurations_list(self) -> typing.List[LinkedAccountSelectiveSyncConfiguration]:
         """
         Get a linked account's selective syncs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/selective-sync/configurations"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -133,15 +133,15 @@
         Replace a linked account's selective syncs.
 
         Parameters:
             - sync_configurations: typing.List[LinkedAccountSelectiveSyncConfigurationRequest]. The selective syncs associated with a linked account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/selective-sync/configurations"),
             json=jsonable_encoder({"sync_configurations": sync_configurations}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
@@ -165,15 +165,15 @@
 
             - cursor: typing.Optional[str]. The pagination cursor value.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/meta"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/selective-sync/meta"),
             params=remove_none_from_dict({"common_model": common_model, "cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedConditionSchemaList, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/stages/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/stages/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "stages"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/stages"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
@@ -103,15 +103,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"stages/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/stages/{id}"),
             params=remove_none_from_dict(
                 {"include_remote_data": include_remote_data, "include_remote_fields": include_remote_fields}
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -143,15 +143,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "stages/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/stages/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
@@ -212,15 +212,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "stages"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/stages"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
@@ -257,15 +257,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"stages/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/stages/{id}"),
             params=remove_none_from_dict(
                 {"include_remote_data": include_remote_data, "include_remote_fields": include_remote_fields}
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -297,15 +297,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "stages/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/stages/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/sync_status/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/sync_status/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         Parameters:
             - cursor: typing.Optional[str]. The pagination cursor value.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "sync-status"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/sync-status"),
             params=remove_none_from_dict({"cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedSyncStatusList, _response.json())  # type: ignore
         try:
@@ -63,15 +63,15 @@
         Parameters:
             - cursor: typing.Optional[str]. The pagination cursor value.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "sync-status"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/sync-status"),
             params=remove_none_from_dict({"cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedSyncStatusList, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/tasks/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/tasks/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tasks"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/tasks"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
@@ -117,15 +117,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: TaskRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tasks"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/tasks"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TaskResponse, _response.json())  # type: ignore
@@ -153,15 +153,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tasks/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/tasks/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                 }
             ),
@@ -194,15 +194,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: PatchedTaskRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tasks/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/tasks/{id}"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TaskResponse, _response.json())  # type: ignore
@@ -217,15 +217,15 @@
         Returns metadata for `Task` PATCHs.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tasks/meta/patch/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/tasks/meta/patch/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -235,15 +235,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Task` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tasks/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/tasks/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -272,15 +272,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tasks/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/tasks/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
@@ -344,15 +344,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tasks"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/tasks"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
@@ -390,15 +390,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: TaskRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tasks"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/tasks"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TaskResponse, _response.json())  # type: ignore
@@ -426,15 +426,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tasks/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/tasks/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                 }
             ),
@@ -467,15 +467,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: PatchedTaskRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tasks/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/tasks/{id}"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TaskResponse, _response.json())  # type: ignore
@@ -490,15 +490,15 @@
         Returns metadata for `Task` PATCHs.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tasks/meta/patch/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/tasks/meta/patch/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -508,15 +508,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Task` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tasks/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/tasks/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -545,15 +545,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tasks/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/tasks/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/users/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/users/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "users"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/users"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
@@ -108,15 +108,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"users/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/users/{id}"),
             params=remove_none_from_dict(
                 {"include_remote_data": include_remote_data, "include_remote_fields": include_remote_fields}
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -134,15 +134,15 @@
         Parameters:
             - model_id: str.
 
             - request: IgnoreCommonModelRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"users/ignore/{model_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/users/ignore/{model_id}"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
@@ -172,15 +172,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "users/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/users/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
@@ -241,15 +241,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "users"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/users"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
@@ -286,15 +286,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"users/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/users/{id}"),
             params=remove_none_from_dict(
                 {"include_remote_data": include_remote_data, "include_remote_fields": include_remote_fields}
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -312,15 +312,15 @@
         Parameters:
             - model_id: str.
 
             - request: IgnoreCommonModelRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"users/ignore/{model_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/users/ignore/{model_id}"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
@@ -350,15 +350,15 @@
 
             - include_remote_fields: typing.Optional[bool]. Whether to include all remote fields, including fields that Merge did not map to common models, in a normalized format.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "users/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/users/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "page_size": page_size,
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/resources/webhook_receivers/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/webhook_receivers/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def list(self) -> typing.List[WebhookReceiver]:
         """
         Returns a list of `WebhookReceiver` objects.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "webhook-receivers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/webhook-receivers"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[WebhookReceiver], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -53,15 +53,15 @@
             - key: typing.Optional[str]. <span style="white-space: nowrap">`non-empty`</span>
         """
         _request: typing.Dict[str, typing.Any] = {"event": event, "is_active": is_active}
         if key is not OMIT:
             _request["key"] = key
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "webhook-receivers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/webhook-receivers"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(WebhookReceiver, _response.json())  # type: ignore
         try:
@@ -80,15 +80,15 @@
 
     async def list(self) -> typing.List[WebhookReceiver]:
         """
         Returns a list of `WebhookReceiver` objects.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "webhook-receivers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/webhook-receivers"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[WebhookReceiver], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -108,15 +108,15 @@
             - key: typing.Optional[str]. <span style="white-space: nowrap">`non-empty`</span>
         """
         _request: typing.Dict[str, typing.Any] = {"event": event, "is_active": is_active}
         if key is not OMIT:
             _request["key"] = key
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "webhook-receivers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/webhook-receivers"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(WebhookReceiver, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/__init__.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/account.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/account.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/account_details.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/account_details.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/account_details_and_actions.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/account_details_and_actions_integration.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/account_details_and_actions_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/account_integration.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/account_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/account_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/account_token.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/account_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/activity_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/activity_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/address.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/address.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/address_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/address_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/address_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/address_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/association.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/association.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/association_sub_type.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/association_sub_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/association_type.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/association_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/association_type_request_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/association_type_request_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/available_actions.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/cardinality_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/cardinality_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/categories_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/category_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/common_model_scopes_body_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/condition_schema.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/condition_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/contact.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/contact.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/contact_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/contact_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/country_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/country_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/crm_account_response.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/crm_account_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/crm_association_type_response.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/crm_association_type_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/crm_contact_response.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/crm_contact_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/crm_custom_object_response.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/crm_custom_object_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/custom_object.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/custom_object.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/custom_object_class.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/custom_object_class.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/custom_object_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/custom_object_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/debug_mode_log.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/debug_model_log_summary.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/direction_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/direction_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/email_address.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/email_address.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/email_address_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/email_address_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/enabled_actions_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/encoding_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/engagement.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/engagement_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_response.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/engagement_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/engagement_type.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/engagement_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/engagements_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/engagements_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/engagements_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/engagements_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/error_validation_problem.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/field_format_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/field_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/field_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/field_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/ignore_common_model_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/ignore_common_model_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/issue.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/issue.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/issue_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/item_format_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/item_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/item_schema.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/item_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/item_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/item_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/lead.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/lead.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/lead_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/lead_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/lead_response.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/lead_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/leads_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/leads_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/leads_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/leads_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/link_token.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/link_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_condition.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_condition_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_selective_sync_configuration.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_selective_sync_configuration_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_account_status.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/linked_accounts_list_request_category.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/meta_response.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/method_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/model_operation.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/multipart_form_field_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/note.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/note.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/note_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/note_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/note_response.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/note_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/notes_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/notes_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/notes_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/notes_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/object_class_description_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/object_class_description_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/operator_schema.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunities_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/opportunities_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunities_list_request_status.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/opportunities_list_request_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunities_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/opportunities_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/opportunity.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/opportunity_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity_response.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/opportunity_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/opportunity_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/opportunity_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/origin_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/origin_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_account_details_and_actions_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_account_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_account_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_association_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_association_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_association_type_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_association_type_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_condition_schema_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_contact_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_contact_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_custom_object_class_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_custom_object_class_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_custom_object_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_custom_object_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_engagement_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_engagement_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_engagement_type_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_engagement_type_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_issue_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_lead_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_lead_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_note_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_note_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_opportunity_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_opportunity_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_remote_field_class_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_remote_field_class_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_stage_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_stage_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_sync_status_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_task_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_task_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/paginated_user_list.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/paginated_user_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_account_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/patched_account_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_contact_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/patched_contact_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_engagement_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/patched_engagement_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_opportunity_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/patched_opportunity_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/patched_task_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/patched_task_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/phone_number.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/phone_number_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/phone_number_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/reason_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_data.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_field.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_class.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_field_class.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_field_class_for_custom_object_class.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_item_schema.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_field_class_for_custom_object_class_item_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_field_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_field_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_key.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/remote_response.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/request_format_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/response_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/selective_sync_configurations_usage_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/stage.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/stage.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/sync_status.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/sync_status_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/task.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/task.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/task_request.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/task_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/task_response.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/task_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/task_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/task_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/tasks_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/tasks_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/tasks_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/tasks_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/user.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/user.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/validation_problem_source.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/warning_validation_problem.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/crm/types/webhook_receiver.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/__init__.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/__init__.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/account_details/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/account_details/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def retrieve(self) -> AccountDetails:
         """
         Get details for a linked account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/account-details"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/account-details"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountDetails, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -46,15 +46,15 @@
 
     async def retrieve(self) -> AccountDetails:
         """
         Get details for a linked account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/account-details"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/account-details"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountDetails, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/account_token/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/account_token/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         Returns the account token for the end user with the provided public token.
 
         Parameters:
             - public_token: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/account-token/{public_token}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/account-token/{public_token}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -52,15 +52,15 @@
         Returns the account token for the end user with the provided public token.
 
         Parameters:
             - public_token: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/account-token/{public_token}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/crm/v1/account-token/{public_token}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/available_actions/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/bank_info/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/bank_info/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/benefits/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/benefits/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/companies/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/companies/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/delete_account/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/delete_account/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     def create(self) -> None:
         """
         Delete a linked account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/delete-account"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/delete-account"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
@@ -43,15 +43,15 @@
 
     async def create(self) -> None:
         """
         Delete a linked account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/delete-account"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/delete-account"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/employee_payroll_runs/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/employee_payroll_runs/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/employees/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/employees/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/employments/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/employments/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/force_resync/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/generate_key/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/regenerate_key/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,61 +12,61 @@
 from .....environment import MergeEnvironment
 from ...types.remote_key import RemoteKey
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class GenerateKeyClient:
+class RegenerateKeyClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def create(self, *, name: str) -> RemoteKey:
         """
-        Create a remote key.
+        Exchange remote keys.
 
         Parameters:
             - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/generate-key"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/regenerate-key"),
             json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncGenerateKeyClient:
+class AsyncRegenerateKeyClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def create(self, *, name: str) -> RemoteKey:
         """
-        Create a remote key.
+        Exchange remote keys.
 
         Parameters:
             - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/generate-key"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/regenerate-key"),
             json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/groups/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/groups/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/issues/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/link_token/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/link_token/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             _request["link_expiry_mins"] = link_expiry_mins
         if should_create_magic_link_url is not OMIT:
             _request["should_create_magic_link_url"] = should_create_magic_link_url
         if common_models is not OMIT:
             _request["common_models"] = common_models
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/link-token"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/link-token"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(LinkToken, _response.json())  # type: ignore
         try:
@@ -138,15 +138,15 @@
             _request["link_expiry_mins"] = link_expiry_mins
         if should_create_magic_link_url is not OMIT:
             _request["should_create_magic_link_url"] = should_create_magic_link_url
         if common_models is not OMIT:
             _request["common_models"] = common_models
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/link-token"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/link-token"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(LinkToken, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/linked_accounts/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/locations/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/locations/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/passthrough/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/passthrough/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             _request["headers"] = headers
         if request_format is not OMIT:
             _request["request_format"] = request_format
         if normalize_response is not OMIT:
             _request["normalize_response"] = normalize_response
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/passthrough"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/passthrough"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteResponse, _response.json())  # type: ignore
         try:
@@ -137,15 +137,15 @@
             _request["headers"] = headers
         if request_format is not OMIT:
             _request["request_format"] = request_format
         if normalize_response is not OMIT:
             _request["normalize_response"] = normalize_response
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/passthrough"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/passthrough"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteResponse, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/pay_groups/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/pay_groups/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/payroll_runs/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/payroll_runs/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/regenerate_key/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/regenerate_key/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         Exchange remote keys.
 
         Parameters:
             - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/regenerate-key"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/regenerate-key"),
             json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
@@ -58,15 +58,15 @@
         Exchange remote keys.
 
         Parameters:
             - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/regenerate-key"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/regenerate-key"),
             json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/selective_sync/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/sync_status/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/teams/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/teams/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/time_off/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/time_off/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/time_off_balances/client.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/resources/time_off_balances/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/resources/webhook_receivers/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/webhook_receivers/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def list(self) -> typing.List[WebhookReceiver]:
         """
         Returns a list of `WebhookReceiver` objects.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/webhook-receivers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/webhook-receivers"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[WebhookReceiver], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -53,15 +53,15 @@
             - key: typing.Optional[str]. <span style="white-space: nowrap">`non-empty`</span>
         """
         _request: typing.Dict[str, typing.Any] = {"event": event, "is_active": is_active}
         if key is not OMIT:
             _request["key"] = key
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/webhook-receivers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/webhook-receivers"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(WebhookReceiver, _response.json())  # type: ignore
         try:
@@ -80,15 +80,15 @@
 
     async def list(self) -> typing.List[WebhookReceiver]:
         """
         Returns a list of `WebhookReceiver` objects.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/webhook-receivers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/webhook-receivers"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[WebhookReceiver], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -108,15 +108,15 @@
             - key: typing.Optional[str]. <span style="white-space: nowrap">`non-empty`</span>
         """
         _request: typing.Dict[str, typing.Any] = {"event": event, "is_active": is_active}
         if key is not OMIT:
             _request["key"] = key
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/webhook-receivers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/webhook-receivers"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(WebhookReceiver, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/__init__.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/account_details.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/account_details.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/account_details_and_actions.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/account_details_and_actions_integration.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/account_details_and_actions_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/account_integration.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/account_token.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/account_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/account_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/account_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/available_actions.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/bank_info.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/bank_info.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/bank_info_list_request_account_type.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/bank_info_list_request_account_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/bank_info_list_request_order_by.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/bank_info_list_request_order_by.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/benefit.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/benefit.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/categories_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/category_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/common_model_scopes_body_request.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/company.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/company.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/condition_schema.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/condition_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/country_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/country_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/debug_mode_log.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/debug_model_log_summary.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/deduction.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/deduction.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/earning.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/earning.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/earning_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/earning_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employee.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employee.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_payroll_run.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_payroll_run.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_request.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employee_response.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employee_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_list_request_employment_status.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employees_list_request_employment_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employees_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_list_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employees_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employees_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employment.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employment.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employment_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employment_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employment_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employments_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_list_request_order_by.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employments_list_request_order_by.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_list_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employments_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employments_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/enabled_actions_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/encoding_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/error_validation_problem.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/ethnicity_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/ethnicity_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/flsa_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/flsa_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/gender_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/gender_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/group.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/group.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/group_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/group_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/issue.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/issue.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/issue_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/link_token.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/link_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_condition.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_condition_request.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_account_status.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/linked_accounts_list_request_category.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/location.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/location.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/marital_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/marital_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/meta_response.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/method_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/model_operation.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/multipart_form_field_request.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/operator_schema.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_bank_info_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_bank_info_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_benefit_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_benefit_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_company_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_company_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_condition_schema_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_employee_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_employee_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_employment_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_employment_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_group_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_group_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_issue_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_location_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_location_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_pay_group_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_pay_group_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_payroll_run_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_payroll_run_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_sync_status_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_team_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_team_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_time_off_balance_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_time_off_balance_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/paginated_time_off_list.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/paginated_time_off_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/pay_currency_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/pay_currency_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/pay_frequency_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/pay_frequency_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/pay_group.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/pay_group.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/pay_period_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/pay_period_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_run.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/payroll_run.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/policy_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/policy_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/reason_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/remote_data.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/remote_key.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/remote_response.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/request_format_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/request_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/request_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/response_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/run_state_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/run_state_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/run_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/run_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/sync_status.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/sync_status_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/tax.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/tax.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/team.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/team.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_balance.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_balance.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_request_type.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_list_request_request_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_list_request_status.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_list_request_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_request.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_response.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/time_off_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/time_off_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/validation_problem_source.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/warning_validation_problem.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/hris/types/webhook_receiver.py` & `mergepythonclient-0.1.2/src/merge/resources/hris/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/__init__.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/client.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/__init__.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/account_details/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/account_details/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def retrieve(self) -> AccountDetails:
         """
         Get details for a linked account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "account-details"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/account-details"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountDetails, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -46,15 +46,15 @@
 
     async def retrieve(self) -> AccountDetails:
         """
         Get details for a linked account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "account-details"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/account-details"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccountDetails, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/account_token/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/generate_key/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,76 @@
 # This file was auto-generated by Fern from our API Definition.
 
+import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.jsonable_encoder import jsonable_encoder
 from .....environment import MergeEnvironment
-from ...types.account_token import AccountToken
+from ...types.remote_key import RemoteKey
 
+# this is used as the default value for optional parameters
+OMIT = typing.cast(typing.Any, ...)
 
-class AccountTokenClient:
+
+class GenerateKeyClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
-    def retrieve(self, public_token: str) -> AccountToken:
+    def create(self, *, name: str) -> RemoteKey:
         """
-        Returns the account token for the end user with the provided public token.
+        Create a remote key.
 
         Parameters:
-            - public_token: str.
+            - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"account-token/{public_token}"),
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/generate-key"),
+            json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AccountToken, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncAccountTokenClient:
+class AsyncGenerateKeyClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
-    async def retrieve(self, public_token: str) -> AccountToken:
+    async def create(self, *, name: str) -> RemoteKey:
         """
-        Returns the account token for the end user with the provided public token.
+        Create a remote key.
 
         Parameters:
-            - public_token: str.
+            - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"account-token/{public_token}"),
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/generate-key"),
+            json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AccountToken, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/accounts/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/teams/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
-from ...types.account import Account
-from ...types.paginated_account_list import PaginatedAccountList
+from ...types.paginated_team_list import PaginatedTeamList
+from ...types.team import Team
 
 
-class AccountsClient:
+class TeamsClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def list(
@@ -29,17 +29,17 @@
         cursor: typing.Optional[str] = None,
         include_deleted_data: typing.Optional[bool] = None,
         include_remote_data: typing.Optional[bool] = None,
         modified_after: typing.Optional[str] = None,
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
-    ) -> PaginatedAccountList:
+    ) -> PaginatedTeamList:
         """
-        Returns a list of `Account` objects.
+        Returns a list of `Team` objects.
 
         Parameters:
             - created_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - created_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
 
             - cursor: typing.Optional[str]. The pagination cursor value.
@@ -54,15 +54,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/teams"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
@@ -72,47 +72,47 @@
                     "remote_id": remote_id,
                 }
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaginatedAccountList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaginatedTeamList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Account:
+    def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Team:
         """
-        Returns an `Account` object with the given `id`.
+        Returns a `Team` object with the given `id`.
 
         Parameters:
             - id: str.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/teams/{id}"),
             params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Account, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Team, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncAccountsClient:
+class AsyncTeamsClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def list(
@@ -123,17 +123,17 @@
         cursor: typing.Optional[str] = None,
         include_deleted_data: typing.Optional[bool] = None,
         include_remote_data: typing.Optional[bool] = None,
         modified_after: typing.Optional[str] = None,
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
-    ) -> PaginatedAccountList:
+    ) -> PaginatedTeamList:
         """
-        Returns a list of `Account` objects.
+        Returns a list of `Team` objects.
 
         Parameters:
             - created_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - created_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
 
             - cursor: typing.Optional[str]. The pagination cursor value.
@@ -148,15 +148,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/teams"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
@@ -166,37 +166,37 @@
                     "remote_id": remote_id,
                 }
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaginatedAccountList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaginatedTeamList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Account:
+    async def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Team:
         """
-        Returns an `Account` object with the given `id`.
+        Returns a `Team` object with the given `id`.
 
         Parameters:
             - id: str.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/teams/{id}"),
             params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Account, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Team, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/attachments/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/attachments/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
 
             - ticket_id: typing.Optional[str]. If provided, will only return comments for this ticket.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "attachments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/attachments"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
@@ -114,15 +114,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: AttachmentRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "attachments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/attachments"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TicketingAttachmentResponse, _response.json())  # type: ignore
@@ -147,15 +147,15 @@
 
             - expand: typing.Optional[typing_extensions.Literal["ticket"]]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"attachments/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/attachments/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Attachment, _response.json())  # type: ignore
         try:
@@ -169,15 +169,15 @@
         Returns an `Attachment` object with the given `id`.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"attachments/{id}/download"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/attachments/{id}/download"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
@@ -187,15 +187,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `TicketingAttachment` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "attachments/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/attachments/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -250,15 +250,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
 
             - ticket_id: typing.Optional[str]. If provided, will only return comments for this ticket.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "attachments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/attachments"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
@@ -296,15 +296,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: AttachmentRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "attachments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/attachments"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TicketingAttachmentResponse, _response.json())  # type: ignore
@@ -329,15 +329,15 @@
 
             - expand: typing.Optional[typing_extensions.Literal["ticket"]]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"attachments/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/attachments/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Attachment, _response.json())  # type: ignore
         try:
@@ -351,15 +351,15 @@
         Returns an `Attachment` object with the given `id`.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"attachments/{id}/download"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/attachments/{id}/download"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
@@ -369,15 +369,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `TicketingAttachment` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "attachments/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/attachments/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/available_actions/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/available_actions/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def retrieve(self) -> AvailableActions:
         """
         Returns a list of models and actions available for an account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "available-actions"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/available-actions"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AvailableActions, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -46,15 +46,15 @@
 
     async def retrieve(self) -> AvailableActions:
         """
         Returns a list of models and actions available for an account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "available-actions"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/available-actions"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AvailableActions, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/collections/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/collections/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["collection_type"]]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "collections"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/collections"),
             params=remove_none_from_dict(
                 {
                     "collection_type": collection_type,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -130,15 +130,15 @@
 
             - remote_fields: typing.Optional[typing_extensions.Literal["collection_type"]]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["collection_type"]]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"collections/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/collections/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
@@ -178,15 +178,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"collections/{parent_id}/users"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/collections/{parent_id}/users"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "page_size": page_size,
@@ -261,15 +261,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["collection_type"]]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "collections"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/collections"),
             params=remove_none_from_dict(
                 {
                     "collection_type": collection_type,
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
@@ -316,15 +316,15 @@
 
             - remote_fields: typing.Optional[typing_extensions.Literal["collection_type"]]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[typing_extensions.Literal["collection_type"]]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"collections/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/collections/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
                 }
@@ -364,15 +364,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"collections/{parent_id}/users"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/collections/{parent_id}/users"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "page_size": page_size,
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/comments/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/comments/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
 
             - ticket_id: typing.Optional[str]. If provided, will only return comments for this ticket.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "comments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/comments"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
@@ -115,15 +115,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: CommentRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "comments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/comments"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CommentResponse, _response.json())  # type: ignore
@@ -148,15 +148,15 @@
 
             - expand: typing.Optional[CommentsRetrieveRequestExpand]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"comments/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/comments/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Comment, _response.json())  # type: ignore
         try:
@@ -167,15 +167,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Comment` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "comments/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/comments/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -230,15 +230,15 @@
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
 
             - ticket_id: typing.Optional[str]. If provided, will only return comments for this ticket.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "comments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/comments"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
@@ -276,15 +276,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: CommentRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "comments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/comments"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CommentResponse, _response.json())  # type: ignore
@@ -309,15 +309,15 @@
 
             - expand: typing.Optional[CommentsRetrieveRequestExpand]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"comments/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/comments/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Comment, _response.json())  # type: ignore
         try:
@@ -328,15 +328,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Comment` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "comments/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/comments/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/contacts/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/contacts/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "contacts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/contacts"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
@@ -103,15 +103,15 @@
 
             - expand: typing.Optional[typing_extensions.Literal["account"]]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"contacts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/contacts/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Contact, _response.json())  # type: ignore
         try:
@@ -164,15 +164,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "contacts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/contacts"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
@@ -209,15 +209,15 @@
 
             - expand: typing.Optional[typing_extensions.Literal["account"]]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"contacts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/contacts/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Contact, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/delete_account/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/delete_account/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     def create(self) -> None:
         """
         Delete a linked account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "delete-account"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/delete-account"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
@@ -43,15 +43,15 @@
 
     async def create(self) -> None:
         """
         Delete a linked account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "delete-account"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/delete-account"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/force_resync/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/force_resync/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     def sync_status_resync_create(self) -> typing.List[SyncStatus]:
         """
         Force re-sync of all models. This is available for all organizations via the dashboard. Force re-sync is also available programmatically via API for monthly, quarterly, and highest sync frequency customers on the Core, Professional, or Enterprise plans. Doing so will consume a sync credit for the relevant linked account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "sync-status/resync"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/sync-status/resync"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[SyncStatus], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -47,15 +47,15 @@
 
     async def sync_status_resync_create(self) -> typing.List[SyncStatus]:
         """
         Force re-sync of all models. This is available for all organizations via the dashboard. Force re-sync is also available programmatically via API for monthly, quarterly, and highest sync frequency customers on the Core, Professional, or Enterprise plans. Doing so will consume a sync credit for the relevant linked account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "sync-status/resync"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/sync-status/resync"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[SyncStatus], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/generate_key/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/generate_key/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         Create a remote key.
 
         Parameters:
             - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "generate-key"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/generate-key"),
             json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
@@ -58,15 +58,15 @@
         Create a remote key.
 
         Parameters:
             - name: str. <span style="white-space: nowrap">`non-empty`</span>
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "generate-key"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/generate-key"),
             json=jsonable_encoder({"name": name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/issues/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/issues/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             - status: typing.Optional[IssuesListRequestStatus]. Status of the issue. Options: ('ONGOING', 'RESOLVED')
 
                                                                 * `ONGOING` - ONGOING
                                                                 * `RESOLVED` - RESOLVED
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "issues"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/issues"),
             params=remove_none_from_dict(
                 {
                     "account_token": account_token,
                     "cursor": cursor,
                     "end_date": end_date,
                     "end_user_organization_name": end_user_organization_name,
                     "first_incident_time_after": first_incident_time_after,
@@ -108,15 +108,15 @@
         Get a specific issue.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"issues/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/issues/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Issue, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -180,15 +180,15 @@
             - status: typing.Optional[IssuesListRequestStatus]. Status of the issue. Options: ('ONGOING', 'RESOLVED')
 
                                                                 * `ONGOING` - ONGOING
                                                                 * `RESOLVED` - RESOLVED
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "issues"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/issues"),
             params=remove_none_from_dict(
                 {
                     "account_token": account_token,
                     "cursor": cursor,
                     "end_date": end_date,
                     "end_user_organization_name": end_user_organization_name,
                     "first_incident_time_after": first_incident_time_after,
@@ -218,15 +218,15 @@
         Get a specific issue.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"issues/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/issues/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Issue, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/link_token/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/link_token/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             _request["link_expiry_mins"] = link_expiry_mins
         if should_create_magic_link_url is not OMIT:
             _request["should_create_magic_link_url"] = should_create_magic_link_url
         if common_models is not OMIT:
             _request["common_models"] = common_models
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "link-token"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/link-token"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(LinkToken, _response.json())  # type: ignore
         try:
@@ -138,15 +138,15 @@
             _request["link_expiry_mins"] = link_expiry_mins
         if should_create_magic_link_url is not OMIT:
             _request["should_create_magic_link_url"] = should_create_magic_link_url
         if common_models is not OMIT:
             _request["common_models"] = common_models
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "link-token"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/link-token"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(LinkToken, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/linked_accounts/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/linked_accounts/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - status: typing.Optional[str]. Filter by status. Options: `COMPLETE`, `INCOMPLETE`, `RELINK_NEEDED`
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "linked-accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/linked-accounts"),
             params=remove_none_from_dict(
                 {
                     "category": category,
                     "cursor": cursor,
                     "end_user_email_address": end_user_email_address,
                     "end_user_organization_name": end_user_organization_name,
                     "end_user_origin_id": end_user_origin_id,
@@ -166,15 +166,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - status: typing.Optional[str]. Filter by status. Options: `COMPLETE`, `INCOMPLETE`, `RELINK_NEEDED`
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "linked-accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/linked-accounts"),
             params=remove_none_from_dict(
                 {
                     "category": category,
                     "cursor": cursor,
                     "end_user_email_address": end_user_email_address,
                     "end_user_organization_name": end_user_organization_name,
                     "end_user_origin_id": end_user_origin_id,
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/passthrough/client.py` & `mergepythonclient-0.1.2/src/merge/resources/crm/resources/passthrough/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             _request["headers"] = headers
         if request_format is not OMIT:
             _request["request_format"] = request_format
         if normalize_response is not OMIT:
             _request["normalize_response"] = normalize_response
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "passthrough"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/passthrough"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteResponse, _response.json())  # type: ignore
         try:
@@ -137,15 +137,15 @@
             _request["headers"] = headers
         if request_format is not OMIT:
             _request["request_format"] = request_format
         if normalize_response is not OMIT:
             _request["normalize_response"] = normalize_response
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "passthrough"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/crm/v1/passthrough"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteResponse, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/projects/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/projects/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "projects"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/projects"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
@@ -92,15 +92,15 @@
         Parameters:
             - id: str.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"projects/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/projects/{id}"),
             params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Project, _response.json())  # type: ignore
         try:
@@ -133,15 +133,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"projects/{parent_id}/users"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/projects/{parent_id}/users"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "page_size": page_size,
@@ -199,15 +199,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "projects"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/projects"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
@@ -235,15 +235,15 @@
         Parameters:
             - id: str.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"projects/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/projects/{id}"),
             params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Project, _response.json())  # type: ignore
         try:
@@ -276,15 +276,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"projects/{parent_id}/users"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/projects/{parent_id}/users"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "page_size": page_size,
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/regenerate_key/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/account_token/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,76 +1,69 @@
 # This file was auto-generated by Fern from our API Definition.
 
-import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
-from .....core.jsonable_encoder import jsonable_encoder
 from .....environment import MergeEnvironment
-from ...types.remote_key import RemoteKey
+from ...types.account_token import AccountToken
 
-# this is used as the default value for optional parameters
-OMIT = typing.cast(typing.Any, ...)
 
-
-class RegenerateKeyClient:
+class AccountTokenClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
-    def create(self, *, name: str) -> RemoteKey:
+    def retrieve(self, public_token: str) -> AccountToken:
         """
-        Exchange remote keys.
+        Returns the account token for the end user with the provided public token.
 
         Parameters:
-            - name: str. <span style="white-space: nowrap">`non-empty`</span>
+            - public_token: str.
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "regenerate-key"),
-            json=jsonable_encoder({"name": name}),
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/account-token/{public_token}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(AccountToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncRegenerateKeyClient:
+class AsyncAccountTokenClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
-    async def create(self, *, name: str) -> RemoteKey:
+    async def retrieve(self, public_token: str) -> AccountToken:
         """
-        Exchange remote keys.
+        Returns the account token for the end user with the provided public token.
 
         Parameters:
-            - name: str. <span style="white-space: nowrap">`non-empty`</span>
+            - public_token: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "regenerate-key"),
-            json=jsonable_encoder({"name": name}),
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/account-token/{public_token}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RemoteKey, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(AccountToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/selective_sync/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/selective_sync/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     def configurations_list(self) -> typing.List[LinkedAccountSelectiveSyncConfiguration]:
         """
         Get a linked account's selective syncs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/selective-sync/configurations"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -51,15 +51,15 @@
         Replace a linked account's selective syncs.
 
         Parameters:
             - sync_configurations: typing.List[LinkedAccountSelectiveSyncConfigurationRequest]. The selective syncs associated with a linked account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/selective-sync/configurations"),
             json=jsonable_encoder({"sync_configurations": sync_configurations}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
@@ -83,15 +83,15 @@
 
             - cursor: typing.Optional[str]. The pagination cursor value.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/meta"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/selective-sync/meta"),
             params=remove_none_from_dict({"common_model": common_model, "cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedConditionSchemaList, _response.json())  # type: ignore
         try:
@@ -110,15 +110,15 @@
 
     async def configurations_list(self) -> typing.List[LinkedAccountSelectiveSyncConfiguration]:
         """
         Get a linked account's selective syncs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/selective-sync/configurations"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -133,15 +133,15 @@
         Replace a linked account's selective syncs.
 
         Parameters:
             - sync_configurations: typing.List[LinkedAccountSelectiveSyncConfigurationRequest]. The selective syncs associated with a linked account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/selective-sync/configurations"),
             json=jsonable_encoder({"sync_configurations": sync_configurations}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
@@ -165,15 +165,15 @@
 
             - cursor: typing.Optional[str]. The pagination cursor value.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "selective-sync/meta"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/selective-sync/meta"),
             params=remove_none_from_dict({"common_model": common_model, "cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedConditionSchemaList, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/sync_status/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/sync_status/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         Parameters:
             - cursor: typing.Optional[str]. The pagination cursor value.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "sync-status"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/sync-status"),
             params=remove_none_from_dict({"cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedSyncStatusList, _response.json())  # type: ignore
         try:
@@ -63,15 +63,15 @@
         Parameters:
             - cursor: typing.Optional[str]. The pagination cursor value.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "sync-status"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/sync-status"),
             params=remove_none_from_dict({"cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedSyncStatusList, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/tags/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/accounts/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
-from ...types.paginated_tag_list import PaginatedTagList
-from ...types.tag import Tag
+from ...types.account import Account
+from ...types.paginated_account_list import PaginatedAccountList
 
 
-class TagsClient:
+class AccountsClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def list(
@@ -29,17 +29,17 @@
         cursor: typing.Optional[str] = None,
         include_deleted_data: typing.Optional[bool] = None,
         include_remote_data: typing.Optional[bool] = None,
         modified_after: typing.Optional[str] = None,
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
-    ) -> PaginatedTagList:
+    ) -> PaginatedAccountList:
         """
-        Returns a list of `Tag` objects.
+        Returns a list of `Account` objects.
 
         Parameters:
             - created_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - created_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
 
             - cursor: typing.Optional[str]. The pagination cursor value.
@@ -54,15 +54,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tags"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/accounts"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
@@ -72,47 +72,47 @@
                     "remote_id": remote_id,
                 }
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaginatedTagList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaginatedAccountList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Tag:
+    def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Account:
         """
-        Returns a `Tag` object with the given `id`.
+        Returns an `Account` object with the given `id`.
 
         Parameters:
             - id: str.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tags/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/accounts/{id}"),
             params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Tag, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Account, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncTagsClient:
+class AsyncAccountsClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def list(
@@ -123,17 +123,17 @@
         cursor: typing.Optional[str] = None,
         include_deleted_data: typing.Optional[bool] = None,
         include_remote_data: typing.Optional[bool] = None,
         modified_after: typing.Optional[str] = None,
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
-    ) -> PaginatedTagList:
+    ) -> PaginatedAccountList:
         """
-        Returns a list of `Tag` objects.
+        Returns a list of `Account` objects.
 
         Parameters:
             - created_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - created_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
 
             - cursor: typing.Optional[str]. The pagination cursor value.
@@ -148,15 +148,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tags"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/accounts"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
@@ -166,37 +166,37 @@
                     "remote_id": remote_id,
                 }
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaginatedTagList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaginatedAccountList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Tag:
+    async def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Account:
         """
-        Returns a `Tag` object with the given `id`.
+        Returns an `Account` object with the given `id`.
 
         Parameters:
             - id: str.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tags/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/accounts/{id}"),
             params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Tag, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Account, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/teams/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/tags/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
-from ...types.paginated_team_list import PaginatedTeamList
-from ...types.team import Team
+from ...types.paginated_tag_list import PaginatedTagList
+from ...types.tag import Tag
 
 
-class TeamsClient:
+class TagsClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def list(
@@ -29,17 +29,17 @@
         cursor: typing.Optional[str] = None,
         include_deleted_data: typing.Optional[bool] = None,
         include_remote_data: typing.Optional[bool] = None,
         modified_after: typing.Optional[str] = None,
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
-    ) -> PaginatedTeamList:
+    ) -> PaginatedTagList:
         """
-        Returns a list of `Team` objects.
+        Returns a list of `Tag` objects.
 
         Parameters:
             - created_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - created_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
 
             - cursor: typing.Optional[str]. The pagination cursor value.
@@ -54,15 +54,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "teams"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/tags"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
@@ -72,47 +72,47 @@
                     "remote_id": remote_id,
                 }
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaginatedTeamList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaginatedTagList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Team:
+    def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Tag:
         """
-        Returns a `Team` object with the given `id`.
+        Returns a `Tag` object with the given `id`.
 
         Parameters:
             - id: str.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"teams/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/tags/{id}"),
             params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Team, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Tag, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncTeamsClient:
+class AsyncTagsClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def list(
@@ -123,17 +123,17 @@
         cursor: typing.Optional[str] = None,
         include_deleted_data: typing.Optional[bool] = None,
         include_remote_data: typing.Optional[bool] = None,
         modified_after: typing.Optional[str] = None,
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
-    ) -> PaginatedTeamList:
+    ) -> PaginatedTagList:
         """
-        Returns a list of `Team` objects.
+        Returns a list of `Tag` objects.
 
         Parameters:
             - created_after: typing.Optional[str]. If provided, will only return objects created after this datetime.
 
             - created_before: typing.Optional[str]. If provided, will only return objects created before this datetime.
 
             - cursor: typing.Optional[str]. The pagination cursor value.
@@ -148,15 +148,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "teams"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/tags"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
@@ -166,37 +166,37 @@
                     "remote_id": remote_id,
                 }
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaginatedTeamList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaginatedTagList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Team:
+    async def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Tag:
         """
-        Returns a `Team` object with the given `id`.
+        Returns a `Tag` object with the given `id`.
 
         Parameters:
             - id: str.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"teams/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/tags/{id}"),
             params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Team, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Tag, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/tickets/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/tickets/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                                                                  * `ON_HOLD` - ON_HOLD
             - tags: typing.Optional[str]. If provided, will only return tickets matching the tags; multiple tags can be separated by commas.
 
             - ticket_type: typing.Optional[str]. If provided, will only return tickets of this type.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tickets"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/tickets"),
             params=remove_none_from_dict(
                 {
                     "account_id": account_id,
                     "assignee_ids": assignee_ids,
                     "collection_ids": collection_ids,
                     "completed_after": completed_after,
                     "completed_before": completed_before,
@@ -213,15 +213,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: TicketRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tickets"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/tickets"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TicketResponse, _response.json())  # type: ignore
@@ -255,15 +255,15 @@
 
             - remote_fields: typing.Optional[TicketsRetrieveRequestRemoteFields]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[TicketsRetrieveRequestShowEnumOrigins]. Which fields should be returned in non-normalized form.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tickets/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/tickets/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
@@ -298,15 +298,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: PatchedTicketRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tickets/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/tickets/{id}"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TicketResponse, _response.json())  # type: ignore
@@ -340,15 +340,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tickets/{parent_id}/collaborators"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/tickets/{parent_id}/collaborators"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "page_size": page_size,
@@ -370,15 +370,15 @@
         Returns metadata for `Ticket` PATCHs.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tickets/meta/patch/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/tickets/meta/patch/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -388,15 +388,15 @@
 
     def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Ticket` POSTs.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tickets/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/tickets/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -422,15 +422,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tickets/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/tickets/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "page_size": page_size,
                 }
@@ -561,15 +561,15 @@
                                                                  * `ON_HOLD` - ON_HOLD
             - tags: typing.Optional[str]. If provided, will only return tickets matching the tags; multiple tags can be separated by commas.
 
             - ticket_type: typing.Optional[str]. If provided, will only return tickets of this type.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tickets"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/tickets"),
             params=remove_none_from_dict(
                 {
                     "account_id": account_id,
                     "assignee_ids": assignee_ids,
                     "collection_ids": collection_ids,
                     "completed_after": completed_after,
                     "completed_before": completed_before,
@@ -627,15 +627,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: TicketRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tickets"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/tickets"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TicketResponse, _response.json())  # type: ignore
@@ -669,15 +669,15 @@
 
             - remote_fields: typing.Optional[TicketsRetrieveRequestRemoteFields]. Deprecated. Use show_enum_origins.
 
             - show_enum_origins: typing.Optional[TicketsRetrieveRequestShowEnumOrigins]. Which fields should be returned in non-normalized form.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tickets/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/tickets/{id}"),
             params=remove_none_from_dict(
                 {
                     "expand": expand,
                     "include_remote_data": include_remote_data,
                     "include_remote_fields": include_remote_fields,
                     "remote_fields": remote_fields,
                     "show_enum_origins": show_enum_origins,
@@ -712,15 +712,15 @@
 
             - run_async: typing.Optional[bool]. Whether or not third-party updates should be run asynchronously.
 
             - model: PatchedTicketRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tickets/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/tickets/{id}"),
             params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TicketResponse, _response.json())  # type: ignore
@@ -754,15 +754,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tickets/{parent_id}/collaborators"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/tickets/{parent_id}/collaborators"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "expand": expand,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "page_size": page_size,
@@ -784,15 +784,15 @@
         Returns metadata for `Ticket` PATCHs.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"tickets/meta/patch/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/tickets/meta/patch/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -802,15 +802,15 @@
 
     async def meta_post_retrieve(self) -> MetaResponse:
         """
         Returns metadata for `Ticket` POSTs.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tickets/meta/post"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/tickets/meta/post"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -836,15 +836,15 @@
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
 
             - page_size: typing.Optional[int]. Number of results to return per page.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "tickets/remote-field-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/tickets/remote-field-classes"),
             params=remove_none_from_dict(
                 {
                     "cursor": cursor,
                     "include_deleted_data": include_deleted_data,
                     "include_remote_data": include_remote_data,
                     "page_size": page_size,
                 }
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/users/client.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/resources/users/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "users"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/users"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "email_address": email_address,
                     "expand": expand,
@@ -108,15 +108,15 @@
 
             - expand: typing.Optional[UsersRetrieveRequestExpand]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"users/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/users/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(User, _response.json())  # type: ignore
         try:
@@ -172,15 +172,15 @@
 
             - page_size: typing.Optional[int]. Number of results to return per page.
 
             - remote_id: typing.Optional[str]. The API provider's ID for the given object.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "users"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ticketing/v1/users"),
             params=remove_none_from_dict(
                 {
                     "created_after": created_after,
                     "created_before": created_before,
                     "cursor": cursor,
                     "email_address": email_address,
                     "expand": expand,
@@ -218,15 +218,15 @@
 
             - expand: typing.Optional[UsersRetrieveRequestExpand]. Which relations should be returned in expanded form. Multiple relation names should be comma separated without spaces.
 
             - include_remote_data: typing.Optional[bool]. Whether to include the original data Merge fetched from the third-party to produce these models.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"users/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ticketing/v1/users/{id}"),
             params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(User, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/resources/webhook_receivers/client.py` & `mergepythonclient-0.1.2/src/merge/resources/accounting/resources/webhook_receivers/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def list(self) -> typing.List[WebhookReceiver]:
         """
         Returns a list of `WebhookReceiver` objects.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "webhook-receivers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/webhook-receivers"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[WebhookReceiver], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -53,15 +53,15 @@
             - key: typing.Optional[str]. <span style="white-space: nowrap">`non-empty`</span>
         """
         _request: typing.Dict[str, typing.Any] = {"event": event, "is_active": is_active}
         if key is not OMIT:
             _request["key"] = key
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "webhook-receivers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/webhook-receivers"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(WebhookReceiver, _response.json())  # type: ignore
         try:
@@ -80,15 +80,15 @@
 
     async def list(self) -> typing.List[WebhookReceiver]:
         """
         Returns a list of `WebhookReceiver` objects.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "webhook-receivers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/webhook-receivers"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[WebhookReceiver], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -108,15 +108,15 @@
             - key: typing.Optional[str]. <span style="white-space: nowrap">`non-empty`</span>
         """
         _request: typing.Dict[str, typing.Any] = {"event": event, "is_active": is_active}
         if key is not OMIT:
             _request["key"] = key
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "webhook-receivers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/accounting/v1/webhook-receivers"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(WebhookReceiver, _response.json())  # type: ignore
         try:
```

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/__init__.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/access_level_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/access_level_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/account.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_details.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/account_details.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_details_and_actions.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_details_and_actions_integration.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_details_and_actions_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_integration.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/account_token.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/account_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/attachment.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/attachment.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/attachment_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/attachment_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/available_actions.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/categories_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/category_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collection.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/collection.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collection_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/collection_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collections_list_request_collection_type.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/collections_list_request_collection_type.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/collections_users_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/collections_users_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comment.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/comment.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comment_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/comment_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comment_response.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/comment_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comments_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/comments_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/comments_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/comments_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/common_model_scopes_body_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/condition_schema.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/condition_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/contact.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/contact.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/debug_mode_log.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/debug_model_log_summary.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/enabled_actions_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/encoding_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/error_validation_problem.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/field_format_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/field_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/field_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/field_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/issue.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/issue.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/issue_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/item_format_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/item_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/item_schema.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/item_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/item_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/item_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/link_token.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/link_token.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_condition.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_condition_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_account_status.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/linked_accounts_list_request_category.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/meta_response.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/method_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/model_operation.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/multipart_form_field_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/operator_schema.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_account_details_and_actions_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_account_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_account_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_attachment_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_attachment_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_collection_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_collection_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_comment_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_comment_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_condition_schema_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_contact_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_contact_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_issue_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_project_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_project_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_remote_field_class_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_remote_field_class_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_sync_status_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_tag_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_tag_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_team_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_team_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_ticket_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_ticket_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/paginated_user_list.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/paginated_user_list.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/patched_ticket_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/patched_ticket_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/priority_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/priority_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/project.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/project.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/projects_users_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/projects_users_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_data.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_field.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/remote_field.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_field_class.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/remote_field_class.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_field_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/remote_field_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_key.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/remote_response.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/request_format_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/response_type_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/selective_sync_configurations_usage_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/sync_status.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/sync_status_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tag.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tag.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/team.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/team.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/ticket.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_request.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/ticket_request.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_response.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/ticket_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticket_status_enum.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/ticket_status_enum.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/ticketing_attachment_response.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/ticketing_attachment_response.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_collaborators_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_collaborators_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_priority.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_list_request_priority.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_list_request_status.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_list_request_status.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_retrieve_request_remote_fields.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/tickets_retrieve_request_show_enum_origins.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/tickets_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/user.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/user.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/users_list_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/users_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/users_retrieve_request_expand.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/users_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/validation_problem_source.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/warning_validation_problem.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/src/merge/resources/ticketing/types/webhook_receiver.py` & `mergepythonclient-0.1.2/src/merge/resources/ticketing/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `mergepythonclient-0.1.1/PKG-INFO` & `mergepythonclient-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergepythonclient
-Version: 0.1.1
+Version: 0.1.2
 Summary: Client library for the merge API
 Home-page: https://github.com/merge-api/merge-python-client
 License: custom
 Author: Merge
 Author-email: hello@merge.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
@@ -38,25 +38,25 @@
 
 ## Instantiation
 
 ```python
 import merge
 from merge.client import Merge
 
-client = Merge(api_key="Bearer YOUR_API_KEY", account_token="YOUR_ACCOUNT_TOKEN")
+client = Merge(api_key="YOUR_API_KEY", account_token="YOUR_ACCOUNT_TOKEN")
 ```
 
 ## Categories
 
 This SDK contains both the ATS, HRIS, CRM, Ticketing, and Accounting categories. Even if you do not plan on using more than one Merge API category right now, the SDK provides upgrade-flexibility in case you find new Merge API categories useful in the future.
 
 Each category is namespaced:
 
 ```python
-client = Merge(api_key="Bearer YOUR_API_KEY")
+client = Merge(api_key="YOUR_API_KEY")
 
 client.ats. # APIs specific to the ATS Category
 
 client.hris. # APIs specific to the HRIS Category
 ```
 
 ## Usage
@@ -102,15 +102,15 @@
 import merge
 from merge.client import Merge
 
 merge_client = Merge(
     api_key="<YOUR_API_KEY>", 
     account_token="<YOUR_ACCOUNT_TOKEN>")
 
-candidate = merge_client.ats.candiates.retrieve(
+candidate = merge_client.ats.candidates.retrieve(
     id="521b18c2-4d01-4297-b451-19858d07c133")
 ```
 
 ## Filter Candidate
 
 ```python
 import merge
```

