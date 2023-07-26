# Comparing `tmp/ceruleo-2.0.4.tar.gz` & `tmp/ceruleo-2.0.5.tar.gz`

## Comparing `ceruleo-2.0.4.tar` & `ceruleo-2.0.5.tar`

### file list

```diff
@@ -1,173 +1,173 @@
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ceruleo-2.0.4/.bumpversion.cfg
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ceruleo-2.0.4/.coveragerc
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 ceruleo-2.0.4/CONTRIBUTING.md
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 ceruleo-2.0.4/RELEASING.md
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 ceruleo-2.0.4/mkdocs.yml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 ceruleo-2.0.4/requirements.txt
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ceruleo-2.0.4/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ceruleo-2.0.4/.github/workflows/joss.yml
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 ceruleo-2.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 ceruleo-2.0.4/.github/workflows/test.yml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/__init__.py
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/transformed.py
--rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/ts_dataset.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/utils.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/analysis/__init__.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/analysis/correlation.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/analysis/distribution.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/analysis/numerical_features.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/analysis/sample_rate.py
--rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/catalog/CMAPSS.py
--rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/catalog/CMAPSS2.py
--rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/catalog/PHMDataset2018.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/catalog/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/graphics/__init__.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/graphics/analysis.py
--rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/graphics/duration.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/graphics/explanations.py
--rw-r--r--   0        0        0    21072 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/graphics/results.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/graphics/utils/__init__.py
--rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/graphics/utils/curly_brace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/iterators/__init__.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/iterators/batcher.py
--rw-r--r--   0        0        0    12822 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/iterators/iterators.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/iterators/sample_weight.py
--rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/iterators/shufflers.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/iterators/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/__init__.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/baseline.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/pytorch.py
--rw-r--r--   0        0        0     8792 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/sklearn.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/inspection/feature_importance.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/__init__.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/callbacks.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/dataset.py
--rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/layers.py
--rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/losses.py
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/weibull.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/CNLSTM.py
--rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/InceptionTime.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/MSWRLRCN.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/MVCNN.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/MultiScaleConvolutional.py
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/MultiTaskRUL.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/XCM.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/XiangQiangJianQiao.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/torch/__init__.py
--rw-r--r--   0        0        0    15678 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/torch/dsanet.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/torch/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/results/__init__.py
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/results/picewise_regression.py
--rw-r--r--   0        0        0    22960 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/results/results.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/target.py
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/__init__.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/cast.py
--rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/denoising.py
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/entropy.py
--rw-r--r--   0        0        0    33816 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/extraction.py
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/extraction_frequency.py
--rw-r--r--   0        0        0     9101 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/hurst.py
--rw-r--r--   0        0        0     9898 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/imputers.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/operations.py
--rw-r--r--   0        0        0    10745 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/outliers.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/resamplers.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/rolling_windows.py
--rw-r--r--   0        0        0    12451 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/scalers.py
--rw-r--r--   0        0        0     8107 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/selection.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/slicing.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/split.py
--rw-r--r--   0        0        0    10869 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/tdigest.py
--rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/transformation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/__init__.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/common.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/concatenate.py
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/graph_utils.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/mixin.py
--rw-r--r--   0        0        0     8446 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/transformers.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/transformerstep.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/__init__.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/cache_store.py
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/pipeline.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/runner.py
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/traversal.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/utils/__init__.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/utils/download.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/utils/lrucache.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/index.md
--rw-r--r--   0        0        0    13289 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/refs.bib
--rw-r--r--   0        0        0   185022 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/Example.ipynb
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/catalog.md
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/dataset.md
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/visualization.md
--rw-r--r--   0        0        0   478504 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/analysis/Sensor Validation.ipynb
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/analysis/correlation.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/analysis/distribution.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/analysis/sample_rate.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/analysis/sensor_validation.md
--rw-r--r--   0        0        0    17517 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/images/cerulean.png
--rw-r--r--   0        0        0    67664 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/images/unipd_logo.png
--rw-r--r--   0        0        0    50083 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/img/duration_histogram.png
--rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/iterators/Iterators.ipynb
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/iterators/batcher.md
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/iterators/iterators.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/iterators/shufflers.md
--rw-r--r--   0        0        0   631762 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/models/Models.ipynb
--rw-r--r--   0        0        0   304534 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/models/Models_sklearn.ipynb
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/models/baseline.md
--rw-r--r--   0        0        0   139463 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/models/models_tf.ipynb
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/models/sklearn.md
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/models/keras/index.md
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/models/keras/catalog/models.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/results/results.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/results/visualization.md
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/pipeline.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/transformers.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/features/cast.md
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/features/denoising.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/features/entropy.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/features/extraction.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/features/imputers.md
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/features/outliers.md
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/features/resamplers.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/features/selection.md
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 ceruleo-2.0.4/paper/paper.bib
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 ceruleo-2.0.4/paper/paper.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/manual_features.py
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_analysis.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_batcher.py
--rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_dataset.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_denoising.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_graph.py
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_graphics.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_imputers.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_iterators.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_lrucache.py
--rw-r--r--   0        0        0    13157 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_models.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_operations.py
--rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_pipeline.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_results.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_scalers.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_shufflers.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_transformation.py
--rw-r--r--   0        0        0    20808 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_transformers.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_utils.py
--rw-r--r--   0        0        0    48809 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_XCM_explanation-expected.png
--rw-r--r--   0        0        0    14744 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_barplot_errors_wrt_RUL-expected.png
--rw-r--r--   0        0        0    22355 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_boxplot_errors_wrt_RUL-expected.png
--rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_correlation_plot-expected.png
--rw-r--r--   0        0        0     9748 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_durations_boxplot-expected.png
--rw-r--r--   0        0        0    23670 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_durations_histogram-expected.png
--rw-r--r--   0        0        0    26658 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_plot_predictions_grid_1-expected.png
--rw-r--r--   0        0        0    38027 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_plot_predictions_grid_2-expected.png
--rw-r--r--   0        0        0    53987 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_shadedline_plot_errors_wrt_RUL-expected.png
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 ceruleo-2.0.4/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ceruleo-2.0.4/LICENSE
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 ceruleo-2.0.4/README.md
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ceruleo-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 ceruleo-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ceruleo-2.0.5/.bumpversion.cfg
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ceruleo-2.0.5/.coveragerc
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 ceruleo-2.0.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 ceruleo-2.0.5/RELEASING.md
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 ceruleo-2.0.5/mkdocs.yml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 ceruleo-2.0.5/requirements.txt
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 ceruleo-2.0.5/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ceruleo-2.0.5/.github/workflows/joss.yml
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 ceruleo-2.0.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 ceruleo-2.0.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/dataset/__init__.py
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/dataset/transformed.py
+-rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/dataset/ts_dataset.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/dataset/utils.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/dataset/analysis/__init__.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/dataset/analysis/correlation.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/dataset/analysis/distribution.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/dataset/analysis/numerical_features.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/dataset/analysis/sample_rate.py
+-rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/dataset/catalog/CMAPSS.py
+-rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/dataset/catalog/CMAPSS2.py
+-rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/dataset/catalog/PHMDataset2018.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/dataset/catalog/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/graphics/__init__.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/graphics/analysis.py
+-rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/graphics/duration.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/graphics/explanations.py
+-rw-r--r--   0        0        0    21072 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/graphics/results.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/graphics/utils/__init__.py
+-rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/graphics/utils/curly_brace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/iterators/__init__.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/iterators/batcher.py
+-rw-r--r--   0        0        0    12822 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/iterators/iterators.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/iterators/sample_weight.py
+-rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/iterators/shufflers.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/iterators/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/__init__.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/baseline.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/pytorch.py
+-rw-r--r--   0        0        0     8792 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/sklearn.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/inspection/feature_importance.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/keras/__init__.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/keras/callbacks.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/keras/dataset.py
+-rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/keras/layers.py
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/keras/losses.py
+-rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/keras/weibull.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/keras/catalog/CNLSTM.py
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/keras/catalog/InceptionTime.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/keras/catalog/MSWRLRCN.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/keras/catalog/MVCNN.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/keras/catalog/MultiScaleConvolutional.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/keras/catalog/MultiTaskRUL.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/keras/catalog/XCM.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/keras/catalog/XiangQiangJianQiao.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/keras/catalog/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/torch/__init__.py
+-rw-r--r--   0        0        0    15678 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/torch/dsanet.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/models/torch/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/results/__init__.py
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/results/picewise_regression.py
+-rw-r--r--   0        0        0    22960 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/results/results.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/target.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/__init__.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/cast.py
+-rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/denoising.py
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/entropy.py
+-rw-r--r--   0        0        0    33816 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/extraction.py
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/extraction_frequency.py
+-rw-r--r--   0        0        0     9101 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/hurst.py
+-rw-r--r--   0        0        0     9898 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/imputers.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/operations.py
+-rw-r--r--   0        0        0    10745 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/outliers.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/resamplers.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/rolling_windows.py
+-rw-r--r--   0        0        0    12451 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/scalers.py
+-rw-r--r--   0        0        0     8107 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/selection.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/slicing.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/split.py
+-rw-r--r--   0        0        0    10869 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/tdigest.py
+-rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/features/transformation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/functional/__init__.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/functional/common.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/functional/concatenate.py
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/functional/graph_utils.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/functional/mixin.py
+-rw-r--r--   0        0        0     8446 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/functional/transformers.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/functional/transformerstep.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/functional/pipeline/__init__.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/functional/pipeline/cache_store.py
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/functional/pipeline/pipeline.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/functional/pipeline/runner.py
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/functional/pipeline/traversal.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/transformation/functional/pipeline/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/utils/__init__.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/utils/download.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ceruleo-2.0.5/ceruleo/utils/lrucache.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/index.md
+-rw-r--r--   0        0        0    13289 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/refs.bib
+-rw-r--r--   0        0        0   185022 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/dataset/Example.ipynb
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/dataset/catalog.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/dataset/dataset.md
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/dataset/visualization.md
+-rw-r--r--   0        0        0   478504 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/dataset/analysis/Sensor Validation.ipynb
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/dataset/analysis/correlation.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/dataset/analysis/distribution.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/dataset/analysis/sample_rate.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/dataset/analysis/sensor_validation.md
+-rw-r--r--   0        0        0    17517 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/images/cerulean.png
+-rw-r--r--   0        0        0    67664 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/images/unipd_logo.png
+-rw-r--r--   0        0        0    50083 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/img/duration_histogram.png
+-rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/iterators/Iterators.ipynb
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/iterators/batcher.md
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/iterators/iterators.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/iterators/shufflers.md
+-rw-r--r--   0        0        0   631762 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/models/Models.ipynb
+-rw-r--r--   0        0        0   304534 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/models/Models_sklearn.ipynb
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/models/baseline.md
+-rw-r--r--   0        0        0   139463 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/models/models_tf.ipynb
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/models/sklearn.md
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/models/keras/index.md
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/models/keras/catalog/models.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/results/results.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/results/visualization.md
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/transformation/pipeline.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/transformation/transformers.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/transformation/features/cast.md
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/transformation/features/denoising.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/transformation/features/entropy.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/transformation/features/extraction.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/transformation/features/imputers.md
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/transformation/features/outliers.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/transformation/features/resamplers.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ceruleo-2.0.5/docs/transformation/features/selection.md
+-rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 ceruleo-2.0.5/paper/paper.bib
+-rw-r--r--   0        0        0     6780 2020-02-02 00:00:00.000000 ceruleo-2.0.5/paper/paper.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/manual_features.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_analysis.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_batcher.py
+-rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_dataset.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_denoising.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_graph.py
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_graphics.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_imputers.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_iterators.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_lrucache.py
+-rw-r--r--   0        0        0    13157 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_models.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_operations.py
+-rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_pipeline.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_results.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_scalers.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_shufflers.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_transformation.py
+-rw-r--r--   0        0        0    20808 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_transformers.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_utils.py
+-rw-r--r--   0        0        0    48809 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_images/test_XCM_explanation-expected.png
+-rw-r--r--   0        0        0    14744 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_images/test_barplot_errors_wrt_RUL-expected.png
+-rw-r--r--   0        0        0    22355 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_images/test_boxplot_errors_wrt_RUL-expected.png
+-rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_images/test_correlation_plot-expected.png
+-rw-r--r--   0        0        0     9748 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_images/test_durations_boxplot-expected.png
+-rw-r--r--   0        0        0    23670 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_images/test_durations_histogram-expected.png
+-rw-r--r--   0        0        0    26658 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_images/test_plot_predictions_grid_1-expected.png
+-rw-r--r--   0        0        0    38027 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_images/test_plot_predictions_grid_2-expected.png
+-rw-r--r--   0        0        0    53987 2020-02-02 00:00:00.000000 ceruleo-2.0.5/tests/test_images/test_shadedline_plot_errors_wrt_RUL-expected.png
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 ceruleo-2.0.5/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ceruleo-2.0.5/LICENSE
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 ceruleo-2.0.5/README.md
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 ceruleo-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 ceruleo-2.0.5/PKG-INFO
```

### Comparing `ceruleo-2.0.4/CONTRIBUTING.md` & `ceruleo-2.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/mkdocs.yml` & `ceruleo-2.0.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/.github/workflows/documentation.yml` & `ceruleo-2.0.5/.github/workflows/documentation.yml`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,14 @@
           python -m pip install --upgrade pip          
           python -m pip install flake8 pytest coverage
           python -m pip install wheel setuptools cython
           python -m pip install tensorflow
           python -m pip install --upgrade nbconvert
           python -m pip install  jinja2
           if [ -f requirements.txt ]; then python -m pip install -r requirements.txt; fi
-          python -m pip install -e $GITHUB_WORKSPACE
+          python -m pip install -e $GITHUB_WORKSPACE[doc]
 
 
       - name: Deploy docs
         run: |
           mkdocs gh-deploy --force
```

### Comparing `ceruleo-2.0.4/.github/workflows/joss.yml` & `ceruleo-2.0.5/.github/workflows/joss.yml`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/.github/workflows/publish.yml` & `ceruleo-2.0.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/.github/workflows/test.yml` & `ceruleo-2.0.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/dataset/transformed.py` & `ceruleo-2.0.5/ceruleo/dataset/transformed.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/dataset/ts_dataset.py` & `ceruleo-2.0.5/ceruleo/dataset/ts_dataset.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/dataset/utils.py` & `ceruleo-2.0.5/ceruleo/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/dataset/analysis/correlation.py` & `ceruleo-2.0.5/ceruleo/dataset/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/dataset/analysis/distribution.py` & `ceruleo-2.0.5/ceruleo/dataset/analysis/distribution.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/dataset/analysis/numerical_features.py` & `ceruleo-2.0.5/ceruleo/dataset/analysis/numerical_features.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/dataset/analysis/sample_rate.py` & `ceruleo-2.0.5/ceruleo/dataset/analysis/sample_rate.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/dataset/catalog/CMAPSS.py` & `ceruleo-2.0.5/ceruleo/dataset/catalog/CMAPSS.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/dataset/catalog/CMAPSS2.py` & `ceruleo-2.0.5/ceruleo/dataset/catalog/CMAPSS2.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/dataset/catalog/PHMDataset2018.py` & `ceruleo-2.0.5/ceruleo/dataset/catalog/PHMDataset2018.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/graphics/analysis.py` & `ceruleo-2.0.5/ceruleo/graphics/analysis.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/graphics/duration.py` & `ceruleo-2.0.5/ceruleo/graphics/duration.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/graphics/explanations.py` & `ceruleo-2.0.5/ceruleo/graphics/explanations.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/graphics/results.py` & `ceruleo-2.0.5/ceruleo/graphics/results.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/graphics/utils/curly_brace.py` & `ceruleo-2.0.5/ceruleo/graphics/utils/curly_brace.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/iterators/batcher.py` & `ceruleo-2.0.5/ceruleo/iterators/batcher.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/iterators/iterators.py` & `ceruleo-2.0.5/ceruleo/iterators/iterators.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/iterators/sample_weight.py` & `ceruleo-2.0.5/ceruleo/iterators/sample_weight.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/iterators/shufflers.py` & `ceruleo-2.0.5/ceruleo/iterators/shufflers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/iterators/utils.py` & `ceruleo-2.0.5/ceruleo/iterators/utils.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/baseline.py` & `ceruleo-2.0.5/ceruleo/models/baseline.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/pytorch.py` & `ceruleo-2.0.5/ceruleo/models/pytorch.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/sklearn.py` & `ceruleo-2.0.5/ceruleo/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/inspection/feature_importance.py` & `ceruleo-2.0.5/ceruleo/models/inspection/feature_importance.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/keras/callbacks.py` & `ceruleo-2.0.5/ceruleo/models/keras/callbacks.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/keras/dataset.py` & `ceruleo-2.0.5/ceruleo/models/keras/dataset.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/keras/layers.py` & `ceruleo-2.0.5/ceruleo/models/keras/layers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/keras/losses.py` & `ceruleo-2.0.5/ceruleo/models/keras/losses.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/keras/weibull.py` & `ceruleo-2.0.5/ceruleo/models/keras/weibull.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/keras/catalog/CNLSTM.py` & `ceruleo-2.0.5/ceruleo/models/keras/catalog/CNLSTM.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/keras/catalog/InceptionTime.py` & `ceruleo-2.0.5/ceruleo/models/keras/catalog/InceptionTime.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/keras/catalog/MSWRLRCN.py` & `ceruleo-2.0.5/ceruleo/models/keras/catalog/MSWRLRCN.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/keras/catalog/MVCNN.py` & `ceruleo-2.0.5/ceruleo/models/keras/catalog/MVCNN.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/keras/catalog/MultiScaleConvolutional.py` & `ceruleo-2.0.5/ceruleo/models/keras/catalog/MultiScaleConvolutional.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/keras/catalog/MultiTaskRUL.py` & `ceruleo-2.0.5/ceruleo/models/keras/catalog/MultiTaskRUL.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/keras/catalog/XCM.py` & `ceruleo-2.0.5/ceruleo/models/keras/catalog/XCM.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/keras/catalog/XiangQiangJianQiao.py` & `ceruleo-2.0.5/ceruleo/models/keras/catalog/XiangQiangJianQiao.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/torch/dsanet.py` & `ceruleo-2.0.5/ceruleo/models/torch/dsanet.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/models/torch/model.py` & `ceruleo-2.0.5/ceruleo/models/torch/model.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/results/picewise_regression.py` & `ceruleo-2.0.5/ceruleo/results/picewise_regression.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/results/results.py` & `ceruleo-2.0.5/ceruleo/results/results.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/target.py` & `ceruleo-2.0.5/ceruleo/transformation/target.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/utils.py` & `ceruleo-2.0.5/ceruleo/transformation/utils.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/features/cast.py` & `ceruleo-2.0.5/ceruleo/transformation/features/cast.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/features/denoising.py` & `ceruleo-2.0.5/ceruleo/transformation/features/denoising.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/features/entropy.py` & `ceruleo-2.0.5/ceruleo/transformation/features/entropy.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/features/extraction.py` & `ceruleo-2.0.5/ceruleo/transformation/features/extraction.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/features/extraction_frequency.py` & `ceruleo-2.0.5/ceruleo/transformation/features/extraction_frequency.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/features/hurst.py` & `ceruleo-2.0.5/ceruleo/transformation/features/hurst.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/features/imputers.py` & `ceruleo-2.0.5/ceruleo/transformation/features/imputers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/features/outliers.py` & `ceruleo-2.0.5/ceruleo/transformation/features/outliers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/features/resamplers.py` & `ceruleo-2.0.5/ceruleo/transformation/features/resamplers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/features/rolling_windows.py` & `ceruleo-2.0.5/ceruleo/transformation/features/rolling_windows.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/features/scalers.py` & `ceruleo-2.0.5/ceruleo/transformation/features/scalers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/features/selection.py` & `ceruleo-2.0.5/ceruleo/transformation/features/selection.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/features/slicing.py` & `ceruleo-2.0.5/ceruleo/transformation/features/slicing.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/features/split.py` & `ceruleo-2.0.5/ceruleo/transformation/features/split.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/features/tdigest.py` & `ceruleo-2.0.5/ceruleo/transformation/features/tdigest.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/features/transformation.py` & `ceruleo-2.0.5/ceruleo/transformation/features/transformation.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/functional/concatenate.py` & `ceruleo-2.0.5/ceruleo/transformation/functional/concatenate.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/functional/graph_utils.py` & `ceruleo-2.0.5/ceruleo/transformation/functional/graph_utils.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/functional/mixin.py` & `ceruleo-2.0.5/ceruleo/transformation/functional/mixin.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/functional/transformers.py` & `ceruleo-2.0.5/ceruleo/transformation/functional/transformers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/functional/transformerstep.py` & `ceruleo-2.0.5/ceruleo/transformation/functional/transformerstep.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/cache_store.py` & `ceruleo-2.0.5/ceruleo/transformation/functional/pipeline/cache_store.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/pipeline.py` & `ceruleo-2.0.5/ceruleo/transformation/functional/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/runner.py` & `ceruleo-2.0.5/ceruleo/transformation/functional/pipeline/runner.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/traversal.py` & `ceruleo-2.0.5/ceruleo/transformation/functional/pipeline/traversal.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/utils.py` & `ceruleo-2.0.5/ceruleo/transformation/functional/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/utils/download.py` & `ceruleo-2.0.5/ceruleo/utils/download.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/ceruleo/utils/lrucache.py` & `ceruleo-2.0.5/ceruleo/utils/lrucache.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/docs/index.md` & `ceruleo-2.0.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/docs/refs.bib` & `ceruleo-2.0.5/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/docs/dataset/Example.ipynb` & `ceruleo-2.0.5/docs/dataset/Example.ipynb`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/docs/dataset/catalog.md` & `ceruleo-2.0.5/docs/dataset/catalog.md`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/docs/dataset/analysis/Sensor Validation.ipynb` & `ceruleo-2.0.5/docs/dataset/analysis/Sensor Validation.ipynb`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/docs/dataset/analysis/sensor_validation.md` & `ceruleo-2.0.5/docs/dataset/analysis/sensor_validation.md`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/docs/images/cerulean.png` & `ceruleo-2.0.5/docs/images/cerulean.png`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/docs/images/unipd_logo.png` & `ceruleo-2.0.5/docs/images/unipd_logo.png`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/docs/img/duration_histogram.png` & `ceruleo-2.0.5/docs/img/duration_histogram.png`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/docs/iterators/Iterators.ipynb` & `ceruleo-2.0.5/docs/iterators/Iterators.ipynb`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/docs/iterators/iterators.md` & `ceruleo-2.0.5/docs/iterators/iterators.md`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/docs/models/Models.ipynb` & `ceruleo-2.0.5/docs/models/Models.ipynb`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/docs/models/Models_sklearn.ipynb` & `ceruleo-2.0.5/docs/models/Models_sklearn.ipynb`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/docs/models/models_tf.ipynb` & `ceruleo-2.0.5/docs/models/models_tf.ipynb`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/paper/paper.md` & `ceruleo-2.0.5/paper/paper.md`

 * *Files 25% similar despite different names*

```diff
@@ -19,32 +19,41 @@
     index: 1
 date: 20 Dic 2022
 bibliography: paper.bib
 ---
 
 # Summary
 
-`CeRULEo`, which stands for Comprehensive utilitiEs for Remaining Useful Life Estimation methOds, is a Python package designed to train and evaluate regression models for predicting remaining useful life (RUL) of equipment. RUL estimation is a process that uses prediction methods to forecast the future performance of machinery and obtain the time left before machinery loses its operation ability.  The remaining useful life  estimation has been considered as a central 
+`CeRULEo`, which stands for Comprehensive utilitiEs for Remaining Useful Life Estimation methOds, is a Python package designed to train and evaluate regression models for predicting remaining useful life (RUL) of equipment. RUL estimation is a process that uses prediction methods to forecast the future performance of machinery and obtain the time left before machinery loses its operation ability.  The RUL  estimation has been considered as a central 
 technology of Predictive Maintenance (PdM) [@heimes2008recurrent; @li2018remaining].  PdM  techniques can statistically evaluate a piece of equipment's health status,  enabling early identification of impending failures and prompt pre-failure  interventions, thanks to prediction tools based on historical data [@susto2014machine].  `CeRULEo` offers a comprehensive suite of tools to help with the analysis and pre-processing of preventive maintenance data. These tools also enable the training and evaluation of RUL models that are tailored to the specific needs of the problem at hand. 
 
  
 # Statement of need
 
-Effective maintenance management helps reduce costs related to defective products and equipment downtime. A well-planned maintenance strategy improves reliability, prevents unexpected outages, and lowers operating costs. In Industry 4.0, data from the manufacturing process can enhance decision-making. RUL estimation uses prediction techniques to forecast a machine's future performance based on historical data and determine its remaining useful life, enabling early identification of potential failures and prompt pre-failure interventions. In this context, `CeRULEo` provides a comprehensive set of utilities designed to train and evaluate regression models for predicting remaining useful life of equipment. 
+Effective maintenance management helps reduce costs related to defective products and equipment downtime. A well-planned maintenance strategy improves reliability, prevents unexpected outages, and lowers operating costs. 
 
-In order to achieve good performance, RUL regression requires data preparation and feature engineering. Typically, machinery data is provided as time series data from various sensors during operation. The first step in data preparation is often to create a dataset based on run-to-failure cycles. This involves dividing the time series into segments where the equipment starts in a healthy state and ends in a failure state, or is close to failure. The second step of data preparation is preprocessing. While predictive maintenance models can be used in a variety of contexts with different data sources and errors, there are some general techniques that can be applied [@serradilla2022deep], such as time-series validation, imputing missing values, handling homogeneous or non-homogeneous sampling rates, addressing values, range and behaviour differences across difference machines and the creation of run-to-failure-cycle-based data. 
 
+In Industry 5.0, the industrial machines produce a large amount of data which can be used to predict an asset’s life [@khan2023changes]. RUL estimation uses prediction techniques to forecast a machine's future performance based on historical data, enabling early identification of potential failures and prompt pre-failure interventions. 
 
-`CeRULEo` addresses these issues by providing a comprehensive toolkit for preprocessing time series data for use in predictive maintenance models, with a focus on run-to-failure cycles. The preprocessing includes sensor data validation methods, for studyng not only missing and corrupted values but also distribution drift among different pieces of equipment. 
+Within the PdM and RUL regression ecosystem, finding a library that effectively combines modelling, feature extraction capabilities, and tools for model comparison poses a significant challenge. While numerous repositories and libraries exist for models and feature extraction in time series data [@christ2018time; @JMLR:v21:20-091], few offer a comprehensive solution that integrates both aspects effectively. The prog_models and prog_als libraries from NASA [@2022_nasa_prog_models] come closest to fulfilling this requirement. However, they have a strong focus on simulation and lack extensive mechanisms for feature extraction from time series data. 
 
-In addition to preprocessing, it enables the iteration of machine data for use in both mini-batch and full-batch regression models, and is compatible with popular machine learning frameworks such as scikit-learn and tensorflow. The library also includes a catalog of successful deep learning models [@jayasinghe2019temporal; @li2020remaining; @CHEN2022104969] from the literature and a collection of commonly used remaining useful life datasets for quick model evaluation.
+On the other hand, `CeRULEo` provides a comprehensive set of utilities designed to train and evaluate regression models for predicting RUL of equipment. `CeRULEo`  emphasizes a data-driven approach using industrial data, particularly when a simulation model is unavailable or costly to develop, prioritizing model library-agnosticism for easy deployment in any production environment. 
 
-In the context of predictive maintenance, explainability is crucial. As such, `CeRULEo` includes two explainable models: one that can select the most relevant features for the model [@lemhadri2021lassonet], and a convolutional model [@fauvel2021xcm] that provides post-hoc explanations of the predictions to understand the reasoning behind the predicted remaining useful life. This helps users better understand and trust the model's predictions.
+In order to achieve good performance, RUL regression requires data preparation and feature engineering. Typically, machinery data is provided as time series data from various sensors during operation. The first step in data preparation is often to create a dataset based on run-to-failure cycles. This involves dividing the time series into segments where the equipment starts in a healthy state and ends in a failure state, or is close to failure. The second step of data preparation is preprocessing. While PdM models can be used in a variety of contexts with different data sources and errors, there are some general techniques that can be applied [@serradilla2022deep], such as time-series validation, imputing missing values, handling homogeneous or non-homogeneous sampling rates, addressing values, range and behaviour differences across different machines and the creation of run-to-failure-cycle-based data. 
+
+
+`CeRULEo` addresses these issues by providing a comprehensive toolkit for preprocessing time series data for use in PdM models, with a focus on run-to-failure cycles. The preprocessing includes sensor data validation methods, for studying not only missing and corrupted values but also distribution drift among different pieces of equipment. 
+
+In addition to preprocessing, it enables the iteration of machine data for use in both mini-batch and full-batch regression models, and is compatible with popular machine learning frameworks such as scikit-learn [@scikit-learn] and tensorflow [@tensorflow2015-whitepaper]. The library also includes a catalog of successful deep learning models [@jayasinghe2019temporal; @li2020remaining; @CHEN2022104969] from the literature and a collection of commonly used RUL datasets for quick model evaluation.
+
+The acceptance of PdM technologies is pivotal in Industry 5.0 for successful implementation, but hesitations or reluctance by decision-makers  can still pose significant barriers [@van2022predictive]. One effective approach to foster acceptance and understanding is through explainability, which plays a crucial role in PdM.
+As such, `CeRULEo`  incorporates explainable models capable of providing additional information about the predictions, enhancing comprehension: one that can select the most relevant features for the model [@lemhadri2021lassonet], and a convolutional model [@fauvel2021xcm] that provides post-hoc explanations of the predictions to understand the reasoning behind the predicted RUL. 
+
+Moreover, `CeRULEo` provides tools for evaluating and comparing PdM models based on not only traditional regression metrics, but also on their ability to prevent errors and reduce costs. In many cases, the costs of not accurately detecting or anticipating faults can be much higher than the cost of inspections or maintenance due to reduced efficiency, unplanned downtime, and corrective maintenance expenses. In PdM, it is particularly important to be accurate about the RUL  of equipment near the end of its lifespan, as an overestimation of RUL can have serious consequences when immediate action is required. `CeRULEo` addresses this issue by providing mechanisms for weighting samples according to their importance and asymmetric losses for training models, as well as visualization tools for understanding model performance in relation to true RUL.
 
-Moreover, `CeRULEo` provides tools for evaluating and comparing predictive maintenance models based on not only traditional regression metrics, but also on their ability to prevent errors and reduce costs. In many cases, the costs of not accurately detecting or anticipating faults can be much higher than the cost of inspections or maintenance due to reduced efficiency, unplanned downtime, and corrective maintenance expenses. In predictive maintenance, it is particularly important to be accurate about the remaining useful life  of equipment near the end of its lifespan, as an overestimation of RUL can have serious consequences when immediate action is required. `CeRULEo` addresses this issue by providing mechanisms for weighting samples according to their importance and asymmetric losses for training models, as well as visualization tools for understanding model performance in relation to true RUL.
 
 
 # Financial Acknowledgement
 
-The Italian Government PNRR iniatiatives 'Partenariato 11: Made in Italy circolare e sostenibile' and 'Ecosistema dell'Innovazione - iNest' are gratefully acknowledged for partially financing this research activity.
+The Italian Government PNRR initiatives 'Partenariato 11: Made in Italy circolare e sostenibile' and 'Ecosistema dell'Innovazione - iNest' are gratefully acknowledged for partially financing this research activity.
 
 # References
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ceruleo-2.0.4/tests/manual_features.py` & `ceruleo-2.0.5/tests/manual_features.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_analysis.py` & `ceruleo-2.0.5/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_batcher.py` & `ceruleo-2.0.5/tests/test_batcher.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_dataset.py` & `ceruleo-2.0.5/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_denoising.py` & `ceruleo-2.0.5/tests/test_denoising.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_graph.py` & `ceruleo-2.0.5/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_graphics.py` & `ceruleo-2.0.5/tests/test_graphics.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_imputers.py` & `ceruleo-2.0.5/tests/test_imputers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_iterators.py` & `ceruleo-2.0.5/tests/test_iterators.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_lrucache.py` & `ceruleo-2.0.5/tests/test_lrucache.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_models.py` & `ceruleo-2.0.5/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_operations.py` & `ceruleo-2.0.5/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_pipeline.py` & `ceruleo-2.0.5/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_results.py` & `ceruleo-2.0.5/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_scalers.py` & `ceruleo-2.0.5/tests/test_scalers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_shufflers.py` & `ceruleo-2.0.5/tests/test_shufflers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_transformation.py` & `ceruleo-2.0.5/tests/test_transformation.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_transformers.py` & `ceruleo-2.0.5/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_utils.py` & `ceruleo-2.0.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_images/test_XCM_explanation-expected.png` & `ceruleo-2.0.5/tests/test_images/test_XCM_explanation-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_images/test_barplot_errors_wrt_RUL-expected.png` & `ceruleo-2.0.5/tests/test_images/test_barplot_errors_wrt_RUL-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_images/test_boxplot_errors_wrt_RUL-expected.png` & `ceruleo-2.0.5/tests/test_images/test_boxplot_errors_wrt_RUL-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_images/test_correlation_plot-expected.png` & `ceruleo-2.0.5/tests/test_images/test_correlation_plot-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_images/test_durations_boxplot-expected.png` & `ceruleo-2.0.5/tests/test_images/test_durations_boxplot-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_images/test_durations_histogram-expected.png` & `ceruleo-2.0.5/tests/test_images/test_durations_histogram-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_images/test_plot_predictions_grid_1-expected.png` & `ceruleo-2.0.5/tests/test_images/test_plot_predictions_grid_1-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_images/test_plot_predictions_grid_2-expected.png` & `ceruleo-2.0.5/tests/test_images/test_plot_predictions_grid_2-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/tests/test_images/test_shadedline_plot_errors_wrt_RUL-expected.png` & `ceruleo-2.0.5/tests/test_images/test_shadedline_plot_errors_wrt_RUL-expected.png`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/.gitignore` & `ceruleo-2.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/LICENSE` & `ceruleo-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.4/README.md` & `ceruleo-2.0.5/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -30,16 +30,29 @@
 
 ```bash
 git clone https://github.com/lucianolorenti/ceruleo.git
 cd ceruleo
 pip install .
 ```
 
+# Contributing
 
+We love your input! We want to make contributing to this project as easy and transparent as possible, whether it's:
 
+* Reporting a bug
+* Discussing the current state of the code
+* Submitting a fix
+* Proposing new features
 
+Please feel free to open an [issue](https://github.com/lucianolorenti/ceruleo/issues/new/choose) if you have any questions, find any bugs, or have any ideas.  
+Further information on how to contribute can be found by clicking  [here](https://github.com/lucianolorenti/ceruleo/blob/main/CONTRIBUTING.md).
 
 
- Made with <3 @   <a href="https://www.dei.unipd.it/">  
+
+
+
+
+
+Made with <3 @   <a href="https://www.dei.unipd.it/">  
          <img alt="University of Padova" src="https://github.com/lucianolorenti/ceruleo/blob/main/docs/images/unipd_logo.png?raw=true" width=100 />
       </a>
```

#### html2text {}

```diff
@@ -12,8 +12,15 @@
 c879c234d7741885576ddc682416b41f) ## What is it? **CeRULeo** is a Python
 package that provides a flexible environment designed to make working with
 predictive maintenance task both easy and intuitive. # Installation It is
 recommended to use pip for installation. Please make sure the latest version is
 installed: ```bash pip install ceruleo # normal install pip install --upgrade
 ceruleo # or update if needed ``` Alternatively, you could clone and install it
 from the sources: ```bash git clone https://github.com/lucianolorenti/
-ceruleo.git cd ceruleo pip install . ``` Made with <3 @ [University_of_Padova]
+ceruleo.git cd ceruleo pip install . ``` # Contributing We love your input! We
+want to make contributing to this project as easy and transparent as possible,
+whether it's: * Reporting a bug * Discussing the current state of the code *
+Submitting a fix * Proposing new features Please feel free to open an [issue]
+(https://github.com/lucianolorenti/ceruleo/issues/new/choose) if you have any
+questions, find any bugs, or have any ideas. Further information on how to
+contribute can be found by clicking [here](https://github.com/lucianolorenti/
+ceruleo/blob/main/CONTRIBUTING.md). Made with <3 @ [University_of_Padova]
```

### Comparing `ceruleo-2.0.4/pyproject.toml` & `ceruleo-2.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,23 +14,23 @@
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Artificial Intelligence"
 ]
 dependencies = [
         "pandas >= 1.5",
         "numpy >= 1.22",
         "tqdm >= 4.56",
-        "scikit-learn >= 0.24",
+        "scikit-learn >= 0.24, <1.3",
         "emd >= 0.4",
         "mmh3   >= 2.0",
         "pyarrow >= 4",
         "gdown >= 4.2",
         "pyinform >= 0.2",
         "pyts >= 0.12",
         "seaborn >= 0.11",
-        "antropy >= 0.1",
+        "antropy >= 0.1.5",
         "uncertainties >= 3.1",
         "PyWavelets >= 1.3",
 ]
 
 
 [tool.hatch.version]
 path = "ceruleo/__init__.py"
@@ -49,12 +49,13 @@
     "xgboost >= 1.5"
 ]
 doc = [
     "mkdocs", 
     "mkdocstrings[python]",
     "mkdocs-material",
     "mkdocs-jupyter",
+    "notebook<=6.5",
     "jupyter_contrib_nbextensions",
     "mkdocstrings",
     "mkdocs-bibtex",
     "sphinxcontrib.bibtex"
 ]
```

