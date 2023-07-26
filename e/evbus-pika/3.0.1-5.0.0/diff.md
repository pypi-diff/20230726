# Comparing `tmp/evbus-pika-3.0.1.tar.gz` & `tmp/evbus-pika-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evbus-pika-3.0.1.tar", last modified: Tue Mar  1 01:30:03 2022, max compression
+gzip compressed data, was "evbus-pika-5.0.0.tar", last modified: Wed Jul 26 15:30:24 2023, max compression
```

## Comparing `evbus-pika-3.0.1.tar` & `evbus-pika-5.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 01:30:03.622907 evbus-pika-3.0.1/
--rw-r--r--   0 root         (0) root         (0)    11343 2022-03-01 01:29:47.000000 evbus-pika-3.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4013 2022-03-01 01:30:03.622907 evbus-pika-3.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3149 2022-03-01 01:29:47.000000 evbus-pika-3.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 01:30:03.621907 evbus-pika-3.0.1/evbus_pika/
--rw-r--r--   0 root         (0) root         (0)       32 2022-03-01 01:29:47.000000 evbus-pika-3.0.1/evbus_pika/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 01:30:03.622907 evbus-pika-3.0.1/evbus_pika/ingress/
--rw-r--r--   0 root         (0) root         (0)     1487 2022-03-01 01:29:47.000000 evbus-pika-3.0.1/evbus_pika/ingress/pika.py
--rw-r--r--   0 root         (0) root         (0)       18 2022-03-01 01:30:03.000000 evbus-pika-3.0.1/evbus_pika/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 01:30:03.622907 evbus-pika-3.0.1/evbus_pika.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4013 2022-03-01 01:30:03.000000 evbus-pika-3.0.1/evbus_pika.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      274 2022-03-01 01:30:03.000000 evbus-pika-3.0.1/evbus_pika.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-01 01:30:03.000000 evbus-pika-3.0.1/evbus_pika.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2022-03-01 01:30:03.000000 evbus-pika-3.0.1/evbus_pika.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-03-01 01:30:03.000000 evbus-pika-3.0.1/evbus_pika.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-03-01 01:30:03.622907 evbus-pika-3.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2743 2022-03-01 01:29:47.000000 evbus-pika-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:30:24.834335 evbus-pika-5.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-07-26 15:30:09.000000 evbus-pika-5.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4206 2023-07-26 15:30:24.834335 evbus-pika-5.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3341 2023-07-26 15:30:09.000000 evbus-pika-5.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:30:24.834335 evbus-pika-5.0.0/evbus_pika/
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-26 15:30:09.000000 evbus-pika-5.0.0/evbus_pika/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:30:24.834335 evbus-pika-5.0.0/evbus_pika/ingress/
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-07-26 15:30:09.000000 evbus-pika-5.0.0/evbus_pika/ingress/pika.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-26 15:30:24.000000 evbus-pika-5.0.0/evbus_pika/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:30:24.834335 evbus-pika-5.0.0/evbus_pika.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4206 2023-07-26 15:30:24.000000 evbus-pika-5.0.0/evbus_pika.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-26 15:30:24.000000 evbus-pika-5.0.0/evbus_pika.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 15:30:24.000000 evbus-pika-5.0.0/evbus_pika.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-26 15:30:24.000000 evbus-pika-5.0.0/evbus_pika.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-26 15:30:24.000000 evbus-pika-5.0.0/evbus_pika.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 15:30:24.834335 evbus-pika-5.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2744 2023-07-26 15:30:09.000000 evbus-pika-5.0.0/setup.py
```

### Comparing `evbus-pika-3.0.1/LICENSE` & `evbus-pika-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evbus-pika-3.0.1/PKG-INFO` & `evbus-pika-5.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: evbus-pika
-Version: 3.0.1
+Version: 5.0.0
 Summary: app-merge component for pop-evbus
 Home-page: https://gitlab.com/vmware/idem/evbus-pika
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ==========
 evbus-pika
 ==========
 
@@ -38,15 +38,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
 
@@ -116,15 +116,22 @@
 =======
 
 The rabbitmq-server binary needs to be installed via your package manager.
 Start a local rabbitmq-server with the default parameters:
 
 .. code-block:: bash
 
-    sudo rabbitmq-server
+    $ docker run -p 5672:5672 \
+    --env RABBITMQ_HOSTS=localhost \
+    --env RABBITMQ_PORT=5672 \
+    --env RABBITMQ_USER=guest \
+    --env RABBITMQ_PASS=guest \
+    --env RABBITMQ_PROTOCOL=amqp \
+    rabbitmq:management
+
 
 Configure credentials for testing with a local rabbitmq server:
 
 .. code-block:: sls
 
     # credentials.yml
     pika:
@@ -138,15 +145,15 @@
 
 Encrypt the credentials file and export the ACCT environment variables
 
 .. code-block:: bash
 
     $ pip install acct
     $ export ACCT_KEY=$(acct encrypt credentials.yml)
-    $ export ACCT_FILE="$PWD/credentials.yml.fernet"
+    $ export ACCT_FILE="$PWD/credentials.yml"
 
 Install testing requirements
 
 .. code-block:: bash
 
     $ pip install -r requirements/test.in
```

### Comparing `evbus-pika-3.0.1/README.rst` & `evbus-pika-5.0.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
 
@@ -92,15 +92,22 @@
 =======
 
 The rabbitmq-server binary needs to be installed via your package manager.
 Start a local rabbitmq-server with the default parameters:
 
 .. code-block:: bash
 
-    sudo rabbitmq-server
+    $ docker run -p 5672:5672 \
+    --env RABBITMQ_HOSTS=localhost \
+    --env RABBITMQ_PORT=5672 \
+    --env RABBITMQ_USER=guest \
+    --env RABBITMQ_PASS=guest \
+    --env RABBITMQ_PROTOCOL=amqp \
+    rabbitmq:management
+
 
 Configure credentials for testing with a local rabbitmq server:
 
 .. code-block:: sls
 
     # credentials.yml
     pika:
@@ -114,15 +121,15 @@
 
 Encrypt the credentials file and export the ACCT environment variables
 
 .. code-block:: bash
 
     $ pip install acct
     $ export ACCT_KEY=$(acct encrypt credentials.yml)
-    $ export ACCT_FILE="$PWD/credentials.yml.fernet"
+    $ export ACCT_FILE="$PWD/credentials.yml"
 
 Install testing requirements
 
 .. code-block:: bash
 
     $ pip install -r requirements/test.in
```

### Comparing `evbus-pika-3.0.1/evbus_pika/ingress/pika.py` & `evbus-pika-5.0.0/evbus_pika/ingress/pika.py`

 * *Files identical despite different names*

### Comparing `evbus-pika-3.0.1/evbus_pika.egg-info/PKG-INFO` & `evbus-pika-5.0.0/evbus_pika.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: evbus-pika
-Version: 3.0.1
+Version: 5.0.0
 Summary: app-merge component for pop-evbus
 Home-page: https://gitlab.com/vmware/idem/evbus-pika
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ==========
 evbus-pika
 ==========
 
@@ -38,15 +38,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
 
@@ -116,15 +116,22 @@
 =======
 
 The rabbitmq-server binary needs to be installed via your package manager.
 Start a local rabbitmq-server with the default parameters:
 
 .. code-block:: bash
 
-    sudo rabbitmq-server
+    $ docker run -p 5672:5672 \
+    --env RABBITMQ_HOSTS=localhost \
+    --env RABBITMQ_PORT=5672 \
+    --env RABBITMQ_USER=guest \
+    --env RABBITMQ_PASS=guest \
+    --env RABBITMQ_PROTOCOL=amqp \
+    rabbitmq:management
+
 
 Configure credentials for testing with a local rabbitmq server:
 
 .. code-block:: sls
 
     # credentials.yml
     pika:
@@ -138,15 +145,15 @@
 
 Encrypt the credentials file and export the ACCT environment variables
 
 .. code-block:: bash
 
     $ pip install acct
     $ export ACCT_KEY=$(acct encrypt credentials.yml)
-    $ export ACCT_FILE="$PWD/credentials.yml.fernet"
+    $ export ACCT_FILE="$PWD/credentials.yml"
 
 Install testing requirements
 
 .. code-block:: bash
 
     $ pip install -r requirements/test.in
```

### Comparing `evbus-pika-3.0.1/setup.py` & `evbus-pika-5.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,24 +70,24 @@
     url="https://gitlab.com/vmware/idem/evbus-pika",
     version=VERSION,
     install_requires=REQUIREMENTS,
     extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
     ],
     packages=discover_packages(),
     cmdclass={"clean": Clean},
 )
```

