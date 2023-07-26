# Comparing `tmp/kafkaesk-0.8.0.tar.gz` & `tmp/kafkaesk-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafkaesk-0.8.0.tar", max compression
+gzip compressed data, was "kafkaesk-0.8.1.tar", max compression
```

## Comparing `kafkaesk-0.8.0.tar` & `kafkaesk-0.8.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1314 2023-06-14 16:04:39.114493 kafkaesk-0.8.0/LICENSE
--rw-r--r--   0        0        0     8653 2023-06-14 16:04:39.114493 kafkaesk-0.8.0/README.md
--rw-r--r--   0        0        0      208 2023-06-14 16:04:39.114493 kafkaesk-0.8.0/kafkaesk/__init__.py
--rw-r--r--   0        0        0    22572 2023-06-14 16:04:39.114493 kafkaesk-0.8.0/kafkaesk/app.py
--rw-r--r--   0        0        0    18351 2023-06-14 16:04:39.114493 kafkaesk-0.8.0/kafkaesk/consumer.py
--rw-r--r--   0        0        0     1121 2023-06-14 16:04:39.114493 kafkaesk-0.8.0/kafkaesk/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-14 16:04:39.114493 kafkaesk-0.8.0/kafkaesk/ext/__init__.py
--rw-r--r--   0        0        0      210 2023-06-14 16:04:39.114493 kafkaesk-0.8.0/kafkaesk/ext/logging/__init__.py
--rw-r--r--   0        0        0     7620 2023-06-14 16:04:39.114493 kafkaesk-0.8.0/kafkaesk/ext/logging/handler.py
--rw-r--r--   0        0        0     1719 2023-06-14 16:04:39.114493 kafkaesk-0.8.0/kafkaesk/ext/logging/record.py
--rw-r--r--   0        0        0     5081 2023-06-14 16:04:39.114493 kafkaesk-0.8.0/kafkaesk/kafka.py
--rw-r--r--   0        0        0     3980 2023-06-14 16:04:39.114493 kafkaesk-0.8.0/kafkaesk/metrics.py
--rw-r--r--   0        0        0        0 2023-06-14 16:04:39.114493 kafkaesk-0.8.0/kafkaesk/publish.py
--rw-r--r--   0        0        0        0 2023-06-14 16:04:39.114493 kafkaesk-0.8.0/kafkaesk/py.typed
--rw-r--r--   0        0        0      904 2023-06-14 16:04:39.114493 kafkaesk-0.8.0/kafkaesk/utils.py
--rw-r--r--   0        0        0     1711 2023-06-14 16:04:39.118490 kafkaesk-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     9776 1970-01-01 00:00:00.000000 kafkaesk-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1314 2023-07-26 18:53:29.170640 kafkaesk-0.8.1/LICENSE
+-rw-r--r--   0        0        0     8657 2023-07-26 18:53:29.170640 kafkaesk-0.8.1/README.md
+-rw-r--r--   0        0        0      208 2023-07-26 18:53:29.170640 kafkaesk-0.8.1/kafkaesk/__init__.py
+-rw-r--r--   0        0        0    22572 2023-07-26 18:53:29.170640 kafkaesk-0.8.1/kafkaesk/app.py
+-rw-r--r--   0        0        0    18351 2023-07-26 18:53:29.170640 kafkaesk-0.8.1/kafkaesk/consumer.py
+-rw-r--r--   0        0        0     1121 2023-07-26 18:53:29.170640 kafkaesk-0.8.1/kafkaesk/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-26 18:53:29.170640 kafkaesk-0.8.1/kafkaesk/ext/__init__.py
+-rw-r--r--   0        0        0      210 2023-07-26 18:53:29.170640 kafkaesk-0.8.1/kafkaesk/ext/logging/__init__.py
+-rw-r--r--   0        0        0     7620 2023-07-26 18:53:29.170640 kafkaesk-0.8.1/kafkaesk/ext/logging/handler.py
+-rw-r--r--   0        0        0     1719 2023-07-26 18:53:29.170640 kafkaesk-0.8.1/kafkaesk/ext/logging/record.py
+-rw-r--r--   0        0        0     5081 2023-07-26 18:53:29.170640 kafkaesk-0.8.1/kafkaesk/kafka.py
+-rw-r--r--   0        0        0     3980 2023-07-26 18:53:29.170640 kafkaesk-0.8.1/kafkaesk/metrics.py
+-rw-r--r--   0        0        0        0 2023-07-26 18:53:29.170640 kafkaesk-0.8.1/kafkaesk/publish.py
+-rw-r--r--   0        0        0        0 2023-07-26 18:53:29.170640 kafkaesk-0.8.1/kafkaesk/py.typed
+-rw-r--r--   0        0        0      904 2023-07-26 18:53:29.170640 kafkaesk-0.8.1/kafkaesk/utils.py
+-rw-r--r--   0        0        0     1711 2023-07-26 18:53:29.174640 kafkaesk-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     9780 1970-01-01 00:00:00.000000 kafkaesk-0.8.1/PKG-INFO
```

### Comparing `kafkaesk-0.8.0/LICENSE` & `kafkaesk-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.8.0/README.md` & `kafkaesk-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -154,20 +154,20 @@
 @app.subscribe("content.*", "group_id")
 async def get_messages(data: ContentMessage, subscriber):
     print(f"{data.foo}")
     await subscriber.consumer.commit()
 ```
 
 ## SSL
-Add these values to your `kafak_settings`:
-    `ssl_context` - this should be a placeholder as the SSL Context is generally created within the application
-    `security_protocol` - one of SSL or PLAINTEXT
-    `sasl_mechanism` - one of PLAIN, GSSAPI, SCRAM-SHA-256, SCRAM-SHA-512, OAUTHBEARER
-    `sasl_plain_username`
-    `sasl_plain_password`
+Add these values to your `kafka_settings`:  
+- `ssl_context` - this should be a placeholder as the SSL Context is generally created within the application  
+- `security_protocol` - one of SSL or PLAINTEXT  
+- `sasl_mechanism` - one of PLAIN, GSSAPI, SCRAM-SHA-256, SCRAM-SHA-512, OAUTHBEARER  
+- `sasl_plain_username` . 
+- `sasl_plain_password` . 
 
 ## kafkaesk contract
 
 This is a library around using kafka.
 Kafka itself does not enforce these concepts.
 
 - Every message must provide a json schema
```

### Comparing `kafkaesk-0.8.0/kafkaesk/app.py` & `kafkaesk-0.8.1/kafkaesk/app.py`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.8.0/kafkaesk/consumer.py` & `kafkaesk-0.8.1/kafkaesk/consumer.py`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.8.0/kafkaesk/exceptions.py` & `kafkaesk-0.8.1/kafkaesk/exceptions.py`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.8.0/kafkaesk/ext/logging/handler.py` & `kafkaesk-0.8.1/kafkaesk/ext/logging/handler.py`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.8.0/kafkaesk/ext/logging/record.py` & `kafkaesk-0.8.1/kafkaesk/ext/logging/record.py`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.8.0/kafkaesk/kafka.py` & `kafkaesk-0.8.1/kafkaesk/kafka.py`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.8.0/kafkaesk/metrics.py` & `kafkaesk-0.8.1/kafkaesk/metrics.py`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.8.0/kafkaesk/utils.py` & `kafkaesk-0.8.1/kafkaesk/utils.py`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.8.0/pyproject.toml` & `kafkaesk-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kafkaesk"
-version = "0.8.0"
+version = "0.8.1"
 description = "Easy publish and subscribe to events with python and Kafka."
 authors = ["vangheem <vangheem@gmail.com>", "pfreixes <pfreixes@gmail.com>"]
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Framework :: AsyncIO",
```

### Comparing `kafkaesk-0.8.0/PKG-INFO` & `kafkaesk-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafkaesk
-Version: 0.8.0
+Version: 0.8.1
 Summary: Easy publish and subscribe to events with python and Kafka.
 Author: vangheem
 Author-email: vangheem@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -182,20 +182,20 @@
 @app.subscribe("content.*", "group_id")
 async def get_messages(data: ContentMessage, subscriber):
     print(f"{data.foo}")
     await subscriber.consumer.commit()
 ```
 
 ## SSL
-Add these values to your `kafak_settings`:
-    `ssl_context` - this should be a placeholder as the SSL Context is generally created within the application
-    `security_protocol` - one of SSL or PLAINTEXT
-    `sasl_mechanism` - one of PLAIN, GSSAPI, SCRAM-SHA-256, SCRAM-SHA-512, OAUTHBEARER
-    `sasl_plain_username`
-    `sasl_plain_password`
+Add these values to your `kafka_settings`:  
+- `ssl_context` - this should be a placeholder as the SSL Context is generally created within the application  
+- `security_protocol` - one of SSL or PLAINTEXT  
+- `sasl_mechanism` - one of PLAIN, GSSAPI, SCRAM-SHA-256, SCRAM-SHA-512, OAUTHBEARER  
+- `sasl_plain_username` . 
+- `sasl_plain_password` . 
 
 ## kafkaesk contract
 
 This is a library around using kafka.
 Kafka itself does not enforce these concepts.
 
 - Every message must provide a json schema
```

