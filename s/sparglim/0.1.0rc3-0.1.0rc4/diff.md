# Comparing `tmp/sparglim-0.1.0rc3.tar.gz` & `tmp/sparglim-0.1.0rc4.tar.gz`

## Comparing `sparglim-0.1.0rc3.tar` & `sparglim-0.1.0rc4.tar`

### file list

```diff
@@ -1,61 +1,60 @@
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/.editorconfig
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/RELEASE.md
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/.github/workflows/docker-publish.yml
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/.github/workflows/lint.yml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/pyspark-app/Dockerfile.jupyterlab-sparglim
--rwxr-xr-x   0        0        0      127 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/pyspark-app/reload.sh
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/pyspark-app/k8s/deployment.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/pyspark-app/k8s/headless-service.yaml
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/pyspark-app/k8s/lab-service.yaml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/sparglim-server/Dockerfile.sparglim-server
--rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/sparglim-server/reload.sh
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/sparglim-server/k8s/connect-server-service.yaml
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/sparglim-server/k8s/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/sparglim-server/k8s/headless-service.yaml
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/docker/Dockerfile.jupyterlab-sparglim
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/docker/Dockerfile.sparglim-server
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/docs/Makefile
--rwxr-xr-x   0        0        0     4786 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/docs/conf.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/docs/index.rst
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/docs/make.bat
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/docs/usage.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/example/pyspark-app/README.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/example/pyspark-app/k8s/deployment.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/example/pyspark-app/k8s/headless-service.yaml
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/example/pyspark-app/k8s/lab-service.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/example/sparglim-server/README.md
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/example/sparglim-server/k8s/connect-server-service.yaml
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/example/sparglim-server/k8s/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/example/sparglim-server/k8s/headless-service.yaml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/exceptions.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/log.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/py.typed
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/utils.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/config/__init__.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/config/builder.py
--rw-r--r--   0        0        0    11568 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/config/configer.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/config/k8s.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/server/__init__.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/server/cli.py
--rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/server/daemon.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/server/tailer.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/sql/__init__.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/sql/magic.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/tests/conftest.py
--rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/tests/test_builder.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/tests/test_daemon.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/tests/test_magic.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/tests/example/people.json
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/tests/mock/sbin/entrypoint.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/tests/mock/sbin/mock_spark_server.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/tests/mock/sbin/start-connect-server.sh
--rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/.gitignore
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/LICENSE
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/README.md
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/pyproject.toml
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/.editorconfig
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/RELEASE.md
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/dev/pyspark-app/Dockerfile.jupyterlab-sparglim
+-rwxr-xr-x   0        0        0      127 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/dev/pyspark-app/reload.sh
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/dev/pyspark-app/k8s/deployment.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/dev/pyspark-app/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/dev/pyspark-app/k8s/lab-service.yaml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/dev/sparglim-server/Dockerfile.sparglim-server
+-rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/dev/sparglim-server/reload.sh
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/dev/sparglim-server/k8s/connect-server-service.yaml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/dev/sparglim-server/k8s/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/dev/sparglim-server/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/docker/Dockerfile.jupyterlab-sparglim
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/docker/Dockerfile.sparglim-server
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/docs/Makefile
+-rwxr-xr-x   0        0        0     4786 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/docs/conf.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/docs/index.rst
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/docs/make.bat
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/docs/usage.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/example/pyspark-app/README.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/example/pyspark-app/k8s/deployment.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/example/pyspark-app/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/example/pyspark-app/k8s/lab-service.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/example/sparglim-server/README.md
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/example/sparglim-server/k8s/connect-server-service.yaml
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/example/sparglim-server/k8s/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/example/sparglim-server/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/sparglim/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/sparglim/exceptions.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/sparglim/log.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/sparglim/py.typed
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/sparglim/utils.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/sparglim/config/__init__.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/sparglim/config/builder.py
+-rw-r--r--   0        0        0    11568 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/sparglim/config/configer.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/sparglim/config/k8s.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/sparglim/server/__init__.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/sparglim/server/cli.py
+-rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/sparglim/server/daemon.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/sparglim/server/tailer.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/sparglim/sql/__init__.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/sparglim/sql/magic.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/tests/conftest.py
+-rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/tests/test_builder.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/tests/test_daemon.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/tests/test_magic.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/tests/example/people.json
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/tests/mock/sbin/entrypoint.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/tests/mock/sbin/mock_spark_server.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/tests/mock/sbin/start-connect-server.sh
+-rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/.gitignore
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/LICENSE
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/README.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 sparglim-0.1.0rc4/PKG-INFO
```

### Comparing `sparglim-0.1.0rc3/.pre-commit-config.yaml` & `sparglim-0.1.0rc4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/RELEASE.md` & `sparglim-0.1.0rc4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/.github/workflows/python-package.yml` & `sparglim-0.1.0rc4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/dev/pyspark-app/Dockerfile.jupyterlab-sparglim` & `sparglim-0.1.0rc4/dev/pyspark-app/Dockerfile.jupyterlab-sparglim`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/dev/pyspark-app/k8s/deployment.yaml` & `sparglim-0.1.0rc4/dev/pyspark-app/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/dev/sparglim-server/k8s/deployment.yaml` & `sparglim-0.1.0rc4/dev/sparglim-server/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/docs/Makefile` & `sparglim-0.1.0rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/docs/conf.py` & `sparglim-0.1.0rc4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/docs/make.bat` & `sparglim-0.1.0rc4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/example/pyspark-app/k8s/deployment.yaml` & `sparglim-0.1.0rc4/example/pyspark-app/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/example/sparglim-server/k8s/deployment.yaml` & `sparglim-0.1.0rc4/example/sparglim-server/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/sparglim/utils.py` & `sparglim-0.1.0rc4/sparglim/utils.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/sparglim/config/builder.py` & `sparglim-0.1.0rc4/sparglim/config/builder.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/sparglim/config/configer.py` & `sparglim-0.1.0rc4/sparglim/config/configer.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/sparglim/config/k8s.py` & `sparglim-0.1.0rc4/sparglim/config/k8s.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/sparglim/server/cli.py` & `sparglim-0.1.0rc4/sparglim/server/cli.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/sparglim/server/daemon.py` & `sparglim-0.1.0rc4/sparglim/server/daemon.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/sparglim/server/tailer.py` & `sparglim-0.1.0rc4/sparglim/server/tailer.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/sparglim/sql/magic.py` & `sparglim-0.1.0rc4/sparglim/sql/magic.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/tests/conftest.py` & `sparglim-0.1.0rc4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/tests/test_builder.py` & `sparglim-0.1.0rc4/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/tests/test_daemon.py` & `sparglim-0.1.0rc4/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/tests/test_magic.py` & `sparglim-0.1.0rc4/tests/test_magic.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/tests/mock/sbin/entrypoint.py` & `sparglim-0.1.0rc4/tests/mock/sbin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/tests/mock/sbin/mock_spark_server.py` & `sparglim-0.1.0rc4/tests/mock/sbin/mock_spark_server.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/.gitignore` & `sparglim-0.1.0rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/LICENSE` & `sparglim-0.1.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/README.md` & `sparglim-0.1.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/pyproject.toml` & `sparglim-0.1.0rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc3/PKG-INFO` & `sparglim-0.1.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparglim
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: sparglim
 Project-URL: Source, https://github.com/wh1isper/sparglim
 Author-email: wh1isper <9573586@qq.com>
 License: BSD license
 License-File: LICENSE
 Keywords: sparglim
 Classifier: Programming Language :: Python :: 3
```

