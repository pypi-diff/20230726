# Comparing `tmp/hyperopt_prophet-0.1.2.tar.gz` & `tmp/hyperopt_prophet-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperopt_prophet-0.1.2.tar", max compression
+gzip compressed data, was "hyperopt_prophet-0.1.3.tar", max compression
```

## Comparing `hyperopt_prophet-0.1.2.tar` & `hyperopt_prophet-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1083 2023-07-26 03:08:56.622334 hyperopt_prophet-0.1.2/LICENSE
--rw-r--r--   0        0        0      980 2023-07-26 03:08:56.622334 hyperopt_prophet-0.1.2/README.md
--rw-r--r--   0        0        0      113 2023-07-26 03:08:56.626334 hyperopt_prophet-0.1.2/hyperopt_prophet/__init__.py
--rw-r--r--   0        0        0      204 2023-07-26 03:08:56.626334 hyperopt_prophet-0.1.2/hyperopt_prophet/hyperopt_prophet.py
--rw-r--r--   0        0        0     5047 2023-07-26 03:08:56.626334 hyperopt_prophet-0.1.2/hyperopt_prophet/inference.py
--rw-r--r--   0        0        0    21410 2023-07-26 03:08:56.626334 hyperopt_prophet-0.1.2/hyperopt_prophet/model.py
--rw-r--r--   0        0        0    10032 2023-07-26 03:08:56.626334 hyperopt_prophet-0.1.2/hyperopt_prophet/training.py
--rw-r--r--   0        0        0     4714 2023-07-26 03:08:56.626334 hyperopt_prophet-0.1.2/hyperopt_prophet/utils.py
--rw-r--r--   0        0        0       85 2023-07-26 03:08:56.626334 hyperopt_prophet-0.1.2/main.py
--rw-r--r--   0        0        0      843 2023-07-26 03:08:56.626334 hyperopt_prophet-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2033 1970-01-01 00:00:00.000000 hyperopt_prophet-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-26 04:22:50.575338 hyperopt_prophet-0.1.3/LICENSE
+-rw-r--r--   0        0        0      980 2023-07-26 04:22:50.575338 hyperopt_prophet-0.1.3/README.md
+-rw-r--r--   0        0        0      150 2023-07-26 04:22:50.579338 hyperopt_prophet-0.1.3/hyperopt_prophet/__init__.py
+-rw-r--r--   0        0        0     5047 2023-07-26 04:22:50.579338 hyperopt_prophet-0.1.3/hyperopt_prophet/inference.py
+-rw-r--r--   0        0        0    21410 2023-07-26 04:22:50.579338 hyperopt_prophet-0.1.3/hyperopt_prophet/model.py
+-rw-r--r--   0        0        0     9108 2023-07-26 04:22:50.579338 hyperopt_prophet-0.1.3/hyperopt_prophet/training.py
+-rw-r--r--   0        0        0     4714 2023-07-26 04:22:50.579338 hyperopt_prophet-0.1.3/hyperopt_prophet/utils.py
+-rw-r--r--   0        0        0       85 2023-07-26 04:22:50.579338 hyperopt_prophet-0.1.3/main.py
+-rw-r--r--   0        0        0      818 2023-07-26 04:22:50.579338 hyperopt_prophet-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1987 1970-01-01 00:00:00.000000 hyperopt_prophet-0.1.3/PKG-INFO
```

### Comparing `hyperopt_prophet-0.1.2/LICENSE` & `hyperopt_prophet-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.2/README.md` & `hyperopt_prophet-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.2/hyperopt_prophet/inference.py` & `hyperopt_prophet-0.1.3/hyperopt_prophet/inference.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.2/hyperopt_prophet/model.py` & `hyperopt_prophet-0.1.3/hyperopt_prophet/model.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.2/hyperopt_prophet/training.py` & `hyperopt_prophet-0.1.3/hyperopt_prophet/training.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,58 +1,31 @@
 import json
-import os
 import random
 import warnings
 from builtins import max
-from pathlib import Path
 from time import time
 
 import mlflow
 import mlflow.prophet
-
-# import mlflow.spark
 import pandas as pd
-from dotenv import load_dotenv
 from hyperopt import hp
 from mlflowops import MLFlowOps
-from pydantic import BaseModel
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 from .model import (
     MultiSeriesProphetModel,
     ProphetHyperoptEstimator,
     mlflow_prophet_log_model,
 )
 from .utils import get_plotly_forecast, plotly_fig2pil
 
 warnings.filterwarnings("ignore")
 
 
-def prophet_hyperopt_training(train_data):
-    this_module_path = Path(__file__).parent.resolve()
-    load_dotenv(f"{this_module_path}/training.env")
-    training_params = {
-        "target_col": os.environ.get("target_col", "y"),
-        "id_cols": ["ts_id"],
-        "time_col": os.environ.get("time_col", "ds"),
-        "horizon": os.environ.get("horizon", "1440"),
-        "experiment_id": os.environ.get("experiment_id", "0"),
-        "max_eval": os.environ.get("max_eval", "5"),
-        "num_folds": os.environ.get("num_folds", "1"),
-        "loss_metric": os.environ.get("loss_metric", "mse"),
-        "base_model_name": os.environ.get("base_model_name", "prohet_hyperopt"),
-        "is_parallel": os.environ.get("is_parallel", "False"),
-    }
-    training_params = ProphetTrainingParams(**training_params)
-
-    return ProphetHyperOptTrainer(
-        training_data=train_data, training_params=training_params
-    ).fit()
-
-
-class ProphetTrainingParams(BaseModel):
+class ProphetTrainingParams(BaseSettings):
     """
     Initialization
     :param horizon: Number of periods to forecast forward
     :param frequency_unit: Frequency of the time series
     :param metric: Metric that will be optimized across trials
     :param interval_width: Width of the uncertainty intervals provided for the forecast
     :param country_holidays: Built-in holidays for the specified country
@@ -65,22 +38,27 @@
     :param is_parallel: Indicators to decide that whether run hyperopt in
     :param regressors: list of column names of external regressors
     :param prophet_kwargs: Optional keyword arguments for Prophet model.
         For information about the parameters see:
         `The Prophet source code <https://github.com/facebook/prophet/blob/master/python/prophet/forecaster.py>`_.
     """
 
+    model_config = SettingsConfigDict(
+        env_file="training.env",
+        env_file_encoding="utf-8",
+        arbitrary_types_allowed=True,
+        extra="ignore",
+    )
     target_col: str = "y"
     time_col: str = "ds"
     unit: str = "minute"
-    id_cols: list = ["ts_id"]
+    id_cols: str = "ts_id"
     horizon: int = 1440
     interval_width: float = 0.8
     experiment_id: str = ""
-    sample_input: pd.DataFrame = None  # type: ignore
     result_columns: list = [
         "ts_id",
         "run_id",
         "prophet_params",
         "start_time",
         "end_time",
         "training_duration",
@@ -112,17 +90,14 @@
         "holidays_prior_scale": hp.loguniform("holidays_prior_scale", -10.9, 5.3),
         "seasonality_mode": hp.choice(
             "seasonality_mode", ["additive", "multiplicative"]
         ),
     }
     use_mlflow: bool = False
 
-    class Config:
-        arbitrary_types_allowed = True
-
 
 class ProphetHyperOptTrainer:
     def __init__(
         self, training_data: pd.DataFrame, training_params: ProphetTrainingParams
     ):
         self.training_data = training_data
         self.training_params = training_params
```

### Comparing `hyperopt_prophet-0.1.2/hyperopt_prophet/utils.py` & `hyperopt_prophet-0.1.3/hyperopt_prophet/utils.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.2/pyproject.toml` & `hyperopt_prophet-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 [tool.poetry]
 name = "hyperopt-prophet"
-version = "0.1.2"
+version = "0.1.3"
 description = "Integration of prophet forecasting with hyperopt, mlflow"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "hyperopt_prophet"},
     {include = "main.py"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "^2.0.3"
 pydantic = "^2.1.0"
 pydantic-settings = "^2.0.2"
+prophet = "^1.0.0"
 hyperopt = "^0.2.7"
 mlflow = "^2.5.0"
-python-dotenv = "^1.0.0"
 cloudpickle = "^2.2.1"
 cython = "^3.0.0"
 pystan = "^2.19.1.1"
-prophet = "^1.0.0"
 mlflowops = '^0.1.2'
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.4.0"
 pylint = "^2.17.4"
```

### Comparing `hyperopt_prophet-0.1.2/PKG-INFO` & `hyperopt_prophet-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperopt-prophet
-Version: 0.1.2
+Version: 0.1.3
 Summary: Integration of prophet forecasting with hyperopt, mlflow
 License: MIT
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,14 @@
 Requires-Dist: mlflow (>=2.5.0,<3.0.0)
 Requires-Dist: mlflowops (>=0.1.2,<0.2.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: prophet (>=1.0.0,<2.0.0)
 Requires-Dist: pydantic (>=2.1.0,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.2,<3.0.0)
 Requires-Dist: pystan (>=2.19.1.1,<3.0.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Hyperopt Prophet
 
 **Integration of prophet forecasting with hyperopt, mlflow**
 This implementation is based on the [Databricks AutoML](https://github.com/databricks/automl) repository.
```

