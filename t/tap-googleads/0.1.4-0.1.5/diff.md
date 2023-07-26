# Comparing `tmp/tap_googleads-0.1.4.tar.gz` & `tmp/tap_googleads-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_googleads-0.1.4.tar", max compression
+gzip compressed data, was "tap_googleads-0.1.5.tar", max compression
```

## Comparing `tap_googleads-0.1.4.tar` & `tap_googleads-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      720 2023-04-03 14:58:45.221626 tap_googleads-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-06 18:20:33.330671 tap_googleads-0.1.4/tap_googleads/__init__.py
--rw-r--r--   0        0        0      539 2023-01-06 18:20:33.330671 tap_googleads-0.1.4/tap_googleads/auth.py
--rw-r--r--   0        0        0     6673 2023-04-03 14:50:49.131720 tap_googleads-0.1.4/tap_googleads/client.py
--rw-r--r--   0        0        0     2238 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/schemas/ad_group.json
--rw-r--r--   0        0        0     1218 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/schemas/ad_group_performance.json
--rw-r--r--   0        0        0      477 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/schemas/campaign.json
--rw-r--r--   0        0        0     1640 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/schemas/campaign_label.json
--rw-r--r--   0        0        0     1284 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/schemas/campaign_performance.json
--rw-r--r--   0        0        0     2309 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/schemas/campaign_performance_by_age_range_and_device.json
--rw-r--r--   0        0        0     2305 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/schemas/campaign_performance_by_gender_and_device.json
--rw-r--r--   0        0        0     1780 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/schemas/campaign_performance_by_location.json
--rw-r--r--   0        0        0     1541 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/schemas/conversion_by_location.json
--rw-r--r--   0        0        0     1659 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/schemas/customer.json
--rw-r--r--   0        0        0      838 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/schemas/geo_target_constant.json
--rw-r--r--   0        0        0    15798 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/streams.py
--rw-r--r--   0        0        0     3208 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/tap.py
--rw-r--r--   0        0        0       36 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/tests/__init__.py
--rw-r--r--   0        0        0      922 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/tests/test_core.py
--rw-r--r--   0        0        0     3475 2023-04-03 14:54:52.941671 tap_googleads-0.1.4/tap_googleads/tests/test_customer_not_found.py
--rw-r--r--   0        0        0      733 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/tests/test_utils.py
--rw-r--r--   0        0        0      982 2023-01-06 18:20:33.340671 tap_googleads-0.1.4/tap_googleads/utils.py
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 tap_googleads-0.1.4/setup.py
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 tap_googleads-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      718 2023-07-26 16:07:00.181819 tap_googleads-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-06 18:20:33.330671 tap_googleads-0.1.5/tap_googleads/__init__.py
+-rw-r--r--   0        0        0      539 2023-01-06 18:20:33.330671 tap_googleads-0.1.5/tap_googleads/auth.py
+-rw-r--r--   0        0        0     5400 2023-07-26 16:06:23.011371 tap_googleads-0.1.5/tap_googleads/client.py
+-rw-r--r--   0        0        0     2238 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/ad_group.json
+-rw-r--r--   0        0        0     1218 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/ad_group_performance.json
+-rw-r--r--   0        0        0      477 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/campaign.json
+-rw-r--r--   0        0        0     1640 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/campaign_label.json
+-rw-r--r--   0        0        0     1659 2023-07-26 16:06:23.011371 tap_googleads-0.1.5/tap_googleads/schemas/campaign_performance.json
+-rw-r--r--   0        0        0     2309 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/campaign_performance_by_age_range_and_device.json
+-rw-r--r--   0        0        0     2305 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/campaign_performance_by_gender_and_device.json
+-rw-r--r--   0        0        0     1780 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/campaign_performance_by_location.json
+-rw-r--r--   0        0        0     1541 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/conversion_by_location.json
+-rw-r--r--   0        0        0     1659 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/customer.json
+-rw-r--r--   0        0        0     1682 2023-07-26 16:06:23.011371 tap_googleads-0.1.5/tap_googleads/schemas/customer_hierarchy.json
+-rw-r--r--   0        0        0      838 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/geo_target_constant.json
+-rw-r--r--   0        0        0    15532 2023-07-26 16:06:23.011371 tap_googleads-0.1.5/tap_googleads/streams.py
+-rw-r--r--   0        0        0     3432 2023-07-26 16:06:23.011371 tap_googleads-0.1.5/tap_googleads/tap.py
+-rw-r--r--   0        0        0       36 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/tests/__init__.py
+-rw-r--r--   0        0        0      711 2023-07-26 16:06:23.011371 tap_googleads-0.1.5/tap_googleads/tests/test_core.py
+-rw-r--r--   0        0        0     3314 2023-07-26 16:06:23.011371 tap_googleads-0.1.5/tap_googleads/tests/test_customer_not_found.py
+-rw-r--r--   0        0        0      733 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/tests/test_utils.py
+-rw-r--r--   0        0        0      982 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/utils.py
+-rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 tap_googleads-0.1.5/PKG-INFO
```

### Comparing `tap_googleads-0.1.4/pyproject.toml` & `tap_googleads-0.1.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "tap-googleads"
-version = "0.1.4"
+version = "0.1.5"
 description = "`tap-googleads` is a Singer tap for GoogleAds, built with the Meltano SDK for Singer Taps."
 authors = ["AutoIDM"]
 keywords = [
     "ELT",
     "GoogleAds",
 ]
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
-python = "<3.11,>=3.6.2"
+python = "<3.11,>=3.8"
 requests = "^2.25.1"
-singer-sdk = "0.3.17"
+singer-sdk = "0.29.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 tox = "^3.24.4"
 flake8 = "^3.9.2"
-black = "^21.9b0"
+black = "^23.7.0"
 pydocstyle = "^6.1.1"
 mypy = "^0.910"
 types-requests = "^2.25.8"
 responses = "0.17.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `tap_googleads-0.1.4/tap_googleads/auth.py` & `tap_googleads-0.1.5/tap_googleads/auth.py`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.4/tap_googleads/client.py` & `tap_googleads-0.1.5/tap_googleads/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,63 @@
 """REST client handling, including GoogleAdsStream base class."""
 
-import requests
+from urllib.parse import urlencode, urljoin
 from pathlib import Path
 from typing import Any, Dict, Optional, Union, List, Iterable
 
 from memoization import cached
 
 from singer_sdk.helpers.jsonpath import extract_jsonpath
 from singer_sdk.streams import RESTStream
 from singer_sdk.exceptions import FatalAPIError, RetriableAPIError
+from singer_sdk.pagination import JSONPathPaginator
 
 from tap_googleads.auth import GoogleAdsAuthenticator
 from tap_googleads.utils import replicate_pk_at_root
 
 
 SCHEMAS_DIR = Path(__file__).parent / Path("./schemas")
 
 
 class GoogleAdsStream(RESTStream):
     """GoogleAds stream class."""
 
-    url_base = "https://googleads.googleapis.com/v12"
+    url_base = "https://googleads.googleapis.com/v14"
 
     records_jsonpath = "$[*]"  # Or override `parse_response`.
-    next_page_token_jsonpath = "$.nextPageToken"  # Or override `get_next_page_token`.
+    next_page_token_jsonpath = "$.nextPageToken"
     primary_keys_jsonpaths = None
     _LOG_REQUEST_METRIC_URLS: bool = True
 
     @property
     @cached
     def authenticator(self) -> GoogleAdsAuthenticator:
         """Return a new authenticator object."""
         base_auth_url = "https://www.googleapis.com/oauth2/v4/token"
-        # Silly way to do parameters but it works
-        auth_url = base_auth_url + f"?refresh_token={self.config['refresh_token']}"
-        auth_url = auth_url + f"&client_id={self.config['client_id']}"
-        auth_url = auth_url + f"&client_secret={self.config['client_secret']}"
-        auth_url = auth_url + f"&grant_type=refresh_token"
+        auth_params = {
+            "refresh_token": self.config["refresh_token"],
+            "client_id": self.config["client_id"],
+            "client_secret": self.config["client_secret"],
+            "grant_type": "refresh_token",
+        }
+        auth_url = urljoin(base_auth_url, "?" + urlencode(auth_params))
         return GoogleAdsAuthenticator(stream=self, auth_endpoint=auth_url)
 
     @property
     def http_headers(self) -> dict:
         """Return the http headers needed."""
         headers = {}
         if "user_agent" in self.config:
             headers["User-Agent"] = self.config.get("user_agent")
         headers["developer-token"] = self.config["developer_token"]
         headers["login-customer-id"] = self.config["login_customer_id"]
         return headers
 
-    def get_next_page_token(
-        self, response: requests.Response, previous_token: Optional[Any]
-    ) -> Optional[Any]:
-        """Return a token for identifying next page or None if no more pages."""
-        # TODO: If pagination is required, return a token which can be used to get the
-        #       next page. If this is the final page, return "None" to end the
-        #       pagination loop.
-        if self.next_page_token_jsonpath:
-            all_matches = extract_jsonpath(
-                self.next_page_token_jsonpath, response.json()
-            )
-            first_match = next(iter(all_matches), None)
-            next_page_token = first_match
-        else:
-            next_page_token = None
-
-        return next_page_token
+    def get_new_paginator(self) -> JSONPathPaginator:
+        return JSONPathPaginator(self.next_page_token_jsonpath)
 
     def get_url_params(
         self, context: Optional[dict], next_page_token: Optional[Any]
     ) -> Dict[str, Any]:
         """Return a dictionary of values to be used in URL parameterization."""
         params: dict = {}
         if next_page_token:
@@ -141,29 +129,14 @@
             self.logger.warning(
                 "We hit the Customer Not Enabled error. "
                 "Happens when we get a customer from the hierarchy list that "
                 "isn't enabled anymore, most likely due to a customer being "
                 f"disabled after the API that lists customers is called.  {e=}"
             )
 
-    def prepare_request_payload(
-        self, context: Optional[dict], next_page_token: Optional[Any]
-    ) -> Optional[dict]:
-        """Prepare the data payload for the REST API request.
-
-        By default, no payload will be sent (return None).
-        """
-        # TODO: Delete this method if no payload is required. (Most REST APIs.)
-        return None
-
-    def parse_response(self, response: requests.Response) -> Iterable[dict]:
-        """Parse the response and return an iterator of result rows."""
-        # TODO: Parse response body and return a set of records.
-        yield from extract_jsonpath(self.records_jsonpath, input=response.json())
-
     def post_process(self, row: dict, context: Optional[dict] = None) -> Optional[dict]:
         """As needed, append or transform raw data to match expected structure."""
         return replicate_pk_at_root(row, self.primary_keys_jsonpaths)
 
 
 class CustomerNotEnabledError(Exception):
     """
```

### Comparing `tap_googleads-0.1.4/tap_googleads/schemas/ad_group.json` & `tap_googleads-0.1.5/tap_googleads/schemas/ad_group.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.4/tap_googleads/schemas/ad_group_performance.json` & `tap_googleads-0.1.5/tap_googleads/schemas/ad_group_performance.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.4/tap_googleads/schemas/campaign_label.json` & `tap_googleads-0.1.5/tap_googleads/schemas/campaign_label.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.4/tap_googleads/schemas/campaign_performance.json` & `tap_googleads-0.1.5/tap_googleads/schemas/campaign_performance.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955357142857143%*

 * *Differences: {"'properties'": "{'campaign': {'properties': {'startDate': OrderedDict([('type', 'string')]), "*

 * *                 "'endDate': OrderedDict([('type', 'string')]), 'advertisingChannelType': "*

 * *                 "OrderedDict([('type', 'string')]), 'AdvertisingChannelSubType': "*

 * *                 "OrderedDict([('type', 'string')])}}}"}*

```diff
@@ -1,20 +1,32 @@
 {
     "properties": {
         "_sdc_primary_key": {
             "type": "string"
         },
         "campaign": {
             "properties": {
+                "AdvertisingChannelSubType": {
+                    "type": "string"
+                },
+                "advertisingChannelType": {
+                    "type": "string"
+                },
+                "endDate": {
+                    "type": "string"
+                },
                 "name": {
                     "type": "string"
                 },
                 "resourceName": {
                     "type": "string"
                 },
+                "startDate": {
+                    "type": "string"
+                },
                 "status": {
                     "type": "string"
                 }
             },
             "type": "object"
         },
         "metrics": {
```

### Comparing `tap_googleads-0.1.4/tap_googleads/schemas/campaign_performance_by_age_range_and_device.json` & `tap_googleads-0.1.5/tap_googleads/schemas/campaign_performance_by_age_range_and_device.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.4/tap_googleads/schemas/campaign_performance_by_gender_and_device.json` & `tap_googleads-0.1.5/tap_googleads/schemas/campaign_performance_by_gender_and_device.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.4/tap_googleads/schemas/campaign_performance_by_location.json` & `tap_googleads-0.1.5/tap_googleads/schemas/campaign_performance_by_location.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.4/tap_googleads/schemas/conversion_by_location.json` & `tap_googleads-0.1.5/tap_googleads/schemas/conversion_by_location.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.4/tap_googleads/schemas/customer.json` & `tap_googleads-0.1.5/tap_googleads/schemas/customer.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.4/tap_googleads/schemas/geo_target_constant.json` & `tap_googleads-0.1.5/tap_googleads/schemas/geo_target_constant.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.4/tap_googleads/streams.py` & `tap_googleads-0.1.5/tap_googleads/streams.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Stream type classes for tap-googleads."""
 
 from pathlib import Path
-from typing import Any, Dict, Optional, Union, List, Iterable
+from typing import Any, Dict, Optional, Iterable
 from datetime import datetime
 
 from singer_sdk import typing as th  # JSON Schema typing helpers
 
 from tap_googleads.client import GoogleAdsStream
-from tap_googleads.auth import GoogleAdsAuthenticator
 
 SCHEMAS_DIR = Path(__file__).parent / Path("./schemas")
 
 
 class AccessibleCustomers(GoogleAdsStream):
     """Accessible Customers"""
 
@@ -38,61 +37,45 @@
     This stream is stictly to be the Parent Stream, to let all Child Streams
     know when to query the down stream apps.
 
     """
 
     # TODO add a seperate stream to get the Customer information and return i
     rest_method = "POST"
+    path = "/customers/{client_id}/googleAds:search"
+    records_jsonpath = "$.results[*]"
+    name = "customer_hierarchy"
+    primary_keys_jsonpaths = ["customerClient.id"]
+    primary_keys = ["_sdc_primary_key"]
+    replication_key = None
+    parent_stream_type = AccessibleCustomers
+    schema_filepath = SCHEMAS_DIR / "customer_hierarchy.json"
 
-    @property
-    def path(self):
-        # Paramas
-        path = "/customers/{client_id}"
-        path = path + "/googleAds:search"
-        path = path + "?pageSize=10000"
-        path = path + f"&query={self.gaql}"
-        return path
+    def get_url_params(
+        self, context: Optional[dict], next_page_token: Optional[Any]
+    ) -> Dict[str, Any]:
+        params = super().get_url_params(context, next_page_token)
+        params["pageSize"] = "10000"
+        params["query"] = self.gaql
+        return params
 
     @property
     def gaql(self):
         return """
-	        SELECT customer_client.client_customer
+            SELECT customer_client.client_customer
                  , customer_client.level
                  , customer_client.manager
                  , customer_client.descriptive_name
                  , customer_client.currency_code
                  , customer_client.time_zone
                  , customer_client.id
             FROM customer_client
             WHERE customer_client.level <= 1
             """
 
-    records_jsonpath = "$.results[*]"
-    name = "customer_hierarchy"
-    primary_keys_jsonpaths = ["customerClient.id"]
-    primary_keys = ["_sdc_primary_key"]
-    replication_key = None
-    parent_stream_type = AccessibleCustomers
-    schema = th.PropertiesList(
-        th.Property(
-            "customerClient",
-            th.ObjectType(
-                th.Property("resourceName", th.StringType),
-                th.Property("clientCustomer", th.StringType),
-                th.Property("level", th.StringType),
-                th.Property("timeZone", th.StringType),
-                th.Property("manager", th.BooleanType),
-                th.Property("descriptiveName", th.StringType),
-                th.Property("currencyCode", th.StringType),
-                th.Property("id", th.StringType),
-            ),
-        ),
-        th.Property("_sdc_primary_key", th.StringType),
-    ).to_dict()
-
     # Goal of this stream is to send to children stream a dict of
     # login-customer-id:customer-id to query for all queries downstream
     def get_records(self, context: Optional[dict]) -> Iterable[Dict[str, Any]]:
         """Return a generator of row-type dictionary objects.
 
         Each row emitted should be a dictionary of property names to their values.
 
@@ -111,58 +94,68 @@
 
         for client in client_ids:
             client_id = client.split("/")[-1]
             context["client_id"] = client_id
             for row in self.request_records(context):
                 row = self.post_process(row, context)
                 # Don't search Manager accounts as we can't query them for everything
-                if row["customerClient"]["manager"] == True:
+                if row["customerClient"]["manager"] is True:
                     continue
                 yield row
 
     def get_child_context(self, record: dict, context: Optional[dict]) -> dict:
         """Return a context dictionary for child streams."""
         return {"client_id": record["customerClient"]["id"]}
 
 
 class GeotargetsStream(GoogleAdsStream):
     """Geotargets, worldwide, constant across all customers"""
 
     rest_method = "POST"
 
-    @property
-    def path(self):
-        # Paramas
-        path = "/customers/{login_customer_id}"
-        path = path + "/googleAds:search"
-        path = path + "?pageSize=10000"
-        path = path + f"&query={self.gaql}"
-        return path
+    records_jsonpath = "$.results[*]"
+    name = "geo_target_constant"
+    primary_keys_jsonpaths = ["geoTargetConstant.resourceName"]
+    primary_keys = ["_sdc_primary_key"]
+    replication_key = None
+    schema_filepath = SCHEMAS_DIR / "geo_target_constant.json"
+    parent_stream_type = None  # Override ReportsStream default as this is a constant
+    path = "/customers/{login_customer_id}/googleAds:search"
+
+    def get_url_params(
+        self, context: Optional[dict], next_page_token: Optional[Any]
+    ) -> Dict[str, Any]:
+        params = super().get_url_params(context, next_page_token)
+        params["pageSize"] = "10000"
+        params["query"] = self.gaql
+        return params
 
     gaql = """
         SELECT geo_target_constant.canonical_name
              , geo_target_constant.country_code
              , geo_target_constant.id
              , geo_target_constant.name
              , geo_target_constant.status
              , geo_target_constant.target_type 
         FROM geo_target_constant
     """
-    records_jsonpath = "$.results[*]"
-    name = "geo_target_constant"
-    primary_keys_jsonpaths = ["geoTargetConstant.resourceName"]
-    primary_keys = ["_sdc_primary_key"]
-    replication_key = None
-    schema_filepath = SCHEMAS_DIR / "geo_target_constant.json"
-    parent_stream_type = None  # Override ReportsStream default as this is a constant
 
 
 class ReportsStream(GoogleAdsStream):
     rest_method = "POST"
     parent_stream_type = CustomerHierarchyStream
+    path = "/customers/{client_id}/googleAds:search"
+
+    def get_url_params(
+        self, context: Optional[dict], next_page_token: Optional[Any]
+    ) -> Dict[str, Any]:
+        params = super().get_url_params(context, next_page_token)
+        params["pageSize"] = "10000"
+        params["query"] = self.gaql
+        return params
 
     @property
     def gaql(self):
         raise NotImplementedError
 
     @property
     def start_date(self):
@@ -180,23 +173,14 @@
         )
         return format_date
 
     @property
     def between_filter(self):
         return f"BETWEEN '{self.start_date}' AND '{self.end_date}'"
 
-    @property
-    def path(self):
-        # Paramas
-        path = "/customers/{client_id}"
-        path = path + "/googleAds:search"
-        path = path + "?pageSize=10000"
-        path = path + f"&query={self.gaql}"
-        return path
-
 
 class CampaignsStream(ReportsStream):
     """Define custom stream."""
 
     @property
     def gaql(self):
         return """
@@ -230,15 +214,14 @@
                  , ad_group.target_cpa_micros
                  , ad_group.resource_name
                  , ad_group.percent_cpc_bid_micros
                  , ad_group.name
                  , ad_group.labels
                  , ad_group.id
                  , ad_group.final_url_suffix
-                 , ad_group.explorer_auto_optimizer_setting.opt_in
                  , ad_group.excluded_parent_asset_field_types
                  , ad_group.effective_target_roas_source
                  , ad_group.effective_target_roas
                  , ad_group.effective_target_cpa_source
                  , ad_group.effective_target_cpa_micros
                  , ad_group.display_custom_bid_dimension
                  , ad_group.cpv_bid_micros
@@ -287,14 +270,18 @@
 
     @property
     def gaql(self) -> str:
         return f"""
             SELECT campaign.id
                  , campaign.name
                  , campaign.status
+                 , campaign.start_date
+                 , campaign.end_date
+                 , campaign.advertising_channel_type
+                 , campaign.advertising_channel_sub_type
                  , segments.device
                  , segments.date
                  , metrics.impressions
                  , metrics.clicks
                  , metrics.ctr
                  , metrics.average_cpc
                  , metrics.cost_micros
```

### Comparing `tap_googleads-0.1.4/tap_googleads/tap.py` & `tap_googleads-0.1.5/tap_googleads/tap.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,34 +68,47 @@
             required=True,
             description="Refresh Token from Oauth dance",
         ),
         th.Property(
             "customer_id",
             th.StringType,
             required=True,
-            description="Customer ID from Google Ads Console, note this should be the top level client. This tap will pull all subaccounts",
+            description=(
+                "Customer ID from Google Ads Console, note this should be the top "
+                "level client. This tap will pull all subaccounts",
+            ),
         ),
         th.Property(
             "login_customer_id",
             th.StringType,
             required=True,
-            description="Customer ID that has access to the customer_id, note that they can be the same, but they don't have to be as this could be a Manager account",
+            description=(
+                "Customer ID that has access to the customer_id, note that they can be "
+                "the same, but they don't have to be as this could be a Manager account"
+            ),
         ),
         th.Property(
             "start_date",
             th.DateTimeType,
             default=(date.today() - timedelta(days=7)).strftime("%Y-%m-%dT%H:%M:%SZ"),
             required=True,
-            description="Date to start our search from, applies to Streams where there is a filter date. Note that Google responds to Data in buckets of 1 Day increments",
+            description=(
+                "Date to start our search from, applies to Streams where there is a "
+                "filter date. Note that Google responds to Data in buckets of 1 Day "
+                "increments"
+            ),
         ),
         th.Property(
             "end_date",
             th.DateTimeType,
             default=date.today().strftime("%Y-%m-%dT%H:%M:%SZ"),
             required=True,
-            description="Date to end our search on, applies to Streams where there is a filter date. Note that the query is BETWEEN start_date AND end_date",
+            description=(
+                "Date to end our search on, applies to Streams where there is a filter "
+                "date. Note that the query is BETWEEN start_date AND end_date"
+            ),
         ),
     ).to_dict()
 
     def discover_streams(self) -> List[Stream]:
         """Return a list of discovered streams."""
         return [stream_class(tap=self) for stream_class in STREAM_TYPES]
```

### Comparing `tap_googleads-0.1.4/tap_googleads/tests/test_core.py` & `tap_googleads-0.1.5/tap_googleads/tests/test_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 """Tests standard tap features using the built-in SDK tests library."""
 
 import datetime
-from pathlib import Path
 
 from singer_sdk.testing import get_standard_tap_tests
-from singer_sdk.tap_base import Tap
-from singer_sdk.streams.core import Stream
-from singer_sdk.exceptions import FatalAPIError
 from tap_googleads.tap import TapGoogleAds
-import pytest
-import json
 
-import responses
-import requests
 
 SAMPLE_CONFIG = {
     "start_date": datetime.datetime.now(datetime.timezone.utc).strftime("%Y-%m-%d"),
     "client_id": "12345",
     "client_secret": "12345",
     "developer_token": "12345",
     "refresh_token": "12345",
```

### Comparing `tap_googleads-0.1.4/tap_googleads/tests/test_customer_not_found.py` & `tap_googleads-0.1.5/tap_googleads/tests/test_customer_not_found.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 """Tests standard tap features using the built-in SDK tests library."""
 
 import datetime
-from pathlib import Path
 
-from singer_sdk.testing import get_standard_tap_tests
 from singer_sdk.tap_base import Tap
 from singer_sdk.streams.core import Stream
-from singer_sdk.exceptions import FatalAPIError
 import tap_googleads.tap
 import pytest
 import json
-import importlib
 
 import responses
-import requests
 
 SAMPLE_CONFIG = {
     "start_date": datetime.datetime.now(datetime.timezone.utc).strftime("%Y-%m-%d"),
     "client_id": "12345",
     "client_secret": "12345",
     "developer_token": "12345",
     "refresh_token": "12345",
@@ -37,15 +32,14 @@
     # Test will pass
     # Ends up being due to the modules for the GoogleAdsTap not being reloaded, and how the authenticator metaclass we're using works
     with responses.RequestsMock(assert_all_requests_are_fired=False) as rsps:
         yield rsps
 
 
 def test_customer_not_enabled(mocked_responses):
-
     auth_response = {
         "access_token": "access_granted",
         "expires_in": "10000000",
     }
 
     customer_not_enabled_body = {
         "error": {
@@ -65,15 +59,15 @@
                 }
             ],
         }
     }
     mocked_responses.add(
         responses.POST,
         # TODO cleanup long url, googleads.googleapis.com/* would suffice
-        "https://googleads.googleapis.com/v12/customers/12345/googleAds:search?pageSize=10000&query=%0A%20%20%20%20%20%20%20%20%20%20%20%20SELECT%20campaign.id%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20,%20campaign.name%0A%20%20%20%20%20%20%20%20%20%20%20%20FROM%20campaign%20%0A%20%20%20%20%20%20%20%20%20%20%20%20ORDER%20BY%20campaign.id%0A%20%20%20%20%20%20%20%20",
+        "https://googleads.googleapis.com/v14/customers/12345/googleAds:search?pageSize=10000&query=%0A%20%20%20%20%20%20%20%20%20%20%20%20SELECT%20campaign.id%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20,%20campaign.name%0A%20%20%20%20%20%20%20%20%20%20%20%20FROM%20campaign%20%0A%20%20%20%20%20%20%20%20%20%20%20%20ORDER%20BY%20campaign.id%0A%20%20%20%20%20%20%20%20",
         body=json.dumps(customer_not_enabled_body).encode("utf-8"),
         status=403,
         content_type="application/json",
     )
     mocked_responses.add(
         responses.POST,
         "https://www.googleapis.com/oauth2/v4/token?refresh_token=12345&client_id=12345&client_secret=12345&grant_type=refresh_token",  # TODO Clean up
```

### Comparing `tap_googleads-0.1.4/tap_googleads/tests/test_utils.py` & `tap_googleads-0.1.5/tap_googleads/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.4/tap_googleads/utils.py` & `tap_googleads-0.1.5/tap_googleads/utils.py`

 * *Files identical despite different names*

