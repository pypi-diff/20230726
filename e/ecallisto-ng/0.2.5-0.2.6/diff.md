# Comparing `tmp/ecallisto_ng-0.2.5.tar.gz` & `tmp/ecallisto_ng-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.2.5.tar", last modified: Wed Jul 19 13:09:25 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.2.6.tar", last modified: Wed Jul 26 02:20:40 2023, max compression
```

## Comparing `ecallisto_ng-0.2.5.tar` & `ecallisto_ng-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 13:09:25.374431 ecallisto_ng-0.2.5/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.2.5/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3525 2023-07-19 13:09:25.374431 ecallisto_ng-0.2.5/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2945 2023-07-19 13:07:49.000000 ecallisto_ng-0.2.5/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-19 13:09:17.000000 ecallisto_ng-0.2.5/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-19 13:09:25.385265 ecallisto_ng-0.2.5/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 13:09:25.363598 ecallisto_ng-0.2.5/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 13:09:25.363598 ecallisto_ng-0.2.5/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.2.5/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 13:09:25.374431 ecallisto_ng-0.2.5/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.2.5/src/ecallisto_ng/data_fetching/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     8924 2023-07-19 09:20:02.000000 ecallisto_ng-0.2.5/src/ecallisto_ng/data_fetching/get_data.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3398 2023-07-18 10:05:42.000000 ecallisto_ng-0.2.5/src/ecallisto_ng/data_fetching/get_information.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 13:09:25.374431 ecallisto_ng-0.2.5/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.2.5/src/ecallisto_ng/data_processing/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5646 2023-07-19 13:08:15.000000 ecallisto_ng-0.2.5/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 13:09:25.374431 ecallisto_ng-0.2.5/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.2.5/src/ecallisto_ng/plotting/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2954 2023-07-19 09:56:22.000000 ecallisto_ng-0.2.5/src/ecallisto_ng/plotting/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-19 13:09:25.374431 ecallisto_ng-0.2.5/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3525 2023-07-19 13:09:25.000000 ecallisto_ng-0.2.5/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-19 13:09:25.000000 ecallisto_ng-0.2.5/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-19 13:09:25.000000 ecallisto_ng-0.2.5/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-19 13:09:25.000000 ecallisto_ng-0.2.5/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-19 13:09:25.000000 ecallisto_ng-0.2.5/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.2.6/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3564 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2945 2023-07-19 13:07:49.000000 ecallisto_ng-0.2.6/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      905 2023-07-26 02:20:13.000000 ecallisto_ng-0.2.6/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.2.6/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.2.6/src/ecallisto_ng/data_fetching/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     9301 2023-07-26 02:08:55.000000 ecallisto_ng-0.2.6/src/ecallisto_ng/data_fetching/get_data.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     4680 2023-07-26 02:15:22.000000 ecallisto_ng-0.2.6/src/ecallisto_ng/data_fetching/get_information.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.2.6/src/ecallisto_ng/data_processing/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5694 2023-07-26 02:08:55.000000 ecallisto_ng-0.2.6/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.2.6/src/ecallisto_ng/plotting/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3025 2023-07-26 02:08:55.000000 ecallisto_ng-0.2.6/src/ecallisto_ng/plotting/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3564 2023-07-26 02:20:40.000000 ecallisto_ng-0.2.6/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-26 02:20:40.000000 ecallisto_ng-0.2.6/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-26 02:20:40.000000 ecallisto_ng-0.2.6/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      137 2023-07-26 02:20:40.000000 ecallisto_ng-0.2.6/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-26 02:20:40.000000 ecallisto_ng-0.2.6/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.2.5/LICENSE` & `ecallisto_ng-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.5/PKG-INFO` & `ecallisto_ng-0.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: ecallisto_ng
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: nb
+Provides-Extra: dev
 License-File: LICENSE
 
 # Ecallisto NG 
 Ecallisto NG is a compact yet effective Python package designed to facilitate seamless interaction with the Ecallisto API. 
 The package is constructed in Python 3.9 and utilizes the `requests` library to directly access the Ecallisto API via the link: [https://v000792.fhnw.ch/api/redoc](https://v000792.fhnw.ch/api/redoc).
 
 ## Installation
```

### Comparing `ecallisto_ng-0.2.5/README.md` & `ecallisto_ng-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.5/pyproject.toml` & `ecallisto_ng-0.2.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [project]
 name = "ecallisto_ng"
-version = "0.2.5"
+version = "0.2.6"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    'ipython>=8.14.0',
-    'nbformat>=5.9.0',
-    'numpy>=1.25.0',
-    'pandas>=2.0.3',
-    'plotly>=5.15.0',
-    'requests>=2.31.0',
-    'scikit-image>=0.21.0',
-    'pyarrow>=12.0.1'
+    'numpy>=1.21.6',
+    'pandas>=2.0.0',
+    'plotly',
+    'requests',
+    'scikit-image>=0.20.0',
+    'pyarrow'
 
 ]
+[project.optional-dependencies]
+nb = ['nbformat', 'ipython', 'ipykernel']
+dev = ['black', 'isort', 'twine', 'build']
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project.urls]
 Homepage = "https://github.com/i4Ds/ecallisto_ng"
```

### Comparing `ecallisto_ng-0.2.5/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.2.6/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def get_data(
     instrument_name,
     start_datetime,
     end_datetime,
     timebucket=None,
     agg_function=None,
-    data_folder='ecallisto_ng_cache',
+    data_folder="ecallisto_ng_cache",
     verbose=False,
     max_retries=3,
 ):
     """
     Get data from the eCallisto API. See: https://v000792.fhnw.ch/api/redoc
     Of course, this is just a wrapper around the requests.post function.
     Depending on the size, the request can take a while. For example, two
@@ -48,39 +48,43 @@
         A DataFrame containing the data from the eCallisto API.
     """
     data = {
         "instrument_name": instrument_name,
         "start_datetime": start_datetime,
         "end_datetime": end_datetime,
         "timebucket": timebucket,
-        "agg_function": agg_function
+        "agg_function": agg_function,
     }
 
-    assert pd.to_datetime(start_datetime) <= pd.to_datetime(end_datetime), (
-        f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
-    )
+    assert pd.to_datetime(start_datetime) <= pd.to_datetime(
+        end_datetime
+    ), f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
 
     # Clean up dates to make it compatible with windows
     start_datetime = start_datetime.replace(":", "-")
     end_datetime = end_datetime.replace(":", "-")
 
     # Create file path
-    file_path = os.path.join(data_folder, f"{instrument_name}_{start_datetime}_{end_datetime}_{timebucket}_{agg_function}.parquet")
+    file_path = os.path.join(
+        data_folder,
+        f"{instrument_name}_{start_datetime}_{end_datetime}_{timebucket}_{agg_function}.parquet",
+    )
     os.makedirs(data_folder, exist_ok=True)
     if os.path.exists(file_path):
         print(f"Reading data from {file_path}")
         return pd.read_parquet(file_path)
 
     # Send the request to the API
     response = requests.post(BASE_URL + "/api/data", json=data, timeout=180)
-
     # Check if the request was successful
     if response.status_code == 200:
         if verbose:
-            print("Data retrieval started successfully. Waiting for file to be ready...")
+            print(
+                "Data retrieval started successfully. Waiting for file to be ready..."
+            )
         # Get the URL for the parquet file
         parquet_url = response.json()["data_parquet_url"]
         json_url = response.json()["info_json_url"]
         file_id = response.json()["file_id"]
 
         # Now we can start polling the URL until the parquet file is ready for download
         n_tries = 0
@@ -93,50 +97,62 @@
                 # If the file is available, save it to disk
                 if file_response.status_code == 200:
                     print("File downloaded successfully")
                     with open(file_path, "wb") as f:
                         f.write(file_response.content)
                     # Check that the file is bigger than 8 bytes (sometimes, the API returns an empty file)
                     if os.path.getsize(file_path) > 8:
-                        # Return the file as a DataFrame  
+                        # Return the file as a DataFrame
                         return pd.read_parquet(file_path)
                     else:
                         # Remove file and try again
                         os.remove(file_path)
-                        raise ValueError(f"Error downloading file: {file_response.status_code}. File is empty.")
+                        raise ValueError(
+                            f"Error downloading file: {file_response.status_code}. File is empty."
+                        )
                 elif file_response.status_code == 204:
                     # Check if the file creation causes any errors
-                    json_response = requests.get(BASE_URL + json_url) # This json contains information about your data request (e.g. status)
-                    # Check the status of the json 
-                    if 'status' in json_response.json():
-                        if json_response.json()['status'] == 'processing':
+                    json_response = requests.get(
+                        BASE_URL + json_url
+                    )  # This json contains information about your data request (e.g. status)
+                    # Check the status of the json
+                    if "status" in json_response.json():
+                        if json_response.json()["status"] == "processing":
                             # If the file is not found, sleep for a short period and try again
                             if verbose:
                                 print(f"File {file_id} not ready yet, waiting...")
                             time.sleep(3)
-                        elif json_response.json()['status'] == 'ok':
+                        elif json_response.json()["status"] == "ok":
                             if verbose:
-                                print(f'File {file_id} succesfully written! Will return file.')
+                                print(
+                                    f"File {file_id} succesfully written! Will return file."
+                                )
                         else:
-                            raise ValueError(f"Error downloading file: {json_response.json()['status']}")
-                    elif 'error' in json_response.json():
-                        raise ValueError(f"Error downloading file: {json_response.json()['error']}")
+                            raise ValueError(
+                                f"Error downloading file: {json_response.json()['status']}"
+                            )
+                    elif "error" in json_response.json():
+                        raise ValueError(
+                            f"Error downloading file: {json_response.json()['error']}"
+                        )
                 else:
                     print(f"Error downloading file: {file_response.status_code}")
                     json_response = requests.get(BASE_URL + json_url)
                     print(json_response.json())
                     break
             except Exception as e:
                 print(
                     f"""Error downloading file: {e}. Try {n_tries} of {max_retries}. Retrying in 3 seconds...
                     """
-                    )
+                )
                 n_tries += 1
                 if n_tries > max_retries:
-                    raise ValueError(f"Error downloading file: {file_response.status_code}. Max retries reached.")
+                    raise ValueError(
+                        f"Error downloading file: {file_response.status_code}. Max retries reached."
+                    )
                 time.sleep(3)
     else:
         print(f"Error starting data retrieval: {response.status_code}")
 
 
 # Because of SQL limitation, the names of the tables do not perfectly match the instrument names.
 # This function converts the instrument name to the table name.
```

### Comparing `ecallisto_ng-0.2.5/src/ecallisto_ng/data_fetching/get_information.py` & `ecallisto_ng-0.2.6/src/ecallisto_ng/data_fetching/get_information.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import pandas as pd
 import requests
 
 BASE_URL = "https://v000792.fhnw.ch"
 
+
 def get_tables(verbose=False):
     """
     Fetch all the available table names from the eCallisto API.
 
     Parameters
     ----------
     verbose : bool
         Whether to print out the response from the API.
-    
+
     Returns
     -------
     list of str
         A list containing the names of the available tables.
     """
     response = requests.get(BASE_URL + "/api/tables")
 
     if response.status_code == 200:
-        table_names = response.json()['tables']
+        table_names = response.json()["tables"]
         if verbose:
             print(f"Received table names: {table_names}")
         return table_names
     else:
         raise ValueError(f"Error getting table names from API: {response.text}")
 
 
-def get_table_names_with_data_between_dates(start_datetime, end_datetime, verbose=False):
+def get_table_names_with_data_between_dates(
+    start_datetime, end_datetime, verbose=False
+):
     """
     Fetch all the available table names that contain data between the specified dates from the eCallisto API.
 
     Parameters
     ----------
     start_datetime : str
         The start datetime of the data availability check.
@@ -47,35 +50,75 @@
         A list containing the names of the available tables that contain data between the specified dates.
     """
     data = {
         "start_datetime": start_datetime,
         "end_datetime": end_datetime,
     }
 
-    assert pd.to_datetime(start_datetime) <= pd.to_datetime(end_datetime), (
-        f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
-    )
+    assert pd.to_datetime(start_datetime) <= pd.to_datetime(
+        end_datetime
+    ), f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
 
     response = requests.post(BASE_URL + "/api/data_availability", json=data)
 
     if response.status_code == 200:
-        table_names = response.json()['table_names']
+        table_names = response.json()["table_names"]
         if verbose:
             print(f"Received table names: {table_names}")
         return table_names
     else:
         raise ValueError(f"Error getting table names from API: {response.text}")
 
-def check_table_data_availability(instrument_name, start_datetime, end_datetime, verbose=False, **kwargs):
+
+def check_min_max_datetime_in_table(instrument_name, verbose=False, **kwargs):
+    """
+    Check the minimum and maximum datetimes in a table using the eCallisto API.
+
+    Parameters
+    ----------
+    instrument_name : str
+        The name of the table to check.
+    verbose : bool
+        Whether to print out the response from the API.
+
+    Returns
+    -------
+    dict
+        A dictionary containing 'min_datetime' and 'max_datetime' if successful,
+        raises ValueError otherwise.
+    """
+    data = {"instrument_name": instrument_name}
+
+    response = requests.post(BASE_URL + "/api/min_max_datetime", json=data)
+
+    if response.status_code == 200:
+        min_max_datetime = response.json()
+        # To pd.Datetime
+        min_datetime, max_datetime = (
+            pd.to_datetime(min_max_datetime["min_datetime"]),
+            pd.to_datetime(min_max_datetime["max_datetime"]),
+        )
+        if verbose:
+            print(
+                f"Table '{instrument_name}' has minimum datetime at {min_datetime} and maximum datetime at {max_datetime}"
+            )
+        return min_datetime, max_datetime
+    else:
+        raise ValueError(f"Error checking min/max datetime from API: {response.text}")
+
+
+def check_table_data_availability(
+    instrument_name, start_datetime, end_datetime, verbose=False, **kwargs
+):
     """
     Check if a table has data between the specified dates using the eCallisto API.
 
     Parameters
     ----------
-    table_name : str
+    instrument_name : str
         The name of the table to check.
     start_datetime : str
         The start datetime of the data availability check.
     end_datetime : str
         The end datetime of the data availability check.
     verbose : bool
         Whether to print out the response from the API.
@@ -87,20 +130,24 @@
     """
     data = {
         "instrument_name": instrument_name,
         "start_datetime": start_datetime,
         "end_datetime": end_datetime,
     }
 
-    assert pd.to_datetime(start_datetime) <= pd.to_datetime(end_datetime), (
-        f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
-    )
+    assert pd.to_datetime(start_datetime) <= pd.to_datetime(
+        end_datetime
+    ), f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
 
     response = requests.post(BASE_URL + "/api/table_data_check", json=data)
 
     if response.status_code == 200:
-        has_data = response.json()['has_data']
+        has_data = response.json()["has_data"]
         if verbose:
-            print(f"Table '{instrument_name}' has data between {start_datetime} and {end_datetime}: {has_data}")
+            print(
+                f"Table '{instrument_name}' has data between {start_datetime} and {end_datetime}: {has_data}"
+            )
         return has_data
     else:
-        raise ValueError(f"Error checking table data availability from API: {response.text}")
+        raise ValueError(
+            f"Error checking table data availability from API: {response.text}"
+        )
```

### Comparing `ecallisto_ng-0.2.5/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.2.6/src/ecallisto_ng/data_processing/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import numpy as np
 import pandas as pd
 from skimage import filters
 
 
-def elimwrongchannels(df, channel_std_mult=5, jump_std_mult=2, nan_interpolation_method='pchip'):
+def elimwrongchannels(
+    df, channel_std_mult=5, jump_std_mult=2, nan_interpolation_method="pchip"
+):
     """
     Remove Radio Frequency Interference (RFI) from a spectrogram represented by a pandas DataFrame.
     This function works even when there is missing data thanks to interpolation of missing values.
     However, it could lead to some false or different results.
     Parameters
     ----------
     df : pandas.DataFrame
@@ -30,15 +32,17 @@
     df = df.copy()
 
     # Store original NaN positions
     nan_positions = df.isna()
 
     # Fill missing data with interpolation
     df.interpolate(method=nan_interpolation_method, inplace=True)
-    df.fillna(method='bfill', inplace=True)  # for cases where NaNs are at the start of a series
+    df.fillna(
+        method="bfill", inplace=True
+    )  # for cases where NaNs are at the start of a series
 
     # Transpose df so that rows represent channels and columns represent time
     df = df.T
 
     # Calculate standard deviation for each channel and scale it to 0-255
     std = df.std(axis=1).fillna(0)
     std = ((std - std.min()) * 255) / (std.max() - std.min())
@@ -95,15 +99,17 @@
         DataFrame with the constant background subtracted. The DataFrame is oriented in the same way as the input DataFrame (time on index and frequency on columns).
 
     """
     df = df.copy()
     return df - df.iloc[0:n].median()
 
 
-def subtract_rolling_background(df, window=30, center=False, how="quantile", quantile_value=0.05, **kwargs):
+def subtract_rolling_background(
+    df, window=30, center=False, how="quantile", quantile_value=0.05, **kwargs
+):
     """
     Subtract a rolling background from a spectrogram represented by a pandas DataFrame.
 
     The rolling background is calculated either as the median or a specific quantile value of each rolling window of size `window`.
 
     Parameters
     ----------
@@ -128,11 +134,13 @@
         DataFrame with the rolling background subtracted. The DataFrame is oriented in the same way as the input DataFrame (time on index and frequency on columns).
 
     """
     df = df.copy()
     if how == "median":
         df_rolling = df.rolling(window=window, center=center, **kwargs).median()
     elif how == "quantile":
-        df_rolling = df.rolling(window=window, center=center, **kwargs).quantile(quantile_value)
+        df_rolling = df.rolling(window=window, center=center, **kwargs).quantile(
+            quantile_value
+        )
     else:
         raise ValueError("`how` must be 'median' or 'quantile'")
     return df - df_rolling
```

### Comparing `ecallisto_ng-0.2.5/src/ecallisto_ng/plotting/utils.py` & `ecallisto_ng-0.2.6/src/ecallisto_ng/plotting/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 import numpy as np
 import pandas as pd
 import plotly.express as px
 
 
-def plot_spectogram(df, instrument_name, start_datetime, end_datetime, size=18, round_precision=1, color_scale=px.colors.sequential.Plasma):
+def plot_spectogram(
+    df,
+    instrument_name,
+    start_datetime,
+    end_datetime,
+    size=18,
+    round_precision=1,
+    color_scale=px.colors.sequential.Plasma,
+):
     # Create a new dataframe with rounded column names
     df_rounded = df.copy()
     df_rounded.columns = [f"{float(col):.{round_precision}f}" for col in df.columns]
 
     # Make datetime prettier
     if isinstance(start_datetime, str):
         start_datetime = pd.to_datetime(start_datetime)
     if isinstance(end_datetime, str):
         end_datetime = pd.to_datetime(end_datetime)
     sd_str = start_datetime.strftime("%Y-%m-%d %H:%M:%S")
     ed_str = end_datetime.strftime("%Y-%m-%d %H:%M:%S")
 
-    fig = px.imshow(df_rounded.T, color_continuous_scale=color_scale, zmin=df.min().min(), zmax=df.max().max())
+    fig = px.imshow(
+        df_rounded.T,
+        color_continuous_scale=color_scale,
+        zmin=df.min().min(),
+        zmax=df.max().max(),
+    )
     fig.update_layout(
         title=f"Spectogram of {instrument_name} between {sd_str} and {ed_str}",
         xaxis_title="Datetime",
         yaxis_title="Frequency",
         font=dict(family="Courier New, monospace", size=size, color="#7f7f7f"),
         plot_bgcolor="black",
         xaxis_showgrid=False,
         yaxis_showgrid=False,
     )
     return fig
 
+
 def fill_missing_timesteps_with_nan(df):
     """
     Fill missing timesteps in a pandas DataFrame with NaN values. Only needed for plotting.
 
     Parameters
     ----------
     df : pandas.DataFrame
```

### Comparing `ecallisto_ng-0.2.5/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.2.6/src/ecallisto_ng.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: ecallisto-ng
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: nb
+Provides-Extra: dev
 License-File: LICENSE
 
 # Ecallisto NG 
 Ecallisto NG is a compact yet effective Python package designed to facilitate seamless interaction with the Ecallisto API. 
 The package is constructed in Python 3.9 and utilizes the `requests` library to directly access the Ecallisto API via the link: [https://v000792.fhnw.ch/api/redoc](https://v000792.fhnw.ch/api/redoc).
 
 ## Installation
```

### Comparing `ecallisto_ng-0.2.5/src/ecallisto_ng.egg-info/SOURCES.txt` & `ecallisto_ng-0.2.6/src/ecallisto_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

