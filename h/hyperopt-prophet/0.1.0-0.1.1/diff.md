# Comparing `tmp/hyperopt_prophet-0.1.0.tar.gz` & `tmp/hyperopt_prophet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperopt_prophet-0.1.0.tar", max compression
+gzip compressed data, was "hyperopt_prophet-0.1.1.tar", max compression
```

## Comparing `hyperopt_prophet-0.1.0.tar` & `hyperopt_prophet-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1083 2023-07-21 05:05:18.611979 hyperopt_prophet-0.1.0/LICENSE
--rw-r--r--   0        0        0      980 2023-07-21 05:05:18.611979 hyperopt_prophet-0.1.0/README.md
--rw-r--r--   0        0        0      113 2023-07-21 05:05:18.615979 hyperopt_prophet-0.1.0/hyperopt_prophet/__init__.py
--rw-r--r--   0        0        0      195 2023-07-21 05:05:18.615979 hyperopt_prophet-0.1.0/hyperopt_prophet/hyperopt_prophet.py
--rw-r--r--   0        0        0     5047 2023-07-21 05:05:18.615979 hyperopt_prophet-0.1.0/hyperopt_prophet/inference.py
--rw-r--r--   0        0        0    21526 2023-07-21 05:05:18.615979 hyperopt_prophet-0.1.0/hyperopt_prophet/model.py
--rw-r--r--   0        0        0     9919 2023-07-21 05:05:18.615979 hyperopt_prophet-0.1.0/hyperopt_prophet/training.py
--rw-r--r--   0        0        0     4714 2023-07-21 05:05:18.615979 hyperopt_prophet-0.1.0/hyperopt_prophet/utils.py
--rw-r--r--   0        0        0       85 2023-07-21 05:05:18.615979 hyperopt_prophet-0.1.0/main.py
--rw-r--r--   0        0        0      793 2023-07-21 05:05:18.615979 hyperopt_prophet-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1889 1970-01-01 00:00:00.000000 hyperopt_prophet-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/LICENSE
+-rw-r--r--   0        0        0      980 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/README.md
+-rw-r--r--   0        0        0      113 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/hyperopt_prophet/__init__.py
+-rw-r--r--   0        0        0      204 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/hyperopt_prophet/hyperopt_prophet.py
+-rw-r--r--   0        0        0     5047 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/hyperopt_prophet/inference.py
+-rw-r--r--   0        0        0    21410 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/hyperopt_prophet/model.py
+-rw-r--r--   0        0        0      198 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/hyperopt_prophet/training.env
+-rw-r--r--   0        0        0    10032 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/hyperopt_prophet/training.py
+-rw-r--r--   0        0        0     4714 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/hyperopt_prophet/utils.py
+-rw-r--r--   0        0        0       85 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/main.py
+-rw-r--r--   0        0        0      843 2023-07-26 01:16:38.929116 hyperopt_prophet-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2033 1970-01-01 00:00:00.000000 hyperopt_prophet-0.1.1/PKG-INFO
```

### Comparing `hyperopt_prophet-0.1.0/LICENSE` & `hyperopt_prophet-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.0/README.md` & `hyperopt_prophet-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.0/hyperopt_prophet/inference.py` & `hyperopt_prophet-0.1.1/hyperopt_prophet/inference.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.0/hyperopt_prophet/model.py` & `hyperopt_prophet-0.1.1/hyperopt_prophet/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,31 @@
+import logging
 from abc import ABC, abstractmethod
-from typing import Dict, List, Optional, Union
+from enum import Enum
+from functools import partial
+from typing import Any, Dict, List, Optional, Union
 
 import cloudpickle
+import hyperopt
 import mlflow
+import numpy as np
 import pandas as pd
 import prophet
+from hyperopt import SparkTrials, Trials, fmin
 from mlflow.exceptions import MlflowException
 from mlflow.models.signature import ModelSignature, infer_signature
 from mlflow.protos.databricks_pb2 import INVALID_PARAMETER_VALUE
 from mlflow.utils.environment import _mlflow_conda_env
-from utils import OFFSET_ALIAS_MAP
+from prophet import Prophet
+from prophet.diagnostics import cross_validation, performance_metrics
+from prophet.serialize import model_to_json
+
+from .utils import OFFSET_ALIAS_MAP, generate_cutoffs, get_validation_horizon
+
+logging.getLogger().setLevel(logging.CRITICAL)
 
 
 class ForecastModel(ABC, mlflow.pyfunc.PythonModel):
     @abstractmethod
     def __init__(self):
         super().__init__()
 
@@ -354,32 +366,14 @@
     Log the model to mlflow
     :param prophet_model: Prophet model wrapper
     :param sample_input: sample input Dataframes for model inference
     """
     mlflow_forecast_log_model(prophet_model, sample_input)
 
 
-import logging
-from abc import ABC
-from enum import Enum
-from functools import partial
-from typing import Any, Dict, List, Optional
-
-import hyperopt
-import numpy as np
-import pandas as pd
-from hyperopt import SparkTrials, Trials, fmin
-from prophet import Prophet
-from prophet.diagnostics import cross_validation, performance_metrics
-from prophet.serialize import model_to_json
-from utils import OFFSET_ALIAS_MAP, generate_cutoffs, get_validation_horizon
-
-logging.getLogger().setLevel(logging.CRITICAL)
-
-
 class ProphetHyperParams(Enum):
     CHANGEPOINT_PRIOR_SCALE = "changepoint_prior_scale"
     SEASONALITY_PRIOR_SCALE = "seasonality_prior_scale"
     HOLIDAYS_PRIOR_SCALE = "holidays_prior_scale"
     SEASONALITY_MODE = "seasonality_mode"
```

### Comparing `hyperopt_prophet-0.1.0/hyperopt_prophet/training.py` & `hyperopt_prophet-0.1.1/hyperopt_prophet/training.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 import mlflow.prophet
 
 # import mlflow.spark
 import pandas as pd
 from dotenv import load_dotenv
 from hyperopt import hp
 from mlflowops import MLFlowOps
-from model import (
+from pydantic import BaseModel
+
+from .model import (
     MultiSeriesProphetModel,
     ProphetHyperoptEstimator,
     mlflow_prophet_log_model,
 )
-from pydantic import BaseModel
-from utils import get_plotly_forecast, plotly_fig2pil
+from .utils import get_plotly_forecast, plotly_fig2pil
 
 warnings.filterwarnings("ignore")
 
 
 def prophet_hyperopt_training(train_data):
     this_module_path = Path(__file__).parent.resolve()
     load_dotenv(f"{this_module_path}/training.env")
@@ -40,15 +41,15 @@
         "base_model_name": os.environ.get("base_model_name", "prohet_hyperopt"),
         "is_parallel": os.environ.get("is_parallel", "False"),
     }
     training_params = ProphetTrainingParams(**training_params)
 
     return ProphetHyperOptTrainer(
         training_data=train_data, training_params=training_params
-    ).train()
+    ).fit()
 
 
 class ProphetTrainingParams(BaseModel):
     """
     Initialization
     :param horizon: Number of periods to forecast forward
     :param frequency_unit: Frequency of the time series
@@ -109,14 +110,15 @@
         ),
         "seasonality_prior_scale": hp.loguniform("seasonality_prior_scale", -10.9, 5.3),
         "holidays_prior_scale": hp.loguniform("holidays_prior_scale", -10.9, 5.3),
         "seasonality_mode": hp.choice(
             "seasonality_mode", ["additive", "multiplicative"]
         ),
     }
+    use_mlflow: bool = False
 
     class Config:
         arbitrary_types_allowed = True
 
 
 class ProphetHyperOptTrainer:
     def __init__(
@@ -135,126 +137,136 @@
             sorting_metric=f"metrics.val_{self.training_params.loss_metric}",
             ascending=True,
         )
         mlops.check_model_improvement_and_transition_in_training_loop(
             training_loss, training_run_id
         )
 
-    def train(self):
-        with mlflow.start_run(
-            experiment_id=self.training_params.experiment_id,
-            run_name=f"prophet_{self.ts_id}",
-        ) as mlflow_run:
-            hyperopt_estim = ProphetHyperoptEstimator(
-                horizon=self.training_params.horizon,
-                frequency_unit=self.training_params.unit,
-                metric=self.training_params.loss_metric,
-                interval_width=self.training_params.interval_width,  # type: ignore
-                country_holidays=self.training_params.country_holidays,
-                search_space=self.training_params.search_space,
-                num_folds=self.training_params.num_folds,
-                max_eval=self.training_params.max_eval,
-                trial_timeout=self.training_params.trial_timeout,
-                is_parallel=self.training_params.is_parallel,
-                random_state=self.training_params.random_state,
-                # **{'uncertainty_samples': False}
-                # regressors=self.training_params.regressors,
-                # prophet_kwargs=self.training_params.prophet_kwargs,
-            )
-
-            result = hyperopt_estim.fit(self.training_data)
-            result["ts_id"] = self.ts_id
-            result["start_time"] = pd.Timestamp(self.training_data["ds"].min())
-            result["end_time"] = pd.Timestamp(self.training_data["ds"].max())
-
-            # Log the metrics to mlflow
-            avg_metrics = (
-                result[["mse", "rmse", "mae", "mape", "mdape", "smape", "coverage"]]
-                .mean()
-                .to_frame(name="mean_metrics")
-                .reset_index()
-            )
-            avg_metrics["index"] = "val_" + avg_metrics["index"].astype(str)
-            avg_metrics.set_index("index", inplace=True)
-
-            # Create mlflow prophet model
-            model_json = (
-                result[["ts_id", "model_json"]]
-                .set_index("ts_id")
-                .to_dict()["model_json"]
-            )
-            start_time = (
-                result[["ts_id", "start_time"]]
-                .set_index("ts_id")
-                .to_dict()["start_time"]
-            )
-            end_time = (
-                result[["ts_id", "end_time"]].set_index("ts_id").to_dict()["end_time"]
-            )
-            end_history_time = max(end_time.values())
-
-            prophet_model = MultiSeriesProphetModel(
-                model_json,
-                start_time,
-                end_history_time,
-                self.training_params.horizon,
-                self.training_params.unit,
-                self.training_params.time_col,
-                self.training_params.id_cols,
-            )
-
-            # Generate sample input dataframe
-            sample_input = self.training_data.head(20)
-            sample_input["ds"] = pd.to_datetime(sample_input["ds"])
-            sample_input.drop(columns=["y"], inplace=True)
-
-            mlflow_prophet_log_model(prophet_model, sample_input=sample_input)
-
-            model_dict = json.loads(model_json[list(model_json.keys())[0]])
-            for model_key in model_dict:
-                if model_key not in [
-                    "changepoints",
-                    "history_dates",
-                    "train_holiday_names",
-                    "changepoints_t",
-                    "history",
-                    "train_component_cols",
-                    "params",
-                ]:
-                    mlflow.log_param(model_key, model_dict[model_key])
-
-            for key in self.training_params.dict():
-                mlflow.log_param(key, self.training_params.dict()[key])
-
-            mlflow.log_param("series_end_time", result["end_time"].iloc[0])
-            mlflow.log_param("series_start_time", result["start_time"].iloc[0])
-            mlflow.log_metrics(avg_metrics.to_dict()["mean_metrics"])
-
-            prediction = prophet_model.predict_timeseries(
-                horizon=self.training_params.horizon, include_history=True
-            )
-
-            id_model = prophet_model.model(self.ts_id)  # type: ignore
-
-            # history = id_model.history
-
-            fig = get_plotly_forecast(id_model, prediction)
-
-            mlflow.log_image(image=plotly_fig2pil(fig), artifact_file="forecast.png")
-
-            training_loss = result[self.training_params.loss_metric].iloc[0]
-            training_run_id = mlflow_run.info.run_id
-
-            result["run_id"] = training_run_id
-
-            # get the start and end times for the run
-            run_start_time = mlflow_run.info.start_time
-
-            # calculate the duration of the run in seconds
-            result["training_duration"] = round(time() * 1000) - run_start_time
-
-            # Register the model
-            self.register_model(
-                training_loss=training_loss, training_run_id=training_run_id
-            )
+    def training(self):
+        hyperopt_estim = ProphetHyperoptEstimator(
+            horizon=self.training_params.horizon,
+            frequency_unit=self.training_params.unit,
+            metric=self.training_params.loss_metric,
+            interval_width=self.training_params.interval_width,  # type: ignore
+            country_holidays=self.training_params.country_holidays,
+            search_space=self.training_params.search_space,
+            num_folds=self.training_params.num_folds,
+            max_eval=self.training_params.max_eval,
+            trial_timeout=self.training_params.trial_timeout,
+            is_parallel=self.training_params.is_parallel,
+            random_state=self.training_params.random_state,
+            # **{'uncertainty_samples': False}
+            # regressors=self.training_params.regressors,
+            # prophet_kwargs=self.training_params.prophet_kwargs,
+        )
+
+        result = hyperopt_estim.fit(self.training_data)
+        result["ts_id"] = self.ts_id
+        result["start_time"] = pd.Timestamp(self.training_data["ds"].min())
+        result["end_time"] = pd.Timestamp(self.training_data["ds"].max())
+
+        # Log the metrics to mlflow
+        avg_metrics = (
+            result[["mse", "rmse", "mae", "mape", "mdape", "smape", "coverage"]]
+            .mean()
+            .to_frame(name="mean_metrics")
+            .reset_index()
+        )
+        avg_metrics["index"] = "val_" + avg_metrics["index"].astype(str)
+        avg_metrics.set_index("index", inplace=True)
+
+        # Create mlflow prophet model
+        model_json = (
+            result[["ts_id", "model_json"]].set_index("ts_id").to_dict()["model_json"]
+        )
+        start_time = (
+            result[["ts_id", "start_time"]].set_index("ts_id").to_dict()["start_time"]
+        )
+        end_time = (
+            result[["ts_id", "end_time"]].set_index("ts_id").to_dict()["end_time"]
+        )
+        end_history_time = max(end_time.values())
+
+        prophet_model = MultiSeriesProphetModel(
+            model_json,
+            start_time,
+            end_history_time,
+            self.training_params.horizon,
+            self.training_params.unit,
+            self.training_params.time_col,
+            self.training_params.id_cols,
+        )
+
+        prediction = prophet_model.predict_timeseries(
+            horizon=self.training_params.horizon, include_history=True
+        )
+
+        return prophet_model, model_json, result, avg_metrics, prediction
+
+    def fit_with_mlflow(self, mlflow_run):
+        prophet_model, model_json, result, avg_metrics, prediction = self.training()
+
+        # Generate sample input dataframe
+        sample_input = self.training_data.head(20)
+        sample_input["ds"] = pd.to_datetime(sample_input["ds"])
+        sample_input.drop(columns=["y"], inplace=True)
+
+        model_dict = json.loads(model_json[list(model_json.keys())[0]])
+
+        mlflow_prophet_log_model(prophet_model, sample_input=sample_input)
+
+        for model_key in model_dict:
+            if model_key not in [
+                "changepoints",
+                "history_dates",
+                "train_holiday_names",
+                "changepoints_t",
+                "history",
+                "train_component_cols",
+                "params",
+            ]:
+                mlflow.log_param(model_key, model_dict[model_key])
+
+        for key in self.training_params.dict():
+            mlflow.log_param(key, self.training_params.dict()[key])
+
+        mlflow.log_param("series_end_time", result["end_time"].iloc[0])
+        mlflow.log_param("series_start_time", result["start_time"].iloc[0])
+        mlflow.log_metrics(avg_metrics.to_dict()["mean_metrics"])
+
+        id_model = prophet_model.model(self.ts_id)  # type: ignore
+
+        # history = id_model.history
+
+        fig = get_plotly_forecast(id_model, prediction)
+
+        mlflow.log_image(image=plotly_fig2pil(fig), artifact_file="forecast.png")
+
+        training_loss = result[self.training_params.loss_metric].iloc[0]
+        training_run_id = mlflow_run.info.run_id
+
+        result["run_id"] = training_run_id
+
+        # get the start and end times for the run
+        run_start_time = mlflow_run.info.start_time
+
+        # calculate the duration of the run in seconds
+        result["training_duration"] = round(time() * 1000) - run_start_time
+
+        # Register the model
+        self.register_model(
+            training_loss=training_loss, training_run_id=training_run_id
+        )
+
+        return result[self.training_params.result_columns]
+
+    def fit(self):
+        if self.training_params.use_mlflow:
+            with mlflow.start_run(
+                experiment_id=self.training_params.experiment_id,
+                run_name=f"prophet_{self.ts_id}",
+            ) as mlflow_run:
+                return self.fit_with_mlflow(mlflow_run)
+        else:
+            prophet_model, model_json, result, avg_metrics, prediction = self.training()
 
             return result[self.training_params.result_columns]
```

### Comparing `hyperopt_prophet-0.1.0/hyperopt_prophet/utils.py` & `hyperopt_prophet-0.1.1/hyperopt_prophet/utils.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.0/pyproject.toml` & `hyperopt_prophet-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [tool.poetry]
 name = "hyperopt-prophet"
-version = "0.1.0"
+version = "0.1.1"
 description = "Integration of prophet forecasting with hyperopt, mlflow"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "hyperopt_prophet"},
     {include = "main.py"}
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 pandas = "^2.0.3"
-pydantic = "^2.0.3"
+pydantic = "^2.1.0"
+pydantic-settings = "^2.0.2"
 hyperopt = "^0.2.7"
 mlflow = "^2.5.0"
 python-dotenv = "^1.0.0"
 cloudpickle = "^2.2.1"
 cython = "^3.0.0"
-prophet = "^1.1.4"
-mlflowops = '^0.1.1'
+pystan = "^2.19.1.1"
+prophet = "^1.0.0"
+mlflowops = '^0.1.2'
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.4.0"
 pylint = "^2.17.4"
```

### Comparing `hyperopt_prophet-0.1.0/PKG-INFO` & `hyperopt_prophet-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: hyperopt-prophet
-Version: 0.1.0
+Version: 0.1.1
 Summary: Integration of prophet forecasting with hyperopt, mlflow
 License: MIT
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
 Requires-Dist: cython (>=3.0.0,<4.0.0)
 Requires-Dist: hyperopt (>=0.2.7,<0.3.0)
 Requires-Dist: mlflow (>=2.5.0,<3.0.0)
-Requires-Dist: mlflowops (>=0.1.1,<0.2.0)
+Requires-Dist: mlflowops (>=0.1.2,<0.2.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
-Requires-Dist: prophet (>=1.1.4,<2.0.0)
-Requires-Dist: pydantic (>=2.0.3,<3.0.0)
+Requires-Dist: prophet (>=1.0.0,<2.0.0)
+Requires-Dist: pydantic (>=2.1.0,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.0.2,<3.0.0)
+Requires-Dist: pystan (>=2.19.1.1,<3.0.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Hyperopt Prophet
 
 **Integration of prophet forecasting with hyperopt, mlflow**
 This implementation is based on the [Databricks AutoML](https://github.com/databricks/automl) repository.
```

