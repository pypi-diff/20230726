# Comparing `tmp/nsedt-0.0.6.tar.gz` & `tmp/nsedt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsedt-0.0.6.tar", last modified: Mon Jul  3 22:19:28 2023, max compression
+gzip compressed data, was "nsedt-0.0.7.tar", last modified: Tue Jul 25 22:05:05 2023, max compression
```

## Comparing `nsedt-0.0.6.tar` & `nsedt-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:19:28.428807 nsedt-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 22:19:18.000000 nsedt-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-03 22:19:28.428807 nsedt-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-07-03 22:19:18.000000 nsedt-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:19:28.428807 nsedt-0.0.6/nsedt/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-03 22:19:18.000000 nsedt-0.0.6/nsedt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-07-03 22:19:18.000000 nsedt-0.0.6/nsedt/equity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-03 22:19:18.000000 nsedt-0.0.6/nsedt/indices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:19:28.428807 nsedt-0.0.6/nsedt/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:19:18.000000 nsedt-0.0.6/nsedt/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-03 22:19:18.000000 nsedt-0.0.6/nsedt/resources/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:19:28.428807 nsedt-0.0.6/nsedt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-03 22:19:18.000000 nsedt-0.0.6/nsedt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-03 22:19:18.000000 nsedt-0.0.6/nsedt/utils/data_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:19:28.428807 nsedt-0.0.6/nsedt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-03 22:19:28.000000 nsedt-0.0.6/nsedt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-03 22:19:28.000000 nsedt-0.0.6/nsedt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:19:28.000000 nsedt-0.0.6/nsedt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 22:19:28.000000 nsedt-0.0.6/nsedt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 22:19:28.000000 nsedt-0.0.6/nsedt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 22:19:28.428807 nsedt-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-03 22:19:18.000000 nsedt-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:05:05.687699 nsedt-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 22:04:53.000000 nsedt-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-25 22:05:05.687699 nsedt-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-25 22:04:53.000000 nsedt-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:05:05.683699 nsedt-0.0.7/nsedt/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-25 22:04:53.000000 nsedt-0.0.7/nsedt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-07-25 22:04:53.000000 nsedt-0.0.7/nsedt/equity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-25 22:04:53.000000 nsedt-0.0.7/nsedt/indices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:05:05.687699 nsedt-0.0.7/nsedt/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 22:04:53.000000 nsedt-0.0.7/nsedt/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-25 22:04:53.000000 nsedt-0.0.7/nsedt/resources/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:05:05.687699 nsedt-0.0.7/nsedt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-25 22:04:53.000000 nsedt-0.0.7/nsedt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-25 22:04:53.000000 nsedt-0.0.7/nsedt/utils/data_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:05:05.687699 nsedt-0.0.7/nsedt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-25 22:05:05.000000 nsedt-0.0.7/nsedt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-25 22:05:05.000000 nsedt-0.0.7/nsedt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 22:05:05.000000 nsedt-0.0.7/nsedt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-25 22:05:05.000000 nsedt-0.0.7/nsedt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 22:05:05.000000 nsedt-0.0.7/nsedt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 22:05:05.687699 nsedt-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-25 22:04:53.000000 nsedt-0.0.7/setup.py
```

### Comparing `nsedt-0.0.6/LICENSE` & `nsedt-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.6/PKG-INFO` & `nsedt-0.0.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,20 @@
-Metadata-Version: 2.1
-Name: nsedt
-Version: 0.0.6
-Summary: Library to collect NSE data in pandas dataframe
-Home-page: https://github.com/pratik141/nsedt
-Author: Pratik Anand
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# NSE (national stock exchange) data
 
-# nse data
-
-Introduction
+Introduction:
+This library serves as an api to fetch data from the NSE about stocks and indices using python
 
 Thank you for using Nsedt. Please feel free to send pull requests, comments, and suggestions, as well as get in touch with me if you require any additional help. I sincerely hope you will find this library useful.
 
+## How to start
+### clone the repository
+`git clone https://github.com/pratik141/nsedt`
+### Install the requirements file after changing to cloned folder above
+`pip install -r requirements.txt`
+
 ---
 ## Run 
 ```py
 from nsedt import equity as eq
 from datetime import date
 
 start_date = date(2022, 1, 1)
@@ -34,14 +26,15 @@
 print(eq.get_event(start_date, end_date))
 print(eq.get_event())
 print(eq.get_marketstatus())
 print(eq.get_marketstatus(response_type="json"))
 print(eq.get_companyinfo(symbol="TCS"))
 print(eq.get_companyinfo(symbol="TCS", response_type="json"))
 print(eq.get_chartdata(symbol="TCS"))
+print(eq.get_symbols_list()) #print the list of symbols used by NSE for equities
 
 ```
 ---
 ## Output
 ```sh
 # get_price
         Date  Open Price  High Price  Low Price  Close Price  ...  52 Week High Price  52 Week Low Price     VWAP  Deliverable Volume  Deliverable Percent
@@ -71,43 +64,47 @@
 
            market marketStatus     tradeDate     index     last  ... percentChange marketStatusMessage   expiryDate underlying tradeDateFormatted
 0  Capital Market        Close   09-Jun-2023  NIFTY 50  18563.4  ...         -0.38    Market is Closed          NaN        NaN                NaN
 4  currencyfuture        Close  Invalid date            82.4975  ...                  Market is Closed  16-Jun-2023     USDINR        09-Jun-2023
 
 
 #get_chartdata
-                 0        1
-0    1686301201000  3300.00
-404  1686301620000  3250.00
-
+        timestamp_milliseconds    price            datetime
+0               1690276500000  3397.80 2023-07-25 09:15:00
+...                       ...      ...                 ...
+12923           1690300782000  3399.15 2023-07-25 15:59:42
 
 ```
 ---
 
 # API Documentation
 
 ## Functions
 
 ### get_companyinfo
 
-Function description goes here.
+Function defines the market status of the company
 
 ### get_marketstatus
 
 Function description goes here.
 
 ### get_price
 
-Function description goes here.
+Function to get the price of the stock or index from a starting date to end date
 
 ### get_corpinfo
 
 Function description goes here.
 
 ### get_event
 
 Function description goes here.
 
 ### get_chartdata
 
 Function description goes here.
 
+### get_symbols_list
+
+Function to get the list of symbols used by NSE for equity companies like "SBIN" for State Bank of India
+
```

### Comparing `nsedt-0.0.6/nsedt/equity.py` & `nsedt-0.0.7/nsedt/equity.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,20 +35,22 @@
     cookies = utils.get_cookies()
     base_url = cns.BASE_URL
     event_api = cns.EQUITY_INFO
 
     params["symbol"] = symbol
 
     url = base_url + event_api + urllib.parse.urlencode(params)
-    data = utils.fetch_url(url, cookies)
-
-    if response_type == "panda_df":
-        return data
+    data = utils.fetch_url(
+        url,
+        cookies,
+        key=None,
+        response_type=response_type,
+    )
 
-    return data.to_json()
+    return data
 
 
 def get_marketstatus(
     response_type="panda_df",
 ):
     """
     Args:
@@ -60,20 +62,22 @@
     """
 
     cookies = utils.get_cookies()
     base_url = cns.BASE_URL
     event_api = cns.MARKETSTATUS
 
     url = base_url + event_api
-    data = utils.fetch_url(url, cookies, key="marketState")
+    data = utils.fetch_url(
+        url,
+        cookies,
+        key="marketState",
+        response_type=response_type,
+    )
 
-    if response_type == "panda_df":
-        return data
-
-    return data.to_json()
+    return data
 
 
 def get_price(
     start_date,
     end_date,
     symbol=None,
     input_type="stock",
@@ -160,20 +164,22 @@
         "to_date": end_date,
         "index": "equities",
     }
     base_url = cns.BASE_URL
     price_api = cns.EQUITY_CORPINFO
     url = base_url + price_api + urllib.parse.urlencode(params)
 
-    data = utils.fetch_url(url, cookies)
-
-    if response_type == "panda_df":
-        return data
+    data = utils.fetch_url(
+        url,
+        cookies,
+        key=None,
+        response_type=response_type,
+    )
 
-    return data.to_json()
+    return data
 
 
 def get_event(
     start_date=None,
     end_date=None,
     index="equities",
 ):
@@ -198,30 +204,79 @@
 
     url = base_url + event_api + urllib.parse.urlencode(params)
     return utils.fetch_url(url, cookies)
 
 
 def get_chartdata(
     symbol,
-    preopen="true",
+    preopen=False,
+    response_type="panda_df",
 ):
     """
     Args:
         symbol (str): stock symbol.
     Returns:
         Pandas DataFrame: df containing chart data of provided date
 
     """
     params = {}
     cookies = utils.get_cookies()
     base_url = cns.BASE_URL
     event_api = cns.EQUITY_CHART
     try:
-        identifier = get_companyinfo(symbol)["info"]["identifier"]
+        identifier = get_companyinfo(
+            symbol,
+            response_type="json",
+        )[
+            "info"
+        ]["identifier"]
+
     except KeyError:
         return f"Invalid symbol name: {symbol}"
 
     params["index"] = identifier
-    params["preopen"] = preopen
+    if preopen:
+        params["preopen"] = "true"
 
     url = base_url + event_api + urllib.parse.urlencode(params)
-    return utils.fetch_url(url, cookies, key="grapthData")
+
+    data = utils.fetch_url(
+        url,
+        cookies,
+        key="grapthData",
+        response_type=response_type,
+    )
+    if response_type == "panda_df":
+        data_frame = data.rename(
+            columns={
+                0: "timestamp_milliseconds",
+                1: "price",
+            }
+        )
+        data_frame["datetime"] = pd.to_datetime(
+            data_frame["timestamp_milliseconds"], unit="ms"
+        )
+        return data_frame
+    return data
+
+
+def get_symbols_list():
+    """
+    Args:
+        No arguments needed
+
+    Returns:
+        List of stock or equity symbols
+
+    """
+    cookies = utils.get_cookies()
+    base_url = cns.BASE_URL
+    event_api = cns.EQUITY_LIST
+
+    url = base_url + event_api
+    data = utils.fetch_url(url, cookies)
+    f_dict = data.to_dict()
+    eq_list = []
+    for i in range(len(f_dict["data"])):
+        eq_list.append(f_dict["data"][i]["metadata"]["symbol"])
+
+    return eq_list
```

### Comparing `nsedt-0.0.6/nsedt/indices.py` & `nsedt-0.0.7/nsedt/indices.py`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.6/nsedt/resources/constants.py` & `nsedt-0.0.7/nsedt/resources/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,13 +20,14 @@
 ### EQUITY
 EQUITY_PRICE_HISTORY = "api/historical/securityArchives?"
 EQUITY_CORPINFO = "api/corporates-corporateActions?"
 MARKETSTATUS = "api/marketStatus"
 EQUITY_EVENT = "api/event-calendar?"
 EQUITY_CHART = "api/chart-databyindex?"
 EQUITY_INFO = "api/quote-equity?"
+EQUITY_LIST = "api/market-data-pre-open?key=ALL"
 
 ### Index
 INDEX_PRICE_HISTORY = "api/historical/indicesHistory?"
 
 ### DERIVATIVES
 DERIVATIVES_PRICE = "api/option-chain-equities?"
```

### Comparing `nsedt-0.0.6/nsedt/utils/__init__.py` & `nsedt-0.0.7/nsedt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.6/nsedt/utils/data_format.py` & `nsedt-0.0.7/nsedt/utils/data_format.py`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.6/nsedt.egg-info/PKG-INFO` & `nsedt-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: nsedt
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library to collect NSE data in pandas dataframe
 Home-page: https://github.com/pratik141/nsedt
 Author: Pratik Anand
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# nse data
+# NSE (national stock exchange) data
 
-Introduction
+Introduction:
+This library serves as an api to fetch data from the NSE about stocks and indices using python
 
 Thank you for using Nsedt. Please feel free to send pull requests, comments, and suggestions, as well as get in touch with me if you require any additional help. I sincerely hope you will find this library useful.
 
+## How to start
+### clone the repository
+`git clone https://github.com/pratik141/nsedt`
+### Install the requirements file after changing to cloned folder above
+`pip install -r requirements.txt`
+
 ---
 ## Run 
 ```py
 from nsedt import equity as eq
 from datetime import date
 
 start_date = date(2022, 1, 1)
@@ -34,14 +41,15 @@
 print(eq.get_event(start_date, end_date))
 print(eq.get_event())
 print(eq.get_marketstatus())
 print(eq.get_marketstatus(response_type="json"))
 print(eq.get_companyinfo(symbol="TCS"))
 print(eq.get_companyinfo(symbol="TCS", response_type="json"))
 print(eq.get_chartdata(symbol="TCS"))
+print(eq.get_symbols_list()) #print the list of symbols used by NSE for equities
 
 ```
 ---
 ## Output
 ```sh
 # get_price
         Date  Open Price  High Price  Low Price  Close Price  ...  52 Week High Price  52 Week Low Price     VWAP  Deliverable Volume  Deliverable Percent
@@ -71,43 +79,47 @@
 
            market marketStatus     tradeDate     index     last  ... percentChange marketStatusMessage   expiryDate underlying tradeDateFormatted
 0  Capital Market        Close   09-Jun-2023  NIFTY 50  18563.4  ...         -0.38    Market is Closed          NaN        NaN                NaN
 4  currencyfuture        Close  Invalid date            82.4975  ...                  Market is Closed  16-Jun-2023     USDINR        09-Jun-2023
 
 
 #get_chartdata
-                 0        1
-0    1686301201000  3300.00
-404  1686301620000  3250.00
-
+        timestamp_milliseconds    price            datetime
+0               1690276500000  3397.80 2023-07-25 09:15:00
+...                       ...      ...                 ...
+12923           1690300782000  3399.15 2023-07-25 15:59:42
 
 ```
 ---
 
 # API Documentation
 
 ## Functions
 
 ### get_companyinfo
 
-Function description goes here.
+Function defines the market status of the company
 
 ### get_marketstatus
 
 Function description goes here.
 
 ### get_price
 
-Function description goes here.
+Function to get the price of the stock or index from a starting date to end date
 
 ### get_corpinfo
 
 Function description goes here.
 
 ### get_event
 
 Function description goes here.
 
 ### get_chartdata
 
 Function description goes here.
 
+### get_symbols_list
+
+Function to get the list of symbols used by NSE for equity companies like "SBIN" for State Bank of India
+
```

### Comparing `nsedt-0.0.6/setup.py` & `nsedt-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
 
 setup(
     name="nsedt",
-    version="0.0.6",
+    version="0.0.7",
     author="Pratik Anand",
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="Library to collect NSE data in pandas dataframe",
     packages=find_packages(),
     url="https://github.com/pratik141/nsedt",
     install_requires=[
```

