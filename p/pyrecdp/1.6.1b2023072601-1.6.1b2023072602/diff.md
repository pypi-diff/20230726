# Comparing `tmp/pyrecdp-1.6.1b2023072601.tar.gz` & `tmp/pyrecdp-1.6.1b2023072602.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrecdp-1.6.1b2023072601.tar", last modified: Wed Jul 26 02:38:23 2023, max compression
+gzip compressed data, was "dist/pyrecdp-1.6.1b2023072602.tar", last modified: Wed Jul 26 05:27:16 2023, max compression
```

## Comparing `pyrecdp-1.6.1b2023072601.tar` & `pyrecdp-1.6.1b2023072602.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.099828 pyrecdp-1.6.1b2023072601/
--rw-r--r--   0 root         (0) root         (0)    94051 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/LICENSE
--rw-r--r--   0 root         (0) root         (0)      205 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8824 2023-07-26 02:38:23.099828 pyrecdp-1.6.1b2023072601/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8315 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.086828 pyrecdp-1.6.1b2023072601/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.086828 pyrecdp-1.6.1b2023072601/pyrecdp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.087828 pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/spark-defaults.conf
--rw-r--r--   0 root         (0) root         (0)      559 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/spark-env.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.088828 pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/target/
--rw-r--r--   0 root         (0) root         (0)   114879 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
--rw-r--r--   0 root         (0) root         (0)     1142 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.089828 pyrecdp-1.6.1b2023072601/pyrecdp/autofe/
--rw-r--r--   0 root         (0) root         (0)     4851 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/autofe/AutoFE.py
--rw-r--r--   0 root         (0) root         (0)    15830 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/autofe/BasePipeline.py
--rw-r--r--   0 root         (0) root         (0)     4812 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/autofe/FeatureEstimator.py
--rw-r--r--   0 root         (0) root         (0)     3114 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/autofe/FeatureProfiler.py
--rw-r--r--   0 root         (0) root         (0)     3127 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/autofe/FeatureWrangler.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/autofe/RelationalBuilder.py
--rw-r--r--   0 root         (0) root         (0)      218 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/autofe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.089828 pyrecdp-1.6.1b2023072601/pyrecdp/core/
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      908 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/core/dataframe.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/core/di_graph.py
--rw-r--r--   0 root         (0) root         (0)      901 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/core/parallel_iterator.py
--rw-r--r--   0 root         (0) root         (0)     6642 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     7159 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.091828 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/
--rw-r--r--   0 root         (0) root         (0)     2942 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/CESM_breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/amazon_product_review.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/base_api.py
--rw-r--r--   0 root         (0) root         (0)      288 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/download.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/ibm_fraud_detect.py
--rw-r--r--   0 root         (0) root         (0)     1208 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/nyc_taxi.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/outbrain.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/pretrained.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/twitter_recsys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.091828 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.091828 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/estimators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/estimators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/estimators/base.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-07-07 05:24:39.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/estimators/lightgbm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.093828 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/
--rw-r--r--   0 root         (0) root         (0)     2043 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/base.py
--rw-r--r--   0 root         (0) root         (0)      269 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/binned.py
--rw-r--r--   0 root         (0) root         (0)     1222 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/category.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/datetime.py
--rw-r--r--   0 root         (0) root         (0)     1398 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/drop.py
--rw-r--r--   0 root         (0) root         (0)     5685 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/encode.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/feature_transform.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-07-10 02:55:58.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/fillna.py
--rw-r--r--   0 root         (0) root         (0)     4666 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/geograph.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/group_category.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/name.py
--rw-r--r--   0 root         (0) root         (0)     3100 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/nlp.py
--rw-r--r--   0 root         (0) root         (0)     4448 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/relation.py
--rw-r--r--   0 root         (0) root         (0)     2975 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.095828 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6919 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/base.py
--rw-r--r--   0 root         (0) root         (0)     5807 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/category.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/custom.py
--rw-r--r--   0 root         (0) root         (0)     2450 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/data.py
--rw-r--r--   0 root         (0) root         (0)     4010 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/dataframe.py
--rw-r--r--   0 root         (0) root         (0)      995 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/drop.py
--rw-r--r--   0 root         (0) root         (0)     9106 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/encode.py
--rw-r--r--   0 root         (0) root         (0)      980 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/fillna.py
--rw-r--r--   0 root         (0) root         (0)      712 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1998 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/merge.py
--rw-r--r--   0 root         (0) root         (0)      769 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/name.py
--rw-r--r--   0 root         (0) root         (0)      772 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/tuple.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.095828 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/
--rw-r--r--   0 root         (0) root         (0)      317 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1711 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/cluster_infer.py
--rw-r--r--   0 root         (0) root         (0)     1711 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/distribution_infer.py
--rw-r--r--   0 root         (0) root         (0)     5752 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/statics.py
--rw-r--r--   0 root         (0) root         (0)     1732 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/time_series_infer.py
--rw-r--r--   0 root         (0) root         (0)     5394 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/type_infer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.096828 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/spark_data_processor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/spark_data_processor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54072 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/spark_data_processor/data_processor.py
--rw-r--r--   0 root         (0) root         (0)     8328 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/spark_data_processor/encoder.py
--rw-r--r--   0 root         (0) root         (0)     9032 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/spark_data_processor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.097828 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/
--rw-r--r--   0 root         (0) root         (0)     1092 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/BaseWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/PlotWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/ProfilerWidget.py
--rw-r--r--   0 root         (0) root         (0)      821 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/TabWidget.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/TableViewWidget.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.098828 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/
--rw-r--r--   0 root         (0) root         (0)      989 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/base.html
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/error.html
--rw-r--r--   0 root         (0) root         (0)      260 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/interactions.html
--rw-r--r--   0 root         (0) root         (0)     1340 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/overview.html
--rw-r--r--   0 root         (0) root         (0)     7110 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/scripts.html
--rw-r--r--   0 root         (0) root         (0)    16515 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/styles.html
--rw-r--r--   0 root         (0) root         (0)     9250 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/variables.html
--rw-r--r--   0 root         (0) root         (0)      166 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.087828 pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8824 2023-07-26 02:38:23.000000 pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3904 2023-07-26 02:38:23.000000 pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 02:38:23.000000 pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 02:38:23.000000 pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      202 2023-07-26 02:38:23.000000 pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-26 02:38:23.000000 pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 02:38:23.099828 pyrecdp-1.6.1b2023072601/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1521 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.099828 pyrecdp-1.6.1b2023072601/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2762 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/test_autofe.py
--rw-r--r--   0 root         (0) root         (0)     2087 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/test_dataconversion.py
--rw-r--r--   0 root         (0) root         (0)     1856 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/test_feature_estimator.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/test_feature_profiler.py
--rw-r--r--   0 root         (0) root         (0)     3316 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/test_feature_wrangler.py
--rw-r--r--   0 root         (0) root         (0)     4911 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/test_individual_method.py
--rw-r--r--   0 root         (0) root         (0)     3808 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/test_pipeline_json.py
--rw-r--r--   0 root         (0) root         (0)     2260 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/test_relational_builder.py
--rw-r--r--   0 root         (0) root         (0)     9017 2023-06-08 08:03:35.000000 pyrecdp-1.6.1b2023072601/tests/test_spark_dataprocessor.py
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-26 02:37:11.000000 pyrecdp-1.6.1b2023072601/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.776441 pyrecdp-1.6.1b2023072602/
+-rw-r--r--   0 root         (0) root         (0)    94051 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      205 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8824 2023-07-26 05:27:16.776441 pyrecdp-1.6.1b2023072602/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.763441 pyrecdp-1.6.1b2023072602/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.763441 pyrecdp-1.6.1b2023072602/pyrecdp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.764441 pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/spark-defaults.conf
+-rw-r--r--   0 root         (0) root         (0)      559 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/spark-env.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.764441 pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/target/
+-rw-r--r--   0 root         (0) root         (0)   114879 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.765441 pyrecdp-1.6.1b2023072602/pyrecdp/autofe/
+-rw-r--r--   0 root         (0) root         (0)     4851 2023-07-26 04:18:12.000000 pyrecdp-1.6.1b2023072602/pyrecdp/autofe/AutoFE.py
+-rw-r--r--   0 root         (0) root         (0)    15830 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/autofe/BasePipeline.py
+-rw-r--r--   0 root         (0) root         (0)     4812 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/autofe/FeatureEstimator.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/autofe/FeatureProfiler.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/autofe/FeatureWrangler.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/autofe/RelationalBuilder.py
+-rw-r--r--   0 root         (0) root         (0)      218 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/autofe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.766441 pyrecdp-1.6.1b2023072602/pyrecdp/core/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      908 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/core/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/core/di_graph.py
+-rw-r--r--   0 root         (0) root         (0)      901 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/core/parallel_iterator.py
+-rw-r--r--   0 root         (0) root         (0)     6642 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     7159 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.767441 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/CESM_breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/amazon_product_review.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/base_api.py
+-rw-r--r--   0 root         (0) root         (0)      288 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/download.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/ibm_fraud_detect.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/nyc_taxi.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/outbrain.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/pretrained.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/twitter_recsys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.767441 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.768441 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/estimators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/estimators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/estimators/base.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-07-07 05:24:39.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/estimators/lightgbm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.770441 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/
+-rw-r--r--   0 root         (0) root         (0)     2043 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/base.py
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/binned.py
+-rw-r--r--   0 root         (0) root         (0)     1222 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/category.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/datetime.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/drop.py
+-rw-r--r--   0 root         (0) root         (0)     5685 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/encode.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/feature_transform.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-07-10 02:55:58.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/fillna.py
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/group_category.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/name.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/nlp.py
+-rw-r--r--   0 root         (0) root         (0)     4448 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/relation.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.771441 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6919 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/base.py
+-rw-r--r--   0 root         (0) root         (0)     5807 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/category.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/custom.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/data.py
+-rw-r--r--   0 root         (0) root         (0)     4010 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)      995 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/drop.py
+-rw-r--r--   0 root         (0) root         (0)     9106 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/encode.py
+-rw-r--r--   0 root         (0) root         (0)      980 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/fillna.py
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/merge.py
+-rw-r--r--   0 root         (0) root         (0)      769 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/name.py
+-rw-r--r--   0 root         (0) root         (0)      772 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.772441 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/
+-rw-r--r--   0 root         (0) root         (0)      317 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/cluster_infer.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/distribution_infer.py
+-rw-r--r--   0 root         (0) root         (0)     5752 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/statics.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/time_series_infer.py
+-rw-r--r--   0 root         (0) root         (0)     5346 2023-07-26 05:14:55.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/type_infer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.773441 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/spark_data_processor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/spark_data_processor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54072 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/spark_data_processor/data_processor.py
+-rw-r--r--   0 root         (0) root         (0)     8328 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/spark_data_processor/encoder.py
+-rw-r--r--   0 root         (0) root         (0)     9032 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/spark_data_processor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.774441 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/BaseWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/PlotWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/ProfilerWidget.py
+-rw-r--r--   0 root         (0) root         (0)      821 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/TabWidget.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/TableViewWidget.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.774441 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/
+-rw-r--r--   0 root         (0) root         (0)      989 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/error.html
+-rw-r--r--   0 root         (0) root         (0)      260 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/interactions.html
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/overview.html
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/scripts.html
+-rw-r--r--   0 root         (0) root         (0)    16515 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/styles.html
+-rw-r--r--   0 root         (0) root         (0)     9250 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/variables.html
+-rw-r--r--   0 root         (0) root         (0)      166 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.764441 pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8824 2023-07-26 05:27:16.000000 pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-07-26 05:27:16.000000 pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 05:27:16.000000 pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 05:27:16.000000 pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      202 2023-07-26 05:27:16.000000 pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-26 05:27:16.000000 pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 05:27:16.776441 pyrecdp-1.6.1b2023072602/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1521 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.776441 pyrecdp-1.6.1b2023072602/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/test_autofe.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/test_dataconversion.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/test_feature_estimator.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/test_feature_profiler.py
+-rw-r--r--   0 root         (0) root         (0)     3316 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/test_feature_wrangler.py
+-rw-r--r--   0 root         (0) root         (0)     4911 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/test_individual_method.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/test_pipeline_json.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/test_relational_builder.py
+-rw-r--r--   0 root         (0) root         (0)     9017 2023-06-08 08:03:35.000000 pyrecdp-1.6.1b2023072602/tests/test_spark_dataprocessor.py
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-26 05:27:02.000000 pyrecdp-1.6.1b2023072602/version
```

### Comparing `pyrecdp-1.6.1b2023072601/LICENSE` & `pyrecdp-1.6.1b2023072602/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/PKG-INFO` & `pyrecdp-1.6.1b2023072602/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.6.1b2023072601
+Version: 1.6.1b2023072602
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrecdp-1.6.1b2023072601/README.md` & `pyrecdp-1.6.1b2023072602/README.md`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/spark-defaults.conf` & `pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/spark-defaults.conf`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/spark-env.sh` & `pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/spark-env.sh`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar` & `pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/__init__.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/autofe/AutoFE.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/autofe/AutoFE.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/autofe/BasePipeline.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/autofe/BasePipeline.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/autofe/FeatureEstimator.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/autofe/FeatureEstimator.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/autofe/FeatureProfiler.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/autofe/FeatureProfiler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/autofe/FeatureWrangler.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/autofe/FeatureWrangler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/autofe/RelationalBuilder.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/autofe/RelationalBuilder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/core/dataframe.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/core/di_graph.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/core/di_graph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/core/parallel_iterator.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/core/parallel_iterator.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/core/schema.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/core/schema.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/core/utils.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/core/utils.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/datasets/CESM_breast_cancer.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/datasets/CESM_breast_cancer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/datasets/amazon_product_review.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/datasets/amazon_product_review.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/datasets/base_api.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/datasets/base_api.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/datasets/ibm_fraud_detect.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/datasets/ibm_fraud_detect.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/datasets/nyc_taxi.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/datasets/nyc_taxi.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/datasets/outbrain.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/datasets/outbrain.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/estimators/base.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/estimators/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/estimators/lightgbm.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/estimators/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/__init__.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/category.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/datetime.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/datetime.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/drop.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/encode.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/encode.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/feature_transform.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/feature_transform.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/featuretools_adaptor.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/fillna.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/geograph.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/group_category.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/group_category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/name.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/nlp.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/nlp.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/relation.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/relation.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/type.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/base.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/category.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/data.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/data.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/dataframe.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/drop.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/encode.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/encode.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/featuretools_adaptor.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/fillna.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/geograph.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/merge.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/merge.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/name.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/tuple.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/tuple.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/type.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/cluster_infer.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/cluster_infer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/distribution_infer.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/distribution_infer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/statics.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/statics.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/time_series_infer.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/time_series_infer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/type_infer.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/type_infer.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,18 +98,16 @@
                 return (',', result.explode().unique().tolist())
     except:
         pass
     
     return False
  
 def is_encoded(s):
-    line_id = s.first_valid_index()
-    if line_id < 0:
-        return False
-    sample_data = s.loc[line_id:(line_id+1000)]
+    if len(s) > 1000:
+        sample_data = s.sample(n=1000, random_state=0)
     from pyrecdp.primitives.generators.nlp import BertTokenizerDecode
     proc_ = BertTokenizerDecode().get_function()
     try:
         proc_(sample_data)
     except Exception as e:
         #print(e)
         return False
```

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/spark_data_processor/data_processor.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/spark_data_processor/data_processor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/spark_data_processor/encoder.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/spark_data_processor/encoder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/spark_data_processor/utils.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/spark_data_processor/utils.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/widgets/BaseWidget.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/widgets/BaseWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/widgets/TabWidget.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/widgets/TabWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/widgets/TableViewWidget.py` & `pyrecdp-1.6.1b2023072602/pyrecdp/widgets/TableViewWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/base.html` & `pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/overview.html` & `pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/overview.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/scripts.html` & `pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/scripts.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/styles.html` & `pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/styles.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/variables.html` & `pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/variables.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/PKG-INFO` & `pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.6.1b2023072601
+Version: 1.6.1b2023072602
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/SOURCES.txt` & `pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/setup.py` & `pyrecdp-1.6.1b2023072602/setup.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/tests/test_autofe.py` & `pyrecdp-1.6.1b2023072602/tests/test_autofe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/tests/test_dataconversion.py` & `pyrecdp-1.6.1b2023072602/tests/test_dataconversion.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/tests/test_feature_estimator.py` & `pyrecdp-1.6.1b2023072602/tests/test_feature_estimator.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/tests/test_feature_profiler.py` & `pyrecdp-1.6.1b2023072602/tests/test_feature_profiler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/tests/test_feature_wrangler.py` & `pyrecdp-1.6.1b2023072602/tests/test_feature_wrangler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/tests/test_individual_method.py` & `pyrecdp-1.6.1b2023072602/tests/test_individual_method.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/tests/test_pipeline_json.py` & `pyrecdp-1.6.1b2023072602/tests/test_pipeline_json.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/tests/test_relational_builder.py` & `pyrecdp-1.6.1b2023072602/tests/test_relational_builder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072601/tests/test_spark_dataprocessor.py` & `pyrecdp-1.6.1b2023072602/tests/test_spark_dataprocessor.py`

 * *Files identical despite different names*

