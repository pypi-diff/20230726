# Comparing `tmp/atlantic-1.0.65-py3-none-any.whl.zip` & `tmp/atlantic-1.0.66-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18639 bytes, number of entries: 12
+Zip file size: 18863 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      389 b- defN 23-Feb-20 00:15 atlantic/__init__.py
 -rw-rw-rw-  2.0 fat     5500 b- defN 23-May-11 19:39 atlantic/atl_feat_eng.py
 -rw-rw-rw-  2.0 fat     8704 b- defN 23-Apr-17 10:49 atlantic/atl_feat_selection.py
 -rw-rw-rw-  2.0 fat     1563 b- defN 23-Apr-17 09:56 atlantic/atl_metrics.py
 -rw-rw-rw-  2.0 fat     2862 b- defN 23-May-06 15:26 atlantic/atl_performance.py
 -rw-rw-rw-  2.0 fat     8541 b- defN 23-Apr-17 10:17 atlantic/atl_pipeline.py
 -rw-rw-rw-  2.0 fat    20571 b- defN 23-May-06 15:42 atlantic/atl_processing.py
--rw-rw-rw-  2.0 fat     1078 b- defN 23-Jun-18 21:45 atlantic-1.0.65.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    12256 b- defN 23-Jun-18 21:45 atlantic-1.0.65.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-18 21:45 atlantic-1.0.65.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-18 21:45 atlantic-1.0.65.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      969 b- defN 23-Jun-18 21:45 atlantic-1.0.65.dist-info/RECORD
-12 files, 62534 bytes uncompressed, 17019 bytes compressed:  72.8%
+-rw-rw-rw-  2.0 fat     1078 b- defN 23-Jul-26 20:55 atlantic-1.0.66.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    12727 b- defN 23-Jul-26 20:55 atlantic-1.0.66.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-26 20:55 atlantic-1.0.66.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-26 20:55 atlantic-1.0.66.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      969 b- defN 23-Jul-26 20:55 atlantic-1.0.66.dist-info/RECORD
+12 files, 63005 bytes uncompressed, 17243 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: atlantic/atl_pipeline.py
 Comment: 
 
 Filename: atlantic/atl_processing.py
 Comment: 
 
-Filename: atlantic-1.0.65.dist-info/LICENSE
+Filename: atlantic-1.0.66.dist-info/LICENSE
 Comment: 
 
-Filename: atlantic-1.0.65.dist-info/METADATA
+Filename: atlantic-1.0.66.dist-info/METADATA
 Comment: 
 
-Filename: atlantic-1.0.65.dist-info/WHEEL
+Filename: atlantic-1.0.66.dist-info/WHEEL
 Comment: 
 
-Filename: atlantic-1.0.65.dist-info/top_level.txt
+Filename: atlantic-1.0.66.dist-info/top_level.txt
 Comment: 
 
-Filename: atlantic-1.0.65.dist-info/RECORD
+Filename: atlantic-1.0.66.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `atlantic-1.0.65.dist-info/LICENSE` & `atlantic-1.0.66.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `atlantic-1.0.65.dist-info/METADATA` & `atlantic-1.0.66.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlantic
-Version: 1.0.65
+Version: 1.0.66
 Summary: Atlantic is an automated preprocessing framework for Supervised Machine Learning
 Home-page: https://github.com/TsLu1s/Atlantic
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,data processing,predictive modeling,data preprocessing,automated data preprocessing,automated machine learning,automl
 Classifier: Intended Audience :: Education
@@ -86,15 +86,15 @@
 * total_vi: Minimal value of the total sum of relative variable\feature importance percentage selected in the "H2O AutoML feature selection" step.
 * h2o_fs_models: Quantity of models generated for competition in step "H2O AutoML feature selection" to evaluate the relative importance of each feature (only leaderboard model will be selected for evaluation).
 * encoding_fs: You can choose if you want to encond your features in order to reduce loading time in "H2O AutoML feature selection" step. If in "True" mode label encoding is applied to categorical features.
 * vif_ratio: This value defines the minimal 'threshold' for Variance Inflation Factor filtering (default value=10).
  
 Importante Notes:
     
-* Default predictive evaluation metric for regression contexts is MAE (Mean Absolute Error) and classification is AUC (Accuracy).
+* Default predictive evaluation metric for regression contexts is Mean Absolute Error and classification is Accuracy.
 * Although functional, `Atlantic` data processing is not optimized for big data purposes yet.
 * Major update is now available in **versions>=1.0.50**
     
 ```py
     
 import atlantic as atl
 import pandas as pd   
@@ -228,14 +228,34 @@
 imputer_iter=atl.fit_IterImp(dataset:pd.DataFrame, 
                              target:str, 
                              order:str='ascending')
 df=atl.transform_IterImp(dataset:pd.DataFrame,
                          target:str,
                          imputer=imputer_iter)
 ```   
+
+## Citation
+
+Feel free to cite Atlantic as following:
+
+```
+
+@article{SANTOS2023100532,
+  author = {LuÃ­s Santos and LuÃ­s Ferreira}
+  title = {Atlantic - Automated data preprocessing framework for supervised machine learning},
+  journal = {Software Impacts},
+  volume = {17},
+  year = {2023},
+  issn = {2665-9638},
+  doi = {http://dx.doi.org/10.1016/j.simpa.2023.100532},
+  url = {https://www.sciencedirect.com/science/article/pii/S2665963823000696}
+}
+
+```
+
     
 ## License
 
 Distributed under the MIT License. See [LICENSE](https://github.com/TsLu1s/Atlantic/blob/main/LICENSE) for more information.
 
 ## Contact
```

## Comparing `atlantic-1.0.65.dist-info/RECORD` & `atlantic-1.0.66.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 atlantic/__init__.py,sha256=aJxiUy0U6d3cxOQQo5m4ATN4A3xAGwAFCqCl21JTvhM,389
 atlantic/atl_feat_eng.py,sha256=Xio6qpJLszw59TkKEgvf9ry-jnODwZAY7O3PxvN-22g,5500
 atlantic/atl_feat_selection.py,sha256=r1H8N7DEbbNgo8jUT9kA-5JRmc9v1WVZ3Bf1zU-ACAI,8704
 atlantic/atl_metrics.py,sha256=ZbP98YCmgf0UTiCtozQDRzVARP4EWy9GvzqbQ1XcJ_s,1563
 atlantic/atl_performance.py,sha256=1O9718eY3Ppko1COIYO8MKMS7eaH0xP5fc2CKX0Hlaw,2862
 atlantic/atl_pipeline.py,sha256=Fn77_CUA09jZNXkgUJc3yqGWBu7KNBXmcC6eLJU-7qc,8541
 atlantic/atl_processing.py,sha256=R97TbF5_4p8XyilGFhWzViIHbwRd4XscXzbC8yBKRvs,20571
-atlantic-1.0.65.dist-info/LICENSE,sha256=KDcNU0R4Ruo5yPyqmRZJGMYbASNPn58LJSr359FVFfA,1078
-atlantic-1.0.65.dist-info/METADATA,sha256=TtVLmZkaTmyIamKUMHlAwOJv-oOkcimgPNBOmW7Gz3M,12256
-atlantic-1.0.65.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-atlantic-1.0.65.dist-info/top_level.txt,sha256=RAc3T5Fn4vx9TZ0hPSO3jINJDLLfOOLdANbFmLJQAnU,9
-atlantic-1.0.65.dist-info/RECORD,,
+atlantic-1.0.66.dist-info/LICENSE,sha256=KDcNU0R4Ruo5yPyqmRZJGMYbASNPn58LJSr359FVFfA,1078
+atlantic-1.0.66.dist-info/METADATA,sha256=_noAOvu-6_2ovBiXGTiCyfZSQP2ynx2QNWghVpyoIEA,12727
+atlantic-1.0.66.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+atlantic-1.0.66.dist-info/top_level.txt,sha256=RAc3T5Fn4vx9TZ0hPSO3jINJDLLfOOLdANbFmLJQAnU,9
+atlantic-1.0.66.dist-info/RECORD,,
```

