# Comparing `tmp/pyrecdp-1.6.1b2023071102.tar.gz` & `tmp/pyrecdp-1.6.1b2023072601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrecdp-1.6.1b2023071102.tar", last modified: Mon Jul 10 18:45:20 2023, max compression
+gzip compressed data, was "dist/pyrecdp-1.6.1b2023072601.tar", last modified: Wed Jul 26 02:38:23 2023, max compression
```

## Comparing `pyrecdp-1.6.1b2023071102.tar` & `pyrecdp-1.6.1b2023072601.tar`

### file list

```diff
@@ -1,124 +1,130 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.920409 pyrecdp-1.6.1b2023071102/
--rw-r--r--   0 root         (0) root         (0)    94051 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/LICENSE
--rw-r--r--   0 root         (0) root         (0)      205 2023-06-28 06:07:34.000000 pyrecdp-1.6.1b2023071102/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8824 2023-07-10 18:45:20.920409 pyrecdp-1.6.1b2023071102/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8315 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.908408 pyrecdp-1.6.1b2023071102/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.908408 pyrecdp-1.6.1b2023071102/pyrecdp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.908408 pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/spark-defaults.conf
--rw-r--r--   0 root         (0) root         (0)      559 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/spark-env.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.908408 pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/target/
--rw-r--r--   0 root         (0) root         (0)   114879 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.908408 pyrecdp-1.6.1b2023071102/pyrecdp/autofe/
--rw-r--r--   0 root         (0) root         (0)     4030 2023-07-07 08:53:54.000000 pyrecdp-1.6.1b2023071102/pyrecdp/autofe/AutoFE.py
--rw-r--r--   0 root         (0) root         (0)    13999 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/autofe/BasePipeline.py
--rw-r--r--   0 root         (0) root         (0)     4523 2023-07-07 08:53:54.000000 pyrecdp-1.6.1b2023071102/pyrecdp/autofe/FeatureEstimator.py
--rw-r--r--   0 root         (0) root         (0)     3114 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/autofe/FeatureProfiler.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/autofe/FeatureWrangler.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-07 08:53:54.000000 pyrecdp-1.6.1b2023071102/pyrecdp/autofe/RelationalBuilder.py
--rw-r--r--   0 root         (0) root         (0)      218 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/autofe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.912408 pyrecdp-1.6.1b2023071102/pyrecdp/core/
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      908 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/core/dataframe.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/core/di_graph.py
--rw-r--r--   0 root         (0) root         (0)      901 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/core/parallel_iterator.py
--rw-r--r--   0 root         (0) root         (0)     5939 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     7012 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.912408 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/
--rw-r--r--   0 root         (0) root         (0)     2942 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/CESM_breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/amazon_product_review.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/base_api.py
--rw-r--r--   0 root         (0) root         (0)      288 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/download.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/ibm_fraud_detect.py
--rw-r--r--   0 root         (0) root         (0)     1208 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/nyc_taxi.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/outbrain.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/pretrained.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/datasets/twitter_recsys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.912408 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.912408 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/estimators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/estimators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/estimators/base.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/estimators/lightgbm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.912408 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/
--rw-r--r--   0 root         (0) root         (0)     1950 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/base.py
--rw-r--r--   0 root         (0) root         (0)      269 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/binned.py
--rw-r--r--   0 root         (0) root         (0)     1222 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/category.py
--rw-r--r--   0 root         (0) root         (0)     1648 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/datetime.py
--rw-r--r--   0 root         (0) root         (0)     1398 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/drop.py
--rw-r--r--   0 root         (0) root         (0)     5497 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/encode.py
--rw-r--r--   0 root         (0) root         (0)     1221 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/feature_transform.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/fillna.py
--rw-r--r--   0 root         (0) root         (0)     4666 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/name.py
--rw-r--r--   0 root         (0) root         (0)     3100 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/nlp.py
--rw-r--r--   0 root         (0) root         (0)     4720 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/relation.py
--rw-r--r--   0 root         (0) root         (0)     2975 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.916408 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/
--rw-r--r--   0 root         (0) root         (0)      153 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6100 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/base.py
--rw-r--r--   0 root         (0) root         (0)     2601 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/category.py
--rw-r--r--   0 root         (0) root         (0)      351 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/custom.py
--rw-r--r--   0 root         (0) root         (0)     2293 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/data.py
--rw-r--r--   0 root         (0) root         (0)     3291 2023-07-07 22:06:49.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/dataframe.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/drop.py
--rw-r--r--   0 root         (0) root         (0)     5272 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/encode.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/fillna.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-07-07 08:53:54.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/merge.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/name.py
--rw-r--r--   0 root         (0) root         (0)      712 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/tuple.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.916408 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/profilers/
--rw-r--r--   0 root         (0) root         (0)      157 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/profilers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5752 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/profilers/statics.py
--rw-r--r--   0 root         (0) root         (0)     4792 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/profilers/type_infer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.916408 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/spark_data_processor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/spark_data_processor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54072 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/spark_data_processor/data_processor.py
--rw-r--r--   0 root         (0) root         (0)     8145 2023-07-07 22:06:49.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/spark_data_processor/encoder.py
--rw-r--r--   0 root         (0) root         (0)     8699 2023-07-07 08:53:54.000000 pyrecdp-1.6.1b2023071102/pyrecdp/primitives/spark_data_processor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.916408 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/
--rw-r--r--   0 root         (0) root         (0)     1092 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/BaseWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/PlotWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/ProfilerWidget.py
--rw-r--r--   0 root         (0) root         (0)      821 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/TabWidget.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/TableViewWidget.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.916408 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/
--rw-r--r--   0 root         (0) root         (0)      989 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/base.html
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/error.html
--rw-r--r--   0 root         (0) root         (0)      260 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/interactions.html
--rw-r--r--   0 root         (0) root         (0)     1340 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/overview.html
--rw-r--r--   0 root         (0) root         (0)     7110 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/scripts.html
--rw-r--r--   0 root         (0) root         (0)    16515 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/styles.html
--rw-r--r--   0 root         (0) root         (0)     9250 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/variables.html
--rw-r--r--   0 root         (0) root         (0)      166 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/pyrecdp/widgets/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.908408 pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8824 2023-07-10 18:45:20.000000 pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3648 2023-07-10 18:45:20.000000 pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 18:45:20.000000 pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 18:45:20.000000 pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      196 2023-07-10 18:45:20.000000 pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-10 18:45:20.000000 pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 18:45:20.920409 pyrecdp-1.6.1b2023071102/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1515 2023-06-28 06:07:34.000000 pyrecdp-1.6.1b2023071102/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:45:20.920409 pyrecdp-1.6.1b2023071102/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 06:07:34.000000 pyrecdp-1.6.1b2023071102/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/tests/test_autofe.py
--rw-r--r--   0 root         (0) root         (0)     1856 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/tests/test_feature_estimator.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-06-27 23:05:53.000000 pyrecdp-1.6.1b2023071102/tests/test_feature_profiler.py
--rw-r--r--   0 root         (0) root         (0)     2911 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/tests/test_feature_wrangler.py
--rw-r--r--   0 root         (0) root         (0)     3808 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/tests/test_pipeline_json.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/tests/test_relational_builder.py
--rw-r--r--   0 root         (0) root         (0)     9017 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023071102/tests/test_spark_dataprocessor.py
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-10 18:45:20.000000 pyrecdp-1.6.1b2023071102/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.099828 pyrecdp-1.6.1b2023072601/
+-rw-r--r--   0 root         (0) root         (0)    94051 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      205 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8824 2023-07-26 02:38:23.099828 pyrecdp-1.6.1b2023072601/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.086828 pyrecdp-1.6.1b2023072601/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.086828 pyrecdp-1.6.1b2023072601/pyrecdp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.087828 pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/spark-defaults.conf
+-rw-r--r--   0 root         (0) root         (0)      559 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/spark-env.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.088828 pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/target/
+-rw-r--r--   0 root         (0) root         (0)   114879 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.089828 pyrecdp-1.6.1b2023072601/pyrecdp/autofe/
+-rw-r--r--   0 root         (0) root         (0)     4851 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/autofe/AutoFE.py
+-rw-r--r--   0 root         (0) root         (0)    15830 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/autofe/BasePipeline.py
+-rw-r--r--   0 root         (0) root         (0)     4812 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/autofe/FeatureEstimator.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/autofe/FeatureProfiler.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/autofe/FeatureWrangler.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/autofe/RelationalBuilder.py
+-rw-r--r--   0 root         (0) root         (0)      218 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/autofe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.089828 pyrecdp-1.6.1b2023072601/pyrecdp/core/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      908 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/core/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/core/di_graph.py
+-rw-r--r--   0 root         (0) root         (0)      901 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/core/parallel_iterator.py
+-rw-r--r--   0 root         (0) root         (0)     6642 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     7159 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.091828 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/CESM_breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/amazon_product_review.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/base_api.py
+-rw-r--r--   0 root         (0) root         (0)      288 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/download.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/ibm_fraud_detect.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/nyc_taxi.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/outbrain.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/pretrained.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/datasets/twitter_recsys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.091828 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.091828 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/estimators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/estimators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/estimators/base.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-07-07 05:24:39.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/estimators/lightgbm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.093828 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/
+-rw-r--r--   0 root         (0) root         (0)     2043 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/base.py
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/binned.py
+-rw-r--r--   0 root         (0) root         (0)     1222 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/category.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/datetime.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/drop.py
+-rw-r--r--   0 root         (0) root         (0)     5685 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/encode.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/feature_transform.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-07-10 02:55:58.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/fillna.py
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/group_category.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/name.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/nlp.py
+-rw-r--r--   0 root         (0) root         (0)     4448 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/relation.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.095828 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6919 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/base.py
+-rw-r--r--   0 root         (0) root         (0)     5807 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/category.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/custom.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/data.py
+-rw-r--r--   0 root         (0) root         (0)     4010 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)      995 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/drop.py
+-rw-r--r--   0 root         (0) root         (0)     9106 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/encode.py
+-rw-r--r--   0 root         (0) root         (0)      980 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/fillna.py
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/merge.py
+-rw-r--r--   0 root         (0) root         (0)      769 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/name.py
+-rw-r--r--   0 root         (0) root         (0)      772 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.095828 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/
+-rw-r--r--   0 root         (0) root         (0)      317 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/cluster_infer.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/distribution_infer.py
+-rw-r--r--   0 root         (0) root         (0)     5752 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/statics.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/time_series_infer.py
+-rw-r--r--   0 root         (0) root         (0)     5394 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/type_infer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.096828 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/spark_data_processor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/spark_data_processor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54072 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/spark_data_processor/data_processor.py
+-rw-r--r--   0 root         (0) root         (0)     8328 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/spark_data_processor/encoder.py
+-rw-r--r--   0 root         (0) root         (0)     9032 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/pyrecdp/primitives/spark_data_processor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.097828 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/BaseWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/PlotWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/ProfilerWidget.py
+-rw-r--r--   0 root         (0) root         (0)      821 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/TabWidget.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/TableViewWidget.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.098828 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/
+-rw-r--r--   0 root         (0) root         (0)      989 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/error.html
+-rw-r--r--   0 root         (0) root         (0)      260 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/interactions.html
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/overview.html
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/scripts.html
+-rw-r--r--   0 root         (0) root         (0)    16515 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/styles.html
+-rw-r--r--   0 root         (0) root         (0)     9250 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/variables.html
+-rw-r--r--   0 root         (0) root         (0)      166 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072601/pyrecdp/widgets/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.087828 pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8824 2023-07-26 02:38:23.000000 pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-07-26 02:38:23.000000 pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 02:38:23.000000 pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 02:38:23.000000 pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      202 2023-07-26 02:38:23.000000 pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-26 02:38:23.000000 pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 02:38:23.099828 pyrecdp-1.6.1b2023072601/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1521 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:38:23.099828 pyrecdp-1.6.1b2023072601/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/test_autofe.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/test_dataconversion.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/test_feature_estimator.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/test_feature_profiler.py
+-rw-r--r--   0 root         (0) root         (0)     3316 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/test_feature_wrangler.py
+-rw-r--r--   0 root         (0) root         (0)     4911 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/test_individual_method.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/test_pipeline_json.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072601/tests/test_relational_builder.py
+-rw-r--r--   0 root         (0) root         (0)     9017 2023-06-08 08:03:35.000000 pyrecdp-1.6.1b2023072601/tests/test_spark_dataprocessor.py
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-26 02:37:11.000000 pyrecdp-1.6.1b2023072601/version
```

### Comparing `pyrecdp-1.6.1b2023071102/LICENSE` & `pyrecdp-1.6.1b2023072601/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/PKG-INFO` & `pyrecdp-1.6.1b2023072601/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.6.1b2023071102
+Version: 1.6.1b2023072601
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrecdp-1.6.1b2023071102/README.md` & `pyrecdp-1.6.1b2023072601/README.md`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/spark-defaults.conf` & `pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/spark-defaults.conf`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/spark-env.sh` & `pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/spark-env.sh`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar` & `pyrecdp-1.6.1b2023072601/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/__init__.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/autofe/AutoFE.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/autofe/AutoFE.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 import logging
 from pyrecdp.core.utils import Timer, infer_problem_type
 from pyrecdp.core.dataframe import DataFrameAPI
 
-from pyrecdp.autofe import FeatureWrangler, FeatureProfiler, RelationalBuilder, FeatureEstimator
+from pyrecdp.autofe import FeatureWrangler, FeatureProfiler, RelationalBuilder, FeatureEstimator, BasePipeline
 
 import os
 
 logging.basicConfig(format='%(asctime)s %(levelname)s:%(message)s', level=logging.ERROR, datefmt='%I:%M:%S')
 logger = logging.getLogger(__name__)
 
 class AutoFE():
-    def __init__(self, dataset, label, *args, **kwargs):
+    def __init__(self, dataset, label, time_series = None, exclude_op = [], include_op = [], *args, **kwargs):
         self.label = label
         self.auto_pipeline = {'relational': None, 'profiler': None, 'wrangler': None, 'estimator': None}
         if isinstance(dataset, dict):
+            print("AutoFE started to build data relation")
             self.auto_pipeline['relational'] = RelationalBuilder(dataset=dataset, label=label)
+            pipeline = self.auto_pipeline['relational']
+            print("AutoFE started to create data pipeline")
+            self.auto_pipeline['wrangler'] = FeatureWrangler(data_pipeline=pipeline, exclude_op = exclude_op, include_op = include_op, time_series = time_series)
+            pipeline = self.auto_pipeline['wrangler']
+            config = {
+                'model_file': 'autofe_lightgbm.mdl',
+                'objective': infer_problem_type(pipeline.dataset[pipeline.main_table], label),
+                'model_name': 'lightgbm'}
+            self.auto_pipeline['estimator'] = FeatureEstimator(data_pipeline = pipeline, config = config)
         else:
             print("AutoFE started to profile data")
             self.auto_pipeline['profiler'] = FeatureProfiler(dataset=dataset, label=label)
             print("AutoFE started to create data pipeline")
-            self.auto_pipeline['wrangler'] = FeatureWrangler(dataset=dataset, label=label)
+            self.auto_pipeline['wrangler'] = FeatureWrangler(dataset=dataset, label=label, time_series = time_series, exclude_op = exclude_op, include_op = include_op)
             pipeline = self.auto_pipeline['wrangler']
             config = {
                 'model_file': 'autofe_lightgbm.mdl',
                 'objective': infer_problem_type(pipeline.dataset[pipeline.main_table], label),
                 'model_name': 'lightgbm'}
             self.auto_pipeline['estimator'] = FeatureEstimator(data_pipeline = pipeline, config = config)
 
     def fit_transform(self, engine_type = 'pandas', no_cache = False, *args, **kwargs):
-        print("AutoFE started to execute data")
+        print("AutoFE started to fit_transform data")
         ret_df = None
-        if self.auto_pipeline['relational']:
-            pipeline = self.auto_pipeline['relational']
-            ret_df = pipeline.fit_transform(engine_type, data = ret_df, **kwargs)
-            print("AutoFE started to profile data")
-
-        if self.auto_pipeline['estimator']:
-            pipeline = self.auto_pipeline['estimator']
-            ret_df = pipeline.fit_transform(engine_type, data = ret_df, **kwargs)
+        pipeline = self.auto_pipeline['estimator']
+        ret_df = pipeline.fit_transform(engine_type, data = ret_df, **kwargs)
         return ret_df
     
     def profile(self, engine_type = 'pandas'):
         if isinstance(self.auto_pipeline['profiler'], type(None)):
             return "feature profile support for multiple table is WIP"
         return self.auto_pipeline['profiler'].visualize_analyze(engine_type)
 
@@ -52,18 +56,15 @@
         fe_imp_dict = self.auto_pipeline['estimator'].get_feature_importance()
         feat_importances = pd.Series([i[1] for i in fe_imp_dict], [i[0] for i in fe_imp_dict])
         feat_importances = feat_importances[feat_importances > 0].sort_values()
         height = int(len(feat_importances) * 0.5)
         return feat_importances.plot(kind='barh', figsize=(15,height))
 
     def plot(self):
-        if self.auto_pipeline['relational']:
-            return self.auto_pipeline['relational'].plot()
-        else:
-            return self.auto_pipeline['estimator'].plot()
+        return self.auto_pipeline['estimator'].plot()
         
     def get_transformed_data(self):
         if self.auto_pipeline['relational']:
             return self.auto_pipeline['relational'].get_transformed_cache()
         else:
             ret_df = self.auto_pipeline['estimator'].get_transformed_cache()
             return ret_df
@@ -79,8 +80,18 @@
         else:
             return self.auto_pipeline['estimator'].add_operation(config)
         
     def delete_operation(self, idx):
         if self.auto_pipeline['relational']:
             return self.auto_pipeline['relational'].delete_operation(idx)
         else:
-            return self.auto_pipeline['estimator'].delete_operation(idx)
+            return self.auto_pipeline['estimator'].delete_operation(idx)
+
+    def export(self, file_path = None):
+        return self.auto_pipeline['wrangler'].export(file_path)
+
+    @classmethod
+    def clone_pipeline(cls, origin_pipeline, data):
+        pipeline_json = origin_pipeline.export()
+        new_pipeline = BasePipeline(data, origin_pipeline.label)
+        new_pipeline.import_from_json(pipeline_json)
+        return new_pipeline
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/autofe/BasePipeline.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/autofe/BasePipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from pyrecdp.primitives.generators import *
 from pyrecdp.core import DataFrameSchema, SparkDataProcessor, DiGraph
-from pyrecdp.primitives.operations import Operation, DataFrameOperation, RDDToDataFrameConverter, TargetEncodeOperation
+from pyrecdp.primitives.operations import Operation, DataFrameOperation, RDDToDataFrameConverter, SparkDataFrameToDataFrameConverter, TargetEncodeOperation
 import pandas as pd
 import logging
 import graphviz
 import json
 from pyrecdp.core.utils import Timer, sample_read, deepcopy
 from pyspark.sql import DataFrame as SparkDataFrame
 from pyspark import RDD as SparkRDD
 from IPython.display import display
 from tqdm import tqdm
 
 logging.basicConfig(format='%(asctime)s %(levelname)s:%(message)s', level=logging.ERROR, datefmt='%I:%M:%S')
 logger = logging.getLogger(__name__)
 
 class BasePipeline:
-    def __init__(self, dataset, label, *args, **kwargs):
+    def __init__(self, dataset, label, exclude_op = [], include_op = [], *args, **kwargs):
         # properties
         # self.main_table: main table names
         # self.dataset: a dictionary, main_table will be indicated with key 'main_table'
         # self.y: target label
         # self.pipeline: a direct graph to store the operation
 
         if isinstance(dataset, pd.DataFrame):
@@ -54,15 +54,16 @@
         if not input_is_path:
             original_data = self.dataset[main_table]
         else:
             original_data = sample_read(self.dataset[main_table])
         
         self.feature_columns = [i for i in original_data.columns if i != self.y]
         #feature_data = original_data[self.feature_columns]
-            
+        self.exclude_op = exclude_op
+        self.include_op = include_op
         self.generators = []
         self.pipeline = DiGraph()
         if not input_is_path:
             op = 'DataFrame'
             config = main_table
         else:
             op = 'DataLoader'
@@ -78,22 +79,27 @@
             self.supplementary = None
         self.rdp = None
 
     def update_label(self):
         leaf_idx = self.pipeline.convert_to_node_chain()[-1]
         pa_schema = self.pipeline[leaf_idx].output
         label_list = [pa_field.name for pa_field in pa_schema if pa_field.is_label]
-        self.y = label_list[0]
+        if len(label_list) > 0:
+            self.y = label_list[0]
+        else:
+            self.y = None
      
     def fit_analyze(self, *args, **kwargs):
         child = list(self.pipeline.keys())[-1]
         max_id = child
         to_run = []
         for i in range(len(self.generators)):
             for generator in self.generators[i]:
+                if generator.__class__.__name__ in self.exclude_op:
+                    continue
                 to_run.append(generator)
         
         pbar = tqdm(to_run, total=len(to_run))
         for generator in pbar:
             pbar.set_description(f"{generator.__class__.__name__}")
             self.pipeline, child, max_id = generator.fit_prepare(self.pipeline, [child], max_id)
         return child, max_id
@@ -104,19 +110,28 @@
     def export(self, file_path = None):
         json_object = self.pipeline.json_dump()
         if file_path:
             # Writing to sample.json
             with open(file_path, "w") as outfile:
                 outfile.write(json_object)
         else:
-            print(json_object)
+            return json_object
     
     def import_from_json(self, file_path):
-        with open(file_path, "r") as infile:
-            json_object = json.load(infile)
+        try:
+            json_object = json.loads(file_path)
+            flag = 'loaded'
+        except ValueError as e:
+            flag = 'try_load_as_file'
+        if flag == 'try_load_as_file':
+            with open(file_path, "r") as infile:
+                json_object = json.load(infile)
+                flag = 'loaded'
+        if flag != 'loaded':
+            raise ValueError("Unable to load as json string or json file")
         for idx, op_config in json_object.items():
             idx = int(idx)
             if idx in self.pipeline:
                 continue
             self.pipeline[idx] = Operation.load(idx, op_config)
         #self.create_executable_pipeline()
         
@@ -246,15 +261,15 @@
         except:
             pass
         return f
 
     def to_chain(self):
         return self.pipeline.convert_to_node_chain()
         
-    def execute(self, engine_type = "pandas", start_op_idx = -1, no_cache = False, transformed_end = -1, data = None):
+    def execute(self, engine_type = "pandas", start_op_idx = -1, no_cache = False, transformed_end = -1, data = None, trans_type = 'fit_transform'):
         # prepare pipeline
         if not hasattr(self, 'executable_pipeline') or not hasattr(self, 'executable_sequence'):
             self.executable_pipeline, self.executable_sequence = self.create_executable_pipeline()
         executable_pipeline = self.executable_pipeline
         executable_sequence = self.executable_sequence
 
         # execute
@@ -270,15 +285,15 @@
                         if data:
                             input_df = data
                         else:
                             input_df = self.dataset if start_op_idx == -1 else {'main_table': self.transformed_cache}
                         input_df = deepcopy(input_df) if no_cache else input_df
                         op.set(input_df)
                     with Timer(f"execute {op}"):
-                        op.execute_pd(executable_pipeline)
+                        op.execute_pd(executable_pipeline, trans_type = trans_type)
             if transformed_end == -1:
                 df = executable_sequence[-1].cache
             else:
                 df = executable_pipeline[transformed_end].cache
         elif engine_type == 'spark':
             with Timer(f"execute with spark"):
                 start = False
@@ -291,21 +306,22 @@
                         if data:
                             input_df = data
                         else:
                             input_df = self.dataset if start_op_idx == -1 else {'main_table': self.transformed_cache}
                         input_df = deepcopy(input_df) if no_cache else input_df
                         op.set(input_df)
                     print(f"append {op}")
-                    op.execute_spark(executable_pipeline, self.rdp)
+                    op.execute_spark(executable_pipeline, self.rdp, trans_type = trans_type)
                 if transformed_end == -1:
                     ret = executable_sequence[-1].cache
                 else:
                     ret = executable_pipeline[transformed_end].cache
                 if isinstance(ret, SparkDataFrame):
-                    df = self.rdp.transform(ret)
+                    _convert = SparkDataFrameToDataFrameConverter().get_function(self.rdp)
+                    df = _convert(ret)
                 elif isinstance(ret, SparkRDD):
                     _convert = RDDToDataFrameConverter().get_function(self.rdp)
                     df = _convert(ret)
                 else:
                     df = ret
         else:
             raise NotImplementedError('pipeline only support pandas and spark as engine')
@@ -329,12 +345,32 @@
         ret = self.execute(engine_type = engine_type, no_cache = no_cache, data = data)
         if engine_type == "spark":
             del self.rdp 
             self.rdp = None
         self.transformed_cache = ret
         return ret
     
+    def transform(self, engine_type = 'pandas', no_cache = False, data = None, *args, **kwargs):
+        if not no_cache and hasattr(self, 'transformed_cache') and self.transformed_cache is not None:
+            print("Detect pre-transformed cache, return cached data")
+            print("If re-transform is required, please use fit_transform(no_cache = True)")
+            return self.transformed_cache
+        if engine_type == "spark":
+            if "spark_master" in kwargs:
+                spark_master = kwargs["spark_master"]
+                spark_mode = 'standalone'
+            else:
+                spark_master = "local[*]"
+                spark_mode = 'local'
+            self.rdp = SparkDataProcessor(spark_mode=spark_mode, spark_master=spark_master)
+        ret = self.execute(engine_type = engine_type, no_cache = no_cache, data = data, trans_type = 'transform')
+        if engine_type == "spark":
+            del self.rdp
+            self.rdp = None
+        self.transformed_cache = ret
+        return ret
+
     def get_transformed_cache(self):
         if hasattr(self, 'transformed_cache') and self.transformed_cache is not None:
             return self.transformed_cache
         else:
             print("No transformed data detected.")
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/autofe/FeatureEstimator.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/autofe/FeatureEstimator.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         if isinstance(data_pipeline, str):
             dataset = config['dataset'] 
             if dataset is not None:
                 super().__init__(dataset, label)
                 self.import_from_json(data_pipeline)
         elif isinstance(data_pipeline, BasePipeline):
             self.nested_pipeline_obj = data_pipeline
-            self.pipeline = data_pipeline.pipeline
+            self.pipeline = data_pipeline.pipeline.copy()
             self.dataset = data_pipeline.dataset
             self.rdp = data_pipeline.rdp
             self.transformed_cache = data_pipeline.transformed_cache if hasattr(data_pipeline, 'transformed_cache') else None
             label = data_pipeline.y if label is None else label
             self.y = label
         else:
             raise NotImplementedError(f"Unsupport input datapipeline is {data_pipeline}")
@@ -81,15 +81,21 @@
 
     def fit_transform(self, engine_type = 'pandas', no_cache = False, data = None, *args, **kwargs):
         if self.transformed_cache is not None and not no_cache: # we can skip data process steps
             start_op_idx = self.estimator_pipeline_start
         else:
             start_op_idx = -1
         if engine_type == "spark":
-            self.rdp = SparkDataProcessor()
+            if "spark_master" in kwargs:
+                spark_master = kwargs["spark_master"]
+                spark_mode = 'standalone'
+            else:
+                spark_master = "local[*]"
+                spark_mode = 'local'
+            self.rdp = SparkDataProcessor(spark_mode=spark_mode, spark_master=spark_master)
         ret = self.execute(engine_type, start_op_idx, no_cache, data = data, transformed_end = self.transformed_end_idx)
         if engine_type == "spark":
             del self.rdp 
             self.rdp = None
         if self.transformed_cache is None:
             self.transformed_cache = ret
         self.feature_importance = self.executable_sequence[-1].cache
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/autofe/FeatureProfiler.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/autofe/FeatureProfiler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/core/dataframe.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/core/di_graph.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/core/di_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,9 +87,12 @@
         ret = graph.chain()
         return ret
 
     def json_dump(self):
         import json
         to_dump = dict((node_id, op.dump()) for node_id, op in self.items())
         return json.dumps(to_dump, indent=4)
-        
+
+    def copy(self):
+        import copy
+        return copy.copy(self)
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/core/parallel_iterator.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/core/parallel_iterator.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/core/schema.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/core/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from woodwork.column_schema import ColumnSchema
 from pandas import StringDtype
-from pyrecdp.core.utils import is_text_series, is_tuple, is_encoded, is_integer_convertable
+from pyrecdp.core.utils import is_text_series, is_tuple, is_integer_convertable
 class TextDtype(StringDtype):
     pass
 
 class SeriesSchema:
     def __init__(self, *args):
         if len(args) == 1:
             s = args[0]
             self.name = s.name
             in_type = s.dtype
             self.config = {}
-            self.config['is_text'] = is_text_series(s)
-            if self.config['is_text']:
-                self.config['is_encoded'] = is_encoded(s)
+            self.config['is_text'] = is_text_series(s) 
             self.config['is_tuple'] = is_tuple(s)
             self.config['is_integer'] = is_integer_convertable(s)
         elif len(args) >= 2:
             # s_dtype is possible to be pandas.dtype or woodwork.dtype       
             self.name = args[0]
             # TODO: convert featuretools return_type to recdp return type
             in_type = args[1]
@@ -66,19 +64,24 @@
             if v:
                 config[k] = v
         return config
     
     def copy_config_from(self, config):
         for k, v in config.items():
             if v is not False:
-                self.config[k] = v
+                if isinstance(v, list):
+                    if k not in self.config:
+                        self.config[k] = []
+                    self.config[k].extend(v)
+                else:
+                    self.config[k] = v
         self.post_fix()
 
     def mydump(self):
-        return (self.name, list(k for k, v in self.config.items() if v is not False))
+        return (self.name, list(k if v == True else (k, v) for k, v in self.config.items() if v is not False))
 
     def __repr__(self):
         return f"{self.mydump()}"
    
     @property
     def dtype_str(self):
         return str(dict((k, v) for k, v in self.config.items() if v))
@@ -150,15 +153,34 @@
     @property
     def is_encoded(self):
         return 'is_encoded' in self.config and self.config['is_encoded']
 
     @property
     def is_text(self):
         return 'is_text' in self.config and self.config["is_text"]
-    
+
+    @property
+    def is_timeseries(self):
+        return 'is_timeseries' in self.config and self.config["is_timeseries"]
+
+    @property
+    def is_grouped_categorical(self):
+        return 'is_grouped_categorical' in self.config and self.config["is_grouped_categorical"]
+
+    @property
+    def is_timebased_categorical(self):
+        return 'is_timebased_categorical' in self.config and self.config["is_timebased_categorical"]
+
+    @property
+    def group_id_list(self):
+        if 'group_id' in self.config:
+            return self.config["group_id"]
+        else:
+            return []
+
 
 class DataFrameSchema(list):
     def __init__(self, df):
         for s_name in df.columns:
             s = df[s_name]
             super().append(SeriesSchema(s))
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/core/utils.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/core/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import pandas as pd
 import copy
 import os
 
 import timeit
+import pickle
 
 # `def pretty(d, indent=0):
 #     from pyrecdp.primitives.operations import Operation
 #     for key, value in d.items():
 #         print('\t' * indent + str(key))
 #         if isinstance(value, dict):
 #             pretty(value, indent+1)
@@ -35,50 +36,65 @@
         b_list = b.tolist()
     elif isinstance(b, list):
         b_list = b
     a_dict = dict((i, 0) for i in a_list)
     [a_list.append(i) for i in b_list if i not in a_dict]
     return np.array(a_list)
 
-def get_encoder_np(encoder, dict_path):
-    if isinstance(dict_path, type(None)):
-        return encoder
-    dirname = os.path.dirname(dict_path)
-    if not os.path.exists(dict_path):
+def get_encoder(dict_path):
+    if dict_path.endswith(".parquet"):
+        return get_encoder_df(dict_path)
+    else:
+        if not os.path.exists(dict_path):
+            return FileNotFoundError(f"{dict_path} is not found")
+        with open(dict_path, 'rb') as f:
+            encoder = pickle.load(f)
         return encoder
-    encoder.classes_ = np.load(dict_path)    
-    return encoder
 
-def save_encoder_np(encoder, dict_path):
-    if isinstance(dict_path, type(None)):
-        return
-    dirname = os.path.dirname(dict_path)
-    if not os.path.exists(dirname):
-        os.mkdir(dirname)
-    np.save(dict_path, encoder.classes_)
+def save_encoder(encoder, dict_path):
+    if isinstance(encoder, pd.DataFrame):
+        return save_encoder_df(encoder, dict_path)
+    else:
+        dirname = os.path.dirname(dict_path)
+        if len(dirname) > 0 and not os.path.exists(dirname):
+            os.mkdir(dirname)
+        with open(dict_path, 'wb') as f:
+            pickle.dump(encoder, f)
 
 def get_encoder_df(dict_path):
-    if isinstance(dict_path, type(None)):
-        return None
-    dirname = os.path.dirname(dict_path)
     if not os.path.exists(dict_path):
-        return None
+        return FileNotFoundError(f"{dict_path} is not found")
     return pd.read_parquet(dict_path)
 
 def save_encoder_df(encoder, dict_path):
     if isinstance(dict_path, type(None)):
         return
     dirname = os.path.dirname(dict_path)
-    if not os.path.exists(dirname):
+    if len(dirname) > 0 and not os.path.exists(dirname):
         os.mkdir(dirname)
     encoder.to_parquet(dict_path)
     
 def deepcopy(dict_df):
     return copy.deepcopy(dict_df)
+
+def fillna_with_series(tgt_s, src_s):
+    nan_loc = tgt_s.isnull().to_list()
+    df_encoded_list = tgt_s.to_list()
+    df_encoded_2_list = src_s.to_list()
+
+    ret = []
+    for idx, is_nan in enumerate(nan_loc):
+        if not is_nan:
+            ret.append(df_encoded_list[idx])
+        else:
+            ret.append(df_encoded_2_list[idx])
     
+    ret = pd.Series(ret, index = tgt_s.index)
+    return ret
+
 def get_sample_indices_pd(indices, target_num_rows):
     if isinstance(indices, pd.DataFrame):
         indices = indices.notna()
     if indices.size > target_num_rows:
         frac = target_num_rows/indices.size
         mask = pd.Series(np.random.choice(a=[False, True], size=(indices.size), p=[1-frac, frac]))
         indices = indices & mask
@@ -102,15 +118,15 @@
             x[k] = dump_fix(v)
     elif isinstance(x, list) or isinstance(x, np.ndarray):
         for idx in range(len(x)):
             x[idx] = dump_fix(x[idx])
     elif isinstance(x, type):
         x = (x.__module__, x.__name__)
     elif isinstance(x, tuple):
-        x = (dump_fix(x[0]), dump_fix(x[1]))
+        x = [dump_fix(i) for i in x]
     elif hasattr(x, 'mydump'):
         x = x.mydump()
     elif callable(x):
         import inspect
         x = inspect.getsource(x)
     else:
         x = x
@@ -175,34 +191,20 @@
     from pandas.api.types import is_numeric_dtype
     if not is_numeric_dtype(s.dtype):
         return False
     s = s.fillna(0)
     if np.array_equal(s, s.astype(int)):
         return True
     return False
-        
-def is_encoded(s):
-    line_id = s.first_valid_index()
-    if line_id < 0:
-        return False
-    sample_data = s.loc[line_id:(line_id+1000)]
-    from pyrecdp.primitives.generators.nlp import BertTokenizerDecode
-    proc_ = BertTokenizerDecode().get_function()
-    try:
-        proc_(sample_data)
-    except Exception as e:
-        #print(e)
-        return False
-    return True
- 
+
 def is_unique(s):
     if isinstance(s, pd.Series):
         return len(s.unique()) == 1
     elif isinstance(s, pd.DataFrame) and len(s.columns) == 1:
-        return len(s[s.columns[0]].unque()) == 1
+        return len(s[s.columns[0]].unique()) == 1
     else:
         return False
 
 class Timer:
     level = 0
     viewer = None
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/datasets/CESM_breast_cancer.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/datasets/CESM_breast_cancer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/datasets/amazon_product_review.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/datasets/amazon_product_review.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/datasets/base_api.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/datasets/base_api.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/datasets/ibm_fraud_detect.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/datasets/ibm_fraud_detect.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/datasets/nyc_taxi.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/datasets/nyc_taxi.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/datasets/outbrain.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/datasets/outbrain.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/estimators/base.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/estimators/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     def get_func_train(self):
         raise NotImplementedError("BaseEstimator is an abstract class")
 
     def get_func_predict(self):
         raise NotImplementedError("BaseEstimator is an abstract class")
 
-    def get_function_pd(self):
+    def get_function_pd(self, trans_type = 'fit_transform'):
         return self.get_func_train()
         
     def get_evaluate_func(self, metric):
         if metric == 'rmse':
             def rmse_func(ground_truth, pred):
                 return np.sqrt(mean_squared_error(ground_truth, pred))
             return rmse_func
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/estimators/lightgbm.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/estimators/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/__init__.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .binned import BinnedFeatureGenerator
 from .category import CategoryFeatureGenerator
+from .group_category import GroupCategoryFeatureGenerator
 from .datetime import DatetimeFeatureGenerator
 from .drop import DropUselessFeatureGenerator
 from .name import RenameFeatureGenerator
 from .fillna import FillNaFeatureGenerator
 from .type import TypeCheckFeatureGenerator,TypeConvertFeatureGenerator
 from .nlp import DecodedTextFeatureGenerator, TextFeatureGenerator
 from .geograph import GeoFeatureGenerator, CoordinatesInferFeatureGenerator
@@ -50,14 +51,15 @@
 pre_enocode_feature_generator_list = [
     #DropUselessFeatureGenerator,
 ]
 
 global_dict_index_generator_list = [
     LabelEncodeFeatureGenerator,
     BinnedFeatureGenerator,
+    GroupCategoryFeatureGenerator,
     CategoryFeatureGenerator,
     TargetEncodeFeatureGenerator,
     CountEncodeFeatureGenerator
 ]
 
 post_feature_generator_list = [
     RenameFeatureGenerator
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/category.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/datetime.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             Day,
             Month,
             Weekday,
             Year,
             Hour,
             #PartOfDay()
         ]
-        self.op_name = 'datetime_feature'            
+        self.op_name = 'datetime_feature'
 
     def fit_prepare(self, pipeline, children, max_idx):
         cur_idx = max_idx
         pa_schema = pipeline[children[0]].output
         for pa_field in pa_schema:
             if pa_field.is_datetime:
                 self.feature_in.append(pa_field.name)
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/drop.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/encode.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/encode.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,19 +84,20 @@
         self.feature_in = []
 
     def fit_prepare(self, pipeline, children, max_idx):
         is_useful = False
         pa_schema = pipeline[children[0]].output
         feature_in_out = {}
         ret_pa_schema = copy.deepcopy(pa_schema)
+        folder = 'pipeline_default'
         for pa_field in pa_schema:
-            if pa_field.is_categorical:
+            if pa_field.is_categorical and not pa_field.is_timebased_categorical:
                 feature = pa_field.name
                 out_schema = SeriesSchema(f"{feature}__TE", float)
-                feature_in_out[feature] = out_schema.name
+                feature_in_out[feature] = (f"{folder}/{feature}_TE_dict.pkl", out_schema.name)
                 is_useful = True
                 ret_pa_schema.append(out_schema)
         if is_useful:
             # find label column
             label_list = [pa_field.name for pa_field in pa_schema if pa_field.is_label]
             cur_idx = max_idx + 1
             config = {}
@@ -113,19 +114,20 @@
         self.feature_in = []
 
     def fit_prepare(self, pipeline, children, max_idx):
         is_useful = False
         pa_schema = pipeline[children[0]].output
         feature_in_out = {}
         ret_pa_schema = copy.deepcopy(pa_schema)
+        folder = 'pipeline_default'
         for pa_field in pa_schema:
             if pa_field.is_categorical:
                 feature = pa_field.name
                 out_schema = SeriesSchema(f"{feature}__CE", int)
-                feature_in_out[feature] = out_schema.name
+                feature_in_out[feature] = (f"{folder}/{feature}_CE_dict.pkl", out_schema.name)
                 is_useful = True
                 ret_pa_schema.append(out_schema)
         if is_useful:
             cur_idx = max_idx + 1
             config = feature_in_out
             pipeline[cur_idx] = Operation(cur_idx, children, ret_pa_schema, op = 'count_encode', config = config)
             return pipeline, cur_idx, cur_idx
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/feature_transform.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/feature_transform.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     def __init__(self):
         pass
 
     def get_function(self):
         def string_to_number(array):
             import re
             import pandas as pd
-            array = array.apply(lambda x: "".join(re.findall(r'\d+.*\d*', x)))
+            array = array.apply(lambda x: "" if pd.isna(x) else "".join(re.findall(r'\d+.*\d*', x)))
             array = pd.to_numeric(array, errors='coerce')
             return array
 
         return string_to_number
     
 class ConvertToNumberFeatureGenerator(FeaturetoolsBasedFeatureGenerator):
     def __init__(self, **kwargs):
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/featuretools_adaptor.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/fillna.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/geograph.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/name.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/nlp.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/nlp.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/relation.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/relation.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,22 +27,14 @@
             else:
                 stop = True
             if len(self.candidates) == 0:
                 stop = True
         pipeline.update(self.pipeline)
         return pipeline, self.pipeline_main_idx, self.pipeline_start_idx
     
-    def get_function_pd(self):
-        def merge_tables(df):                
-            return df
-        return merge_tables
-
-    def get_function_spark(self, rdp):        
-        raise NotImplementedError("RelationalFeatureGenerator spark implementation is WIP")
-    
     #======== Private utility funcs ==========#
     def dry_run_merge_tables(self, target_table_schema, related_tables):            
         def _dry_merge(child_idx, on, tgt_schema, src_schema):
             tgt_col_names = [col.name for col in tgt_schema]
             src_col_names = [col.name for col in src_schema]
             error = False
             # check on is containing in both tgt and src
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/generators/type.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/generators/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/base.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         }
         return dump_dict
     
     def instantiate(self):
         from .data import DataFrameOperation, DataLoader
         from .merge import MergeOperation
         from .name import RenameOperation
-        from .category import CategorifyOperation
+        from .category import CategorifyOperation, GroupCategorifyOperation
         from .drop import DropOperation
         from .fillna import FillNaOperation
         from .featuretools_adaptor import FeaturetoolsOperation
         from .geograph import HaversineOperation
         from .type import TypeInferOperation
         from .tuple import TupleOperation
         from .custom import CustomOperation
@@ -44,25 +44,27 @@
 
         operations_ = {
             'DataFrame': DataFrameOperation,
             'DataLoader': DataLoader,
             'merge': MergeOperation,
             'rename': RenameOperation,
             'categorify': CategorifyOperation,
+            'group_categorify': GroupCategorifyOperation,
             'drop': DropOperation,
             'fillna': FillNaOperation,
             'haversine': HaversineOperation,
             'tuple': TupleOperation,
             'type_infer': TypeInferOperation,
             'lightgbm': LightGBM,
             'onehot_encode': OnehotEncodeOperation,
             'list_onehot_encode': ListOnehotEncodeOperation,
             'target_encode': TargetEncodeOperation,
             'count_encode': CountEncodeOperation,
-            'custom_operator': CustomOperation
+            'custom_operator': CustomOperation,
+            'time_series_infer': DummyOperation,
         }
 
         if self.op in operations_:
             return operations_[self.op](self)
         else:
             try:
                 return FeaturetoolsOperation(self)
@@ -88,67 +90,83 @@
        
     def __repr__(self) -> str:
         return self.op.op
 
     def describe(self) -> str:
         return str(self.op.dump())
         
-    def execute_pd(self, pipeline):
-        _proc = self.get_function_pd()
+    def execute_pd(self, pipeline, trans_type = 'fit_transform'):
+        _proc = self.get_function_pd(trans_type)
         if not self.op.children or len(self.op.children) == 0:
             pass
         else:
             child_output = pipeline[self.op.children[0]].cache
             self.cache = _proc(child_output)
             
-    def execute_spark(self, pipeline, rdp):
+    def execute_spark(self, pipeline, rdp, trans_type = 'fit_transform'):
         _convert = None
         if not self.op.children or len(self.op.children) == 0:
             pass
         else:
             child_output = pipeline[self.op.children[0]].cache
             if isinstance(child_output, SparkDataFrame):
                 if self.support_spark_dataframe:
-                    _proc = self.get_function_spark(rdp)
+                    _proc = self.get_function_spark(rdp, trans_type)
                 elif self.support_spark_rdd:
                     _convert = SparkDataFrameToRDDConverter().get_function(rdp)
-                    _proc = self.get_function_spark_rdd(rdp)
+                    _proc = self.get_function_spark_rdd(rdp, trans_type)
                 else:
                     _convert = SparkDataFrameToDataFrameConverter().get_function(rdp)
-                    _proc = self.get_function_pd()
+                    _proc = self.get_function_pd(trans_type)
             elif isinstance(child_output, SparkRDD):
                 if self.support_spark_rdd:
-                    _proc = self.get_function_spark_rdd(rdp)
+                    _proc = self.get_function_spark_rdd(rdp, trans_type)
                 elif self.support_spark_dataframe:
                     _convert = RDDToSparkDataFrameConverter().get_function(rdp)
-                    _proc = self.get_function_spark(rdp)
+                    _proc = self.get_function_spark(rdp, trans_type)
                 else:
                     _convert = RDDToDataFrameConverter().get_function(rdp)
-                    _proc = self.get_function_pd()
+                    _proc = self.get_function_pd(trans_type)
             elif isinstance(child_output, pd.DataFrame):
                 if self.fast_without_dpp:
-                    _proc = self.get_function_pd()
+                    _proc = self.get_function_pd(trans_type)
                 elif self.support_spark_rdd:
                     _convert = DataFrameToRDDConverter().get_function(rdp)
-                    _proc = self.get_function_spark_rdd(rdp)
+                    _proc = self.get_function_spark_rdd(rdp, trans_type)
                 elif self.support_spark_dataframe:
                     _convert = DataFrameToSparkDataFrameConverter().get_function(rdp)
-                    _proc = self.get_function_spark(rdp)
+                    _proc = self.get_function_spark(rdp, trans_type)
                 else:
-                    _proc = self.get_function_pd()
+                    _proc = self.get_function_pd(trans_type)
             else:
                 raise ValueError(f"child cache is not recognized {child_output}")
         
             if _convert:
                 child_output = _convert(child_output)
                 pipeline[self.op.children[0]].cache = child_output
             self.cache = _proc(child_output)
             #print(self.cache.take(1))
 
-    def get_function_spark_rdd(self, rdp):
-        actual_func = self.get_function_pd()
+    def get_function_spark_rdd(self, rdp, trans_type = 'fit_transform'):
+        actual_func = self.get_function_pd(trans_type)
         def transform(iter, *args):
             for x in iter:
                 yield actual_func(x, *args)
         def base_spark_feature_generator(rdd):
             return rdd.mapPartitions(transform)
-        return base_spark_feature_generator
+        return base_spark_feature_generator
+
+class DummyOperation(BaseOperation):
+    def __init__(self, op_base):
+        super().__init__(op_base)
+        self.support_spark_dataframe = True
+        self.support_spark_rdd = True
+
+    def get_function_pd(self, trans_type = 'fit_transform'):
+        def dummy_op(df):
+            return df
+        return dummy_op
+
+    def get_function_spark(self, rdp, trans_type = 'fit_transform'):
+        def dummy_op(df):
+            return df
+        return dummy_op
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/data.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,53 +9,53 @@
         self.fast_without_dpp = True
 
     def set(self, dataset):
         # this condition is very important, so place holder dataframe won't copy data
         if self.op.children is None or len(self.op.children) == 0:
             self.cache = dataset[self.op.config]
         
-    def get_function_pd(self):
+    def get_function_pd(self, trans_type = 'fit_transform'):
         cache = self.cache.copy() if self.cache is not None else None
         def get_dataframe(df):
             if df is not None:
                 return df
             else:
                 return cache
         return get_dataframe
     
 class DataLoader(BaseOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
         self.support_spark_dataframe = True
         self.support_spark_rdd = False
         
-    def get_function_pd(self):
+    def get_function_pd(self, trans_type = 'fit_transform'):
         def get_dataframe():
             file_path = self.op.config['file_path']
             if file_path.endswith('.csv'):
                 return pd.read_csv(file_path)
             elif file_path.endswith('.parquet'):
                 return pd.read_parquet(file_path)
             else:
                 raise NotImplementedError("now sample read only support csv and parquet")
         return get_dataframe
     
-    def get_function_spark(self, rdp, method = None):
+    def get_function_spark(self, rdp, trans_type = 'fit_transform'):
         def get_dataframe():
             file_path = self.op.config['file_path']
             if file_path.endswith('.csv'):
                 return rdp.spark.read.csv(file_path, header=True, inferSchema=True)
             elif file_path.endswith('.parquet'):
                 return rdp.spark.read.parquet(file_path)
             else:
                 raise NotImplementedError("now sample read only support csv and parquet")
         return get_dataframe
     
-    def execute_pd(self, pipeline):
+    def execute_pd(self, pipeline, trans_type = 'fit_transform'):
         assert not self.op.children or len(self.op.children) == 0
-        _proc = self.get_function_pd()
+        _proc = self.get_function_pd(trans_type)
         self.cache = _proc()
     
-    def execute_spark(self, pipeline, rdp):
+    def execute_spark(self, pipeline, rdp, trans_type = 'fit_transform'):
         assert not self.op.children or len(self.op.children) == 0
-        _proc = self.get_function_spark(rdp)
+        _proc = self.get_function_spark(rdp, trans_type)
         self.cache = _proc()
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/dataframe.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/dataframe.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,16 +18,21 @@
         return convert
    
 class RDDToSparkDataFrameConverter:
     @staticmethod
     def get_function(rdp):
         print("append RDDToSparkDataFrameConverter")
         def convert(rdd):
-            df = rdd.flatMap(lambda pdf: pdf.to_dict('records')).toDF()
-            return df
+            start_time = time.time()
+            sdf = rdd.flatMap(lambda pdf: pdf.to_dict('records')).toDF()
+            sdf.cache()
+            sdf.count()
+            end_time = time.time()
+            print(f"SparkRDD To SparkDataFrame Conversion took {(end_time - start_time):.3f} secs")
+            return sdf
             
         return convert
 
 class DataFrameToRDDConverter:
     @staticmethod
     def get_function(rdp):
         print("append DataFrameToRDDConverter")
@@ -64,28 +69,39 @@
             # id_pdfs = [tpl[1] for tpl in pdfs]
             # nr_pdfs = [tpl[0].shape[0] for tpl in pdfs]
             # ordered_pdfs = [tpl[0] for tpl in sorted(pdfs, key = lambda x: x[1])]
             nr_pdfs = [tpl.shape[0] for tpl in pdfs]
             ordered_pdfs = pdfs
             print(f"DataframeTransform took {(end_time - start_time):.3f} secs, processed {sum(nr_pdfs)} rows with num_partitions as {len(pdfs)}")
             start_time = time.time()
-            combined = pd.concat(ordered_pdfs)
+            combined = pd.concat(ordered_pdfs, ignore_index=True).infer_objects()
             end_time = time.time()
             print(f"DataframeTransform combine to one pandas dataframe took {(end_time - start_time):.3f} secs")
             return combined
             
         return convert
 
 class DataFrameToSparkDataFrameConverter:
+    @staticmethod
     def get_function(rdp):
         print("append DataFrameToSparkDataFrameConverter")
         def convert(pdf):
-            return rdp.spark.createDataFrame(pdf) 
+            start_time = time.time()
+            sdf = rdp.spark.createDataFrame(pdf)
+            sdf.cache()
+            sdf.count()
+            end_time = time.time()
+            print(f"Dataframe To SparkDataFrame Conversion took {(end_time - start_time):.3f} secs")
+            return sdf
         return convert
     
 class SparkDataFrameToDataFrameConverter:
     @staticmethod
     def get_function(rdp):
         print("append SparkDataFrameToDataFrameConverter")
         def convert(df):
-            return df.to_pandas()          
+            start_time = time.time()
+            pdf = df.toPandas()          
+            end_time = time.time()
+            print(f"SparkDataFrame to DataFrame Conversion took {(end_time - start_time):.3f} secs")
+            return pdf        
         return convert
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/drop.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/drop.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,21 +9,21 @@
     def __init__(self, op_base):
         super().__init__(op_base)
         self.feature_in = self.op.config
         self.support_spark_dataframe = True
         self.support_spark_rdd = True
         self.fast_without_dpp = True
 
-    def get_function_pd(self):
+    def get_function_pd(self, trans_type = 'fit_transform'):
         feature_in = copy.deepcopy(self.feature_in)
 
         def drop_useless_feature(df):
             for i in df.columns:
                 if i not in feature_in and is_unique(df[i]):
                     feature_in.append(i)
             return df.drop(columns = feature_in)
         return drop_useless_feature
     
-    def get_function_spark(self, rdp):
+    def get_function_spark(self, rdp, trans_type = 'fit_transform'):
         def drop_feature(df):
             return df.drop(*self.feature_in)
         return drop_feature
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/encode.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/category.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,130 +1,126 @@
 from .base import BaseOperation
 import pandas as pd
 from pyspark.sql import DataFrame as SparkDataFrame
-import copy
-import numpy as np
 from pyrecdp.core.utils import *
+import copy
+from sklearn.preprocessing import LabelEncoder
 from pyrecdp.core.parallel_iterator import ParallelIterator
 from IPython.display import display
-from category_encoders import TargetEncoder
-from category_encoders.count import CountEncoder
-from sklearn.preprocessing import MultiLabelBinarizer
 
-class OnehotEncodeOperation(BaseOperation):
+class CategorifyOperation(BaseOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
-        self.config = self.op.config
+        self.feature_in_out = self.op.config
         self.support_spark_dataframe = False
         self.support_spark_rdd = False
 
     @classmethod
-    def onehot_encode(cls, item):
-        feature, df_x, keys = item
-        selected_columns = [f"{feature}__{key}" for key in keys]
-        one_hot_df = pd.get_dummies(df_x, prefix = f"{feature}_")
-        one_hot_df = one_hot_df.loc[:, one_hot_df.columns.isin(selected_columns)]
-        return one_hot_df
-
-    def get_function_pd(self):
-        config = copy.deepcopy(self.config)
-        def encode(df):
-            df_features = [(col, df[col], keys) for col, keys in config.items()]
-            results = ParallelIterator.execute(df_features, OnehotEncodeOperation.onehot_encode, len(df_features), "OnehotEncode")
-            df = pd.concat([df] + results, axis=1)
-            return df
-        return encode
-    
-class ListOnehotEncodeOperation(BaseOperation):
-    def __init__(self, op_base):
-        super().__init__(op_base)
-        self.config = self.op.config
-        self.support_spark_dataframe = False
-        self.support_spark_rdd = False
-
-    @classmethod
-    def multi_label_encode(cls, item):
-        feature, df_x, sep, keys = item
-        splitted_s = df_x.str.split(sep).apply(lambda x: [i for i in x if i != ""])
-        mlb = MultiLabelBinarizer()
-        encoded = mlb.fit_transform(splitted_s)
-        names = [f"{feature}_{key}" for key in mlb.classes_]
-        selected_columns = [f"{feature}_{key}" for key in keys]
-        one_hot_df = pd.DataFrame(encoded, columns=names)
-        one_hot_df = one_hot_df.loc[:, one_hot_df.columns.isin(selected_columns)]
-        return one_hot_df
-    
-    def get_function_pd(self):
-        config = copy.deepcopy(self.config)
-        def encode(df):
-            df_features = [(col, df[col], sep, keys) for col, (sep, keys) in config.items()]
-            results = ParallelIterator.execute(df_features, ListOnehotEncodeOperation.multi_label_encode, len(df_features), "ListOnehotEncode")
-            df = pd.concat([df] + results, axis=1)
-            return df
-        return encode
-
-class TargetEncodeOperation(BaseOperation):
-    def __init__(self, op_base):
-        super().__init__(op_base)
-        self.feature_in_out = self.op.config['feature_in_out']
-        self.label = self.op.config['label']
-        self.support_spark_dataframe = False
-        self.support_spark_rdd = False
+    def label_encode(cls, item):
+        feature, df_x, dict_path, feature_out = item
+        encoder = LabelEncoder()
+        ret = pd.DataFrame()
+        ret[feature_out] = encoder.fit_transform(df_x)
+        save_encoder(encoder, dict_path)
+        ret.index = df_x.index
+        #display(encoder.classes_)
+        return ret
 
     @classmethod
-    def target_encode(cls, item):
-        (feature, df_x, df_y), feature_out = item
-        if is_unique(df_x):
-            df_encoded = pd.DataFrame()
-            df_encoded[feature_out] = [np.nan]*len(df_x)
-            df_encoded.index = df_x.index
-        else:
-            encoder = TargetEncoder(cols=[feature], min_samples_leaf=20, smoothing=10)
-            df_encoded = encoder.fit_transform(df_x, df_y).rename(columns={feature: feature_out})
-        return df_encoded
+    def label_encode_transform(cls, item):
+        feature, df_x, dict_path, feature_out = item
+        encoder = get_encoder(dict_path)
+        # combine encoder with new data
+        encoder_class_list = encoder.classes_.tolist()
+        encoder_new = LabelEncoder()
+        encoder_new.fit(df_x)
+        combined_classes = encoder_class_list + [i for i in encoder_new.classes_ if i not in encoder_class_list]
+        encoder.classes_ = np.array(combined_classes)
+        # start to transform
+        ret = pd.DataFrame()
+        ret[feature_out] = encoder.transform(df_x)
+        ret.index = df_x.index
+        #display(encoder.classes_)
+        return ret
 
-    def get_function_pd(self):
+    def get_function_pd(self, trans_type = 'fit_transform'):
         feature_in_out = copy.deepcopy(self.feature_in_out)
-        label = self.label
+        if trans_type == 'fit_transform':
+            def categorify(df):
+                df_features = [(col, df[col], dict_path, feature_out) for col, (dict_path, feature_out) in feature_in_out.items()]
+                results = ParallelIterator.execute(df_features, CategorifyOperation.label_encode, len(df_features), "Categorify")
+                df = df.loc[:, ~df.columns.isin([sdf.columns[0] for sdf in results])]
+                df = pd.concat([df] + results, axis=1)
+                return df
+        elif trans_type == 'transform':
+            def categorify(df):
+                df_features = [(col, df[col], dict_path, feature_out) for col, (dict_path, feature_out) in feature_in_out.items()]
+                results = ParallelIterator.execute(df_features, CategorifyOperation.label_encode_transform, len(df_features), "Categorify")
+                df = df.loc[:, ~df.columns.isin([sdf.columns[0] for sdf in results])]
+                df = pd.concat([df] + results, axis=1)
+                return df
 
-        def encode(df):
-            df_y = df[label]
-            df_features = [(col, df[col], df_y) for col in feature_in_out.keys()]
-            te_in_out = zip(df_features, feature_in_out.values())
-            results = ParallelIterator.execute(te_in_out, TargetEncodeOperation.target_encode, len(feature_in_out), "TargetEncode")
-            to_concat_df = pd.concat(results, axis=1)
-            df = pd.concat([df, to_concat_df], axis=1)
-            return df
-        return encode
+        return categorify
 
-class CountEncodeOperation(BaseOperation):
+class GroupCategorifyOperation(BaseOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
-        self.feature_in = self.op.config
+        self.feature_in_out = self.op.config
         self.support_spark_dataframe = False
         self.support_spark_rdd = False
 
     @classmethod
-    def count_encode(cls, item):
-        dict_path = None
-        feature, df_x = item
-        if is_unique(df_x):
-            df_encoded = pd.DataFrame()
-            df_encoded[f"{feature}_CE"] = [np.nan]*len(df_x)
-            df_encoded.index = df_x.index
-        else:
-            encoder = CountEncoder(cols=[feature])
-            encoder = get_encoder_np(encoder, dict_path)
-            df_encoded = encoder.fit_transform(df_x).rename(columns={feature: f"{feature}_CE"})
-            save_encoder_np(encoder, dict_path)
-        return df_encoded
-
-    def get_function_pd(self):
-        feature_in = copy.deepcopy(self.feature_in)
-
-        def encode(df):
-            df_features = [(col, df[col]) for col in feature_in]
-            results = ParallelIterator.execute(df_features, CountEncodeOperation.count_encode, len(df_features), "CountEncode")
-            to_concat_df = pd.concat(results, axis=1)
-            df = pd.concat([df, to_concat_df], axis=1)
-            return df
-        return encode
+    def group_label_encode(cls, item):
+        grouped_features, df_x, dict_path, feature_out = item
+        df_x['index'] = df_x.index
+        k = 'index'
+        # print(grouped_features)
+        encoder = df_x.groupby(by = grouped_features, as_index = False)[k].count().drop(k, axis = 1)
+        encoder[feature_out] = encoder.index
+        save_encoder(encoder, dict_path)
+        #display(encoder)
+        ret = df_x.merge(encoder, on = grouped_features, how = 'left')[feature_out]
+        return ret
+
+    @classmethod
+    def group_label_encode_transform(cls, item):
+        grouped_features, df_x, dict_path, feature_out = item
+        encoder_df = get_encoder(dict_path)
+        # convert df to dict
+        key_feats = [i for i in encoder_df.columns if i != feature_out]
+        encoder_df['key'] = encoder_df[key_feats].apply(lambda x: str(list(x)), axis=1)
+        encoder_dict = dict(zip(encoder_df['key'].to_list(), encoder_df[feature_out].to_list()))
+        max_id = max(list(encoder_dict.values())) + 1
+
+        # get sub df
+        sub_df = df_x[grouped_features]
+        sub_df['key'] = sub_df[key_feats].apply(lambda x: str(list(x)), axis=1)
+
+        cate_id_list = []
+        for key_id in sub_df['key'].to_list():
+            if key_id not in encoder_dict:
+                encoder_dict[key_id] = max_id
+                max_id += 1
+            cate_id_list.append(encoder_dict[key_id])
+
+        #display(encoder_dict)
+        return pd.Series(cate_id_list, name = feature_out, index = sub_df.index)
+
+    def get_function_pd(self, trans_type = 'fit_transform'):
+        feature_in_out = copy.deepcopy(self.feature_in_out)
+        if trans_type == 'fit_transform':
+            def group_categorify(df):
+                df_features = [(group_parts, df[group_parts], dict_path, feature_out) for col, (group_parts, dict_path, feature_out) in feature_in_out.items()]
+                results = ParallelIterator.execute(df_features, GroupCategorifyOperation.group_label_encode, len(df_features), "GroupCategorify")
+                to_concat_df = pd.concat(results, axis=1)
+                to_concat_df.index = df.index
+                df = pd.concat([df, to_concat_df], axis=1)
+                return df
+        if trans_type == 'transform':
+            def group_categorify(df):
+                df_features = [(group_parts, df[group_parts], dict_path, feature_out) for col, (group_parts, dict_path, feature_out) in feature_in_out.items()]
+                results = ParallelIterator.execute(df_features, GroupCategorifyOperation.group_label_encode_transform, len(df_features), "GroupCategorify")
+                to_concat_df = pd.concat(results, axis=1)
+                to_concat_df.index = df.index
+                df = pd.concat([df, to_concat_df], axis=1)
+                return df
+        return group_categorify
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/featuretools_adaptor.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/featuretools_adaptor.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class FeaturetoolsOperation(BaseOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
         self.feature_in_out_map = self.op.config
         self.support_spark_dataframe = False
         self.support_spark_rdd = True
 
-    def get_function_pd(self):
+    def get_function_pd(self, trans_type = 'fit_transform'):
         feature_in_out_map = copy.deepcopy(self.feature_in_out_map)
         def generate_ft_feature(df):
             for in_feat_name, ops in feature_in_out_map.items():
                 if in_feat_name in df.columns:
                     for op in ops:
                         op_object = class_name_fix(op[1])()
                         df[op[0]] = op_object(df[in_feat_name])
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/fillna.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/fillna.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 class FillNaOperation(BaseOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
         self._fillna_feature_map = self.op.config
         self.support_spark_dataframe = True
         self.support_spark_rdd = True
     
-    def get_function_pd(self):
+    def get_function_pd(self, trans_type = 'fit_transform'):
         _fillna_feature_map = copy.deepcopy(self._fillna_feature_map)
         def fill_na(df):
             df.fillna(_fillna_feature_map, inplace=True, downcast=False)
             return df
         return fill_na
 
-    def get_function_spark(self, rdp):
+    def get_function_spark(self, rdp, trans_type = 'fit_transform'):
         def fill_na(df):
             return df.na.fill(self._fillna_feature_map)
         return fill_na
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/name.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/name.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,20 +5,20 @@
     def __init__(self, op_base):
         super().__init__(op_base)
         self.renamed = self.op.config
         self.support_spark_dataframe = True
         self.support_spark_rdd = True
         self.fast_without_dpp = True
         
-    def get_function_pd(self):
+    def get_function_pd(self, trans_type = 'fit_transform'):
         renamed = copy.deepcopy(self.renamed)
         def rename(df):
             return df.rename(columns = renamed)
         return rename
 
-    def get_function_spark(self, rdp):
+    def get_function_spark(self, rdp, trans_type = 'fit_transform'):
         def rename(df):
             for src, dst in self.renamed.items():
                 df = df.withColumnRenamed(src, dst)
             
             return df
         return rename
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/operations/tuple.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/operations/geograph.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from .base import BaseOperation
+from .featuretools_adaptor import FeaturetoolsOperation
+import copy
+from pyrecdp.core.utils import class_name_fix
 
-class TupleOperation(BaseOperation):        
+class HaversineOperation(FeaturetoolsOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
-        self.support_spark_dataframe = False
-        self.support_spark_rdd = True
-        self.feature_in = self.op.config['src']
-        self.feature_out = self.op.config['dst']
 
-    def get_function_pd(self):
-        feature_in = self.feature_in.copy()
-        feature_out = self.feature_out
-        def process(df):
-            df[feature_out] = df[feature_in].apply(tuple, axis=1)
+    def get_function_pd(self, trans_type = 'fit_transform'):
+        feature_in_out_map = copy.deepcopy(self.feature_in_out_map)
+        def generate_ft_feature(df):
+            for inputs_str, op in feature_in_out_map.items():
+                inputs = eval(inputs_str)
+                op_object = class_name_fix(op[1])()
+                df[op[0]] = op_object(df[inputs[0]], df[inputs[1]])
             return df
-        return process
+        return generate_ft_feature
 
-    def get_function_spark(self, rdp):
-        raise NotImplementedError(f"CoordinatesOperation spark dataframe is not supported yet.")
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/profilers/statics.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/statics.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/profilers/type_infer.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/profilers/type_infer.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,30 +96,48 @@
             estimated_size = result.explode().nunique()
             if estimated_size < 100:
                 return (',', result.explode().unique().tolist())
     except:
         pass
     
     return False
+ 
+def is_encoded(s):
+    line_id = s.first_valid_index()
+    if line_id < 0:
+        return False
+    sample_data = s.loc[line_id:(line_id+1000)]
+    from pyrecdp.primitives.generators.nlp import BertTokenizerDecode
+    proc_ = BertTokenizerDecode().get_function()
+    try:
+        proc_(sample_data)
+    except Exception as e:
+        #print(e)
+        return False
+    return True
          
 class TypeInferFeatureGenerator():
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
    
-    def fit_prepare(self, pipeline, children, max_idx, df, y = None):
+    def fit_prepare(self, pipeline, children, max_idx, df, y = None, ts = None):
         ret_pa_fields = []
         pa_schema = pipeline[children[0]].output
         for pa_field, feature_name in tqdm(zip(pa_schema, df.columns), total=len(df.columns)):
             config = {}
             # Add y_label to y column
             if feature_name == y:
                 config['is_label'] = True
                 if pa_field.is_string:
                     config['is_categorical_label'] = True
             else:
+                if feature_name == ts:
+                    config['is_timeseries'] = True
+                if pa_field.is_text and is_encoded(df[feature_name]):
+                    config['is_encoded'] = True
                 if try_datetime(df[feature_name]):
                     config['is_datetime'] = True
                 if try_category(df[feature_name]):
                     config['is_categorical'] = True
                 if try_numeric(df[feature_name]):
                     config['is_numeric'] = True
                 elif try_re_numeric(df[feature_name]):
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/spark_data_processor/data_processor.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/spark_data_processor/data_processor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/spark_data_processor/encoder.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/spark_data_processor/encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,34 +42,38 @@
             save_path = "%s/%s/%s" % (self.path_prefix,
                                       self.current_path, df_name)
         df.write.format('parquet').mode('overwrite').save(save_path)
         return self.spark.read.parquet(save_path)
 
 
 class TargetEncoder(Encoder):
-    def __init__(self, proc, x_col_list, y_col_list, out_col_list, out_name, out_dtype=None, y_mean_list=None, smooth=20, seed=42,threshold=0):
+    def __init__(self, proc, x_col_list, y_col_list, out_col_list, out_name, out_dtype=None, y_mean_list=None, smooth=20, seed=42,threshold=0, with_fold=True):
         super().__init__(proc)
         self.op_name = "TargetEncoder"
         self.x_col_list = x_col_list
         self.y_col_list = y_col_list
         self.out_col_list = out_col_list
         self.out_dtype = out_dtype
         self.out_name = out_name
         self.y_mean_list = y_mean_list
         self.seed = seed
         self.smooth = smooth
         self.expected_list_size = len(y_col_list)
         self.threshold = threshold
+        self.with_fold = with_fold
         if len(self.out_col_list) < self.expected_list_size:
             raise ValueError("TargetEncoder __init__, input out_col_list should be same size as y_col_list")      
         if y_mean_list != None and len(self.y_mean_list) < self.expected_list_size:
             raise ValueError("TargetEncoder __init__, input y_mean_list should be same size as y_col_list")        
 
     def transform(self, df):
         x_col = self.x_col_list
+        if not self.with_fold or "fold" not in df.columns:
+            numFolds = 5
+            df = df.withColumn("fold", f.round(f.rand(seed=42)*(numFolds-1)).cast("int"))
         cols = ['fold', x_col] if isinstance(x_col, str) else ['fold'] + x_col
         agg_per_fold = df.groupBy(cols)
         agg_all = df.groupBy(x_col)
 
         per_fold_list = []
         all_list = []
 
@@ -94,16 +98,14 @@
             y_mean = self.y_mean_list[i] if self.y_mean_list != None else None
             
             if y_mean is None:
                 y_mean = np.array(df.groupBy().mean(y_col).collect())[0][0]
             mean = float(y_mean)
             smooth = self.smooth
 
-            # print(agg_per_fold.dtypes)
-
             # prepare for agg_per_fold
             agg_per_fold = agg_per_fold.withColumn(
                 f'count_all_{y_col}', f.col(f'count_all_{y_col}')-f.col(f'count_{y_col}'))
             agg_per_fold = agg_per_fold.withColumn(
                 f'sum_all_{y_col}', f.col(f'sum_all_{y_col}')-f.col(f'sum_{y_col}'))
             agg_per_fold = agg_per_fold.withColumn(
                 out_col,
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/primitives/spark_data_processor/utils.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/primitives/spark_data_processor/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,37 +9,45 @@
 import pyspark.sql.functions as spk_func
 import psutil
 
 from pathlib import Path
 pathlib = Path(__file__).parent.parent.resolve()
 
 def create_spark_context(spark_mode='local', spark_master=None):
+    paral = psutil.cpu_count(logical=False)
+    total_mem = int((psutil.virtual_memory().total / (1 << 20)) * 0.8)
     if spark_mode == 'yarn' or spark_mode == 'standalone':
         if spark_master is None:
             raise ValueError("Spark master is None, please set correct spark master!")
-        spark = SparkSession.builder.master(spark_master)\
-                    .config("spark.sql.parquet.int96RebaseModeInWrite","CORRECTED")\
-                    .config("spark.sql.execution.arrow.pyspark.enabled","true")\
-                    .getOrCreate()
+    if spark_master is None:
+        spark_master = f'local[{paral}]'
+    
+    print(f"Will assign {paral} cores and {total_mem} M memory for spark")
+    conf = SparkConf()
+    conf_pairs = [("spark.executorEnv.TRANSFORMERS_OFFLINE", "1"), 
+                ("spark.executorEnv.TF_CPP_MIN_LOG_LEVEL", "2"),
+                ("spark.executorEnv.PYTHONPATH", pathlib),
+                ("spark.driver.maxResultSize", "64g"),
+                ("spark.sql.execution.arrow.pyspark.enabled", "true"),
+                ("spark.sql.parquet.int96RebaseModeInWrite", "CORRECTED")]
+    if spark_mode == 'yarn' or spark_mode == 'standalone':
+        ss = SparkSession.builder.master(spark_master).getOrCreate()
+        ss_conf = ss.conf
+        conf_pairs.append(("spark.driver.memory", ss_conf.get("spark.driver.memory", f"{total_mem}M")))
+        conf_pairs.append(("spark.executor.memory", ss_conf.get("spark.executor.memory", f"{total_mem}M")))
+        conf_pairs.append(("spark.executor.memoryOverhead", ss_conf.get("spark.executor.memoryOverhead", f"{int(total_mem)*0.1}M")))
+        conf_pairs.append(("spark.executor.cores", ss_conf.get("spark.executor.cores", f"{paral}M")))
+        ss.sparkContext.stop()
     else:
-        hname = os.uname()[1]
-        paral = psutil.cpu_count(logical=False)
-        total_mem = int((psutil.virtual_memory().total / (1 << 20)) * 0.8)
-        print(f"Will assign {paral} cores and {total_mem} M memory for spark")
-        spark = SparkSession.builder.master(f'local[{paral}]')\
-                    .appName("pyrecdp_spark_local")\
-                    .config("spark.executorEnv.HF_DATASETS_OFFLINE", "1")\
-                    .config("spark.executorEnv.TRANSFORMERS_OFFLINE", "1")\
-                    .config("spark.executorEnv.TF_CPP_MIN_LOG_LEVEL", "2")\
-                    .config("spark.executorEnv.PYTHONPATH", pathlib)\
-                    .config("spark.driver.memory", f"{total_mem}M")\
-                    .config("spark.driver.maxResultSize","64g")\
-                    .config("spark.sql.execution.arrow.pyspark.enabled","true")\
-                    .config("spark.sql.parquet.int96RebaseModeInWrite","CORRECTED")\
-                    .getOrCreate()
+        conf_pairs.append(("spark.driver.memory", f"{total_mem}M"))
+    conf.setAll(conf_pairs)
+    spark = SparkSession.builder.master(spark_master)\
+                .appName("pyrecdp_spark")\
+                .config(conf=conf)\
+                .getOrCreate()
     spark.sparkContext.setLogLevel("ERROR")
     # try:
     #     spark = SparkSession.builder.master(f'spark://{hname}:7077')\
     #             .appName("pyrecdp_spark_standalone").getOrCreate()
     #     SparkContext.addPyFile() //this need to be zip, implement later
     # except:
     #     spark = SparkSession.builder.master(f'local[*]')\
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/widgets/BaseWidget.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/widgets/BaseWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/widgets/TabWidget.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/widgets/TabWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/widgets/TableViewWidget.py` & `pyrecdp-1.6.1b2023072601/pyrecdp/widgets/TableViewWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/base.html` & `pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/overview.html` & `pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/overview.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/scripts.html` & `pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/scripts.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/styles.html` & `pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/styles.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp/widgets/templates/variables.html` & `pyrecdp-1.6.1b2023072601/pyrecdp/widgets/templates/variables.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/PKG-INFO` & `pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.6.1b2023071102
+Version: 1.6.1b2023072601
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrecdp-1.6.1b2023071102/pyrecdp.egg-info/SOURCES.txt` & `pyrecdp-1.6.1b2023072601/pyrecdp.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 pyrecdp/primitives/generators/datetime.py
 pyrecdp/primitives/generators/drop.py
 pyrecdp/primitives/generators/encode.py
 pyrecdp/primitives/generators/feature_transform.py
 pyrecdp/primitives/generators/featuretools_adaptor.py
 pyrecdp/primitives/generators/fillna.py
 pyrecdp/primitives/generators/geograph.py
+pyrecdp/primitives/generators/group_category.py
 pyrecdp/primitives/generators/name.py
 pyrecdp/primitives/generators/nlp.py
 pyrecdp/primitives/generators/relation.py
 pyrecdp/primitives/generators/type.py
 pyrecdp/primitives/operations/__init__.py
 pyrecdp/primitives/operations/base.py
 pyrecdp/primitives/operations/category.py
@@ -70,15 +71,18 @@
 pyrecdp/primitives/operations/fillna.py
 pyrecdp/primitives/operations/geograph.py
 pyrecdp/primitives/operations/merge.py
 pyrecdp/primitives/operations/name.py
 pyrecdp/primitives/operations/tuple.py
 pyrecdp/primitives/operations/type.py
 pyrecdp/primitives/profilers/__init__.py
+pyrecdp/primitives/profilers/cluster_infer.py
+pyrecdp/primitives/profilers/distribution_infer.py
 pyrecdp/primitives/profilers/statics.py
+pyrecdp/primitives/profilers/time_series_infer.py
 pyrecdp/primitives/profilers/type_infer.py
 pyrecdp/primitives/spark_data_processor/__init__.py
 pyrecdp/primitives/spark_data_processor/data_processor.py
 pyrecdp/primitives/spark_data_processor/encoder.py
 pyrecdp/primitives/spark_data_processor/utils.py
 pyrecdp/widgets/BaseWidget.py
 pyrecdp/widgets/PlotWidget.py
@@ -92,13 +96,15 @@
 pyrecdp/widgets/templates/interactions.html
 pyrecdp/widgets/templates/overview.html
 pyrecdp/widgets/templates/scripts.html
 pyrecdp/widgets/templates/styles.html
 pyrecdp/widgets/templates/variables.html
 tests/__init__.py
 tests/test_autofe.py
+tests/test_dataconversion.py
 tests/test_feature_estimator.py
 tests/test_feature_profiler.py
 tests/test_feature_wrangler.py
+tests/test_individual_method.py
 tests/test_pipeline_json.py
 tests/test_relational_builder.py
 tests/test_spark_dataprocessor.py
```

### Comparing `pyrecdp-1.6.1b2023071102/setup.py` & `pyrecdp-1.6.1b2023072601/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,11 +46,11 @@
         "transformers",
         "ipywidgets",
         "shapely",
         "graphviz",
         "requests",
         "distro",
         "pyspark",
-        "lightgbm",
+        "lightgbm<4.0.0",
         "matplotlib",
         "category_encoders"
         ])
```

### Comparing `pyrecdp-1.6.1b2023071102/tests/test_autofe.py` & `pyrecdp-1.6.1b2023072601/tests/test_autofe.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,25 +11,37 @@
     sys.path.append(pathlib)
 from pyrecdp.autofe import AutoFE
 from IPython.display import display
 
 
 class TestFE(unittest.TestCase):
 
-    def test_nyc_taxi(self):
+    def test_nyc_taxi_pandas(self):
+        train_data = pd.read_parquet(f"{pathlib}/tests/data/test_nyc_taxi_fare.parquet")
+        pipeline = AutoFE(dataset=train_data, label="fare_amount")
+        ret_df = pipeline.fit_transform(engine_type = 'pandas')
+        # test with shape
+        #pipeline.feature_importance()
+        
+    def test_nyc_taxi_spark(self):
         train_data = pd.read_parquet(f"{pathlib}/tests/data/test_nyc_taxi_fare.parquet")
         pipeline = AutoFE(dataset=train_data, label="fare_amount")
         ret_df = pipeline.fit_transform(engine_type = 'spark')
         # test with shape
         #pipeline.feature_importance()
         
-    def test_fraud_detect(self):
+    def test_fraud_detect_pandas(self):
         train_data = pd.read_parquet(f"{pathlib}/tests/data/test_frdtct.parquet")
         pipeline = AutoFE(dataset=train_data, label="Is Fraud?")
         ret_df = pipeline.fit_transform(engine_type = 'pandas')
+        
+    def test_fraud_detect_spark(self):
+        train_data = pd.read_parquet(f"{pathlib}/tests/data/test_frdtct.parquet")
+        pipeline = AutoFE(dataset=train_data, label="Is Fraud?")
+        ret_df = pipeline.fit_transform(engine_type = 'spark')
         # test with shape
         #pipeline.feature_importance()
         
     # def test_twitter_recsys(self):
     #     train_data = pd.read_parquet(f"{pathlib}/tests/data/test_twitter_recsys.parquet")
     #     pipeline = FeatureWrangler(dataset=train_data, label="reply")
     #     ret_df = pipeline.fit_transform(engine_type = 'pandas')
```

### Comparing `pyrecdp-1.6.1b2023071102/tests/test_feature_estimator.py` & `pyrecdp-1.6.1b2023072601/tests/test_feature_estimator.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/tests/test_feature_profiler.py` & `pyrecdp-1.6.1b2023072601/tests/test_feature_profiler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/tests/test_feature_wrangler.py` & `pyrecdp-1.6.1b2023072601/tests/test_feature_wrangler.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,22 @@
         display(ret_df)
         
     def test_frauddetect(self):
         train_data = pd.read_parquet(f"{pathlib}/tests/data/test_frdtct.parquet")
         pipeline = FeatureWrangler(dataset=train_data, label="Is Fraud?")
         ret_df = pipeline.fit_transform(engine_type = 'pandas')
         display(ret_df)
+
+    def test_ppdt(self):
+        train_data = pd.read_parquet(f"{pathlib}/tests/data/recsys2023_train.parquet")
+        #train_data = train_data[:10000]
+        pipeline = FeatureWrangler(dataset=train_data, label="is_installed", time_series = 'f_1')
+        # pipeline.export(f"{pathlib}/tests/ppdt_pipeline.json")
+        ret_df = pipeline.fit_transform(engine_type = 'pandas')
+        display(ret_df)
         
 class TestFeatureWranglerSparkBased(unittest.TestCase):
 
     def test_nyc_taxi(self):
         train_data = pd.read_parquet(f"{pathlib}/tests/data/test_nyc_taxi_fare.parquet")
         pipeline = FeatureWrangler(dataset=train_data, label="fare_amount")
         ret_df = pipeline.fit_transform(engine_type = 'spark')
```

### Comparing `pyrecdp-1.6.1b2023071102/tests/test_pipeline_json.py` & `pyrecdp-1.6.1b2023072601/tests/test_pipeline_json.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023071102/tests/test_relational_builder.py` & `pyrecdp-1.6.1b2023072601/tests/test_relational_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 pathlib = str(Path(__file__).parent.parent.resolve())
 print(pathlib)
 try:
     import pyrecdp
 except:
     print("Not detect system installed pyrecdp, using local one")
     sys.path.append(pathlib)
-from pyrecdp.autofe import RelationalBuilder
+from pyrecdp.autofe import RelationalBuilder, FeatureWrangler
 
 class TestRelationalBuilder(unittest.TestCase):
     def test_outbrain(self):
         train_data = {
             'clicks': "clicks_train.csv",
             'documents_categories': "documents_categories.csv",
             'documents_entities': "documents_entities.csv",
             'documents_meta': "documents_meta.csv",
             'documents_topics': "documents_topics.csv",
             'events': "events.csv",
             'page_views': "page_views_sample.csv",
             'promoted_content': "promoted_content.csv"}
         dir_path = f"{pathlib}/tests/data/outbrain/"
         train_data = dict((f_name, pd.read_csv(f"{dir_path}/{f_path}")) for f_name, f_path in train_data.items())
-        pipeline = RelationalBuilder(dataset=train_data, label="clicked")
+        relation_pipeline = RelationalBuilder(dataset=train_data, label="clicked")
+        pipeline = FeatureWrangler(data_pipeline=relation_pipeline)
         #print(pipeline.export())
         ret_df = pipeline.fit_transform(engine_type = 'pandas')
         # test with shape
         #self.assertEqual(ret_df.shape[0], 10000)
         #print(ret_df.dtypes)
         #self.assertTrue(ret_df.shape[1] >= 12)
 
@@ -40,9 +41,10 @@
             'documents_meta': "documents_meta.csv",
             'documents_topics': "documents_topics.csv",
             'events': "events.csv",
             'page_views': "page_views_sample.csv",
             'promoted_content': "promoted_content.csv"}
         dir_path = f"{pathlib}/tests/data/outbrain/"
         train_data = dict((f_name, f"{dir_path}/{f_path}") for f_name, f_path in train_data.items())
-        pipeline = RelationalBuilder(dataset=train_data, label="clicked")
+        relation_pipeline = RelationalBuilder(dataset=train_data, label="clicked")
+        pipeline = FeatureWrangler(data_pipeline=relation_pipeline)
         ret_df = pipeline.fit_transform(engine_type = 'spark')
```

### Comparing `pyrecdp-1.6.1b2023071102/tests/test_spark_dataprocessor.py` & `pyrecdp-1.6.1b2023072601/tests/test_spark_dataprocessor.py`

 * *Files identical despite different names*

