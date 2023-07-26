# Comparing `tmp/factor_pricing_model_risk_model-2023.6.0.tar.gz` & `tmp/factor_pricing_model_risk_model-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factor_pricing_model_risk_model-2023.6.0.tar", max compression
+gzip compressed data, was "factor_pricing_model_risk_model-2023.6.1.tar", max compression
```

## Comparing `factor_pricing_model_risk_model-2023.6.0.tar` & `factor_pricing_model_risk_model-2023.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1078 2023-07-26 16:40:31.459883 factor_pricing_model_risk_model-2023.6.0/LICENSE
--rw-r--r--   0        0        0     7586 2023-07-26 16:40:31.459883 factor_pricing_model_risk_model-2023.6.0/README.md
--rw-r--r--   0        0        0     2642 2023-07-26 16:40:35.771986 factor_pricing_model_risk_model-2023.6.0/pyproject.toml
--rw-r--r--   0        0        0      225 2023-07-26 16:40:35.739985 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/__init__.py
--rw-r--r--   0        0        0      253 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/accuracy/__init__.py
--rw-r--r--   0        0        0     3410 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/accuracy/bias.py
--rw-r--r--   0        0        0     5663 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/accuracy/value_at_risk.py
--rw-r--r--   0        0        0      113 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/config.py
--rw-r--r--   0        0        0     4181 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/cov_estimator.py
--rw-r--r--   0        0        0        0 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/dataset/__init__.py
--rw-r--r--   0        0        0     3255 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/dataset/crypto.py
--rw-r--r--   0        0        0     4210 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/engine.py
--rw-r--r--   0        0        0    11187 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/factor_risk_model.py
--rw-r--r--   0        0        0     7438 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/pipeline/__init__.py
--rw-r--r--   0        0        0      621 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/pipeline/portfolio.py
--rw-r--r--   0        0        0      796 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/pipeline/returns.py
--rw-r--r--   0        0        0        0 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/py.typed
--rw-r--r--   0        0        0       59 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/regressor/__init__.py
--rw-r--r--   0        0        0     1138 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/regressor/ewls.py
--rw-r--r--   0        0        0     2514 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/regressor/wls.py
--rw-r--r--   0        0        0     3092 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/risk_model.py
--rw-r--r--   0        0        0     5657 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/rolling_factor_risk_model.py
--rw-r--r--   0        0        0     5097 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/rolling_risk_model.py
--rw-r--r--   0        0        0       59 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/statistical/__init__.py
--rw-r--r--   0        0        0     3926 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/statistical/apca.py
--rw-r--r--   0        0        0     4722 2023-07-26 16:40:31.547885 factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/statistical/pca.py
--rw-r--r--   0        0        0     9269 1970-01-01 00:00:00.000000 factor_pricing_model_risk_model-2023.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-26 21:29:05.569873 factor_pricing_model_risk_model-2023.6.1/LICENSE
+-rw-r--r--   0        0        0     7586 2023-07-26 21:29:05.569873 factor_pricing_model_risk_model-2023.6.1/README.md
+-rw-r--r--   0        0        0     2642 2023-07-26 21:29:10.065856 factor_pricing_model_risk_model-2023.6.1/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-07-26 21:29:10.033856 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/__init__.py
+-rw-r--r--   0        0        0      253 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/accuracy/__init__.py
+-rw-r--r--   0        0        0     3410 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/accuracy/bias.py
+-rw-r--r--   0        0        0     5663 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/accuracy/value_at_risk.py
+-rw-r--r--   0        0        0      113 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/config.py
+-rw-r--r--   0        0        0     4181 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/cov_estimator.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/dataset/__init__.py
+-rw-r--r--   0        0        0     3279 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/dataset/crypto.py
+-rw-r--r--   0        0        0     4210 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/engine.py
+-rw-r--r--   0        0        0    11187 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/factor_risk_model.py
+-rw-r--r--   0        0        0     7438 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/pipeline/__init__.py
+-rw-r--r--   0        0        0      621 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/pipeline/portfolio.py
+-rw-r--r--   0        0        0      796 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/pipeline/returns.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/py.typed
+-rw-r--r--   0        0        0       59 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/regressor/__init__.py
+-rw-r--r--   0        0        0     1138 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/regressor/ewls.py
+-rw-r--r--   0        0        0     2514 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/regressor/wls.py
+-rw-r--r--   0        0        0     3092 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/risk_model.py
+-rw-r--r--   0        0        0     5657 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/rolling_factor_risk_model.py
+-rw-r--r--   0        0        0     5097 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/rolling_risk_model.py
+-rw-r--r--   0        0        0       59 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/statistical/__init__.py
+-rw-r--r--   0        0        0     3926 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/statistical/apca.py
+-rw-r--r--   0        0        0     4722 2023-07-26 21:29:05.657873 factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/statistical/pca.py
+-rw-r--r--   0        0        0     9269 1970-01-01 00:00:00.000000 factor_pricing_model_risk_model-2023.6.1/PKG-INFO
```

### Comparing `factor_pricing_model_risk_model-2023.6.0/LICENSE` & `factor_pricing_model_risk_model-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/README.md` & `factor_pricing_model_risk_model-2023.6.1/README.md`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/pyproject.toml` & `factor_pricing_model_risk_model-2023.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "factor-pricing-model-risk-model"
-version = "2023.6.0"
+version = "2023.6.1"
 description = "Package to build risk models for factor pricing model"
 authors = ["Factor Pricing Model <factor.pricing.model@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/factorpricingmodel/factor-pricing-model-risk-model"
 documentation = "https://factor-pricing-model-risk-model.readthedocs.io"
 classifiers = [
```

### Comparing `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/accuracy/bias.py` & `factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/accuracy/bias.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/accuracy/value_at_risk.py` & `factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/accuracy/value_at_risk.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/cov_estimator.py` & `factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/cov_estimator.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/dataset/crypto.py` & `factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/dataset/crypto.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     :return: Dict of sample data with prices, returns, marketcap
       and volumes.
     """
     data = {}
     response = requests.get(
         "https://github.com/factorpricingmodel/factor-pricing-model-risk-model"
-        "/raw/main/examples/notebook/crypto_estimation_universe.zip",
+        "/raw/main/examples/notebook/crypto_estimation_universe_sample_data.zip",
         stream=True,
     )
     with ZipFile(io.BytesIO(response.content)) as zip_ref:
         with TemporaryDirectory() as temp_dir:
             zip_ref.extractall(temp_dir)
             files = [
                 (join(temp_dir, f), f.replace(".csv", ""))
@@ -71,15 +71,15 @@
 
     :return: Dict of sample data with prices, returns, volumes
       (in crypto) and volumes (in USD).
     """
     data = {}
     response = requests.get(
         "https://github.com/factorpricingmodel/factor-pricing-model-risk-model"
-        "/raw/main/examples/notebook/crypto_model_universe.zip",
+        "/raw/main/examples/notebook/crypto_model_universe_sample_data.zip",
         stream=True,
     )
     with ZipFile(io.BytesIO(response.content)) as zip_ref:
         with TemporaryDirectory() as temp_dir:
             zip_ref.extractall(temp_dir)
             price_data_dir = join(temp_dir, "Price-Data")
             files = [
```

### Comparing `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/engine.py` & `factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/engine.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/factor_risk_model.py` & `factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/factor_risk_model.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/pipeline/__init__.py` & `factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/pipeline/portfolio.py` & `factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/pipeline/portfolio.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/pipeline/returns.py` & `factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/pipeline/returns.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/regressor/ewls.py` & `factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/regressor/ewls.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/regressor/wls.py` & `factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/regressor/wls.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/risk_model.py` & `factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/risk_model.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/rolling_factor_risk_model.py` & `factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/rolling_factor_risk_model.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/rolling_risk_model.py` & `factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/rolling_risk_model.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/statistical/apca.py` & `factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/statistical/apca.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/src/fpm_risk_model/statistical/pca.py` & `factor_pricing_model_risk_model-2023.6.1/src/fpm_risk_model/statistical/pca.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.6.0/PKG-INFO` & `factor_pricing_model_risk_model-2023.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factor-pricing-model-risk-model
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: Package to build risk models for factor pricing model
 Home-page: https://github.com/factorpricingmodel/factor-pricing-model-risk-model
 License: MIT
 Author: Factor Pricing Model
 Author-email: factor.pricing.model@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: factor-pricing-model-risk-model Version: 2023.6.0
+Metadata-Version: 2.1 Name: factor-pricing-model-risk-model Version: 2023.6.1
 Summary: Package to build risk models for factor pricing model Home-page:
 https://github.com/factorpricingmodel/factor-pricing-model-risk-model License:
 MIT Author: Factor Pricing Model Author-email: factor.pricing.model@gmail.com
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
```

