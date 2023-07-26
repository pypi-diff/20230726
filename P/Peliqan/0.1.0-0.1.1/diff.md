# Comparing `tmp/Peliqan-0.1.0.tar.gz` & `tmp/Peliqan-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Peliqan-0.1.0.tar", last modified: Wed Jul 12 13:17:49 2023, max compression
+gzip compressed data, was "Peliqan-0.1.1.tar", last modified: Wed Jul 26 07:00:06 2023, max compression
```

## Comparing `Peliqan-0.1.0.tar` & `Peliqan-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-12 13:17:49.694638 Peliqan-0.1.0/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2023-07-12 13:17:49.694531 Peliqan-0.1.0/PKG-INFO
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-12 13:17:49.694263 Peliqan-0.1.0/Peliqan.egg-info/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2023-07-12 13:17:49.000000 Peliqan-0.1.0/Peliqan.egg-info/PKG-INFO
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      192 2023-07-12 13:17:49.000000 Peliqan-0.1.0/Peliqan.egg-info/SOURCES.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2023-07-12 13:17:49.000000 Peliqan-0.1.0/Peliqan.egg-info/dependency_links.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2023-07-12 13:17:49.000000 Peliqan-0.1.0/Peliqan.egg-info/requires.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2023-07-12 13:17:49.000000 Peliqan-0.1.0/Peliqan.egg-info/top_level.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1365 2023-07-12 11:25:49.000000 Peliqan-0.1.0/README.md
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-12 13:17:49.694358 Peliqan-0.1.0/peliqan/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    36034 2023-07-12 11:28:18.000000 Peliqan-0.1.0/peliqan/__init__.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2023-07-12 13:17:49.694670 Peliqan-0.1.0/setup.cfg
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1335 2023-07-12 11:15:54.000000 Peliqan-0.1.0/setup.py
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-26 07:00:06.422699 Peliqan-0.1.1/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2023-07-26 07:00:06.422554 Peliqan-0.1.1/PKG-INFO
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-26 07:00:06.421940 Peliqan-0.1.1/Peliqan.egg-info/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2023-07-26 07:00:06.000000 Peliqan-0.1.1/Peliqan.egg-info/PKG-INFO
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      192 2023-07-26 07:00:06.000000 Peliqan-0.1.1/Peliqan.egg-info/SOURCES.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2023-07-26 07:00:06.000000 Peliqan-0.1.1/Peliqan.egg-info/dependency_links.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2023-07-26 07:00:06.000000 Peliqan-0.1.1/Peliqan.egg-info/requires.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2023-07-26 07:00:06.000000 Peliqan-0.1.1/Peliqan.egg-info/top_level.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-07-14 07:23:16.000000 Peliqan-0.1.1/README.md
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-26 07:00:06.422267 Peliqan-0.1.1/peliqan/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    37222 2023-07-26 06:45:43.000000 Peliqan-0.1.1/peliqan/__init__.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2023-07-26 07:00:06.422792 Peliqan-0.1.1/setup.cfg
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1335 2023-07-25 13:32:11.000000 Peliqan-0.1.1/setup.py
```

### Comparing `Peliqan-0.1.0/PKG-INFO` & `Peliqan-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-0.1.0/Peliqan.egg-info/PKG-INFO` & `Peliqan-0.1.1/Peliqan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-0.1.0/README.md` & `Peliqan-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,31 +17,30 @@
 jwt = "MY_JWT_TOKEN"
 backend_url="MY_PELIQAN_URL"
 
 pq = Peliqan(jwt, backend_url) 
 ```
 
 ### Argument List
-The **PeliqanClient** takes two arguments:
+The **`Peliqan`** class takes two arguments:
 
-- **jwt** (*required*): This is the jwt token provided to you and is used to authenticating the requests to the server. 
+- **jwt** (*required*): This is the JWT token provided to you and is used to authenticate requests from the client to the server. 
 
 
-- **backend_url** (*optional*): This is the url that points to the specific Peliqan environment. 
+- **backend_url** (*optional*): This is the `instance_url` that points to a specific Peliqan environment. 
 If no value is provided, the client will look for the `PELIQAN_URL` environment variable. If it is not set, 
-then the value defaults to **https://app.eu.peliqan.io/**.
+then the value defaults to *https://app.eu.peliqan.io/*.
 
-See [here](https://peliqan.notion.site/Peliqan-API-ab7e96d5122d427b877fd488ea812966) 
-to know how to find your Peliqan environment and JWT token.
+Learn how to find your Peliqan environment and JWT token [here](https://peliqan.notion.site/Peliqan-API-ab7e96d5122d427b877fd488ea812966/).
 
 ### Environment Variables
 Currently, only one environment variable is available.
 
 - **PELIQAN_UR**: If this variable is set then we need not provide a backend_url, while instantiating the client.
 - 
 ## Documentation
-See [here](https://peliqan.notion.site/Building-data-apps-bfd91569d0824629b090dc439d39ca63) 
-to learn more about available methods.
+See [here](https://peliqan.notion.site/Building-data-apps-bfd91569d0824629b090dc439d39ca63/) 
+to learn more about building data apps.
 
-See [here](https://peliqan.notion.site/Peliqan-documentation-52f91ae8f3364157a7a7fe063c9f694d) 
-to learn more about Peliqan.
+See [here](https://peliqan.notion.site/Peliqan-documentation-52f91ae8f3364157a7a7fe063c9f694d/) 
+to learn more about [Peliqan.io](https://www.peliqan.io/).
```

### Comparing `Peliqan-0.1.0/peliqan/__init__.py` & `Peliqan-0.1.1/peliqan/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __author__ = 'Peliqan.io'
 __credits__ = 'Peliqan.io'
 
 # import necessary modules
 import logging
 
 import pandas
@@ -436,14 +436,27 @@
         if description:
             data["description"] = description
         if tags:
             data["tags"] = tags
         response_dict = self.call_backend("patch", url, json=data)
         return response_dict
 
+    def get_interface(self, interface_id):
+        url = f"{self.BACKEND_URL}/api/interfaces/{interface_id}/"
+        return self.call_backend("get", url)
+
+    def get_interface_state(self, interface_id):
+        data = self.get_interface(interface_id)
+        return data.get('state', '')
+
+    def set_interface_state(self, interface_id, state):
+        url = f"{self.BACKEND_URL}/api/interfaces/{interface_id}/"
+        data = {'state': state}
+        return self.call_backend("patch", url, json=data)
+
 
 class BasePeliqanClient:
     """
     This base class wraps all operations we want to expose to our internal and external clients.
     """
 
     def __init__(self, jwt, backend_url):
@@ -459,15 +472,14 @@
            :param resource_name: name of the resource.
            :param kwargs: additional kwargs can also be passed.
            :return: resource details as a dict.
         """
         return self.__service_client__.find_resource(resource_type, resource_id, resource_name, **kwargs)
 
     # todo allow user to set a PK column for the query (or update the guessed PK)
-    # todo accept database id and table id as inputs too
     def load_table(self, table_name='', query='', table_id=None, fillna_with=''):
         """
         Return the records in a table.
 
         :param table_name: The name of a table.
         :param query: A valid Trino sql query.
         :param table_id: An integer value that uniquely identifies a table.
@@ -835,14 +847,33 @@
 
             table_select = "SELECT %s FROM %s" % (table_select_fields_str, table["name"])
             table_selects.append(table_select)
 
         union = " UNION ALL ".join(table_selects)
         return union
 
+    def get_interface_state(self, interface_id):
+        """
+        An interface is a saved program. Get the stored state for a specific interface.
+
+        :param interface_id: The id of the interface.
+        :return: Any
+        """
+        return self.__service_client__.get_interface_state(interface_id)
+
+    def set_interface_state(self, interface_id, state):
+        """
+        An interface is a saved program. Set the state for a specific interface in the peliqan environment.
+
+        :param interface_id: The id of the interface.
+        :param state: The data that will be stored as the state value for an interface.
+        :return:
+        """
+        return self.__service_client__.set_interface_state(interface_id, state)
+
 
 class Peliqan(BasePeliqanClient):
     """
         Import this API client to connect to a Peliqan environment and perform valid operations.
 
         :param jwt: The jwt token assigned to an Account.
```

### Comparing `Peliqan-0.1.0/setup.py` & `Peliqan-0.1.1/setup.py`

 * *Files identical despite different names*

