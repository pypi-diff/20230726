# Comparing `tmp/astronomer_cosmos-0.7.5.tar.gz` & `tmp/astronomer_cosmos-1.0.0.tar.gz`

## Comparing `astronomer_cosmos-0.7.5.tar` & `astronomer_cosmos-1.0.0.tar`

### file list

```diff
@@ -1,49 +1,59 @@
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/__init__.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/constants.py
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/dag.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/dataset.py
--rw-r--r--   0        0        0    11460 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/render.py
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/core/__init__.py
--rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/dbt/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/dbt/parser/__init__.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/dbt/parser/output.py
--rw-r--r--   0        0        0    11165 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/dbt/parser/project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/hooks/__init__.py
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/hooks/subprocess.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/operators/__init__.py
--rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/operators/base.py
--rw-r--r--   0        0        0     5057 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/operators/docker.py
--rw-r--r--   0        0        0     5462 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/operators/kubernetes.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/operators/lazy_load.py
--rw-r--r--   0        0        0    19892 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/operators/local.py
--rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/operators/virtualenv.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/__init__.py
--rw-r--r--   0        0        0     5525 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/base.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/bigquery/__init__.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/bigquery/service_account_file.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/databricks/__init__.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/databricks/token.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/exasol/__init__.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/exasol/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/postgres/__init__.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/postgres/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/redshift/__init__.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/redshift/user_pass.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/snowflake/__init__.py
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/snowflake/user_pass.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/spark/__init__.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/spark/thrift.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/trino/__init__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/trino/base.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/trino/certificate.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/trino/jwt.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/trino/ldap.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/LICENSE
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/README.rst
--rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     7004 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/__init__.py
+-rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/config.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/constants.py
+-rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/converter.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dataset.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/airflow/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/airflow/dag.py
+-rw-r--r--   0        0        0     9952 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/airflow/graph.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/airflow/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dbt/__init__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dbt/executable.py
+-rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dbt/graph.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dbt/project.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dbt/selector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dbt/parser/__init__.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dbt/parser/output.py
+-rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dbt/parser/project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/hooks/__init__.py
+-rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/hooks/subprocess.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/operators/__init__.py
+-rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/operators/base.py
+-rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/operators/docker.py
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/operators/kubernetes.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/operators/lazy_load.py
+-rw-r--r--   0        0        0    18067 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/operators/local.py
+-rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/operators/virtualenv.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/__init__.py
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/base.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/bigquery/__init__.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/bigquery/service_account_file.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/bigquery/service_account_keyfile_dict.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/databricks/__init__.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/databricks/token.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/exasol/__init__.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/exasol/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/postgres/__init__.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/postgres/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/redshift/__init__.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/redshift/user_pass.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/snowflake/__init__.py
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/snowflake/user_pass.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/snowflake/user_privatekey.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/spark/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/spark/thrift.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/trino/__init__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/trino/base.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/trino/certificate.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/trino/jwt.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/trino/ldap.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/README.rst
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7004 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/PKG-INFO
```

### Comparing `astronomer_cosmos-0.7.5/cosmos/__init__.py` & `astronomer_cosmos-1.0.0/cosmos/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+# type: ignore # ignores "Cannot assign to a type" MyPy error
+
 """
 Astronomer Cosmos is a library for rendering dbt workflows in Airflow.
 
 Contains dags, task groups, and operators.
 """
+__version__ = "1.0.0"
 
-__version__ = "0.7.5"
-
+from cosmos.airflow.dag import DbtDag
+from cosmos.airflow.task_group import DbtTaskGroup
+from cosmos.constants import LoadMode, TestBehavior, ExecutionMode
 from cosmos.dataset import get_dbt_dataset
+from cosmos.operators.lazy_load import MissingPackage
+from cosmos.config import (
+    ProjectConfig,
+    ProfileConfig,
+    ExecutionConfig,
+    RenderConfig,
+)
 
-# re-export the dag and task group
-from cosmos.dag import DbtDag
-from cosmos.task_group import DbtTaskGroup
-
-# re-export the operators
 from cosmos.operators.local import (
     DbtDepsLocalOperator,
     DbtLSLocalOperator,
     DbtRunLocalOperator,
     DbtRunOperationLocalOperator,
     DbtSeedLocalOperator,
     DbtSnapshotLocalOperator,
@@ -29,16 +35,14 @@
         DbtRunDockerOperator,
         DbtRunOperationDockerOperator,
         DbtSeedDockerOperator,
         DbtSnapshotDockerOperator,
         DbtTestDockerOperator,
     )
 except ImportError:
-    from cosmos.operators.lazy_load import MissingPackage
-
     DbtLSDockerOperator = MissingPackage("cosmos.operators.docker.DbtLSDockerOperator", "docker")
     DbtRunDockerOperator = MissingPackage("cosmos.operators.docker.DbtRunDockerOperator", "docker")
     DbtRunOperationDockerOperator = MissingPackage(
         "cosmos.operators.docker.DbtRunOperationDockerOperator",
         "docker",
     )
     DbtSeedDockerOperator = MissingPackage("cosmos.operators.docker.DbtSeedDockerOperator", "docker")
@@ -51,16 +55,14 @@
         DbtRunKubernetesOperator,
         DbtRunOperationKubernetesOperator,
         DbtSeedKubernetesOperator,
         DbtSnapshotKubernetesOperator,
         DbtTestKubernetesOperator,
     )
 except ImportError:
-    from cosmos.operators.lazy_load import MissingPackage
-
     DbtLSKubernetesOperator = MissingPackage(
         "cosmos.operators.kubernetes.DbtLSKubernetesOperator",
         "kubernetes",
     )
     DbtRunKubernetesOperator = MissingPackage(
         "cosmos.operators.kubernetes.DbtRunKubernetesOperator",
         "kubernetes",
@@ -79,14 +81,18 @@
     )
     DbtTestKubernetesOperator = MissingPackage(
         "cosmos.operators.kubernetes.DbtTestKubernetesOperator",
         "kubernetes",
     )
 
 __all__ = [
+    "ProjectConfig",
+    "ProfileConfig",
+    "ExecutionConfig",
+    "RenderConfig",
     "DbtLSLocalOperator",
     "DbtRunOperationLocalOperator",
     "DbtRunLocalOperator",
     "DbtSeedLocalOperator",
     "DbtTestLocalOperator",
     "DbtDepsLocalOperator",
     "DbtSnapshotLocalOperator",
@@ -101,8 +107,11 @@
     "DbtSnapshotDockerOperator",
     "DbtLSKubernetesOperator",
     "DbtRunOperationKubernetesOperator",
     "DbtRunKubernetesOperator",
     "DbtSeedKubernetesOperator",
     "DbtTestKubernetesOperator",
     "DbtSnapshotKubernetesOperator",
+    "ExecutionMode",
+    "LoadMode",
+    "TestBehavior",
 ]
```

### Comparing `astronomer_cosmos-0.7.5/cosmos/render.py` & `astronomer_cosmos-1.0.0/cosmos/dbt/parser/project.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,277 +1,360 @@
 """
-This module contains a function to render a dbt project into Cosmos entities.
+Used to parse and extract information from dbt projects.
 """
 from __future__ import annotations
 
-import itertools
 import logging
+import os
+import ast
 
-try:
-    from typing import Literal
-except ImportError:
-    from typing_extensions import Literal
-
-from typing import Any, Callable, Dict, List, Optional
-
-from airflow.exceptions import AirflowException
-
-from cosmos.core.graph.entities import CosmosEntity, Group, Task
-from cosmos.dataset import get_dbt_dataset
-from cosmos.dbt.parser.project import DbtModelType, DbtProject
+from dataclasses import dataclass, field
+from enum import Enum
+from pathlib import Path
+from typing import Any, ClassVar, Dict, List, Set
+
+import jinja2
+import yaml
 
 logger = logging.getLogger(__name__)
 
 
-def calculate_operator_class(
-    execution_mode: str,
-    dbt_class: str,
-) -> str:
-    "Given an execution mode and dbt class, return the operator class to use"
-    return f"cosmos.operators.{execution_mode}.{dbt_class}{execution_mode.capitalize()}Operator"
-
-
-def render_project(
-    dbt_project_name: str,
-    dbt_root_path: str = "/usr/local/airflow/dags/dbt",
-    dbt_models_dir: str = "models",
-    dbt_snapshots_dir: str = "snapshots",
-    dbt_seeds_dir: str = "seeds",
-    task_args: Dict[str, Any] = {},
-    operator_args: Dict[str, Any] = {},
-    test_behavior: Literal["none", "after_each", "after_all"] = "after_each",
-    emit_datasets: bool = True,
-    conn_id: str = "default_conn_id",
-    profile_args: Dict[str, str] = {},
-    profile_name: str | None = None,
-    target_name: str | None = None,
-    select: Dict[str, List[str]] = {},
-    exclude: Dict[str, List[str]] = {},
-    execution_mode: Literal["local", "docker", "kubernetes"] = "local",
-    on_warning_callback: Optional[Callable] = None,
-) -> Group:
+DBT_PY_MODEL_METHOD_NAME = "model"
+DBT_PY_DEP_METHOD_NAME = "ref"
+PYTHON_FILE_SUFFIX = ".py"
+
+
+class DbtModelType(Enum):
     """
-    Turn a dbt project into a Group
+    Represents type of dbt unit (model, snapshot, seed)
+    """
+
+    DBT_MODEL = "model"
+    DBT_SNAPSHOT = "snapshot"
+    DBT_SEED = "seed"
+
 
-    :param dbt_project_name: The name of the dbt project
-    :param dbt_root_path: The root path to your dbt folder. Defaults to /usr/local/airflow/dags/dbt
-    :param task_args: Arguments to pass to the underlying dbt operators
-    :param operator_args: Parameters to pass to the underlying operators, can include KubernetesPodOperator
-        or DockerOperator parameters
-    :param test_behavior: The behavior for running tests. Options are "none", "after_each", and "after_all".
-        Defaults to "after_each"
-    :param emit_datasets: If enabled test nodes emit Airflow Datasets for downstream cross-DAG dependencies
-    :param conn_id: The Airflow connection ID to use
-    :param profile_args: Arguments to pass to the dbt profile
-    :param profile_name: A name to use for the dbt profile. If not provided, and no profile target is found
-        in your project's dbt_project.yml, "cosmos_profile" is used.
-    :param target_name: A name to use for the dbt target. If not provided, "cosmos_target" is used.
-    :param select: A dict of dbt selector arguments (i.e., {"tags": ["tag_1", "tag_2"]})
-    :param exclude: A dict of dbt exclude arguments (i.e., {"tags": ["tag_1", "tag_2]}})
-    :param execution_mode: The execution mode in which the dbt project should be run.
-        Options are "local", "docker", and "kubernetes".
-        Defaults to "local"
-     :param on_warning_callback: A callback function called on warnings with additional Context variables "test_names"
-        and "test_results" of type `List`. Each index in "test_names" corresponds to the same index in "test_results".
+@dataclass
+class DbtModelConfig:
+    """
+    Represents a single model config.
     """
-    # first, get the dbt project
-    project = DbtProject(
-        dbt_root_path=dbt_root_path,
-        dbt_models_dir=dbt_models_dir,
-        dbt_snapshots_dir=dbt_snapshots_dir,
-        dbt_seeds_dir=dbt_seeds_dir,
-        project_name=dbt_project_name,
-    )
-
-    # this is the group that will be returned
-    base_group = Group(id=dbt_project_name)
-    entities: Dict[str, CosmosEntity] = {}  # this is a dict of all the entities we create
-
-    # add project_dir arg to task_args
-    if execution_mode == "local":
-        task_args["project_dir"] = project.project_dir
-
-    # ensures the same tag isn't in select & exclude
-    if "tags" in select and "tags" in exclude:
-        if set(select["tags"]).intersection(exclude["tags"]):
-            raise AirflowException(
-                f"Can't specify the same tag in `select` and `include`: "
-                f"{set(select['tags']).intersection(exclude['tags'])}"
-            )
 
-    if "paths" in select and "paths" in exclude:
-        if set(select["paths"]).intersection(exclude["paths"]):
-            raise AirflowException(
-                f"Can't specify the same path in `select` and `include`: "
-                f"{set(select['paths']).intersection(exclude['paths'])}"
-            )
+    config_types: ClassVar[List[str]] = ["materialized", "schema", "tags"]
+    config_selectors: Set[str] = field(default_factory=set)
+    upstream_models: Set[str] = field(default_factory=set)
+
+    def __add__(self, other_config: DbtModelConfig) -> DbtModelConfig:
+        """
+        Add one config to another. Necessary because configs can come from different places
+        """
+        # ensures proper order of operations between sql models and properties.yml
+        result = self._config_selector_ooo(
+            sql_configs=self.config_selectors,
+            properties_configs=other_config.config_selectors,
+        )
 
-    # if task_args has a schema, add it to the profile args and add a deprecated warning
-    if "schema" in task_args:
-        profile_args["schema"] = task_args["schema"]
-        logger.warning("Specifying a schema in the task_args is deprecated. Please use the profile_args instead.")
-
-    # iterate over each model once to create the initial tasks
-    for model_name, model in itertools.chain(project.models.items(), project.snapshots.items(), project.seeds.items()):
-        # filters down to a path within the project_dir
-        if "paths" in select:
-            root_directories = [project.project_dir / path.strip("/") for path in select.get("paths", [])]
-            if not set(root_directories).intersection(model.path.parents):
-                continue
+        # get the unique combination of each list
+        return DbtModelConfig(
+            config_selectors=result,
+            upstream_models=self.upstream_models | other_config.upstream_models,
+        )
 
-        # filters out any specified paths
-        if "paths" in exclude:
-            root_directories = [project.project_dir / path.strip("/") for path in exclude.get("paths")]
-            if set(root_directories).intersection(model.path.parents):
-                continue
+    def _config_selector_ooo(
+        self,
+        sql_configs: Set[str],
+        properties_configs: Set[str],
+        prefixes: List[str] | None = None,
+    ) -> Set[str]:
+        """
+        this will force values from the sql files to override whatever is in the properties.yml. So ooo:
+        # 1. model sql files
+        # 2. properties.yml files
+        """
+
+        # iterate on each properties.yml config
+        # excluding tags because we just want to collect all of them
+        if prefixes is None:
+            prefixes = ["materialized", "schema"]
+
+        for config in properties_configs:
+            # identify the config_type and its associated value (i.e. materialized:table)
+            config_type, value = config.split(":")
+            # if the config_type matches is even in a list of prefixes then
+            if config_type in prefixes:
+                # make sure that it's prefix doesn't already exist in the sql configs
+                if not any([element.startswith(config_type) for element in sql_configs]):
+                    # if it does let's double-check against each prefix and add it
+                    for prefix in prefixes:
+                        # if the actual config doesn't exist in the sql_configs then add it
+                        if not any([element.startswith(prefix) for element in sql_configs]):
+                            sql_configs.add(config)
+            else:
+                sql_configs.add(config)
 
-        if "configs" in select:
-            # TODO: coverme
-            if not set(select["configs"]).intersection(model.config.config_selectors):
-                continue
+        return sql_configs
 
-        if "configs" in exclude:
-            # TODO: coverme
-            if set(exclude["configs"]).intersection(model.config.config_selectors):
-                continue
 
-        run_args: Dict[str, Any] = {
-            **task_args,
-            **operator_args,
-            "models": model_name,
-            "profile_args": profile_args,
-            "profile_name": profile_name,
-            "target_name": target_name,
-        }
-        test_args: Dict[str, Any] = {
-            **task_args,
-            **operator_args,
-            "models": model_name,
-            "profile_args": profile_args,
-            "profile_name": profile_name,
-            "target_name": target_name,
-        }
-        # DbtTestOperator specific arg
-        test_args["on_warning_callback"] = on_warning_callback
-        if emit_datasets:
-            outlets = [get_dbt_dataset(conn_id, dbt_project_name, model_name)]
+def extract_python_file_upstream_requirements(code: str) -> list[str]:
+    """
+    Given a dbt Python model source code, identify other dbt entities which are upstream requirements.
 
-            if test_behavior == "after_each":
-                test_args["outlets"] = outlets
-            else:
-                # TODO: coverme
-                run_args["outlets"] = outlets
+    This method tries to find a `model` function and `dbt.ref` calls within it. Return a list of upstream entities IDs.
+    """
+    source_code = ast.parse(code)
 
-        if model.type == DbtModelType.DBT_MODEL:
-            # make the run task for model
-            run_task = Task(
-                id=f"{model_name}_run",
-                operator_class=calculate_operator_class(
-                    execution_mode=execution_mode,
-                    dbt_class="DbtRun",
-                ),
-                arguments=run_args,
-            )
-        elif model.type == DbtModelType.DBT_SNAPSHOT:
-            # make the run task for snapshot
-            run_task = Task(
-                id=f"{model_name}_snapshot",
-                operator_class=calculate_operator_class(
-                    execution_mode=execution_mode,
-                    dbt_class="DbtSnapshot",
-                ),
-                arguments=run_args,
-            )
-        elif model.type == DbtModelType.DBT_SEED:
-            # make the run task for snapshot
-            run_task = Task(
-                id=f"{model_name}_seed",
-                operator_class=calculate_operator_class(
-                    execution_mode=execution_mode,
-                    dbt_class="DbtSeed",
-                ),
-                arguments=run_args,
-            )
-        else:
-            # TODO: coverme
-            logger.error("Unknown dbt type.")
-            continue
-
-        # if test_behavior isn't "after_each", we can just add the task to the
-        # base group and do nothing else for now
-        if test_behavior != "after_each":
-            entities[model_name] = run_task
-            base_group.add_entity(entity=run_task)
-            continue
-
-        # otherwise, we need to make a test task after run tasks and turn them into a group
-        entities[run_task.id] = run_task
-
-        if model.type == DbtModelType.DBT_MODEL:
-            test_task = Task(
-                id=f"{model_name}_test",
-                operator_class=calculate_operator_class(
-                    execution_mode=execution_mode,
-                    dbt_class="DbtTest",
-                ),
-                upstream_entity_ids=[run_task.id],
-                arguments=test_args,
-            )
-            entities[test_task.id] = test_task
-            # make the group
-            model_group = Group(
-                id=f"{model_name}",
-                entities=[run_task, test_task],
-            )
-            entities[model_group.id] = model_group
-            base_group.add_entity(entity=model_group)
+    upstream_entities = []
+    model_function = None
+    for node in source_code.body:
+        if isinstance(node, ast.FunctionDef) and node.name == DBT_PY_MODEL_METHOD_NAME:
+            model_function = node
+            break
+
+    if model_function:
+        for item in ast.walk(model_function):
+            if isinstance(item, ast.Call) and item.func.attr == DBT_PY_DEP_METHOD_NAME:  # type: ignore[attr-defined]
+                upstream_entity_id = hasattr(item.args[-1], "value") and item.args[-1].value
+                if upstream_entity_id:
+                    upstream_entities.append(upstream_entity_id)
 
-        # all other non-run tasks don't need to be grouped with test tasks
-        else:
-            entities[model_name] = run_task
-            base_group.add_entity(entity=run_task)
+    return upstream_entities
 
-    # add dependencies now that we have all the entities
-    for model_name, model in itertools.chain(project.models.items(), project.snapshots.items(), project.seeds.items()):
-        upstream_deps = model.config.upstream_models
-        for upstream_model_name in upstream_deps:
+
+@dataclass
+class DbtModel:
+    """
+    Represents a single dbt model. (This class also hold snapshots)
+    """
+
+    # instance variables
+    name: str
+    type: DbtModelType
+    path: Path
+    config: DbtModelConfig = field(default_factory=DbtModelConfig)
+
+    def __post_init__(self) -> None:
+        """
+        Parses the file and extracts metadata (dependencies, tags, etc)
+        """
+        # first, get an empty config
+        config = DbtModelConfig()
+
+        if self.type == DbtModelType.DBT_MODEL:
+            # get the code from the file
+            code = self.path.read_text()
+
+        # we remove first and last line if the code is a snapshot
+        elif self.type == DbtModelType.DBT_SNAPSHOT:
+            code = self.path.read_text()
+            snapshot_name = code.split("{%")[1]
+            snapshot_name = snapshot_name.split("%}")[0]
+            snapshot_name = snapshot_name.split(" ")[2]
+            snapshot_name = snapshot_name.strip()
+            self.name = snapshot_name
+            code = code.split("%}")[1]
+            code = code.split("{%")[0]
+
+        elif self.type == DbtModelType.DBT_SEED:
+            code = ""
+
+        if self.path.suffix == PYTHON_FILE_SUFFIX:
+            config.upstream_models = config.upstream_models.union(set(extract_python_file_upstream_requirements(code)))
+        else:
+            # get the dependencies
+            env = jinja2.Environment()
+            jinja2_ast = env.parse(code)
+            # iterate over the jinja nodes to extract info
+            for base_node in jinja2_ast.find_all(jinja2.nodes.Call):
+                if hasattr(base_node.node, "name"):
+                    # check we have a ref - this indicates a dependency
+                    if base_node.node.name == "ref":
+                        # if it is, get the first argument
+                        first_arg = base_node.args[0]
+                        if isinstance(first_arg, jinja2.nodes.Const):
+                            # and add it to the config
+                            config.upstream_models.add(first_arg.value)
+
+                    # check if we have a config - this could contain tags
+                    if base_node.node.name == "config":
+                        # if it is, check if any kwargs are tags
+                        for kwarg in base_node.kwargs:
+                            for selector in self.config.config_types:
+                                extracted_config = self._extract_config(kwarg=kwarg, config_name=selector)
+                                config.config_selectors |= (
+                                    set(extracted_config) if isinstance(extracted_config, (str, List)) else set()
+                                )
+
+        # set the config and set the parsed file flag to true
+        self.config = config
+
+    # TODO following needs coverage:
+    def _extract_config(self, kwarg: Any, config_name: str) -> Any:
+        if hasattr(kwarg, "key") and kwarg.key == config_name:
             try:
-                dep_task = entities[upstream_model_name]
-                entities[model_name].add_upstream(dep_task)
-            except KeyError:
-                logger.error(f"Dependency {upstream_model_name} not found for model {model}")
-    if test_behavior == "after_all":
-        # make a test task
-        test_task = Task(
-            id=f"{dbt_project_name}_test",
-            operator_class=calculate_operator_class(
-                execution_mode=execution_mode,
-                dbt_class="DbtTest",
-            ),
-            arguments={**task_args, **operator_args},
+                # try to convert it to a constant and get the value
+                value = kwarg.value.as_const()
+                if isinstance(value, List):
+                    value = [f"{config_name}:{item}" for item in value]
+
+                if isinstance(value, str):
+                    value = [f"{config_name}:{value}"]
+
+                return value
+
+            except Exception as e:
+                # if we can't convert it to a constant, we can't do anything with it
+                logger.warning(f"Could not parse {config_name} from config in {self.path}: {e}")
+                pass
+
+    def __repr__(self) -> str:
+        """
+        Returns the string representation of the model.
+        """
+        return f"DbtModel(name='{self.name}', type='{self.type}', path='{self.path}', config={self.config})"
+
+
+@dataclass
+class DbtProject:
+    """
+    Represents a single dbt project.
+    """
+
+    # required, user-specified instance variables
+    project_name: str
+
+    # optional, user-specified instance variables
+    dbt_root_path: str | None = None
+    dbt_models_dir: str | None = None
+    dbt_snapshots_dir: str | None = None
+    dbt_seeds_dir: str | None = None
+
+    # private instance variables for managing state
+    models: Dict[str, DbtModel] = field(default_factory=dict)
+    snapshots: Dict[str, DbtModel] = field(default_factory=dict)
+    seeds: Dict[str, DbtModel] = field(default_factory=dict)
+    project_dir: Path = field(init=False)
+    models_dir: Path = field(init=False)
+    snapshots_dir: Path = field(init=False)
+    seeds_dir: Path = field(init=False)
+
+    def __post_init__(self) -> None:
+        """
+        Initializes the parser.
+        """
+        if self.dbt_root_path is None:
+            self.dbt_root_path = "/usr/local/airflow/dags/dbt"
+        if self.dbt_models_dir is None:
+            self.dbt_models_dir = "models"
+        if self.dbt_snapshots_dir is None:
+            self.dbt_snapshots_dir = "snapshots"
+        if self.dbt_seeds_dir is None:
+            self.dbt_seeds_dir = "seeds"
+
+        # set the project and model dirs
+        self.project_dir = Path(os.path.join(self.dbt_root_path, self.project_name))
+        self.models_dir = self.project_dir / self.dbt_models_dir
+        self.snapshots_dir = self.project_dir / self.dbt_snapshots_dir
+        self.seeds_dir = self.project_dir / self.dbt_seeds_dir
+
+        # crawl the models in the project
+        for file_name in self.models_dir.rglob("*.sql"):
+            self._handle_sql_file(file_name)
+
+        # crawl the models in the project
+        for file_name in self.models_dir.rglob("*.py"):
+            self._handle_sql_file(file_name)
+
+        # crawl the snapshots in the project
+        for file_name in self.snapshots_dir.rglob("*.sql"):
+            self._handle_sql_file(file_name)
+
+        # crawl the seeds in the project
+        for file_name in self.seeds_dir.rglob("*.csv"):
+            self._handle_csv_file(file_name)
+
+        # crawl the config files in the project
+        for file_name in self.models_dir.rglob("*.yml"):
+            self._handle_config_file(file_name)
+
+    def _handle_csv_file(self, path: Path) -> None:
+        """
+        Handles a single sql file.
+        """
+        # get the model name
+        model_name = path.stem
+
+        # construct the model object, which we'll use to store metadata
+        model = DbtModel(
+            name=model_name,
+            type=DbtModelType.DBT_SEED,
+            path=path,
         )
-        entities[test_task.id] = test_task
+        # add the model to the project
+        self.seeds[model_name] = model
 
-        # add it to the base group
-        base_group.add_entity(test_task)
+    def _handle_sql_file(self, path: Path) -> None:
+        """
+        Handles a single sql file.
+        """
+        # get the model name
+        model_name = path.stem
+
+        # construct the model object, which we'll use to store metadata
+        if str(self.models_dir) in str(path):
+            model = DbtModel(
+                name=model_name,
+                type=DbtModelType.DBT_MODEL,
+                path=path,
+            )
+            # add the model to the project
+            self.models[model.name] = model
 
-        # add it as an upstream to all the models that don't have downstream tasks
-        # since we don't have downstream info readily available, we have to iterate
-        # start with all models, and remove them as we find downstream tasks
-        models_with_no_downstream_tasks = [model_name for model_name, model in project.models.items()]
-
-        # iterate over all models
-        for model_name, model in project.models.items():
-            # iterate over all upstream models
-            for upstream_model_name in model.config.upstream_models:
-                # remove the upstream model from the list of models with no downstream tasks
-                try:
-                    models_with_no_downstream_tasks.remove(upstream_model_name)
-                except ValueError:
-                    pass
-
-        # add the test task as an upstream to all models with no downstream tasks
-        for model_name in models_with_no_downstream_tasks:
-            if model_name in entities:
-                test_task.add_upstream(entity=entities[model_name])
+        elif str(self.snapshots_dir) in str(path):
+            model = DbtModel(
+                name=model_name,
+                type=DbtModelType.DBT_SNAPSHOT,
+                path=path,
+            )
+            # add the snapshot to the project
+            self.snapshots[model.name] = model
+
+    def _handle_config_file(self, path: Path) -> None:
+        """
+        Handles a single config file.
+        """
+        # parse the yml file
+        config_dict = yaml.safe_load(path.read_text())
+
+        # iterate over the models in the config
+        if not (config_dict and config_dict.get("models")):
+            return
+
+        for model in config_dict["models"]:
+            model_name = model.get("name")
+
+            # if the model doesn't exist, we can't do anything
+            if model_name not in self.models:
+                continue
 
-    return base_group
+            # config_selectors
+            config_selectors = []
+            for selector in self.models[model_name].config.config_types:
+                config_value = model.get("config", {}).get(selector)
+                if config_value:
+                    if isinstance(config_value, str):
+                        config_selectors.append(f"{selector}:{config_value}")
+                    else:
+                        for item in config_value:
+                            if item:
+                                config_selectors.append(f"{selector}:{item}")
+
+            # dbt default ensures "materialized:view" is set for all models if nothing is specified so that it will
+            # work in a select/exclude list
+            config_types = [
+                selector_name for selector in config_selectors for selector_name in [selector.split(":")[0]]
+            ]
+            if "materialized" not in config_types:
+                config_selectors.append("materialized:view")
+
+            # then, get the model and merge the configs
+            model = self.models[model_name]
+            model.config = model.config + DbtModelConfig(config_selectors=set(config_selectors))
```

### Comparing `astronomer_cosmos-0.7.5/cosmos/core/graph/entities.py` & `astronomer_cosmos-1.0.0/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.5/cosmos/dbt/parser/output.py` & `astronomer_cosmos-1.0.0/cosmos/dbt/parser/output.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.5/cosmos/hooks/subprocess.py` & `astronomer_cosmos-1.0.0/cosmos/hooks/subprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 # stdout or stderr. This option proves to be highly beneficial for any text analysis that depends on the stdout or
 # stderr output of a dbt command.
 from __future__ import annotations
 
 import contextlib
 import os
 import signal
-from collections import namedtuple
+from typing import NamedTuple
 from subprocess import PIPE, STDOUT, Popen
 from tempfile import TemporaryDirectory, gettempdir
 
 from airflow.hooks.base import BaseHook
 
-FullOutputSubprocessResult = namedtuple("FullOutputSubprocessResult", ["exit_code", "output", "full_output"])
 
+class FullOutputSubprocessResult(NamedTuple):
+    exit_code: int
+    output: str
+    full_output: list[str]
 
-class FullOutputSubprocessHook(BaseHook):
+
+class FullOutputSubprocessHook(BaseHook):  # type: ignore[misc] # ignores subclass MyPy error
     """Hook for running processes with the ``subprocess`` module."""
 
     def __init__(self) -> None:
         self.sub_process: Popen[bytes] | None = None
         super().__init__()
 
     def run_command(
@@ -52,15 +56,15 @@
         """
         self.log.info("Tmp dir root location: \n %s", gettempdir())
         log_lines = []
         with contextlib.ExitStack() as stack:
             if cwd is None:
                 cwd = stack.enter_context(TemporaryDirectory(prefix="airflowtmp"))
 
-            def pre_exec():
+            def pre_exec() -> None:
                 # Restore default signal disposition and invoke setsid
                 for sig in ("SIGPIPE", "SIGXFZ", "SIGXFSZ"):
                     if hasattr(signal, sig):
                         signal.signal(getattr(signal, sig), signal.SIG_DFL)
                 os.setsid()
 
             self.log.info("Running command: %s", command)
@@ -89,12 +93,12 @@
             self.sub_process.wait()
 
             self.log.info("Command exited with return code %s", self.sub_process.returncode)
             return_code: int = self.sub_process.returncode
 
         return FullOutputSubprocessResult(exit_code=return_code, output=line, full_output=log_lines)
 
-    def send_sigterm(self):
+    def send_sigterm(self) -> None:
         """Sends SIGTERM signal to ``self.sub_process`` if one exists."""
         self.log.info("Sending SIGTERM signal to process group")
         if self.sub_process and hasattr(self.sub_process, "pid"):
             os.killpg(os.getpgid(self.sub_process.pid), signal.SIGTERM)
```

### Comparing `astronomer_cosmos-0.7.5/cosmos/operators/__init__.py` & `astronomer_cosmos-1.0.0/cosmos/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.5/cosmos/operators/base.py` & `astronomer_cosmos-1.0.0/cosmos/operators/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from airflow.models.baseoperator import BaseOperator
 from airflow.utils.context import Context
 from airflow.utils.operator_helpers import context_to_airflow_vars
 
 logger = logging.getLogger(__name__)
 
 
-class DbtBaseOperator(BaseOperator):
+class DbtBaseOperator(BaseOperator):  # type: ignore[misc] # ignores subclass MyPy error
     """
     Executes a dbt core cli command.
 
     :param project_dir: Which directory to look in for the dbt_project.yml file. Default is the current working
     directory and its parents.
     :param conn_id: The airflow connection to use as the target
     :param base_cmd: dbt sub-command to run (i.e ls, seed, run, test, etc.)
@@ -73,36 +73,36 @@
     )
 
     intercept_flag = True
 
     def __init__(
         self,
         project_dir: str,
-        conn_id: str,
-        base_cmd: str | list[str] = None,
-        select: str = None,
-        exclude: str = None,
-        selector: str = None,
-        vars: dict = None,
-        models: str = None,
+        conn_id: str | None = None,
+        base_cmd: list[str] | None = None,
+        select: str | None = None,
+        exclude: str | None = None,
+        selector: str | None = None,
+        vars: dict[str, str] | None = None,
+        models: str | None = None,
         cache_selected_only: bool = False,
         no_version_check: bool = False,
         fail_fast: bool = False,
         quiet: bool = False,
         warn_error: bool = False,
-        db_name: str = None,
-        schema: str = None,
-        env: dict = None,
+        db_name: str | None = None,
+        schema: str | None = None,
+        env: dict[str, Any] | None = None,
         append_env: bool = False,
         output_encoding: str = "utf-8",
         skip_exit_code: int = 99,
         cancel_query_on_kill: bool = True,
         dbt_executable_path: str = "dbt",
-        dbt_cmd_flags: list[str] = None,
-        **kwargs,
+        dbt_cmd_flags: list[str] | None = None,
+        **kwargs: str,
     ) -> None:
         self.project_dir = project_dir
         self.conn_id = conn_id
         self.base_cmd = base_cmd
         self.select = select
         self.exclude = exclude
         self.selector = selector
@@ -128,15 +128,15 @@
         elif dbt_executable_path == "dbt":
             self.dbt_executable_path = shutil.which("dbt")
         else:
             self.dbt_executable_path = dbt_executable_path
         self.dbt_cmd_flags = dbt_cmd_flags
         super().__init__(**kwargs)
 
-    def get_env(self, context: Context) -> dict[str, str | bytes | os.PathLike]:
+    def get_env(self, context: Context) -> dict[str, str | bytes | os.PathLike[Any]]:
         """
         Builds the set of environment variables to be exposed for the bash command.
 
         The order of determination is:
             1. If append_env is True, the current process environment.
             2. The Airflow context as environment variables.
             3. The env parameter passed to the Operator
@@ -155,15 +155,15 @@
         # env parameter passed to the Operator
         if self.env and isinstance(self.env, dict):
             env.update(self.env)
 
         # filter out invalid types and give a warning when a value is removed
         accepted_types = (str, bytes, os.PathLike)
 
-        filtered_env: dict[str, str | bytes | os.PathLike] = {}
+        filtered_env: dict[str, str | bytes | os.PathLike[Any]] = {}
 
         for key, val in env.items():
             if isinstance(key, accepted_types) and isinstance(val, accepted_types):
                 filtered_env[key] = val
             else:
                 if isinstance(key, accepted_types):
                     logger.warning(
@@ -201,20 +201,18 @@
                 flags.append(f"--{global_boolean_flag.replace('_', '-')}")
         return flags
 
     def build_cmd(
         self,
         context: Context,
         cmd_flags: list[str] | None = None,
-    ) -> Tuple[list[str], dict]:
+    ) -> Tuple[list[str | None], dict[str, str | bytes | os.PathLike[Any]]]:
         dbt_cmd = [self.dbt_executable_path]
 
-        if isinstance(self.base_cmd, str):
-            dbt_cmd.append(self.base_cmd)
-        else:
+        if self.base_cmd:
             dbt_cmd.extend(self.base_cmd)
 
         dbt_cmd.extend(self.add_global_flags())
 
         # add command specific flags
         if cmd_flags:
             dbt_cmd.extend(cmd_flags)
```

### Comparing `astronomer_cosmos-0.7.5/cosmos/operators/docker.py` & `astronomer_cosmos-1.0.0/cosmos/operators/docker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import logging
-from typing import Callable, Optional, Sequence
+from typing import Any, Callable, Sequence
 
 import yaml
 from airflow.utils.context import Context
 
 from cosmos.operators.base import DbtBaseOperator
 
 logger = logging.getLogger(__name__)
@@ -16,158 +16,158 @@
 except ImportError:
     raise ImportError(
         "Could not import DockerOperator. Ensure you've installed the docker provider separately or "
         "with with `pip install astronomer-cosmos[...,docker]`."
     )
 
 
-class DbtDockerBaseOperator(DockerOperator, DbtBaseOperator):
+class DbtDockerBaseOperator(DockerOperator, DbtBaseOperator):  # type: ignore[misc] # ignores subclass MyPy error
     """
     Executes a dbt core cli command in a Docker container.
 
     """
 
     template_fields: Sequence[str] = DbtBaseOperator.template_fields + DockerOperator.template_fields
 
     intercept_flag = False
 
     def __init__(
         self,
         image: str,  # Make image a required argument since it's required by DockerOperator
-        **kwargs,
+        **kwargs: Any,
     ) -> None:
         super().__init__(image=image, **kwargs)
 
-    def build_and_run_cmd(self, context: Context, cmd_flags: list[str] | None = None):
+    def build_and_run_cmd(self, context: Context, cmd_flags: list[str] | None = None) -> Any:
         self.build_command(cmd_flags, context)
-        self.log.info(f"Running command: {self.command}")
+        self.log.info(f"Running command: {self.command}")  # type: ignore[has-type]
         return super().execute(context)
 
-    def build_command(self, cmd_flags, context):
+    def build_command(self, context: Context, cmd_flags: list[str] | None = None) -> None:
         # For the first round, we're going to assume that the command is dbt
         # This means that we don't have openlineage support, but we will create a ticket
         # to add that in the future
         self.dbt_executable_path = "dbt"
         dbt_cmd, env_vars = self.build_cmd(context=context, cmd_flags=cmd_flags)
         # set env vars
-        self.environment = {**env_vars, **self.environment}
+        self.environment = {**env_vars, **self.environment}  # type: ignore[has-type]
         self.command = dbt_cmd
 
 
 class DbtLSDockerOperator(DbtDockerBaseOperator):
     """
     Executes a dbt core ls command.
     """
 
     ui_color = "#DBCDF6"
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, **kwargs: str) -> None:
         super().__init__(**kwargs)
-        self.base_cmd = "ls"
+        self.base_cmd = ["ls"]
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> Any:
         return self.build_and_run_cmd(context=context)
 
 
 class DbtSeedDockerOperator(DbtDockerBaseOperator):
     """
     Executes a dbt core seed command.
 
     :param full_refresh: dbt optional arg - dbt will treat incremental models as table models
     """
 
     ui_color = "#F58D7E"
 
-    def __init__(self, full_refresh: bool = False, **kwargs) -> None:
+    def __init__(self, full_refresh: bool = False, **kwargs: str) -> None:
         self.full_refresh = full_refresh
         super().__init__(**kwargs)
-        self.base_cmd = "seed"
+        self.base_cmd = ["seed"]
 
-    def add_cmd_flags(self):
+    def add_cmd_flags(self) -> list[str]:
         flags = []
         if self.full_refresh is True:
             flags.append("--full-refresh")
 
         return flags
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> Any:
         cmd_flags = self.add_cmd_flags()
         return self.build_and_run_cmd(context=context, cmd_flags=cmd_flags)
 
 
 class DbtSnapshotDockerOperator(DbtDockerBaseOperator):
     """
     Executes a dbt core snapshot command.
 
     """
 
     ui_color = "#964B00"
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, **kwargs: str) -> None:
         super().__init__(**kwargs)
-        self.base_cmd = "snapshot"
+        self.base_cmd = ["snapshot"]
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> Any:
         return self.build_and_run_cmd(context=context)
 
 
 class DbtRunDockerOperator(DbtDockerBaseOperator):
     """
     Executes a dbt core run command.
     """
 
     ui_color = "#7352BA"
     ui_fgcolor = "#F4F2FC"
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, **kwargs: str) -> None:
         super().__init__(**kwargs)
-        self.base_cmd = "run"
+        self.base_cmd = ["run"]
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> Any:
         return self.build_and_run_cmd(context=context)
 
 
 class DbtTestDockerOperator(DbtDockerBaseOperator):
     """
     Executes a dbt core test command.
     """
 
     ui_color = "#8194E0"
 
-    def __init__(self, on_warning_callback: Optional[Callable] = None, **kwargs) -> None:
+    def __init__(self, on_warning_callback: Callable[..., Any] | None = None, **kwargs: str) -> None:
         super().__init__(**kwargs)
-        self.base_cmd = "test"
+        self.base_cmd = ["test"]
         # as of now, on_warning_callback in docker executor does nothing
         self.on_warning_callback = on_warning_callback
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> Any:
         return self.build_and_run_cmd(context=context)
 
 
 class DbtRunOperationDockerOperator(DbtDockerBaseOperator):
     """
     Executes a dbt core run-operation command.
 
     :param macro_name: name of macro to execute
     :param args: Supply arguments to the macro. This dictionary will be mapped to the keyword arguments defined in the
         selected macro.
     """
 
     ui_color = "#8194E0"
-    template_fields: Sequence[str] = "args"
+    template_fields: Sequence[str] = ("args",)
 
-    def __init__(self, macro_name: str, args: dict = None, **kwargs) -> None:
+    def __init__(self, macro_name: str, args: dict[str, Any] | None = None, **kwargs: str) -> None:
         self.macro_name = macro_name
         self.args = args
         super().__init__(**kwargs)
         self.base_cmd = ["run-operation", macro_name]
 
-    def add_cmd_flags(self):
+    def add_cmd_flags(self) -> list[str]:
         flags = []
         if self.args is not None:
             flags.append("--args")
             flags.append(yaml.dump(self.args))
         return flags
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> Any:
         cmd_flags = self.add_cmd_flags()
         return self.build_and_run_cmd(context=context, cmd_flags=cmd_flags)
```

### Comparing `astronomer_cosmos-0.7.5/cosmos/operators/kubernetes.py` & `astronomer_cosmos-1.0.0/cosmos/operators/kubernetes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,60 @@
 from __future__ import annotations
 
 import logging
-from typing import Callable, Optional, Sequence
+from os import PathLike
+from typing import Any, Callable, Sequence
 
 import yaml
 from airflow.utils.context import Context
 
 from cosmos.operators.base import DbtBaseOperator
 
 logger = logging.getLogger(__name__)
 
 # kubernetes is an optional dependency, so we need to check if it's installed
 try:
     from airflow.providers.cncf.kubernetes.backcompat.backwards_compat_converters import (
         convert_env_vars,
     )
     from airflow.providers.cncf.kubernetes.operators.pod import KubernetesPodOperator
-    from kubernetes.client import models as k8s
 except ImportError:
     raise ImportError(
         "Could not import KubernetesPodOperator. Ensure you've installed the Kubernetes provider "
         "separately or with with `pip install astronomer-cosmos[...,kubernetes]`."
     )
 
 
-class DbtKubernetesBaseOperator(KubernetesPodOperator, DbtBaseOperator):
+class DbtKubernetesBaseOperator(KubernetesPodOperator, DbtBaseOperator):  # type: ignore[misc]
     """
     Executes a dbt core cli command in a Kubernetes Pod.
 
     """
 
     template_fields: Sequence[str] = DbtBaseOperator.template_fields + KubernetesPodOperator.template_fields
 
     intercept_flag = False
 
-    def __init__(
-        self,
-        **kwargs,
-    ) -> None:
+    def __init__(self, **kwargs: Any) -> None:
         super().__init__(**kwargs)
 
-    def build_env_args(self, env: dict) -> list[k8s.V1EnvVar]:
-        env_vars_dict = {}
-        for env_var in self.env_vars:
+    def build_env_args(self, env: dict[str, str | bytes | PathLike[Any]]) -> None:
+        env_vars_dict = dict()
+
+        for env_var in self.env_vars:  # type: ignore[has-type]
             env_vars_dict[env_var.name] = env_var.value
 
         self.env_vars = convert_env_vars({**env, **env_vars_dict})
 
-    def build_and_run_cmd(self, context: Context, cmd_flags: list[str] | None = None):
+    def build_and_run_cmd(self, context: Context, cmd_flags: list[str] | None = None) -> Any:
         self.build_kube_args(cmd_flags, context)
         self.log.info(f"Running command: {self.arguments}")
         return super().execute(context)
 
-    def build_kube_args(self, cmd_flags, context):
+    def build_kube_args(self, context: Context, cmd_flags: list[str] | None = None) -> None:
         # For the first round, we're going to assume that the command is dbt
         # This means that we don't have openlineage support, but we will create a ticket
         # to add that in the future
         self.dbt_executable_path = "dbt"
         dbt_cmd, env_vars = self.build_cmd(context=context, cmd_flags=cmd_flags)
         # set env vars
         self.build_env_args(env_vars)
@@ -66,118 +64,118 @@
 class DbtLSKubernetesOperator(DbtKubernetesBaseOperator):
     """
     Executes a dbt core ls command.
     """
 
     ui_color = "#DBCDF6"
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, **kwargs: str) -> None:
         super().__init__(**kwargs)
-        self.base_cmd = "ls"
+        self.base_cmd = ["ls"]
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> Any:
         return self.build_and_run_cmd(context=context)
 
 
 class DbtSeedKubernetesOperator(DbtKubernetesBaseOperator):
     """
     Executes a dbt core seed command.
 
     :param full_refresh: dbt optional arg - dbt will treat incremental models as table models
     """
 
     ui_color = "#F58D7E"
 
-    def __init__(self, full_refresh: bool = False, **kwargs) -> None:
+    def __init__(self, full_refresh: bool = False, **kwargs: str) -> None:
         self.full_refresh = full_refresh
         super().__init__(**kwargs)
-        self.base_cmd = "seed"
+        self.base_cmd = ["seed"]
 
-    def add_cmd_flags(self):
+    def add_cmd_flags(self) -> list[str]:
         flags = []
         if self.full_refresh is True:
             flags.append("--full-refresh")
 
         return flags
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> Any:
         cmd_flags = self.add_cmd_flags()
         return self.build_and_run_cmd(context=context, cmd_flags=cmd_flags)
 
 
 class DbtSnapshotKubernetesOperator(DbtKubernetesBaseOperator):
     """
     Executes a dbt core snapshot command.
 
     """
 
     ui_color = "#964B00"
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, **kwargs: str) -> None:
         super().__init__(**kwargs)
-        self.base_cmd = "snapshot"
+        self.base_cmd = ["snapshot"]
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> Any:
         return self.build_and_run_cmd(context=context)
 
 
 class DbtRunKubernetesOperator(DbtKubernetesBaseOperator):
     """
     Executes a dbt core run command.
     """
 
     ui_color = "#7352BA"
     ui_fgcolor = "#F4F2FC"
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, **kwargs: str) -> None:
         super().__init__(**kwargs)
-        self.base_cmd = "run"
+        self.base_cmd = ["run"]
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> Any:
         return self.build_and_run_cmd(context=context)
 
 
 class DbtTestKubernetesOperator(DbtKubernetesBaseOperator):
     """
     Executes a dbt core test command.
     """
 
     ui_color = "#8194E0"
 
-    def __init__(self, on_warning_callback: Optional[Callable] = None, **kwargs) -> None:
+    def __init__(self, on_warning_callback: Callable[..., Any] | None = None, **kwargs: str) -> None:
         super().__init__(**kwargs)
-        self.base_cmd = "test"
+        self.base_cmd = ["test"]
         # as of now, on_warning_callback in kubernetes executor does nothing
         self.on_warning_callback = on_warning_callback
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> Any:
         return self.build_and_run_cmd(context=context)
 
 
 class DbtRunOperationKubernetesOperator(DbtKubernetesBaseOperator):
     """
     Executes a dbt core run-operation command.
 
     :param macro_name: name of macro to execute
     :param args: Supply arguments to the macro. This dictionary will be mapped to the keyword arguments defined in the
         selected macro.
     """
 
     ui_color = "#8194E0"
-    template_fields: Sequence[str] = "args"
+    template_fields: Sequence[str] = ("args",)
 
-    def __init__(self, macro_name: str, args: dict = None, **kwargs) -> None:
+    def __init__(self, macro_name: str, args: dict[str, Any] | None = None, **kwargs: str) -> None:
         self.macro_name = macro_name
         self.args = args
         super().__init__(**kwargs)
         self.base_cmd = ["run-operation", macro_name]
 
-    def add_cmd_flags(self):
+    def add_cmd_flags(self) -> list[str]:
         flags = []
         if self.args is not None:
             flags.append("--args")
             flags.append(yaml.dump(self.args))
         return flags
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> Any:
         cmd_flags = self.add_cmd_flags()
         return self.build_and_run_cmd(context=context, cmd_flags=cmd_flags)
```

### Comparing `astronomer_cosmos-0.7.5/cosmos/operators/local.py` & `astronomer_cosmos-1.0.0/cosmos/operators/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 
 import logging
 import os
 import shutil
 import signal
 import tempfile
 from pathlib import Path
-from typing import Callable, Optional, Sequence
+from typing import Any, Callable, Sequence, Tuple
 
 import yaml
 from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException, AirflowSkipException
 from airflow.utils.context import Context
 from airflow.utils.session import NEW_SESSION, provide_session
 from sqlalchemy.orm import Session
 
-from cosmos.constants import DEFAULT_DBT_PROFILE_NAME, DEFAULT_DBT_TARGET_NAME
+from cosmos.config import ProfileConfig
 from cosmos.operators.base import DbtBaseOperator
-from cosmos.profiles import get_profile_mapping
 from cosmos.hooks.subprocess import (
     FullOutputSubprocessHook,
     FullOutputSubprocessResult,
 )
 from cosmos.dbt.parser.output import (
     extract_log_issues,
     parse_output,
@@ -41,53 +40,49 @@
     :param install_deps: If true, install dependencies before running the command
     :param callback: A callback function called on after a dbt run with a path to the dbt project directory.
     :param target_name: A name to use for the dbt target. If not provided, and no target is found
         in your project's dbt_project.yml, "cosmos_target" is used.
     :param should_store_compiled_sql: If true, store the compiled SQL in the compiled_sql rendered template.
     """
 
-    template_fields: Sequence[str] = DbtBaseOperator.template_fields + ("compiled_sql",)
+    template_fields: Sequence[str] = DbtBaseOperator.template_fields + ("compiled_sql",)  # type: ignore[operator]
     template_fields_renderers = {
         "compiled_sql": "sql",
     }
 
     def __init__(
         self,
+        profile_config: ProfileConfig,
         install_deps: bool = False,
-        callback: Optional[Callable[[str], None]] = None,
-        profile_args: dict[str, str] = {},
-        profile_name: str | None = None,
-        target_name: str | None = None,
+        callback: Callable[[str], None] | None = None,
         should_store_compiled_sql: bool = True,
-        **kwargs,
+        **kwargs: Any,
     ) -> None:
+        self.profile_config = profile_config
         self.install_deps = install_deps
-        self.profile_args = profile_args
         self.callback = callback
-        self.profile_name = profile_name
-        self.target_name = target_name
         self.compiled_sql = ""
         self.should_store_compiled_sql = should_store_compiled_sql
         super().__init__(**kwargs)
 
-    @cached_property
-    def subprocess_hook(self):
+    @cached_property  # type: ignore[misc] # ignores internal untyped decorator
+    def subprocess_hook(self) -> FullOutputSubprocessHook:
         """Returns hook for running the bash command."""
         return FullOutputSubprocessHook()
 
-    def exception_handling(self, result: FullOutputSubprocessResult):
+    def exception_handling(self, result: FullOutputSubprocessResult) -> None:
         if self.skip_exit_code is not None and result.exit_code == self.skip_exit_code:
             raise AirflowSkipException(f"dbt command returned exit code {self.skip_exit_code}. Skipping.")
         elif result.exit_code != 0:
             raise AirflowException(
                 f"dbt command failed. The command returned a non-zero exit code {result.exit_code}. Details: ",
                 *result.full_output,
             )
 
-    @provide_session
+    @provide_session  # type: ignore[misc] # ignores internal untyped decorator
     def store_compiled_sql(self, tmp_project_dir: str, context: Context, session: Session = NEW_SESSION) -> None:
         """
         Takes the compiled SQL files from the dbt run and stores them in the compiled_sql rendered template.
         Gets called after every dbt run.
         """
         if not self.should_store_compiled_sql:
             return
@@ -122,64 +117,22 @@
         session.query(RenderedTaskInstanceFields).filter(
             RenderedTaskInstanceFields.dag_id == self.dag_id,
             RenderedTaskInstanceFields.task_id == self.task_id,
             RenderedTaskInstanceFields.run_id == ti.run_id,
         ).delete()
         session.add(rtif)
 
-    def run_subprocess(self, *args, **kwargs):
-        return self.subprocess_hook.run_command(*args, **kwargs)
-
-    def get_profile_name(self, project_dir: str) -> str:
-        """
-        Returns the profile name to use. Precedence is:
-        1. The profile name passed in to the operator
-        2. The profile name in the dbt_project.yml file
-        3. "cosmos_profile"
-        """
-        if self.profile_name:
-            return self.profile_name
-
-        # get the profile name from the dbt_project.yml file
-        dbt_project_path = os.path.join(project_dir, "dbt_project.yml")
-
-        # if there's no dbt_project.yml file, we're not in a dbt project
-        # and need to raise an error
-        if not os.path.exists(dbt_project_path):
-            raise AirflowException(f"dbt project directory {self.project_dir} does not contain a dbt_project.yml file.")
-
-        # get file contents using path
-        dbt_project = yaml.safe_load(Path(dbt_project_path).read_text(encoding="utf-8")) or {}
-
-        profile_name = dbt_project.get("profile", DEFAULT_DBT_PROFILE_NAME)
-
-        if not isinstance(profile_name, str):
-            raise AirflowException(
-                f"dbt project directory {self.project_dir} contains a dbt_project.yml file, but the profile "
-                f"specified in the file is not a string. Please specify a string profile name, or pass a profile "
-                f"name to the operator."
-            )
-
-        return profile_name
-
-    def get_target_name(self) -> str:
-        """
-        Returns the target name to use. Precedence is:
-        1. The target name passed in to the operator
-        2. "cosmos_target"
-        """
-        if self.target_name:
-            return self.target_name
-
-        return DEFAULT_DBT_TARGET_NAME
+    def run_subprocess(self, *args: Tuple[Any], **kwargs: Any) -> FullOutputSubprocessResult:
+        subprocess_result: FullOutputSubprocessResult = self.subprocess_hook.run_command(*args, **kwargs)
+        return subprocess_result
 
     def run_command(
         self,
-        cmd: list[str],
-        env: dict[str, str],
+        cmd: list[str | None],
+        env: dict[str, str | bytes | os.PathLike[Any]],
         context: Context,
     ) -> FullOutputSubprocessResult:
         """
         Copies the dbt project to a temporary directory and runs the command.
         """
         with tempfile.TemporaryDirectory() as tmp_dir:
             logger.info(
@@ -191,58 +144,48 @@
             # need a subfolder because shutil.copytree will fail if the destination dir already exists
             tmp_project_dir = os.path.join(tmp_dir, "dbt_project")
             shutil.copytree(
                 self.project_dir,
                 tmp_project_dir,
             )
 
-            profile_name = self.get_profile_name(tmp_project_dir)
-            target_name = self.get_target_name()
-
-            # need to write the profile to a file because dbt requires a profile file
-            # and doesn't accept a profile as a string
-            profile_mapping = get_profile_mapping(
-                conn_id=self.conn_id,
-                profile_args=self.profile_args,
-            )
-            profile_file_contents = profile_mapping.get_profile_file_contents(
-                profile_name=profile_name,
-                target_name=target_name,
-            )
-            profile_file_path = os.path.join(tmp_project_dir, "profiles.yml")
-            with open(profile_file_path, "w", encoding="utf-8") as f:
-                f.write(profile_file_contents)
-
-            # we also need to get the env from the profile mapping
-            env.update(profile_mapping.env_vars)
-
             # if we need to install deps, do so
             if self.install_deps:
                 self.run_subprocess(
                     command=[self.dbt_executable_path, "deps"],
                     env=env,
                     output_encoding=self.output_encoding,
                     cwd=tmp_project_dir,
                 )
 
-            logger.info("Trying to run the command:\n %s\nFrom %s", cmd, tmp_project_dir)
-
-            result = self.run_subprocess(
-                command=cmd + ["--profile", profile_name, "--target", target_name],
-                env=env,
-                output_encoding=self.output_encoding,
-                cwd=tmp_project_dir,
-            )
+            with self.profile_config.ensure_profile() as (profile_path, env_vars):
+                env.update(env_vars)
+                full_cmd = cmd + [
+                    "--profiles-dir",
+                    str(profile_path.parent),
+                    "--profile",
+                    self.profile_config.profile_name,
+                    "--target",
+                    self.profile_config.target_name,
+                ]
+
+                logger.info("Trying to run the command:\n %s\nFrom %s", full_cmd, tmp_project_dir)
+                result = self.run_subprocess(
+                    command=full_cmd,
+                    env=env,
+                    output_encoding=self.output_encoding,
+                    cwd=tmp_project_dir,
+                )
 
-            self.exception_handling(result)
-            self.store_compiled_sql(tmp_project_dir, context)
-            if self.callback:
-                self.callback(tmp_project_dir)
+                self.exception_handling(result)
+                self.store_compiled_sql(tmp_project_dir, context)
+                if self.callback:
+                    self.callback(tmp_project_dir)
 
-            return result
+                return result
 
     def build_and_run_cmd(self, context: Context, cmd_flags: list[str] | None = None) -> FullOutputSubprocessResult:
         dbt_cmd, env = self.build_cmd(context=context, cmd_flags=cmd_flags)
         return self.run_command(cmd=dbt_cmd, env=env, context=context)
 
     def execute(self, context: Context) -> str:
         # TODO is this going to put loads of unnecessary stuff in to xcom?
@@ -260,80 +203,80 @@
 class DbtLSLocalOperator(DbtLocalBaseOperator):
     """
     Executes a dbt core ls command.
     """
 
     ui_color = "#DBCDF6"
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, **kwargs: Any) -> None:
         super().__init__(**kwargs)
-        self.base_cmd = "ls"
+        self.base_cmd = ["ls"]
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> str:
         result = self.build_and_run_cmd(context=context)
         return result.output
 
 
 class DbtSeedLocalOperator(DbtLocalBaseOperator):
     """
     Executes a dbt core seed command.
 
     :param full_refresh: dbt optional arg - dbt will treat incremental models as table models
     """
 
     ui_color = "#F58D7E"
 
-    def __init__(self, full_refresh: bool = False, **kwargs) -> None:
+    def __init__(self, full_refresh: bool = False, **kwargs: Any) -> None:
         self.full_refresh = full_refresh
         super().__init__(**kwargs)
-        self.base_cmd = "seed"
+        self.base_cmd = ["seed"]
 
-    def add_cmd_flags(self):
+    def add_cmd_flags(self) -> list[str]:
         flags = []
         if self.full_refresh is True:
             flags.append("--full-refresh")
 
         return flags
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> str:
         cmd_flags = self.add_cmd_flags()
         result = self.build_and_run_cmd(context=context, cmd_flags=cmd_flags)
         return result.output
 
 
 class DbtSnapshotLocalOperator(DbtLocalBaseOperator):
     """
     Executes a dbt core snapshot command.
 
     """
 
     ui_color = "#964B00"
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, **kwargs: Any) -> None:
         super().__init__(**kwargs)
-        self.base_cmd = "snapshot"
+        self.base_cmd = ["snapshot"]
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> str:
         result = self.build_and_run_cmd(context=context)
         return result.output
 
 
 class DbtRunLocalOperator(DbtLocalBaseOperator):
     """
     Executes a dbt core run command.
     """
 
     ui_color = "#7352BA"
     ui_fgcolor = "#F4F2FC"
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, **kwargs: Any) -> None:
         super().__init__(**kwargs)
-        self.base_cmd = "run"
+        self.base_cmd = ["run"]
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> str:
         result = self.build_and_run_cmd(context=context)
         return result.output
 
 
 class DbtTestLocalOperator(DbtLocalBaseOperator):
     """
     Executes a dbt core test command.
@@ -341,34 +284,34 @@
         and "test_results" of type `List`. Each index in "test_names" corresponds to the same index in "test_results".
     """
 
     ui_color = "#8194E0"
 
     def __init__(
         self,
-        on_warning_callback: Optional[Callable] = None,
-        **kwargs,
+        on_warning_callback: Callable[..., Any] | None = None,
+        **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
-        self.base_cmd = "test"
+        self.base_cmd = ["test"]
         self.on_warning_callback = on_warning_callback
 
     def _should_run_tests(
         self,
         result: FullOutputSubprocessResult,
         no_tests_message: str = "Nothing to do",
     ) -> bool:
         """
         Check if any tests are defined to run in the DAG. If tests are defined
         and on_warning_callback is set, then function returns True.
 
         :param result: The output from the build and run command.
         """
 
-        return self.on_warning_callback and no_tests_message not in result.output
+        return self.on_warning_callback is not None and no_tests_message not in result.output
 
     def _handle_warnings(self, result: FullOutputSubprocessResult, context: Context) -> None:
         """
          Handles warnings by extracting log issues, creating additional context, and calling the
          on_warning_callback with the updated context.
 
         :param result: The result object from the build and run command.
@@ -376,17 +319,18 @@
         """
         test_names, test_results = extract_log_issues(result.full_output)
 
         warning_context = dict(context)
         warning_context["test_names"] = test_names
         warning_context["test_results"] = test_results
 
-        self.on_warning_callback(warning_context)
+        if self.on_warning_callback:
+            self.on_warning_callback(warning_context)
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> str:
         result = self.build_and_run_cmd(context=context)
 
         if not self._should_run_tests(result):
             return result.output
 
         warnings = parse_output(result, "WARN")
         if warnings > 0:
@@ -401,30 +345,30 @@
 
     :param macro_name: name of macro to execute
     :param args: Supply arguments to the macro. This dictionary will be mapped to the keyword arguments defined in the
         selected macro.
     """
 
     ui_color = "#8194E0"
-    template_fields: Sequence[str] = "args"
+    template_fields: Sequence[str] = ("args",)
 
-    def __init__(self, macro_name: str, args: dict = None, **kwargs) -> None:
+    def __init__(self, macro_name: str, args: dict[str, Any] | None = None, **kwargs: Any) -> None:
         self.macro_name = macro_name
         self.args = args
         super().__init__(**kwargs)
         self.base_cmd = ["run-operation", macro_name]
 
-    def add_cmd_flags(self):
+    def add_cmd_flags(self) -> list[str]:
         flags = []
         if self.args is not None:
             flags.append("--args")
             flags.append(yaml.dump(self.args))
         return flags
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> str:
         cmd_flags = self.add_cmd_flags()
         result = self.build_and_run_cmd(context=context, cmd_flags=cmd_flags)
         return result.output
 
 
 class DbtDocsLocalOperator(DbtLocalBaseOperator):
     """
@@ -432,19 +376,19 @@
     Use the `callback` parameter to specify a callback function to run after the command completes.
     """
 
     ui_color = "#8194E0"
 
     required_files = ["index.html", "manifest.json", "graph.gpickle", "catalog.json"]
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         self.base_cmd = ["docs", "generate"]
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> str:
         result = self.build_and_run_cmd(context=context)
         return result.output
 
 
 class DbtDocsS3LocalOperator(DbtDocsLocalOperator):
     """
     Executes `dbt docs generate` command and upload to S3 storage. Returns the S3 path to the generated documentation.
@@ -458,15 +402,15 @@
     ui_color = "#FF9900"
 
     def __init__(
         self,
         aws_conn_id: str,
         bucket_name: str,
         folder_dir: str | None = None,
-        **kwargs,
+        **kwargs: str,
     ) -> None:
         "Initializes the operator."
         self.aws_conn_id = aws_conn_id
         self.bucket_name = bucket_name
         self.folder_dir = folder_dir
 
         super().__init__(**kwargs)
@@ -518,15 +462,15 @@
     ui_color = "#007FFF"
 
     def __init__(
         self,
         azure_conn_id: str,
         container_name: str,
         folder_dir: str | None = None,
-        **kwargs,
+        **kwargs: str,
     ) -> None:
         "Initializes the operator."
         self.azure_conn_id = azure_conn_id
         self.container_name = container_name
         self.folder_dir = folder_dir
 
         super().__init__(**kwargs)
@@ -569,11 +513,11 @@
 class DbtDepsLocalOperator(DbtLocalBaseOperator):
     """
     Executes a dbt core deps command.
     """
 
     ui_color = "#8194E0"
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, **kwargs: str) -> None:
         raise DeprecationWarning(
             "The DbtDepsOperator has been deprecated. " "Please use the `install_deps` flag in dbt_args instead."
         )
```

### Comparing `astronomer_cosmos-0.7.5/cosmos/operators/virtualenv.py` & `astronomer_cosmos-1.0.0/cosmos/operators/virtualenv.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import logging
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Tuple
 
 
 from airflow.compat.functools import cached_property
 from airflow.utils.python_virtualenv import prepare_virtualenv
+from cosmos.hooks.subprocess import FullOutputSubprocessResult
 
 from cosmos.operators.local import (
     DbtDocsLocalOperator,
     DbtLocalBaseOperator,
     DbtLSLocalOperator,
     DbtRunLocalOperator,
     DbtRunOperationLocalOperator,
@@ -41,22 +42,22 @@
            Avoid using unless the dbt job requires it.
     """
 
     def __init__(
         self,
         py_requirements: list[str] | None = None,
         py_system_site_packages: bool = False,
-        **kwargs,
+        **kwargs: Any,
     ) -> None:
         self.py_requirements = py_requirements or []
         self.py_system_site_packages = py_system_site_packages
         super().__init__(**kwargs)
-        self._venv_tmp_dir = ""
+        self._venv_tmp_dir = TemporaryDirectory()
 
-    @cached_property
+    @cached_property  # type: ignore[misc] # ignores internal untyped decorator
     def venv_dbt_path(
         self,
     ) -> str:
         """
         Path to the dbt binary within a Python virtualenv.
 
         The first time this property is called, it creates a virtualenv and installs the dependencies based on the
@@ -80,23 +81,22 @@
                 "from importlib.metadata import version; print(version('dbt-core'))",
             ]
         )
         dbt_version = cmd_output.output
         self.log.info("Using dbt version %s available at %s", dbt_version, dbt_binary)
         return str(dbt_binary)
 
-    def run_subprocess(self, command, *args, **kwargs):
+    def run_subprocess(  # type: ignore[override]
+        self, *args: Tuple[Any], command: list[str], **kwargs: Any
+    ) -> FullOutputSubprocessResult:
         if self.py_requirements:
             command[0] = self.venv_dbt_path
 
-        return self.subprocess_hook.run_command(
-            command,
-            *args,
-            **kwargs,
-        )
+        subprocess_result: FullOutputSubprocessResult = self.subprocess_hook.run_command(command, *args, **kwargs)
+        return subprocess_result
 
     def execute(self, context: Context) -> str:
         output = super().execute(context)
         if self._venv_tmp_dir:
             self._venv_tmp_dir.cleanup()
         return output
```

### Comparing `astronomer_cosmos-0.7.5/cosmos/profiles/base.py` & `astronomer_cosmos-1.0.0/cosmos/profiles/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 This module contains a base class that other profile mappings should
 inherit from to ensure consistency.
 """
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-
 from logging import getLogger
 from typing import Any
 
 from typing import TYPE_CHECKING
 import yaml
 
+from airflow.hooks.base import BaseHook
+from cosmos.exceptions import CosmosValueError
+
 if TYPE_CHECKING:
     from airflow.models import Connection
 
 logger = getLogger(__name__)
 
 
 class BaseProfileMapping(ABC):
@@ -27,37 +29,54 @@
     airflow_connection_type: str = "generic"
     is_community: bool = False
 
     required_fields: list[str] = []
     secret_fields: list[str] = []
     airflow_param_mapping: dict[str, str | list[str]] = {}
 
-    def __init__(self, conn: Connection, profile_args: dict[str, Any] | None = None):
-        self.conn = conn
+    _conn: Connection | None = None
+
+    def __init__(self, conn_id: str, profile_args: dict[str, Any] | None = None):
+        self.conn_id = conn_id
         self.profile_args = profile_args or {}
 
+    @property
+    def conn(self) -> Connection:
+        "Returns the Airflow connection."
+        if not self._conn:
+            conn = BaseHook.get_connection(self.conn_id)
+            if not conn:
+                raise CosmosValueError(f"Could not find connection {self.conn_id}.")
+
+            self._conn = conn
+
+        return self._conn
+
     def can_claim_connection(self) -> bool:
         """
         Return whether the connection is valid for this profile mapping.
         """
         if self.conn.conn_type != self.airflow_connection_type:
             return False
 
+        logger.info(dir(self.conn))
+        logger.info(self.conn.__dict__)
+
         for field in self.required_fields:
             try:
                 if not getattr(self, field):
                     logger.info(
-                        "Not using mapping %s because %s is not set",
+                        "1 Not using mapping %s because %s is not set",
                         self.__class__.__name__,
                         field,
                     )
                     return False
             except AttributeError:
                 logger.info(
-                    "Not using mapping %s because %s is not set",
+                    "2 Not using mapping %s because %s is not set",
                     self.__class__.__name__,
                     field,
                 )
                 return False
 
         return True
 
@@ -93,15 +112,14 @@
 
         profile_contents = {
             profile_name: {
                 "target": target_name,
                 "outputs": {target_name: profile_vars},
             }
         }
-
         return str(yaml.dump(profile_contents, indent=4))
 
     def get_dbt_value(self, name: str) -> Any:
         """
         Gets values for the dbt profile based on the required_by_dbt and required_in_profile_args lists.
         Precedence is:
         1. profile_args
```

### Comparing `astronomer_cosmos-0.7.5/cosmos/profiles/bigquery/service_account_file.py` & `astronomer_cosmos-1.0.0/cosmos/profiles/bigquery/service_account_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "project",
         "dataset",
         "keyfile",
     ]
 
     airflow_param_mapping = {
         "project": "extra.project",
-        "dataset": "dataset",
+        "dataset": "extra.dataset",
         "keyfile": "extra.key_path",
     }
 
     @property
     def profile(self) -> dict[str, Any | None]:
         "Generates profile. Defaults `threads` to 1."
         return {
```

### Comparing `astronomer_cosmos-0.7.5/cosmos/profiles/databricks/token.py` & `astronomer_cosmos-1.0.0/cosmos/profiles/databricks/token.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.5/cosmos/profiles/exasol/user_pass.py` & `astronomer_cosmos-1.0.0/cosmos/profiles/exasol/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.5/cosmos/profiles/postgres/user_pass.py` & `astronomer_cosmos-1.0.0/cosmos/profiles/postgres/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.5/cosmos/profiles/redshift/user_pass.py` & `astronomer_cosmos-1.0.0/cosmos/profiles/redshift/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.5/cosmos/profiles/snowflake/user_pass.py` & `astronomer_cosmos-1.0.0/cosmos/profiles/snowflake/user_pass.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,31 +36,32 @@
         "password": "password",
         "database": "extra.database",
         "warehouse": "extra.warehouse",
         "schema": "schema",
         "role": "extra.role",
     }
 
-    def __init__(self, conn: Connection, profile_args: dict[str, Any | None] | None = None) -> None:
+    @property
+    def conn(self) -> Connection:
         """
         Snowflake can be odd because the fields used to be stored with keys in the format
         'extra__snowflake__account', but now are stored as 'account'.
 
         This standardizes the keys to be 'account', 'database', etc.
         """
+        conn = super().conn
+
         conn_dejson = conn.extra_dejson
 
         if conn_dejson.get("extra__snowflake__account"):
             conn_dejson = {key.replace("extra__snowflake__", ""): value for key, value in conn_dejson.items()}
 
         conn.extra = json.dumps(conn_dejson)
 
-        self.conn = conn
-        self.profile_args = profile_args or {}
-        super().__init__(conn, profile_args)
+        return conn
 
     @property
     def profile(self) -> dict[str, Any | None]:
         "Gets profile."
         profile_vars = {
             "type": "snowflake",
             "account": self.account,
```

### Comparing `astronomer_cosmos-0.7.5/cosmos/profiles/spark/thrift.py` & `astronomer_cosmos-1.0.0/cosmos/profiles/spark/thrift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.5/cosmos/profiles/trino/base.py` & `astronomer_cosmos-1.0.0/cosmos/profiles/trino/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.5/cosmos/profiles/trino/certificate.py` & `astronomer_cosmos-1.0.0/cosmos/profiles/trino/certificate.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.5/cosmos/profiles/trino/jwt.py` & `astronomer_cosmos-1.0.0/cosmos/profiles/trino/jwt.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         "jwt_token": "extra.jwt__token",
         **TrinoBaseProfileMapping.airflow_param_mapping,
     }
 
     @property
     def profile(self) -> dict[str, Any | None]:
         "Gets profile."
-        common_profile_vars = super().profile
+        common_profile_vars: dict[str, Any] = super().profile
 
         # need to remove jwt from profile_args because it will be set as an environment variable
         profile_args = self.profile_args.copy()
         profile_args.pop("jwt", None)
 
         profile_vars = {
             **common_profile_vars,
```

### Comparing `astronomer_cosmos-0.7.5/cosmos/profiles/trino/ldap.py` & `astronomer_cosmos-1.0.0/cosmos/profiles/trino/ldap.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.5/.gitignore` & `astronomer_cosmos-1.0.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 .vscode/
 
 # pycharm
 .DS_Store
 
 # dbt
 logs/
+*.user.yml
 
 # integration tests
 dev/dags/.airflowignore
 
 # Local Airflow standalone
 airflow.cfg
 airflow.db
```

### Comparing `astronomer_cosmos-0.7.5/LICENSE` & `astronomer_cosmos-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.5/README.rst` & `astronomer_cosmos-1.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 This will generate an Airflow Task Group that looks like this:
 
 .. image:: https://raw.githubusercontent.com/astronomer/astronomer-cosmos/main/docs/jaffle_shop_task_group.png
 
 Community
 _________
-- Join us on the Airflow `Slack <https://join.slack.com/t/apache-airflow/shared_invite/zt-1vo1rxgc3-EfsbdDzqrV51fddWOc6GOQ>`_ at #airflow-dbt
+- Join us on the Airflow `Slack <https://join.slack.com/t/apache-airflow/shared_invite/zt-1zy8e8h85-es~fn19iMzUmkhPwnyRT6Q>`_ at #airflow-dbt
 
 Changelog
 _________
 
 We follow `Semantic Versioning <https://semver.org/>`_ for releases.
 Check `CHANGELOG.rst <https://github.com/astronomer/astronomer-cosmos/blob/main/CHANGELOG.rst>`_
 for the latest changes.
```

### Comparing `astronomer_cosmos-0.7.5/pyproject.toml` & `astronomer_cosmos-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -145,31 +145,46 @@
     { value = "apache-airflow==2.4", if = ["2.4"] },
     { value = "apache-airflow==2.5", if = ["2.5"] },
     { value = "apache-airflow==2.6", if = ["2.6"] },
 ]
 
 [tool.hatch.envs.tests.scripts]
 freeze = "pip freeze"
-test = 'pytest -vv --durations=0 . -m "not integration"'
-test-cov = 'pytest -vv --cov=cosmos --cov-report=term-missing --cov-report=xml --durations=0 -m "not integration"'
+test = 'pytest -vv --durations=0 . -m "not integration" --ignore=tests/test_example_dags.py'
+test-cov = 'pytest -vv --cov=cosmos --cov-report=term-missing --cov-report=xml --durations=0 -m "not integration" --ignore=tests/test_example_dags.py'
 # we install using the following workaround to overcome installation conflicts, such as:
 # apache-airflow 2.3.0 and dbt-core [0.13.0 - 1.5.2] and jinja2>=3.0.0 because these package versions have conflicting dependencies
 test-integration-setup = """pip uninstall dbt-postgres; \
 rm -rf airflow.*; \
 airflow db init; \
-pip install dbt-postgres;"""
-test-integration = """pytest -vv --cov=cosmos --cov-report=term-missing --cov-report=xml --durations=0 -m integration"""
+pip install dbt-postgres; \
+pip install dbt-databricks"""
+test-integration = """pytest -vv \
+--cov=cosmos \
+--cov-report=term-missing \
+--cov-report=xml \
+--durations=0 \
+-m integration  \
+-k 'not test_example_dag[example_cosmos_python_models]'
+"""
+test-integration-expensive = """pytest -vv \
+--cov=cosmos \
+--cov-report=term-missing \
+--cov-report=xml \
+--durations=0 \
+-m integration  \
+-k 'test_example_dag[example_cosmos_python_models]'"""
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::DeprecationWarning",
 ]
 minversion = "6.0"
 markers = [
-    "integration"
+    "integration",
 ]
 
 ######################################
 # DOCS
 ######################################
 
 [tool.hatch.envs.docs]
```

### Comparing `astronomer_cosmos-0.7.5/PKG-INFO` & `astronomer_cosmos-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 0.7.5
+Version: 1.0.0
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
@@ -150,15 +150,15 @@
 
 This will generate an Airflow Task Group that looks like this:
 
 .. image:: https://raw.githubusercontent.com/astronomer/astronomer-cosmos/main/docs/jaffle_shop_task_group.png
 
 Community
 _________
-- Join us on the Airflow `Slack <https://join.slack.com/t/apache-airflow/shared_invite/zt-1vo1rxgc3-EfsbdDzqrV51fddWOc6GOQ>`_ at #airflow-dbt
+- Join us on the Airflow `Slack <https://join.slack.com/t/apache-airflow/shared_invite/zt-1zy8e8h85-es~fn19iMzUmkhPwnyRT6Q>`_ at #airflow-dbt
 
 Changelog
 _________
 
 We follow `Semantic Versioning <https://semver.org/>`_ for releases.
 Check `CHANGELOG.rst <https://github.com/astronomer/astronomer-cosmos/blob/main/CHANGELOG.rst>`_
 for the latest changes.
```

