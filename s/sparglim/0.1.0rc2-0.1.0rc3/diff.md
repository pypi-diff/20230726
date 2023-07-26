# Comparing `tmp/sparglim-0.1.0rc2.tar.gz` & `tmp/sparglim-0.1.0rc3.tar.gz`

## Comparing `sparglim-0.1.0rc2.tar` & `sparglim-0.1.0rc3.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/.editorconfig
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/RELEASE.md
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/.github/workflows/lint.yml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/dev/pyspark-app/Dockerfile.lab
--rwxr-xr-x   0        0        0      127 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/dev/pyspark-app/reload.sh
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/dev/pyspark-app/k8s/deployment.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/dev/pyspark-app/k8s/headless-service.yaml
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/dev/pyspark-app/k8s/lab-service.yaml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/dev/sparglim-server/Dockerfile.sparglim-server
--rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/dev/sparglim-server/reload.sh
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/dev/sparglim-server/k8s/connect-server-service.yaml
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/dev/sparglim-server/k8s/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/dev/sparglim-server/k8s/headless-service.yaml
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/docker/Dockerfile.lab
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/docker/Dockerfile.sparglim-server
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/docs/Makefile
--rwxr-xr-x   0        0        0     4786 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/docs/conf.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/docs/index.rst
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/docs/make.bat
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/docs/usage.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/example/pyspark-app/README.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/example/pyspark-app/k8s/deployment.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/example/pyspark-app/k8s/headless-service.yaml
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/example/pyspark-app/k8s/lab-service.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/example/sparglim-server/README.md
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/example/sparglim-server/k8s/connect-server-service.yaml
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/example/sparglim-server/k8s/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/example/sparglim-server/k8s/headless-service.yaml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/sparglim/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/sparglim/exceptions.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/sparglim/log.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/sparglim/py.typed
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/sparglim/utils.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/sparglim/config/__init__.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/sparglim/config/builder.py
--rw-r--r--   0        0        0    11568 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/sparglim/config/configer.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/sparglim/config/k8s.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/sparglim/server/__init__.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/sparglim/server/cli.py
--rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/sparglim/server/daemon.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/sparglim/server/tailer.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/sparglim/sql/__init__.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/sparglim/sql/magic.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/tests/conftest.py
--rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/tests/test_builder.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/tests/test_daemon.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/tests/test_magic.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/tests/example/people.json
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/tests/mock/sbin/entrypoint.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/tests/mock/sbin/mock_spark_server.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/tests/mock/sbin/start-connect-server.sh
--rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/.gitignore
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/LICENSE
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/README.md
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/pyproject.toml
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 sparglim-0.1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/.editorconfig
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/RELEASE.md
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/.github/workflows/docker-publish.yml
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/pyspark-app/Dockerfile.jupyterlab-sparglim
+-rwxr-xr-x   0        0        0      127 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/pyspark-app/reload.sh
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/pyspark-app/k8s/deployment.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/pyspark-app/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/pyspark-app/k8s/lab-service.yaml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/sparglim-server/Dockerfile.sparglim-server
+-rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/sparglim-server/reload.sh
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/sparglim-server/k8s/connect-server-service.yaml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/sparglim-server/k8s/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/dev/sparglim-server/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/docker/Dockerfile.jupyterlab-sparglim
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/docker/Dockerfile.sparglim-server
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/docs/Makefile
+-rwxr-xr-x   0        0        0     4786 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/docs/conf.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/docs/index.rst
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/docs/make.bat
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/docs/usage.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/example/pyspark-app/README.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/example/pyspark-app/k8s/deployment.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/example/pyspark-app/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/example/pyspark-app/k8s/lab-service.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/example/sparglim-server/README.md
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/example/sparglim-server/k8s/connect-server-service.yaml
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/example/sparglim-server/k8s/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/example/sparglim-server/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/exceptions.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/log.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/py.typed
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/utils.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/config/__init__.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/config/builder.py
+-rw-r--r--   0        0        0    11568 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/config/configer.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/config/k8s.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/server/__init__.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/server/cli.py
+-rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/server/daemon.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/server/tailer.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/sql/__init__.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/sparglim/sql/magic.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/tests/conftest.py
+-rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/tests/test_builder.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/tests/test_daemon.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/tests/test_magic.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/tests/example/people.json
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/tests/mock/sbin/entrypoint.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/tests/mock/sbin/mock_spark_server.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/tests/mock/sbin/start-connect-server.sh
+-rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/.gitignore
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/LICENSE
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/README.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 sparglim-0.1.0rc3/PKG-INFO
```

### Comparing `sparglim-0.1.0rc2/.pre-commit-config.yaml` & `sparglim-0.1.0rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/RELEASE.md` & `sparglim-0.1.0rc3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/.github/workflows/python-package.yml` & `sparglim-0.1.0rc3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/.github/workflows/python-publish.yml` & `sparglim-0.1.0rc3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/dev/pyspark-app/k8s/deployment.yaml` & `sparglim-0.1.0rc3/dev/pyspark-app/k8s/deployment.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   template:
     metadata:
       labels:
         app: sparglim-app
     spec:
       containers:
         - name: sparglim-app
-          image: wh1isper/sparglim-lab:dev
+          image: wh1isper/jupyterlab-sparglim:dev
           ports:
             - containerPort: 8888
           imagePullPolicy: Never
           env:
             - name: SPARGLIM_SQL_MODE
               value: "k8s"
             - name: SPARGLIM_DRIVER_HOST
```

### Comparing `sparglim-0.1.0rc2/dev/sparglim-server/k8s/deployment.yaml` & `sparglim-0.1.0rc3/example/sparglim-server/k8s/deployment.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -14,18 +14,18 @@
   template:
     metadata:
       labels:
         app: sparglim-server
     spec:
       containers:
         - name: sparglim-server
-          image: wh1isper/sparglim-server:dev
+          image: wh1isper/sparglim-server
           ports:
             - containerPort: 15002
-          imagePullPolicy: IfNotPresent
+          imagePullPolicy: Always
           env:
             - name: SPARGLIM_SERVER_MODE
               value: "k8s"
             - name: SPARGLIM_DRIVER_HOST
               valueFrom:
                 fieldRef:
                   fieldPath: status.podIP
```

### Comparing `sparglim-0.1.0rc2/docs/Makefile` & `sparglim-0.1.0rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/docs/conf.py` & `sparglim-0.1.0rc3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/docs/make.bat` & `sparglim-0.1.0rc3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/example/pyspark-app/k8s/deployment.yaml` & `sparglim-0.1.0rc3/example/pyspark-app/k8s/deployment.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   template:
     metadata:
       labels:
         app: sparglim-app
     spec:
       containers:
         - name: sparglim-app
-          image: wh1isper/sparglim-lab:latest
+          image: wh1isper/jupyterlab-sparglim
           ports:
             - containerPort: 8888
           imagePullPolicy: Always
           env:
             - name: SPARGLIM_SQL_MODE
               value: "k8s"
             - name: SPARGLIM_DRIVER_HOST
```

### Comparing `sparglim-0.1.0rc2/example/sparglim-server/k8s/deployment.yaml` & `sparglim-0.1.0rc3/dev/sparglim-server/k8s/deployment.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -14,18 +14,18 @@
   template:
     metadata:
       labels:
         app: sparglim-server
     spec:
       containers:
         - name: sparglim-server
-          image: wh1isper/sparglim-server
+          image: wh1isper/sparglim-server:dev
           ports:
             - containerPort: 15002
-          imagePullPolicy: IfNotPresent
+          imagePullPolicy: Never
           env:
             - name: SPARGLIM_SERVER_MODE
               value: "k8s"
             - name: SPARGLIM_DRIVER_HOST
               valueFrom:
                 fieldRef:
                   fieldPath: status.podIP
```

### Comparing `sparglim-0.1.0rc2/sparglim/utils.py` & `sparglim-0.1.0rc3/sparglim/utils.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/sparglim/config/builder.py` & `sparglim-0.1.0rc3/sparglim/config/builder.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/sparglim/config/configer.py` & `sparglim-0.1.0rc3/sparglim/config/configer.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/sparglim/config/k8s.py` & `sparglim-0.1.0rc3/sparglim/config/k8s.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/sparglim/server/cli.py` & `sparglim-0.1.0rc3/sparglim/server/cli.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/sparglim/server/daemon.py` & `sparglim-0.1.0rc3/sparglim/server/daemon.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/sparglim/server/tailer.py` & `sparglim-0.1.0rc3/sparglim/server/tailer.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/sparglim/sql/magic.py` & `sparglim-0.1.0rc3/sparglim/sql/magic.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/tests/conftest.py` & `sparglim-0.1.0rc3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/tests/test_builder.py` & `sparglim-0.1.0rc3/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/tests/test_daemon.py` & `sparglim-0.1.0rc3/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/tests/test_magic.py` & `sparglim-0.1.0rc3/tests/test_magic.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/tests/mock/sbin/entrypoint.py` & `sparglim-0.1.0rc3/tests/mock/sbin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/tests/mock/sbin/mock_spark_server.py` & `sparglim-0.1.0rc3/tests/mock/sbin/mock_spark_server.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/.gitignore` & `sparglim-0.1.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/LICENSE` & `sparglim-0.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/README.md` & `sparglim-0.1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/pyproject.toml` & `sparglim-0.1.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc2/PKG-INFO` & `sparglim-0.1.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparglim
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: sparglim
 Project-URL: Source, https://github.com/wh1isper/sparglim
 Author-email: wh1isper <9573586@qq.com>
 License: BSD license
 License-File: LICENSE
 Keywords: sparglim
 Classifier: Programming Language :: Python :: 3
```

