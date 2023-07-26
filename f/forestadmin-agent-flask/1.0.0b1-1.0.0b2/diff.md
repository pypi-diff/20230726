# Comparing `tmp/forestadmin_agent_flask-1.0.0b1.tar.gz` & `tmp/forestadmin_agent_flask-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_agent_flask-1.0.0b1.tar", max compression
+gzip compressed data, was "forestadmin_agent_flask-1.0.0b2.tar", max compression
```

## Comparing `forestadmin_agent_flask-1.0.0b1.tar` & `forestadmin_agent_flask-1.0.0b2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-07-21 14:38:11.871842 forestadmin_agent_flask-1.0.0b1/README.md
--rw-r--r--   0        0        0        0 2023-07-21 14:38:11.871842 forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/__init__.py
--rw-r--r--   0        0        0     7476 2023-07-21 14:38:11.871842 forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/agent.py
--rw-r--r--   0        0        0      125 2023-07-21 14:38:11.871842 forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/exception.py
--rw-r--r--   0        0        0        0 2023-07-21 14:38:11.871842 forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/utils/__init__.py
--rw-r--r--   0        0        0      581 2023-07-21 14:38:11.871842 forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/utils/dispatcher.py
--rw-r--r--   0        0        0     1449 2023-07-21 14:38:11.871842 forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/utils/requests.py
--rw-r--r--   0        0        0     1797 2023-07-21 14:38:35.884063 forestadmin_agent_flask-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 forestadmin_agent_flask-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 13:25:02.497040 forestadmin_agent_flask-1.0.0b2/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 13:25:02.497040 forestadmin_agent_flask-1.0.0b2/forestadmin/flask_agent/__init__.py
+-rw-r--r--   0        0        0     7476 2023-07-26 13:25:02.497040 forestadmin_agent_flask-1.0.0b2/forestadmin/flask_agent/agent.py
+-rw-r--r--   0        0        0      125 2023-07-26 13:25:02.497040 forestadmin_agent_flask-1.0.0b2/forestadmin/flask_agent/exception.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:25:02.497040 forestadmin_agent_flask-1.0.0b2/forestadmin/flask_agent/utils/__init__.py
+-rw-r--r--   0        0        0      581 2023-07-26 13:25:02.497040 forestadmin_agent_flask-1.0.0b2/forestadmin/flask_agent/utils/dispatcher.py
+-rw-r--r--   0        0        0     1449 2023-07-26 13:25:02.497040 forestadmin_agent_flask-1.0.0b2/forestadmin/flask_agent/utils/requests.py
+-rw-r--r--   0        0        0     1797 2023-07-26 13:25:28.085331 forestadmin_agent_flask-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 forestadmin_agent_flask-1.0.0b2/PKG-INFO
```

### Comparing `forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/agent.py` & `forestadmin_agent_flask-1.0.0b2/forestadmin/flask_agent/agent.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/utils/dispatcher.py` & `forestadmin_agent_flask-1.0.0b2/forestadmin/flask_agent/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/utils/requests.py` & `forestadmin_agent_flask-1.0.0b2/forestadmin/flask_agent/utils/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_flask-1.0.0b1/pyproject.toml` & `forestadmin_agent_flask-1.0.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-agent-flask"
-version = "1.0.0-beta.1"
+version = "1.0.0-beta.2"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 typing-extensions = "~=4.2"
 tzdata = "~=2022.6"
-forestadmin-agent-toolkit = "^1.0.0-beta.1"
-forestadmin-datasource-toolkit = "^1.0.0-beta.1"
+forestadmin-agent-toolkit = "^1.0.0-beta.2"
+forestadmin-datasource-toolkit = "^1.0.0-beta.2"
 Flask-Cors = "^3.0.8"
 
 [tool.poetry.dependencies.flask]
 extras = [ "async",]
 version = "^2.0.0"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
```

### Comparing `forestadmin_agent_flask-1.0.0b1/PKG-INFO` & `forestadmin_agent_flask-1.0.0b2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: forestadmin-agent-flask
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: 
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Flask-Cors (>=3.0.8,<4.0.0)
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: flask[async] (>=2.0.0,<3.0.0)
-Requires-Dist: forestadmin-agent-toolkit (>=1.0.0-beta.1,<2.0.0)
-Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.1,<2.0.0)
+Requires-Dist: forestadmin-agent-toolkit (>=1.0.0-beta.2,<2.0.0)
+Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.2,<2.0.0)
 Requires-Dist: typing-extensions (>=4.2,<5.0)
 Requires-Dist: tzdata (>=2022.6,<2023.0)
 Description-Content-Type: text/markdown
```

