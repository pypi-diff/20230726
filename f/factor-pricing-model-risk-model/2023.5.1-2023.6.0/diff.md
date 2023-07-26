# Comparing `tmp/factor_pricing_model_risk_model-2023.5.1.tar.gz` & `tmp/factor_pricing_model_risk_model-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factor_pricing_model_risk_model-2023.5.1.tar", max compression
+gzip compressed data, was "factor_pricing_model_risk_model-2023.6.0.tar", max compression
```

## Comparing `factor_pricing_model_risk_model-2023.5.1.tar` & `factor_pricing_model_risk_model-2023.6.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1078 2023-06-23 15:18:55.250002 factor_pricing_model_risk_model-2023.5.1/LICENSE
--rw-r--r--   0        0        0     7067 2023-06-23 15:18:55.250002 factor_pricing_model_risk_model-2023.5.1/README.md
--rw-r--r--   0        0        0     2642 2023-06-23 15:19:00.942463 factor_pricing_model_risk_model-2023.5.1/pyproject.toml
--rw-r--r--   0        0        0      150 2023-06-23 15:19:00.906460 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/__init__.py
--rw-r--r--   0        0        0      253 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/accuracy/__init__.py
--rw-r--r--   0        0        0     3410 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/accuracy/bias.py
--rw-r--r--   0        0        0     5663 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/accuracy/value_at_risk.py
--rw-r--r--   0        0        0      113 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/config.py
--rw-r--r--   0        0        0     4181 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/cov_estimator.py
--rw-r--r--   0        0        0        0 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/dataset/__init__.py
--rw-r--r--   0        0        0     3255 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/dataset/crypto.py
--rw-r--r--   0        0        0       46 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/engine/__init__.py
--rw-r--r--   0        0        0      183 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/engine/numpy.py
--rw-r--r--   0        0        0    11187 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/factor_risk_model.py
--rw-r--r--   0        0        0     7438 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/pipeline/__init__.py
--rw-r--r--   0        0        0      621 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/pipeline/portfolio.py
--rw-r--r--   0        0        0      796 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/pipeline/returns.py
--rw-r--r--   0        0        0        0 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/py.typed
--rw-r--r--   0        0        0       59 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/regressor/__init__.py
--rw-r--r--   0        0        0     1138 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/regressor/ewls.py
--rw-r--r--   0        0        0     2514 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/regressor/wls.py
--rw-r--r--   0        0        0     3251 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/risk_model.py
--rw-r--r--   0        0        0     5657 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/rolling_factor_risk_model.py
--rw-r--r--   0        0        0     5097 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/rolling_risk_model.py
--rw-r--r--   0        0        0       59 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/statistical/__init__.py
--rw-r--r--   0        0        0     3932 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/statistical/apca.py
--rw-r--r--   0        0        0     4728 2023-06-23 15:18:55.354010 factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/statistical/pca.py
--rw-r--r--   0        0        0     8750 1970-01-01 00:00:00.000000 factor_pricing_model_risk_model-2023.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-26 16:40:31.459883 factor_pricing_model_risk_model-2023.6.0/LICENSE
+-rw-r--r--   0        0        0     7586 2023-07-26 16:40:31.459883 factor_pricing_model_risk_model-2023.6.0/README.md
+-rw-r--r--   0        0        0     2642 2023-07-26 16:40:35.771986 factor_pricing_model_risk_model-2023.6.0/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-07-26 16:40:35.739985 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/__init__.py
+-rw-r--r--   0        0        0      253 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/accuracy/__init__.py
+-rw-r--r--   0        0        0     3410 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/accuracy/bias.py
+-rw-r--r--   0        0        0     5663 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/accuracy/value_at_risk.py
+-rw-r--r--   0        0        0      113 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/config.py
+-rw-r--r--   0        0        0     4181 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/cov_estimator.py
+-rw-r--r--   0        0        0        0 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/dataset/__init__.py
+-rw-r--r--   0        0        0     3255 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/dataset/crypto.py
+-rw-r--r--   0        0        0     4210 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/engine.py
+-rw-r--r--   0        0        0    11187 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/factor_risk_model.py
+-rw-r--r--   0        0        0     7438 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/pipeline/__init__.py
+-rw-r--r--   0        0        0      621 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/pipeline/portfolio.py
+-rw-r--r--   0        0        0      796 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/pipeline/returns.py
+-rw-r--r--   0        0        0        0 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/py.typed
+-rw-r--r--   0        0        0       59 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/regressor/__init__.py
+-rw-r--r--   0        0        0     1138 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/regressor/ewls.py
+-rw-r--r--   0        0        0     2514 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/regressor/wls.py
+-rw-r--r--   0        0        0     3092 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/risk_model.py
+-rw-r--r--   0        0        0     5657 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/rolling_factor_risk_model.py
+-rw-r--r--   0        0        0     5097 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/rolling_risk_model.py
+-rw-r--r--   0        0        0       59 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/statistical/__init__.py
+-rw-r--r--   0        0        0     3926 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/statistical/apca.py
+-rw-r--r--   0        0        0     4722 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/statistical/pca.py
+-rw-r--r--   0        0        0     9269 1970-01-01 00:00:00.000000 factor_pricing_model_risk_model-2023.6.0/PKG-INFO
```

### Comparing `factor_pricing_model_risk_model-2023.5.1/LICENSE` & `factor_pricing_model_risk_model-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.5.1/README.md` & `factor_pricing_model_risk_model-2023.6.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -110,18 +110,42 @@
 ```
 risk_model.transform(y=model_returns)
 
 cov = risk_model.cov()
 corr = risk_model.corr()
 ```
 
-The following features will be supported in the near future
+Alternatively, covariance estimator `CovarianceEstimator`
+(or `RollingCovarianceEstimator` in a rolling basis) provides advanced
+features, including covariance shrinkage and variance adjustment.
+The following shrinkage methods are supported
+
+- Constant
+- Ledoit Wolf shrinkage (Q3 2023)
+- Oracle Approximating shrinkage (Q3 2023)
 
-- Covariance shrinkage
-- Covariance estimation from returns
+For example, to construct a rolling covariance estimator with constant
+shrinkage delta 0.2,
+
+```
+from fpm_risk_model import RollingCovarianceEstimator
+
+estimator = RollingCovarianceEstimator(
+  rolling_risk_model,
+  shrinkage_method="constant",
+  delta=0.2
+)
+```
+
+then the covariance can be computed with the rolling risk model and
+volatilities with better forecasting accuracy
+
+```
+estimator.cov(volatility=another_estimated_vol)
+```
 
 For further details, please refer to the [section](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/risk_model/covariance.html) in the documentation.
 
 ## Tracking risk model accuracy
 
 The library also focuses on the predictability interpretation of the risk
 model, and provides a few benchmarks to examine the following metrics
@@ -145,18 +169,16 @@
 )
 ```
 
 ## Roadmap
 
 The following major features will be enhanced
 
-- Factor exposures computation from factor returns (Q2 2023)
-- Shrinking covariance (Q2 2023)
-- Exponential decay weighted least squares regression (Q3 2023)
-- Multiple types of running engine, e.g. Tensorflow (Q3 2023)
-- Multi-asset class factor model (Q3 2023)
+- Factor exposures computation from factor returns (Q3 2023)
+- Shrinking covariance (Q3 2023)
+- Multi-asset class factor model (Q4 2023)
 - Fundamental type risk model (Q4 2023)
 
 ## Contribution
 
 All levels of contributions are welcomed. Please refer to the [contributing](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/contributing.html)
 section for development and release guidelines.
```

#### html2text {}

```diff
@@ -30,31 +30,37 @@
 risk_model.transform(y=model_returns) ``` For further details, please refer to
 the [section](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/
 risk_model/factor_risk_model.html) in the documentation. ## Covariance
 estimation Currently, covariance estimation is supported in factor risk model,
 and the estimation depends on the fitted results. For example, a risk model
 transformed by model universe returns can derive the pairwise covariance and
 correlation for the model universe. ``` risk_model.transform(y=model_returns)
-cov = risk_model.cov() corr = risk_model.corr() ``` The following features will
-be supported in the near future - Covariance shrinkage - Covariance estimation
-from returns For further details, please refer to the [section](https://factor-
-pricing-model-risk-model.readthedocs.io/en/latest/risk_model/covariance.html)
-in the documentation. ## Tracking risk model accuracy The library also focuses
-on the predictability interpretation of the risk model, and provides a few
-benchmarks to examine the following metrics - [Bias](https://factor-pricing-
-model-risk-model.readthedocs.io/en/latest/accuracy/bias.html) - [Value at Risk
-(VaR)](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/
-accuracy/value_at_risk.html) For example, to examine the bias statistics of a
-risk model regarding an equally weighted portfolio (of which its weights are
-denoted as `weights`), pass the instrument observed returns (denoted as
-`returns`), and either a rolling risk model (to compute the volatility
-forecast) or a time series of volatility forecasts. ``` from
-fpm_risk_model.accuracy import compute_bias_statistics compute_bias_statistics
-( X=returns, weights=weights, window=window ... ) ``` ## Roadmap The following
-major features will be enhanced - Factor exposures computation from factor
-returns (Q2 2023) - Shrinking covariance (Q2 2023) - Exponential decay weighted
-least squares regression (Q3 2023) - Multiple types of running engine, e.g.
-Tensorflow (Q3 2023) - Multi-asset class factor model (Q3 2023) - Fundamental
-type risk model (Q4 2023) ## Contribution All levels of contributions are
-welcomed. Please refer to the [contributing](https://factor-pricing-model-risk-
-model.readthedocs.io/en/latest/contributing.html) section for development and
-release guidelines.
+cov = risk_model.cov() corr = risk_model.corr() ``` Alternatively, covariance
+estimator `CovarianceEstimator` (or `RollingCovarianceEstimator` in a rolling
+basis) provides advanced features, including covariance shrinkage and variance
+adjustment. The following shrinkage methods are supported - Constant - Ledoit
+Wolf shrinkage (Q3 2023) - Oracle Approximating shrinkage (Q3 2023) For
+example, to construct a rolling covariance estimator with constant shrinkage
+delta 0.2, ``` from fpm_risk_model import RollingCovarianceEstimator estimator
+= RollingCovarianceEstimator( rolling_risk_model, shrinkage_method="constant",
+delta=0.2 ) ``` then the covariance can be computed with the rolling risk model
+and volatilities with better forecasting accuracy ``` estimator.cov
+(volatility=another_estimated_vol) ``` For further details, please refer to the
+[section](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/
+risk_model/covariance.html) in the documentation. ## Tracking risk model
+accuracy The library also focuses on the predictability interpretation of the
+risk model, and provides a few benchmarks to examine the following metrics -
+[Bias](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/
+accuracy/bias.html) - [Value at Risk (VaR)](https://factor-pricing-model-risk-
+model.readthedocs.io/en/latest/accuracy/value_at_risk.html) For example, to
+examine the bias statistics of a risk model regarding an equally weighted
+portfolio (of which its weights are denoted as `weights`), pass the instrument
+observed returns (denoted as `returns`), and either a rolling risk model (to
+compute the volatility forecast) or a time series of volatility forecasts. ```
+from fpm_risk_model.accuracy import compute_bias_statistics
+compute_bias_statistics( X=returns, weights=weights, window=window ... ) ``` ##
+Roadmap The following major features will be enhanced - Factor exposures
+computation from factor returns (Q3 2023) - Shrinking covariance (Q3 2023) -
+Multi-asset class factor model (Q4 2023) - Fundamental type risk model (Q4
+2023) ## Contribution All levels of contributions are welcomed. Please refer to
+the [contributing](https://factor-pricing-model-risk-model.readthedocs.io/en/
+latest/contributing.html) section for development and release guidelines.
```

### Comparing `factor_pricing_model_risk_model-2023.5.1/pyproject.toml` & `factor_pricing_model_risk_model-2023.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "factor-pricing-model-risk-model"
-version = "2023.5.1"
+version = "2023.6.0"
 description = "Package to build risk models for factor pricing model"
 authors = ["Factor Pricing Model <factor.pricing.model@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/factorpricingmodel/factor-pricing-model-risk-model"
 documentation = "https://factor-pricing-model-risk-model.readthedocs.io"
 classifiers = [
@@ -25,15 +25,15 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 
 # Documentation Dependencies
 Sphinx = {version = "^5.0", optional = true}
 insipid-sphinx-theme = {version = "^0.3.6", optional = true}
 myst-parser = {version = "^0.18", optional = true}
-pandas = ">=1.3.5,<1.4.0"
+pandas = ">=1.3.5,<3.0.0"
 scikit-learn = "^1.1.3"
 tqdm = "^4.64.1"
 pydantic = "^1.10.4"
 
 [tool.poetry.extras]
 docs = [
     "myst-parser",
```

### Comparing `factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/accuracy/bias.py` & `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/accuracy/bias.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/accuracy/value_at_risk.py` & `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/accuracy/value_at_risk.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/cov_estimator.py` & `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/cov_estimator.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/dataset/crypto.py` & `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/dataset/crypto.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/factor_risk_model.py` & `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/factor_risk_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import json
 from os.path import join
 from typing import Optional
 
 from numpy import any, diag_indices_from, nan, ndarray
 from pandas import DataFrame, Series
 
+from .engine import NumpyEngine
 from .regressor import WLS
 from .risk_model import RiskModel
 
+np = NumpyEngine()
+
 
 class FactorRiskModel(RiskModel):
     """
     Factor Risk Model.
 
     The class is an abstract class to fit the factor risk model.
 
@@ -133,26 +136,25 @@
           Degrees of freedom.
 
         Returns
         -------
         ndarray
           Specific variances of the instruments.
         """
-        eg = self._engine
         T = self._residual_returns.shape[0]
         residual_returns = self._residual_returns
         if isinstance(self._residual_returns, DataFrame):
             residual_returns = residual_returns.values
 
         if weights is not None:
-            r_mean = eg.mean(residual_returns * weights[:, eg.newaxis], axis=0)
+            r_mean = np.mean(residual_returns * weights[:, np.newaxis], axis=0)
             variances = (residual_returns - r_mean) ** 2
-            variances *= weights[:, eg.newaxis]
+            variances *= weights[:, np.newaxis]
         else:
-            r_mean = eg.mean(residual_returns, axis=0)
+            r_mean = np.mean(residual_returns, axis=0)
             variances = (residual_returns - r_mean) ** 2
 
         variances = sum(variances) / (T - ddof)
 
         if isinstance(self._residual_returns, DataFrame):
             variances = Series(variances, index=self._residual_returns.columns)
 
@@ -238,29 +240,28 @@
 
         Returns
         -------
         numpy.ndarray
             A square pairwise covariance matrix which its
             diagonal entries are the variances.
         """
-        eg = self._engine
         B = self._factor_exposures
         F = self._factor_returns
         if F is None:
             raise ValueError("Factor return cannot be None")
         elif isinstance(F, DataFrame):
             F = F.values
 
         W = None
         T = F.shape[0]
         if halflife is not None:
-            W = eg.array([2 ** (-(T - 1 - t) / halflife) for t in range(0, T)])
-            F = F * (W[:, eg.newaxis] ** 0.5)
+            W = np.array([2 ** (-(T - 1 - t) / halflife) for t in range(0, T)])
+            F = F * (W[:, np.newaxis] ** 0.5)
 
-        F = F - eg.mean(F, axis=0)
+        F = F - np.mean(F, axis=0)
         factor_covariances = (F.T @ F) / (T - ddof)
         specific_variances = self.specific_variances(weights=W, ddof=ddof)
 
         R = specific_variances
         if isinstance(B, DataFrame):
             instruments = self._factor_exposures.columns
             B = B.values
```

### Comparing `factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/pipeline/__init__.py` & `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/pipeline/portfolio.py` & `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/pipeline/portfolio.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/pipeline/returns.py` & `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/pipeline/returns.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/regressor/ewls.py` & `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/regressor/ewls.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/regressor/wls.py` & `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/regressor/wls.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/risk_model.py` & `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/risk_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from abc import ABC, abstractmethod
-from typing import Any, Union
+from typing import Union
 
 from numpy import diagonal, ndarray, sqrt
 from pandas import DataFrame, Series
 
 from .config import Config
 from .engine import NumpyEngine
 
+np = NumpyEngine()
+
 
 class RiskModelConfig(Config):
     """
     Risk model configuration.
 
     Parameters
     ----------
@@ -29,31 +31,25 @@
 
     The class is an abstract class to compute covariance and other
     related metrics.
     """
 
     ConfigClass = RiskModelConfig
 
-    def __init__(
-        self, engine: Any = None, show_all_instruments: bool = False, **kwargs
-    ):
+    def __init__(self, show_all_instruments: bool = False, **kwargs):
         """
         Constructor.
 
         Parameters
         ----------
-        engine : Engine object.
-            Engine used in computation.
-
         show_all_instruments : bool.
             Indicate whether to show all instruments. Default is False.
             If True, the instruments outside of the universe in each
             period may not be filtered out.
         """
-        self._engine = engine or NumpyEngine()
         self._config = self.ConfigClass(
             show_all_instruments=show_all_instruments, **kwargs
         )
 
     @property
     def config(self):
         """
@@ -95,15 +91,15 @@
         Returns
         -------
         numpy.ndarray
             A square pairwise correlation matrix which its
             diagonal entries are all ones.
         """
         cov = self.cov(**kwargs)
-        vol = self._engine.sqrt(self._engine.diagonal(cov))
+        vol = np.sqrt(np.diagonal(cov))
         return ((cov / vol).T / vol).T
 
     def asdict(self):
         """
         Returns a dict representation of the object.
         """
         return self.config.dict()
```

### Comparing `factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/rolling_factor_risk_model.py` & `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/rolling_factor_risk_model.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/rolling_risk_model.py` & `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/rolling_risk_model.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/statistical/apca.py` & `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/statistical/apca.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from typing import Optional, Union
 
 from numpy import ndarray
 from pandas import DataFrame
 from sklearn.decomposition import PCA as sklearn_PCA
 
+from ..engine import NumpyEngine
 from ..factor_risk_model import FactorRiskModel
 from ..regressor import WLS
 
+np = NumpyEngine()
+
 
 class APCAConfig(FactorRiskModel.ConfigClass):
     """
     Asymptotic PCA statistics model configuration class.
 
 
     Parameters
@@ -72,25 +75,22 @@
         object
           The object itself.
         """
         # First convert all the numpy ndarray type first
         X_fit = self._to_numpy(X)
         N = X.shape[1]
 
-        # Initialize the engine
-        eg = self._engine
-
         # Normalize the instrument return by full history mean
         if self._config.demean:
-            X_mean = eg.array(eg.mean(X, axis=0))[eg.newaxis, :]
-            X_fit = eg.subtract(X_fit, X_mean)
+            X_mean = np.array(np.mean(X, axis=0))[np.newaxis, :]
+            X_fit = np.subtract(X_fit, X_mean)
 
         # Remove the instruments without any returns always
         # Select the instruments of which the returns are not always 0
-        X_reindex = ~eg.all(eg.abs(X_fit) < 1e-20, axis=0)
+        X_reindex = ~np.all(np.abs(X_fit) < 1e-20, axis=0)
         X_fit = X_fit[:, X_reindex]
 
         # Factor model - R = B @ F + residual_returns
         # Fit with skilearn PCA on the return matrix (T, N) in t-space
         self._model.fit(X_fit.T)
         # Eigenvectors
         U_m = self._model.components_
@@ -103,16 +103,16 @@
         wls = WLS()
         wls_result = wls.fit(X=F, y=X_fit)
         B = wls_result.beta
         residual_returns = wls_result.alpha
 
         # Fill back the instruments which don't have any returns
         # with 0.0 exposures and residual returns
-        B_reindex = eg.zeros((B.shape[0], N))
-        residual_returns_reindex = eg.zeros(X.shape)
+        B_reindex = np.zeros((B.shape[0], N))
+        residual_returns_reindex = np.zeros(X.shape)
         B_reindex[:, X_reindex] = B[:, :]
         residual_returns_reindex[:, X_reindex] = residual_returns[:, :]
         B = B_reindex
         residual_returns = residual_returns_reindex
 
         # Convert back to dataframe if necessary
         if isinstance(X, DataFrame):
```

### Comparing `factor_pricing_model_risk_model-2023.5.1/src/fpm_risk_model/statistical/pca.py` & `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/statistical/pca.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from typing import Optional, Union
 
 from numpy import ndarray
 from pandas import DataFrame, Series
 from sklearn.decomposition import PCA as sklearn_PCA
 
+from ..engine import NumpyEngine
 from ..factor_risk_model import FactorRiskModel
 from ..regressor import WLS
 
+np = NumpyEngine()
+
 
 class PCAConfig(FactorRiskModel.ConfigClass):
     """
     PCA statistics model configuration class.
 
 
     Parameters
@@ -82,54 +85,51 @@
         object
           The object itself.
         """
         # First convert all the numpy ndarray type first
         X_fit = self._to_numpy(X)
         weights_fit = self._to_numpy(weights)
 
-        # Initialize the engine
-        eg = self._engine
-
         # Normalize the instrument return by full history mean
         if self._config.demean:
-            X_mean = eg.array(eg.mean(X, axis=0))[eg.newaxis, :]
-            X_fit = eg.subtract(X_fit, X_mean)
+            X_mean = np.array(np.mean(X, axis=0))[np.newaxis, :]
+            X_fit = np.subtract(X_fit, X_mean)
 
         # Remove the instruments without any returns always
         if self._config.speedup:
             # Select the instruments of which the returns are not always 0
-            X_reindex = ~eg.all(eg.abs(X_fit) < 1e-20, axis=0)
+            X_reindex = ~np.all(np.abs(X_fit) < 1e-20, axis=0)
             X_fit = X_fit[:, X_reindex]
             if weights_fit is not None:
                 weights_fit = weights_fit[X_reindex]
 
         # Fit with skilearn PCA on the return matrix (T, N)
         self._model.fit(X_fit)
         # N is the number of instruments and T is the number of time frames
         T = X.shape[0]
         N = X.shape[1]
         # Dimension (n, N) where n is the number of instruments
         # Eigenvectors
         U_m = self._model.components_
         # Exposure matrix (n, N)
-        B = eg.multiply(
+        B = np.multiply(
             U_m,
-            eg.array(self._model.singular_values_ * eg.sqrt(T))[:, eg.newaxis],
+            np.array(self._model.singular_values_ * np.sqrt(T))[:, np.newaxis],
         )
         # Factor matrix (T, n)
         wls = WLS()
         wls_result = wls.fit(X=B.T, y=X_fit.T, weights=weights_fit)
         F = wls_result.beta.T
         residual_returns = wls_result.alpha.T
 
         # Fill back the instruments which don't have any returns
         # with 0.0 exposures and residual returns
         if self._config.speedup:
-            B_reindex = eg.zeros((B.shape[0], N))
-            residual_returns_reindex = eg.zeros(X.shape)
+            B_reindex = np.zeros((B.shape[0], N))
+            residual_returns_reindex = np.zeros(X.shape)
             B_reindex[:, X_reindex] = B[:, :]
             residual_returns_reindex[:, X_reindex] = residual_returns[:, :]
             B = B_reindex
             residual_returns = residual_returns_reindex
 
         # Convert back to dataframe if necessary
         if isinstance(X, DataFrame):
```

### Comparing `factor_pricing_model_risk_model-2023.5.1/PKG-INFO` & `factor_pricing_model_risk_model-2023.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factor-pricing-model-risk-model
-Version: 2023.5.1
+Version: 2023.6.0
 Summary: Package to build risk models for factor pricing model
 Home-page: https://github.com/factorpricingmodel/factor-pricing-model-risk-model
 License: MIT
 Author: Factor Pricing Model
 Author-email: factor.pricing.model@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs"
 Requires-Dist: insipid-sphinx-theme (>=0.3.6,<0.4.0) ; extra == "docs"
 Requires-Dist: myst-parser (>=0.18,<0.19) ; extra == "docs"
-Requires-Dist: pandas (>=1.3.5,<1.4.0)
+Requires-Dist: pandas (>=1.3.5,<3.0.0)
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Requires-Dist: scikit-learn (>=1.1.3,<2.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/factorpricingmodel/factor-pricing-model-risk-model/issues
 Project-URL: Changelog, https://github.com/factorpricingmodel/factor-pricing-model-risk-model/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://factor-pricing-model-risk-model.readthedocs.io
 Project-URL: Repository, https://github.com/factorpricingmodel/factor-pricing-model-risk-model
@@ -144,18 +144,42 @@
 ```
 risk_model.transform(y=model_returns)
 
 cov = risk_model.cov()
 corr = risk_model.corr()
 ```
 
-The following features will be supported in the near future
+Alternatively, covariance estimator `CovarianceEstimator`
+(or `RollingCovarianceEstimator` in a rolling basis) provides advanced
+features, including covariance shrinkage and variance adjustment.
+The following shrinkage methods are supported
 
-- Covariance shrinkage
-- Covariance estimation from returns
+- Constant
+- Ledoit Wolf shrinkage (Q3 2023)
+- Oracle Approximating shrinkage (Q3 2023)
+
+For example, to construct a rolling covariance estimator with constant
+shrinkage delta 0.2,
+
+```
+from fpm_risk_model import RollingCovarianceEstimator
+
+estimator = RollingCovarianceEstimator(
+  rolling_risk_model,
+  shrinkage_method="constant",
+  delta=0.2
+)
+```
+
+then the covariance can be computed with the rolling risk model and
+volatilities with better forecasting accuracy
+
+```
+estimator.cov(volatility=another_estimated_vol)
+```
 
 For further details, please refer to the [section](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/risk_model/covariance.html) in the documentation.
 
 ## Tracking risk model accuracy
 
 The library also focuses on the predictability interpretation of the risk
 model, and provides a few benchmarks to examine the following metrics
@@ -179,19 +203,17 @@
 )
 ```
 
 ## Roadmap
 
 The following major features will be enhanced
 
-- Factor exposures computation from factor returns (Q2 2023)
-- Shrinking covariance (Q2 2023)
-- Exponential decay weighted least squares regression (Q3 2023)
-- Multiple types of running engine, e.g. Tensorflow (Q3 2023)
-- Multi-asset class factor model (Q3 2023)
+- Factor exposures computation from factor returns (Q3 2023)
+- Shrinking covariance (Q3 2023)
+- Multi-asset class factor model (Q4 2023)
 - Fundamental type risk model (Q4 2023)
 
 ## Contribution
 
 All levels of contributions are welcomed. Please refer to the [contributing](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/contributing.html)
 section for development and release guidelines.
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: factor-pricing-model-risk-model Version: 2023.5.1
+Metadata-Version: 2.1 Name: factor-pricing-model-risk-model Version: 2023.6.0
 Summary: Package to build risk models for factor pricing model Home-page:
 https://github.com/factorpricingmodel/factor-pricing-model-risk-model License:
 MIT Author: Factor Pricing Model Author-email: factor.pricing.model@gmail.com
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Software Development :: Libraries Provides-Extra: docs Requires-Dist: Sphinx
 (>=5.0,<6.0) ; extra == "docs" Requires-Dist: insipid-sphinx-theme
 (>=0.3.6,<0.4.0) ; extra == "docs" Requires-Dist: myst-parser (>=0.18,<0.19) ;
-extra == "docs" Requires-Dist: pandas (>=1.3.5,<1.4.0) Requires-Dist: pydantic
+extra == "docs" Requires-Dist: pandas (>=1.3.5,<3.0.0) Requires-Dist: pydantic
 (>=1.10.4,<2.0.0) Requires-Dist: scikit-learn (>=1.1.3,<2.0.0) Requires-Dist:
 tqdm (>=4.64.1,<5.0.0) Project-URL: Bug Tracker, https://github.com/
 factorpricingmodel/factor-pricing-model-risk-model/issues Project-URL:
 Changelog, https://github.com/factorpricingmodel/factor-pricing-model-risk-
 model/blob/master/CHANGELOG.md Project-URL: Documentation, https://factor-
 pricing-model-risk-model.readthedocs.io Project-URL: Repository, https://
 github.com/factorpricingmodel/factor-pricing-model-risk-model Description-
@@ -52,31 +52,37 @@
 risk_model.transform(y=model_returns) ``` For further details, please refer to
 the [section](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/
 risk_model/factor_risk_model.html) in the documentation. ## Covariance
 estimation Currently, covariance estimation is supported in factor risk model,
 and the estimation depends on the fitted results. For example, a risk model
 transformed by model universe returns can derive the pairwise covariance and
 correlation for the model universe. ``` risk_model.transform(y=model_returns)
-cov = risk_model.cov() corr = risk_model.corr() ``` The following features will
-be supported in the near future - Covariance shrinkage - Covariance estimation
-from returns For further details, please refer to the [section](https://factor-
-pricing-model-risk-model.readthedocs.io/en/latest/risk_model/covariance.html)
-in the documentation. ## Tracking risk model accuracy The library also focuses
-on the predictability interpretation of the risk model, and provides a few
-benchmarks to examine the following metrics - [Bias](https://factor-pricing-
-model-risk-model.readthedocs.io/en/latest/accuracy/bias.html) - [Value at Risk
-(VaR)](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/
-accuracy/value_at_risk.html) For example, to examine the bias statistics of a
-risk model regarding an equally weighted portfolio (of which its weights are
-denoted as `weights`), pass the instrument observed returns (denoted as
-`returns`), and either a rolling risk model (to compute the volatility
-forecast) or a time series of volatility forecasts. ``` from
-fpm_risk_model.accuracy import compute_bias_statistics compute_bias_statistics
-( X=returns, weights=weights, window=window ... ) ``` ## Roadmap The following
-major features will be enhanced - Factor exposures computation from factor
-returns (Q2 2023) - Shrinking covariance (Q2 2023) - Exponential decay weighted
-least squares regression (Q3 2023) - Multiple types of running engine, e.g.
-Tensorflow (Q3 2023) - Multi-asset class factor model (Q3 2023) - Fundamental
-type risk model (Q4 2023) ## Contribution All levels of contributions are
-welcomed. Please refer to the [contributing](https://factor-pricing-model-risk-
-model.readthedocs.io/en/latest/contributing.html) section for development and
-release guidelines.
+cov = risk_model.cov() corr = risk_model.corr() ``` Alternatively, covariance
+estimator `CovarianceEstimator` (or `RollingCovarianceEstimator` in a rolling
+basis) provides advanced features, including covariance shrinkage and variance
+adjustment. The following shrinkage methods are supported - Constant - Ledoit
+Wolf shrinkage (Q3 2023) - Oracle Approximating shrinkage (Q3 2023) For
+example, to construct a rolling covariance estimator with constant shrinkage
+delta 0.2, ``` from fpm_risk_model import RollingCovarianceEstimator estimator
+= RollingCovarianceEstimator( rolling_risk_model, shrinkage_method="constant",
+delta=0.2 ) ``` then the covariance can be computed with the rolling risk model
+and volatilities with better forecasting accuracy ``` estimator.cov
+(volatility=another_estimated_vol) ``` For further details, please refer to the
+[section](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/
+risk_model/covariance.html) in the documentation. ## Tracking risk model
+accuracy The library also focuses on the predictability interpretation of the
+risk model, and provides a few benchmarks to examine the following metrics -
+[Bias](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/
+accuracy/bias.html) - [Value at Risk (VaR)](https://factor-pricing-model-risk-
+model.readthedocs.io/en/latest/accuracy/value_at_risk.html) For example, to
+examine the bias statistics of a risk model regarding an equally weighted
+portfolio (of which its weights are denoted as `weights`), pass the instrument
+observed returns (denoted as `returns`), and either a rolling risk model (to
+compute the volatility forecast) or a time series of volatility forecasts. ```
+from fpm_risk_model.accuracy import compute_bias_statistics
+compute_bias_statistics( X=returns, weights=weights, window=window ... ) ``` ##
+Roadmap The following major features will be enhanced - Factor exposures
+computation from factor returns (Q3 2023) - Shrinking covariance (Q3 2023) -
+Multi-asset class factor model (Q4 2023) - Fundamental type risk model (Q4
+2023) ## Contribution All levels of contributions are welcomed. Please refer to
+the [contributing](https://factor-pricing-model-risk-model.readthedocs.io/en/
+latest/contributing.html) section for development and release guidelines.
```

