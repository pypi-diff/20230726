# Comparing `tmp/airflow_mcd-0.1.7.tar.gz` & `tmp/airflow_mcd-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow_mcd-0.1.7.tar", last modified: Mon Jul 24 21:15:55 2023, max compression
+gzip compressed data, was "dist/airflow_mcd-0.1.8.tar", last modified: Wed Jul 26 16:15:43 2023, max compression
```

## Comparing `airflow_mcd-0.1.7.tar` & `airflow_mcd-0.1.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.552064 airflow_mcd-0.1.7/.circleci/
--rw-r--r--   0 root         (0) root         (0)      168 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/.circleci/README
--rw-r--r--   0 root         (0) root         (0)     3102 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/.circleci/config.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.552064 airflow_mcd-0.1.7/.circleci/trufflehog_config/
--rw-r--r--   0 root         (0) root         (0)      377 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/.circleci/trufflehog_config/allowlist.json
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     1818 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/.gitignore
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1129 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/Makefile
--rw-r--r--   0 root         (0) root         (0)     7468 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/README-dev.md
--rw-r--r--   0 root         (0) root         (0)     6655 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.552064 airflow_mcd-0.1.7/airflow_mcd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/airflow_mcd/callbacks/
--rw-r--r--   0 root         (0) root         (0)     7042 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/callbacks/client.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/callbacks/mcd_callbacks.py
--rw-r--r--   0 root         (0) root         (0)     6336 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/airflow_mcd/hooks/
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2784 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/hooks/session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/airflow_mcd/operators/
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/operators/base_operator.py
--rw-r--r--   0 root         (0) root         (0)     3895 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/operators/circuit_breaker_operators.py
--rw-r--r--   0 root         (0) root         (0)    15407 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/operators/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.552064 airflow_mcd-0.1.7/airflow_mcd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7468 2023-07-24 21:15:55.000000 airflow_mcd-0.1.7/airflow_mcd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1137 2023-07-24 21:15:55.000000 airflow_mcd-0.1.7/airflow_mcd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 21:15:55.000000 airflow_mcd-0.1.7/airflow_mcd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-24 21:15:55.000000 airflow_mcd-0.1.7/airflow_mcd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-24 21:15:55.000000 airflow_mcd-0.1.7/airflow_mcd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/examples/
--rw-r--r--   0 root         (0) root         (0)     2050 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/examples/sample_circuit_dag.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/requirements-ci.txt
--rw-r--r--   0 root         (0) root         (0)      195 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1483 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/tests/callbacks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/callbacks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15028 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/callbacks/test_callbacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/tests/hooks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3780 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/hooks/test_session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/tests/operators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      719 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/operators/test_base_op.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/operators/test_circuit_breaker_op.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/operators/test_dbt_cli_config.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/operators/test_dbt_default_config_provider.py
--rw-r--r--   0 root         (0) root         (0)    21136 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/operators/test_dbt_operator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.105794 airflow_mcd-0.1.8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/.circleci/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/.circleci/README
+-rw-r--r--   0 root         (0) root         (0)     3102 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/.circleci/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/.circleci/trufflehog_config/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/.circleci/trufflehog_config/allowlist.json
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/Makefile
+-rw-r--r--   0 root         (0) root         (0)     9568 2023-07-26 16:15:43.105794 airflow_mcd-0.1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/README-dev.md
+-rw-r--r--   0 root         (0) root         (0)     8755 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/airflow_mcd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/airflow_mcd/callbacks/
+-rw-r--r--   0 root         (0) root         (0)     7042 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/callbacks/client.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/callbacks/mcd_callbacks.py
+-rw-r--r--   0 root         (0) root         (0)     6336 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/airflow_mcd/hooks/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2784 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/hooks/session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/airflow_mcd/operators/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/operators/base_operator.py
+-rw-r--r--   0 root         (0) root         (0)     3895 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/operators/circuit_breaker_operators.py
+-rw-r--r--   0 root         (0) root         (0)    15407 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/airflow_mcd/operators/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/airflow_mcd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9568 2023-07-26 16:15:43.000000 airflow_mcd-0.1.8/airflow_mcd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-07-26 16:15:43.000000 airflow_mcd-0.1.8/airflow_mcd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 16:15:43.000000 airflow_mcd-0.1.8/airflow_mcd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-26 16:15:43.000000 airflow_mcd-0.1.8/airflow_mcd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-26 16:15:43.000000 airflow_mcd-0.1.8/airflow_mcd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/examples/
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/examples/sample_circuit_dag.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/requirements-ci.txt
+-rw-r--r--   0 root         (0) root         (0)      195 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-26 16:15:43.105794 airflow_mcd-0.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/tests/callbacks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/callbacks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15028 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/callbacks/test_callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.101794 airflow_mcd-0.1.8/tests/hooks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/hooks/test_session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 16:15:43.105794 airflow_mcd-0.1.8/tests/operators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/operators/test_base_op.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/operators/test_circuit_breaker_op.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/operators/test_dbt_cli_config.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/operators/test_dbt_default_config_provider.py
+-rw-r--r--   0 root         (0) root         (0)    21136 2023-07-26 16:14:42.000000 airflow_mcd-0.1.8/tests/operators/test_dbt_operator.py
```

### Comparing `airflow_mcd-0.1.7/.circleci/config.yml` & `airflow_mcd-0.1.8/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/.gitignore` & `airflow_mcd-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/LICENSE` & `airflow_mcd-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/Makefile` & `airflow_mcd-0.1.8/Makefile`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/PKG-INFO` & `airflow_mcd-0.1.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: airflow_mcd
-Version: 0.1.7
-Summary: Monte Carlo's Apache Airflow Provider
-Home-page: https://www.montecarlodata.com/
-Author: Monte Carlo Data, Inc
-Author-email: info@montecarlodata.com
-License: Apache Software License (Apache 2.0)
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # airflow-mcd
 
 Monte Carlo's beta Airflow provider.
 
 ## Installation
 
 Requires Python 3.7 or greater and is compatible with Airflow 1.10.14 or greater.
@@ -175,20 +153,74 @@
         filtering down the query output to improve performance (e.g limit WHERE clause). If you expect a query to
         take the full 15 minutes we recommend padding the timeout to 20 minutes.
    - `fail_open` [default=True]: Prevent any errors or timeouts when executing a rule from stopping your pipeline.
         Raises `AirflowSkipException` if set to True and any issues are encountered. Recommended to set the 
        [trigger_rule](https://airflow.apache.org/docs/apache-airflow/stable/concepts/dags.html#trigger-rules)
         param for any downstream tasks to `none_failed` in this case.
 
+- **dbt Operators**
+  
+  The following suite of Airflow operators can be used to execute dbt commands. They include our [dbt Core](https://docs.getmontecarlo.com/docs/dbt-core) integration (via our [Python SDK](https://pypi.org/project/pycarlo/)), to automatically send dbt artifacts to Monte Carlo.
+    - `DbtBuildOperator`
+    - `DbtRunOperator`
+    - `DbtSeedOperator`
+    - `DbtSnapshotOperator`
+    - `DbtTestOperator`
+
+  Example of usage:
+  ```
+  from airflow_mcd.operators.dbt import DbtRunOperator
+
+  dbt_run = DbtRunOperator(
+      task_id='run-model',          # Airflow task id
+      project_name='some_project',  # name of project to associate dbt results
+      job_name='some_job',          # name of job to associate dbt results
+      models='some_model',          # dbt model selector
+      mc_conn_id='monte_carlo',     # id of Monte Carlo API connection configured in Airflow
+  )
+  ```
+  
+  Many more operator options are available. See the base `DbtOperator` for a comprehensive list.
+
+  ***Advanced Configuration***
+
+  To reduce repetitive configuration of the dbt operators, you can define a `DefaultConfigProvider` that would apply
+  configuration to every Monte Carlo dbt operator.
+
+  Example of usage:
+  ```
+  from airflow_mcd.operators.dbt import DefaultConfig, DefaultConfigProvider
+
+  class DefaultConfig(DefaultConfigProvider):
+    """
+    This default configuration will be applied to all Monte Carlo dbt operators.
+    Any property defined here can be overridden with arguments provided to an operator.
+    """
+    def config(self) -> DbtConfig:
+        return DbtConfig(
+            mc_conn_id='monte_carlo',
+            env={
+                'foo': 'bar',
+            }
+        )
+  ```
+  The location of this class should be provided in an environment variable:
+  ``` 
+  AIRFLOW_MCD_DBT_CONFIG_PROVIDER=configs.dbt.DefaultConfig
+  ```
+  
+  If you are using AWS Managed Apache Airflow (MWAA), the location of this class should be defined in a configuration
+  option in your Airflow environment:
+  ```
+  mc.airflow_mcd_dbt_config_provider=configs.dbt.DefaultConfig
+  ```
 ## Tests and releases
 
 Locally make test will run all tests. See [README-dev.md](README-dev.md) for additional details on development. When 
 ready for a review, create a PR against main.
 
 When ready to release, create a new Github release with a tag using semantic versioning (e.g. v0.42.0) and CircleCI will 
 test and publish to PyPI. Note that an existing version will not be deployed.
 
 ## License
 
 Apache 2.0 - See the [LICENSE](http://www.apache.org/licenses/LICENSE-2.0) for more information.
-
-
```

### Comparing `airflow_mcd-0.1.7/README-dev.md` & `airflow_mcd-0.1.8/README-dev.md`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/airflow_mcd/callbacks/client.py` & `airflow_mcd-0.1.8/airflow_mcd/callbacks/client.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/airflow_mcd/callbacks/mcd_callbacks.py` & `airflow_mcd-0.1.8/airflow_mcd/callbacks/mcd_callbacks.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/airflow_mcd/callbacks/utils.py` & `airflow_mcd-0.1.8/airflow_mcd/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/airflow_mcd/hooks/session_hook.py` & `airflow_mcd-0.1.8/airflow_mcd/hooks/session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/airflow_mcd/operators/base_operator.py` & `airflow_mcd-0.1.8/airflow_mcd/operators/base_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/airflow_mcd/operators/circuit_breaker_operators.py` & `airflow_mcd-0.1.8/airflow_mcd/operators/circuit_breaker_operators.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/airflow_mcd/operators/dbt.py` & `airflow_mcd-0.1.8/airflow_mcd/operators/dbt.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/airflow_mcd.egg-info/PKG-INFO` & `airflow_mcd-0.1.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: airflow-mcd
-Version: 0.1.7
+Name: airflow_mcd
+Version: 0.1.8
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -175,14 +175,70 @@
         filtering down the query output to improve performance (e.g limit WHERE clause). If you expect a query to
         take the full 15 minutes we recommend padding the timeout to 20 minutes.
    - `fail_open` [default=True]: Prevent any errors or timeouts when executing a rule from stopping your pipeline.
         Raises `AirflowSkipException` if set to True and any issues are encountered. Recommended to set the 
        [trigger_rule](https://airflow.apache.org/docs/apache-airflow/stable/concepts/dags.html#trigger-rules)
         param for any downstream tasks to `none_failed` in this case.
 
+- **dbt Operators**
+  
+  The following suite of Airflow operators can be used to execute dbt commands. They include our [dbt Core](https://docs.getmontecarlo.com/docs/dbt-core) integration (via our [Python SDK](https://pypi.org/project/pycarlo/)), to automatically send dbt artifacts to Monte Carlo.
+    - `DbtBuildOperator`
+    - `DbtRunOperator`
+    - `DbtSeedOperator`
+    - `DbtSnapshotOperator`
+    - `DbtTestOperator`
+
+  Example of usage:
+  ```
+  from airflow_mcd.operators.dbt import DbtRunOperator
+
+  dbt_run = DbtRunOperator(
+      task_id='run-model',          # Airflow task id
+      project_name='some_project',  # name of project to associate dbt results
+      job_name='some_job',          # name of job to associate dbt results
+      models='some_model',          # dbt model selector
+      mc_conn_id='monte_carlo',     # id of Monte Carlo API connection configured in Airflow
+  )
+  ```
+  
+  Many more operator options are available. See the base `DbtOperator` for a comprehensive list.
+
+  ***Advanced Configuration***
+
+  To reduce repetitive configuration of the dbt operators, you can define a `DefaultConfigProvider` that would apply
+  configuration to every Monte Carlo dbt operator.
+
+  Example of usage:
+  ```
+  from airflow_mcd.operators.dbt import DefaultConfig, DefaultConfigProvider
+
+  class DefaultConfig(DefaultConfigProvider):
+    """
+    This default configuration will be applied to all Monte Carlo dbt operators.
+    Any property defined here can be overridden with arguments provided to an operator.
+    """
+    def config(self) -> DbtConfig:
+        return DbtConfig(
+            mc_conn_id='monte_carlo',
+            env={
+                'foo': 'bar',
+            }
+        )
+  ```
+  The location of this class should be provided in an environment variable:
+  ``` 
+  AIRFLOW_MCD_DBT_CONFIG_PROVIDER=configs.dbt.DefaultConfig
+  ```
+  
+  If you are using AWS Managed Apache Airflow (MWAA), the location of this class should be defined in a configuration
+  option in your Airflow environment:
+  ```
+  mc.airflow_mcd_dbt_config_provider=configs.dbt.DefaultConfig
+  ```
 ## Tests and releases
 
 Locally make test will run all tests. See [README-dev.md](README-dev.md) for additional details on development. When 
 ready for a review, create a PR against main.
 
 When ready to release, create a new Github release with a tag using semantic versioning (e.g. v0.42.0) and CircleCI will 
 test and publish to PyPI. Note that an existing version will not be deployed.
```

### Comparing `airflow_mcd-0.1.7/airflow_mcd.egg-info/SOURCES.txt` & `airflow_mcd-0.1.8/airflow_mcd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/examples/sample_circuit_dag.py` & `airflow_mcd-0.1.8/examples/sample_circuit_dag.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/setup.py` & `airflow_mcd-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/tests/callbacks/test_callbacks.py` & `airflow_mcd-0.1.8/tests/callbacks/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/tests/hooks/test_session_hook.py` & `airflow_mcd-0.1.8/tests/hooks/test_session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/tests/operators/test_base_op.py` & `airflow_mcd-0.1.8/tests/operators/test_base_op.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/tests/operators/test_circuit_breaker_op.py` & `airflow_mcd-0.1.8/tests/operators/test_circuit_breaker_op.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/tests/operators/test_dbt_cli_config.py` & `airflow_mcd-0.1.8/tests/operators/test_dbt_cli_config.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/tests/operators/test_dbt_default_config_provider.py` & `airflow_mcd-0.1.8/tests/operators/test_dbt_default_config_provider.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.7/tests/operators/test_dbt_operator.py` & `airflow_mcd-0.1.8/tests/operators/test_dbt_operator.py`

 * *Files identical despite different names*

