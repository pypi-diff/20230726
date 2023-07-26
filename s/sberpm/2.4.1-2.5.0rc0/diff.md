# Comparing `tmp/sberpm-2.4.1.tar.gz` & `tmp/sberpm-2.5.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sberpm-2.4.1.tar", last modified: Thu May 25 06:05:38 2023, max compression
+gzip compressed data, was "sberpm-2.5.0rc0.tar", last modified: Wed Jul 26 11:24:23 2023, max compression
```

## Comparing `sberpm-2.4.1.tar` & `sberpm-2.5.0rc0.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.363329 sberpm-2.4.1/
--rw-rw-rw-   0        0        0      274 2023-03-14 12:01:36.000000 sberpm-2.4.1/.gitignore
--rw-rw-rw-   0        0        0    29507 2023-01-26 18:07:31.000000 sberpm-2.4.1/LICENSE
--rw-rw-rw-   0        0        0    62148 2023-01-26 18:07:31.000000 sberpm-2.4.1/LICENSE_RUS
--rw-rw-rw-   0        0        0      242 2023-01-26 18:07:31.000000 sberpm-2.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2887 2023-05-25 06:05:38.364340 sberpm-2.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2213 2023-04-05 21:34:08.000000 sberpm-2.4.1/README.md
--rw-rw-rw-   0        0        0     1147 2023-05-25 05:48:29.000000 sberpm-2.4.1/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.111308 sberpm-2.4.1/sberpm/
--rw-rw-rw-   0        0        0      542 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/__init__.py
--rw-rw-rw-   0        0        0    31800 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/_holder.py
--rw-rw-rw-   0        0        0      947 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/_utils.py
--rw-rw-rw-   0        0        0       21 2023-05-25 05:50:57.000000 sberpm-2.4.1/sberpm/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.149312 sberpm-2.4.1/sberpm/autoinsights/
--rw-rw-rw-   0        0        0      120 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/autoinsights/__init__.py
--rw-rw-rw-   0        0        0      188 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/autoinsights/_influencing_activities.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.151311 sberpm-2.4.1/sberpm/autoinsights/file_obf/
--rw-rw-rw-   0        0        0    12828 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/autoinsights/file_obf/_influencing_activities.obfsbpm
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.156309 sberpm-2.4.1/sberpm/bpmn/
--rw-rw-rw-   0        0        0      177 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/bpmn/__init__.py
--rw-rw-rw-   0        0        0    26484 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/bpmn/_bpmn_file_to_graph.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.173312 sberpm-2.4.1/sberpm/bpmn/_bpmn_graph_to_file/
--rw-rw-rw-   0        0        0      103 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/bpmn/_bpmn_graph_to_file/__init__.py
--rw-rw-rw-   0        0        0     4093 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_exporter.py
--rw-rw-rw-   0        0        0     6642 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_xml_maker.py
--rw-rw-rw-   0        0        0     4680 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/bpmn/_bpmn_graph_to_file/_petri_net_to_bpmn.py
--rw-rw-rw-   0        0        0     1545 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/bpmn/_bpmn_graph_to_file/grandalf.py
--rw-rw-rw-   0        0        0     5350 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/bpmn/_bpmn_graph_to_file/graphviz.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.180312 sberpm-2.4.1/sberpm/column_matching/
--rw-rw-rw-   0        0        0      102 2023-03-14 12:01:36.000000 sberpm-2.4.1/sberpm/column_matching/__init__.py
--rw-rw-rw-   0        0        0      182 2023-03-14 12:01:36.000000 sberpm-2.4.1/sberpm/column_matching/_column_matching.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.182311 sberpm-2.4.1/sberpm/column_matching/file_obf/
--rw-rw-rw-   0        0        0     5710 2023-03-14 12:01:36.000000 sberpm-2.4.1/sberpm/column_matching/file_obf/_column_matching_.obfsbpm
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.189312 sberpm-2.4.1/sberpm/conformance_checking/
--rw-rw-rw-   0        0        0      202 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/conformance_checking/__init__.py
--rw-rw-rw-   0        0        0     6061 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/conformance_checking/_conformance_checking.py
--rw-rw-rw-   0        0        0     9883 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/conformance_checking/_token_replay.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.195316 sberpm-2.4.1/sberpm/decision_mining/
--rw-rw-rw-   0        0        0      100 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/decision_mining/__init__.py
--rw-rw-rw-   0        0        0    33758 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/decision_mining/_decision_mining.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.199316 sberpm-2.4.1/sberpm/graph_stats/
--rw-rw-rw-   0        0        0      146 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/graph_stats/__init__.py
--rw-rw-rw-   0        0        0     3336 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/graph_stats/centrality.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.206316 sberpm-2.4.1/sberpm/imitation/
--rw-rw-rw-   0        0        0      160 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/imitation/__init__.py
--rw-rw-rw-   0        0        0      176 2023-05-25 05:48:29.000000 sberpm-2.4.1/sberpm/imitation/_simulation.py
--rw-rw-rw-   0        0        0      176 2023-05-25 05:48:29.000000 sberpm-2.4.1/sberpm/imitation/_validation.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.212315 sberpm-2.4.1/sberpm/imitation/file_obf/
--rw-rw-rw-   0        0        0    21873 2023-05-25 05:48:29.000000 sberpm-2.4.1/sberpm/imitation/file_obf/_simulation.obfsbpm
--rw-rw-rw-   0        0        0    11229 2023-05-25 05:48:29.000000 sberpm-2.4.1/sberpm/imitation/file_obf/_validation.obfsbpm
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.234316 sberpm-2.4.1/sberpm/metrics/
--rw-rw-rw-   0        0        0      371 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/metrics/__init__.py
--rw-rw-rw-   0        0        0     5524 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/metrics/_activity_metric.py
--rw-rw-rw-   0        0        0     6918 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/metrics/_base_metric.py
--rw-rw-rw-   0        0        0     4077 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/metrics/_id_metric.py
--rw-rw-rw-   0        0        0     5173 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/metrics/_trace_metric.py
--rw-rw-rw-   0        0        0     6093 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/metrics/_transition_metric.py
--rw-rw-rw-   0        0        0     3995 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/metrics/_user_metric.py
--rw-rw-rw-   0        0        0      389 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/metrics/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.269317 sberpm-2.4.1/sberpm/miners/
--rw-rw-rw-   0        0        0     1374 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/miners/__init__.py
--rw-rw-rw-   0        0        0     9571 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/miners/_abstract_miner.py
--rw-rw-rw-   0        0        0    19774 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/miners/_alpha_miner.py
--rw-rw-rw-   0        0        0    10578 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/miners/_alpha_plus_miner.py
--rw-rw-rw-   0        0        0      174 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/miners/_auto_miner.py
--rw-rw-rw-   0        0        0     3153 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/miners/_causal_miner.py
--rw-rw-rw-   0        0        0    18462 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/miners/_correlation_miner.py
--rw-rw-rw-   0        0        0     9122 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/miners/_heu_miner.py
--rw-rw-rw-   0        0        0     3896 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/miners/_inductive_miner.py
--rw-rw-rw-   0        0        0     8354 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/miners/_inductive_utils.py
--rw-rw-rw-   0        0        0      174 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/miners/_ml_miner.py
--rw-rw-rw-   0        0        0      178 2023-05-25 05:48:29.000000 sberpm-2.4.1/sberpm/miners/_parallel_miner.py
--rw-rw-rw-   0        0        0     2678 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/miners/_simple_miner.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.277318 sberpm-2.4.1/sberpm/miners/file_obf/
--rw-rw-rw-   0        0        0     3192 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/miners/file_obf/_auto_miner.obfsbpm
--rw-rw-rw-   0        0        0     5082 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/miners/file_obf/_ml_miner.obfsbpm
--rw-rw-rw-   0        0        0     5874 2023-05-25 05:48:29.000000 sberpm-2.4.1/sberpm/miners/file_obf/_parallel_miner.obfsbpm
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.282318 sberpm-2.4.1/sberpm/miners/mining_utils/
--rw-rw-rw-   0        0        0     8347 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/miners/mining_utils/_inductive_utils.py
--rw-rw-rw-   0        0        0    25893 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/miners/mining_utils/_node_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.285319 sberpm-2.4.1/sberpm/ml/
--rw-rw-rw-   0        0        0      179 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/ml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.306321 sberpm-2.4.1/sberpm/ml/anomaly_detection/
--rw-rw-rw-   0        0        0      571 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/ml/anomaly_detection/__init__.py
--rw-rw-rw-   0        0        0    11459 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/ml/anomaly_detection/_outlier_detector.py
--rw-rw-rw-   0        0        0     4669 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/ml/anomaly_detection/_outlier_detector_ensemble.py
--rw-rw-rw-   0        0        0     5295 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/ml/anomaly_detection/_outliercblof.py
--rw-rw-rw-   0        0        0     2404 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/ml/anomaly_detection/_outliercustom.py
--rw-rw-rw-   0        0        0     4911 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/ml/anomaly_detection/_outlierforest.py
--rw-rw-rw-   0        0        0     6340 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/ml/anomaly_detection/_outlierlof.py
--rw-rw-rw-   0        0        0     4804 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/ml/anomaly_detection/_outlierocsvm.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.312321 sberpm-2.4.1/sberpm/ml/chronometrage/
--rw-rw-rw-   0        0        0       76 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/ml/chronometrage/__init__.py
--rw-rw-rw-   0        0        0     6531 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/ml/chronometrage/_chronometrage.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.317322 sberpm-2.4.1/sberpm/ml/stages_clustering/
--rw-rw-rw-   0        0        0      111 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/ml/stages_clustering/__init__.py
--rw-rw-rw-   0        0        0      183 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/ml/stages_clustering/_stages_clustering.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.319322 sberpm-2.4.1/sberpm/ml/stages_clustering/file_obf/
--rw-rw-rw-   0        0        0     5116 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/ml/stages_clustering/file_obf/_stages_clustering.obfsbpm
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.325324 sberpm-2.4.1/sberpm/ml/utils/
--rw-rw-rw-   0        0        0      107 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/ml/utils/__init__.py
--rw-rw-rw-   0        0        0     3935 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/ml/utils/_perm_importance.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.330323 sberpm-2.4.1/sberpm/models/
--rw-rw-rw-   0        0        0      300 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/models/__init__.py
--rw-rw-rw-   0        0        0     1846 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/models/_check_models.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.349325 sberpm-2.4.1/sberpm/visual/
--rw-rw-rw-   0        0        0      608 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/visual/__init__.py
--rw-rw-rw-   0        0        0    76564 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/visual/_chart_painter.py
--rw-rw-rw-   0        0        0    18529 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/visual/_graph.py
--rw-rw-rw-   0        0        0    12406 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/visual/_graphviz_painter.py
--rw-rw-rw-   0        0        0    25598 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/visual/_matplotlib_painter.py
--rw-rw-rw-   0        0        0      594 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/visual/_types.py
--rw-rw-rw-   0        0        0     6935 2023-01-26 18:07:31.000000 sberpm-2.4.1/sberpm/visual/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.143309 sberpm-2.4.1/sberpm.egg-info/
--rw-rw-rw-   0        0        0     2887 2023-05-25 06:05:37.000000 sberpm-2.4.1/sberpm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3325 2023-05-25 06:05:37.000000 sberpm-2.4.1/sberpm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 06:05:37.000000 sberpm-2.4.1/sberpm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      814 2023-05-25 06:05:37.000000 sberpm-2.4.1/sberpm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-25 06:05:37.000000 sberpm-2.4.1/sberpm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 06:05:38.367326 sberpm-2.4.1/setup.cfg
--rw-rw-rw-   0        0        0     2606 2023-04-19 07:36:42.000000 sberpm-2.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:05:38.361328 sberpm-2.4.1/tutorials/
--rw-rw-rw-   0        0        0    19319 2023-01-26 18:07:31.000000 sberpm-2.4.1/tutorials/chrono_data.xlsx
--rw-rw-rw-   0        0        0   132942 2023-01-26 18:07:31.000000 sberpm-2.4.1/tutorials/example.xlsx
--rw-rw-rw-   0        0        0    95944 2023-05-25 05:48:29.000000 sberpm-2.4.1/tutorials/tutorial_en.ipynb
--rw-rw-rw-   0        0        0   128045 2023-05-25 05:48:29.000000 sberpm-2.4.1/tutorials/tutorial_ru.ipynb
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:23.516274 sberpm-2.5.0rc0/
+-rw-rw-rw-   0        0        0      274 2023-03-14 12:01:36.000000 sberpm-2.5.0rc0/.gitignore
+-rw-rw-rw-   0        0        0    29507 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/LICENSE
+-rw-rw-rw-   0        0        0    62148 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/LICENSE_RUS
+-rw-rw-rw-   0        0        0      242 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2890 2023-07-26 11:24:23.520274 sberpm-2.5.0rc0/PKG-INFO
+-rw-rw-rw-   0        0        0     2213 2023-04-05 21:34:08.000000 sberpm-2.5.0rc0/README.md
+-rw-rw-rw-   0        0        0     1147 2023-05-25 05:48:29.000000 sberpm-2.5.0rc0/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:15.987090 sberpm-2.5.0rc0/sberpm/
+-rw-rw-rw-   0        0        0      542 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/__init__.py
+-rw-rw-rw-   0        0        0    31800 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/_holder.py
+-rw-rw-rw-   0        0        0      947 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/_utils.py
+-rw-rw-rw-   0        0        0       24 2023-07-26 11:21:03.000000 sberpm-2.5.0rc0/sberpm/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:16.300306 sberpm-2.5.0rc0/sberpm/autoinsights/
+-rw-rw-rw-   0        0        0      120 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/autoinsights/__init__.py
+-rw-rw-rw-   0        0        0      188 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/autoinsights/_influencing_activities.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:16.388341 sberpm-2.5.0rc0/sberpm/autoinsights/file_obf/
+-rw-rw-rw-   0        0        0    12828 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/autoinsights/file_obf/_influencing_activities.obfsbpm
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:16.538301 sberpm-2.5.0rc0/sberpm/bpmn/
+-rw-rw-rw-   0        0        0      177 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/bpmn/__init__.py
+-rw-rw-rw-   0        0        0    26484 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/bpmn/_bpmn_file_to_graph.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:17.018985 sberpm-2.5.0rc0/sberpm/bpmn/_bpmn_graph_to_file/
+-rw-rw-rw-   0        0        0      103 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/bpmn/_bpmn_graph_to_file/__init__.py
+-rw-rw-rw-   0        0        0     4093 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_exporter.py
+-rw-rw-rw-   0        0        0     6642 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_xml_maker.py
+-rw-rw-rw-   0        0        0     4680 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/bpmn/_bpmn_graph_to_file/_petri_net_to_bpmn.py
+-rw-rw-rw-   0        0        0     1545 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/bpmn/_bpmn_graph_to_file/grandalf.py
+-rw-rw-rw-   0        0        0     5350 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/bpmn/_bpmn_graph_to_file/graphviz.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:17.131012 sberpm-2.5.0rc0/sberpm/column_matching/
+-rw-rw-rw-   0        0        0      102 2023-03-14 12:01:36.000000 sberpm-2.5.0rc0/sberpm/column_matching/__init__.py
+-rw-rw-rw-   0        0        0      182 2023-03-14 12:01:36.000000 sberpm-2.5.0rc0/sberpm/column_matching/_column_matching.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:17.219039 sberpm-2.5.0rc0/sberpm/column_matching/file_obf/
+-rw-rw-rw-   0        0        0     5710 2023-03-14 12:01:36.000000 sberpm-2.5.0rc0/sberpm/column_matching/file_obf/_column_matching_.obfsbpm
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:17.467091 sberpm-2.5.0rc0/sberpm/conformance_checking/
+-rw-rw-rw-   0        0        0      202 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/conformance_checking/__init__.py
+-rw-rw-rw-   0        0        0     6061 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/conformance_checking/_conformance_checking.py
+-rw-rw-rw-   0        0        0     9883 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/conformance_checking/_token_replay.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:17.624317 sberpm-2.5.0rc0/sberpm/decision_mining/
+-rw-rw-rw-   0        0        0      100 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/decision_mining/__init__.py
+-rw-rw-rw-   0        0        0    33758 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/decision_mining/_decision_mining.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:17.800358 sberpm-2.5.0rc0/sberpm/graph_stats/
+-rw-rw-rw-   0        0        0      146 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/graph_stats/__init__.py
+-rw-rw-rw-   0        0        0     3336 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/graph_stats/centrality.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:17.968397 sberpm-2.5.0rc0/sberpm/imitation/
+-rw-rw-rw-   0        0        0      160 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/imitation/__init__.py
+-rw-rw-rw-   0        0        0      176 2023-05-25 05:48:29.000000 sberpm-2.5.0rc0/sberpm/imitation/_simulation.py
+-rw-rw-rw-   0        0        0      176 2023-05-25 05:48:29.000000 sberpm-2.5.0rc0/sberpm/imitation/_validation.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:18.141696 sberpm-2.5.0rc0/sberpm/imitation/file_obf/
+-rw-rw-rw-   0        0        0    21873 2023-05-25 05:48:29.000000 sberpm-2.5.0rc0/sberpm/imitation/file_obf/_simulation.obfsbpm
+-rw-rw-rw-   0        0        0    11229 2023-05-25 05:48:29.000000 sberpm-2.5.0rc0/sberpm/imitation/file_obf/_validation.obfsbpm
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:19.081970 sberpm-2.5.0rc0/sberpm/metrics/
+-rw-rw-rw-   0        0        0      371 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/metrics/__init__.py
+-rw-rw-rw-   0        0        0     5524 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/metrics/_activity_metric.py
+-rw-rw-rw-   0        0        0     6918 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/metrics/_base_metric.py
+-rw-rw-rw-   0        0        0     4077 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/metrics/_id_metric.py
+-rw-rw-rw-   0        0        0     5173 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/metrics/_trace_metric.py
+-rw-rw-rw-   0        0        0     6093 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/metrics/_transition_metric.py
+-rw-rw-rw-   0        0        0     3995 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/metrics/_user_metric.py
+-rw-rw-rw-   0        0        0      389 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/metrics/_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:20.312769 sberpm-2.5.0rc0/sberpm/miners/
+-rw-rw-rw-   0        0        0     1374 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/miners/__init__.py
+-rw-rw-rw-   0        0        0     9571 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/miners/_abstract_miner.py
+-rw-rw-rw-   0        0        0    19774 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/miners/_alpha_miner.py
+-rw-rw-rw-   0        0        0    10578 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/miners/_alpha_plus_miner.py
+-rw-rw-rw-   0        0        0      174 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/miners/_auto_miner.py
+-rw-rw-rw-   0        0        0     3153 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/miners/_causal_miner.py
+-rw-rw-rw-   0        0        0    18462 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/miners/_correlation_miner.py
+-rw-rw-rw-   0        0        0     9122 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/miners/_heu_miner.py
+-rw-rw-rw-   0        0        0     3896 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/miners/_inductive_miner.py
+-rw-rw-rw-   0        0        0     8354 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/miners/_inductive_utils.py
+-rw-rw-rw-   0        0        0      174 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/miners/_ml_miner.py
+-rw-rw-rw-   0        0        0      178 2023-05-25 05:48:29.000000 sberpm-2.5.0rc0/sberpm/miners/_parallel_miner.py
+-rw-rw-rw-   0        0        0     2678 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/miners/_simple_miner.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:20.568820 sberpm-2.5.0rc0/sberpm/miners/file_obf/
+-rw-rw-rw-   0        0        0     3192 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/miners/file_obf/_auto_miner.obfsbpm
+-rw-rw-rw-   0        0        0     5082 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/miners/file_obf/_ml_miner.obfsbpm
+-rw-rw-rw-   0        0        0     5874 2023-05-25 05:48:29.000000 sberpm-2.5.0rc0/sberpm/miners/file_obf/_parallel_miner.obfsbpm
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:20.761708 sberpm-2.5.0rc0/sberpm/miners/mining_utils/
+-rw-rw-rw-   0        0        0     8347 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/miners/mining_utils/_inductive_utils.py
+-rw-rw-rw-   0        0        0    25893 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/miners/mining_utils/_node_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:20.849739 sberpm-2.5.0rc0/sberpm/ml/
+-rw-rw-rw-   0        0        0      179 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/ml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:21.599136 sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/
+-rw-rw-rw-   0        0        0      571 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/__init__.py
+-rw-rw-rw-   0        0        0    11459 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/_outlier_detector.py
+-rw-rw-rw-   0        0        0     4669 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/_outlier_detector_ensemble.py
+-rw-rw-rw-   0        0        0     5295 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/_outliercblof.py
+-rw-rw-rw-   0        0        0     2404 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/_outliercustom.py
+-rw-rw-rw-   0        0        0     4911 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/_outlierforest.py
+-rw-rw-rw-   0        0        0     6340 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/_outlierlof.py
+-rw-rw-rw-   0        0        0     4804 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/_outlierocsvm.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:21.764389 sberpm-2.5.0rc0/sberpm/ml/chronometrage/
+-rw-rw-rw-   0        0        0       76 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/ml/chronometrage/__init__.py
+-rw-rw-rw-   0        0        0     6531 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/ml/chronometrage/_chronometrage.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:21.880416 sberpm-2.5.0rc0/sberpm/ml/stages_clustering/
+-rw-rw-rw-   0        0        0      111 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/ml/stages_clustering/__init__.py
+-rw-rw-rw-   0        0        0      183 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/ml/stages_clustering/_stages_clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:21.960441 sberpm-2.5.0rc0/sberpm/ml/stages_clustering/file_obf/
+-rw-rw-rw-   0        0        0     5116 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/ml/stages_clustering/file_obf/_stages_clustering.obfsbpm
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:22.124486 sberpm-2.5.0rc0/sberpm/ml/utils/
+-rw-rw-rw-   0        0        0      107 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/ml/utils/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/ml/utils/_perm_importance.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:22.353830 sberpm-2.5.0rc0/sberpm/models/
+-rw-rw-rw-   0        0        0      300 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/models/__init__.py
+-rw-rw-rw-   0        0        0     1846 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/models/_check_models.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:23.047021 sberpm-2.5.0rc0/sberpm/visual/
+-rw-rw-rw-   0        0        0      608 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/visual/__init__.py
+-rw-rw-rw-   0        0        0    76564 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/visual/_chart_painter.py
+-rw-rw-rw-   0        0        0    18529 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/visual/_graph.py
+-rw-rw-rw-   0        0        0    12406 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/visual/_graphviz_painter.py
+-rw-rw-rw-   0        0        0    25598 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/visual/_matplotlib_painter.py
+-rw-rw-rw-   0        0        0      594 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/visual/_types.py
+-rw-rw-rw-   0        0        0     6935 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/sberpm/visual/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:16.188344 sberpm-2.5.0rc0/sberpm.egg-info/
+-rw-rw-rw-   0        0        0     2890 2023-07-26 11:24:11.000000 sberpm-2.5.0rc0/sberpm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3325 2023-07-26 11:24:14.000000 sberpm-2.5.0rc0/sberpm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 11:24:11.000000 sberpm-2.5.0rc0/sberpm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      814 2023-07-26 11:24:11.000000 sberpm-2.5.0rc0/sberpm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 11:24:11.000000 sberpm-2.5.0rc0/sberpm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 11:24:23.532266 sberpm-2.5.0rc0/setup.cfg
+-rw-rw-rw-   0        0        0     2606 2023-04-19 07:36:42.000000 sberpm-2.5.0rc0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:23.484258 sberpm-2.5.0rc0/tutorials/
+-rw-rw-rw-   0        0        0    19319 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/tutorials/chrono_data.xlsx
+-rw-rw-rw-   0        0        0   132942 2023-01-26 18:07:31.000000 sberpm-2.5.0rc0/tutorials/example.xlsx
+-rw-rw-rw-   0        0        0    95944 2023-05-25 05:48:29.000000 sberpm-2.5.0rc0/tutorials/tutorial_en.ipynb
+-rw-rw-rw-   0        0        0   128045 2023-05-25 05:48:29.000000 sberpm-2.5.0rc0/tutorials/tutorial_ru.ipynb
```

### Comparing `sberpm-2.4.1/LICENSE` & `sberpm-2.5.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/LICENSE_RUS` & `sberpm-2.5.0rc0/LICENSE_RUS`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/PKG-INFO` & `sberpm-2.5.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sberpm
-Version: 2.4.1
+Version: 2.5.0rc0
 Summary: Library that is intended to operate with various process mining tasks.
 Author: Sberbank Process Mining Team
 Author-email: AABugaenko@sberbank.ru
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `sberpm-2.4.1/README.md` & `sberpm-2.5.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/requirements.txt` & `sberpm-2.5.0rc0/requirements.txt`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/__init__.py` & `sberpm-2.5.0rc0/sberpm/__init__.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/_holder.py` & `sberpm-2.5.0rc0/sberpm/_holder.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/_utils.py` & `sberpm-2.5.0rc0/sberpm/_utils.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/autoinsights/file_obf/_influencing_activities.obfsbpm` & `sberpm-2.5.0rc0/sberpm/autoinsights/file_obf/_influencing_activities.obfsbpm`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/bpmn/_bpmn_file_to_graph.py` & `sberpm-2.5.0rc0/sberpm/bpmn/_bpmn_file_to_graph.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_exporter.py` & `sberpm-2.5.0rc0/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_exporter.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_xml_maker.py` & `sberpm-2.5.0rc0/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_xml_maker.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/bpmn/_bpmn_graph_to_file/_petri_net_to_bpmn.py` & `sberpm-2.5.0rc0/sberpm/bpmn/_bpmn_graph_to_file/_petri_net_to_bpmn.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/bpmn/_bpmn_graph_to_file/grandalf.py` & `sberpm-2.5.0rc0/sberpm/bpmn/_bpmn_graph_to_file/grandalf.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/bpmn/_bpmn_graph_to_file/graphviz.py` & `sberpm-2.5.0rc0/sberpm/bpmn/_bpmn_graph_to_file/graphviz.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/column_matching/file_obf/_column_matching_.obfsbpm` & `sberpm-2.5.0rc0/sberpm/column_matching/file_obf/_column_matching_.obfsbpm`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/conformance_checking/_conformance_checking.py` & `sberpm-2.5.0rc0/sberpm/conformance_checking/_conformance_checking.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/conformance_checking/_token_replay.py` & `sberpm-2.5.0rc0/sberpm/conformance_checking/_token_replay.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/decision_mining/_decision_mining.py` & `sberpm-2.5.0rc0/sberpm/decision_mining/_decision_mining.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/graph_stats/centrality.py` & `sberpm-2.5.0rc0/sberpm/graph_stats/centrality.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/imitation/file_obf/_simulation.obfsbpm` & `sberpm-2.5.0rc0/sberpm/imitation/file_obf/_simulation.obfsbpm`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/imitation/file_obf/_validation.obfsbpm` & `sberpm-2.5.0rc0/sberpm/imitation/file_obf/_validation.obfsbpm`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/metrics/_activity_metric.py` & `sberpm-2.5.0rc0/sberpm/metrics/_activity_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/metrics/_base_metric.py` & `sberpm-2.5.0rc0/sberpm/metrics/_base_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/metrics/_id_metric.py` & `sberpm-2.5.0rc0/sberpm/metrics/_id_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/metrics/_trace_metric.py` & `sberpm-2.5.0rc0/sberpm/metrics/_trace_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/metrics/_transition_metric.py` & `sberpm-2.5.0rc0/sberpm/metrics/_transition_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/metrics/_user_metric.py` & `sberpm-2.5.0rc0/sberpm/metrics/_user_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/miners/__init__.py` & `sberpm-2.5.0rc0/sberpm/miners/__init__.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/miners/_abstract_miner.py` & `sberpm-2.5.0rc0/sberpm/miners/_abstract_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/miners/_alpha_miner.py` & `sberpm-2.5.0rc0/sberpm/miners/_alpha_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/miners/_alpha_plus_miner.py` & `sberpm-2.5.0rc0/sberpm/miners/_alpha_plus_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/miners/_causal_miner.py` & `sberpm-2.5.0rc0/sberpm/miners/_causal_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/miners/_correlation_miner.py` & `sberpm-2.5.0rc0/sberpm/miners/_correlation_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/miners/_heu_miner.py` & `sberpm-2.5.0rc0/sberpm/miners/_heu_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/miners/_inductive_miner.py` & `sberpm-2.5.0rc0/sberpm/miners/_inductive_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/miners/_inductive_utils.py` & `sberpm-2.5.0rc0/sberpm/miners/_inductive_utils.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/miners/_simple_miner.py` & `sberpm-2.5.0rc0/sberpm/miners/_simple_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/miners/file_obf/_auto_miner.obfsbpm` & `sberpm-2.5.0rc0/sberpm/miners/file_obf/_auto_miner.obfsbpm`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/miners/file_obf/_ml_miner.obfsbpm` & `sberpm-2.5.0rc0/sberpm/miners/file_obf/_ml_miner.obfsbpm`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/miners/file_obf/_parallel_miner.obfsbpm` & `sberpm-2.5.0rc0/sberpm/miners/file_obf/_parallel_miner.obfsbpm`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/miners/mining_utils/_inductive_utils.py` & `sberpm-2.5.0rc0/sberpm/miners/mining_utils/_inductive_utils.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/miners/mining_utils/_node_utils.py` & `sberpm-2.5.0rc0/sberpm/miners/mining_utils/_node_utils.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/ml/anomaly_detection/__init__.py` & `sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/ml/anomaly_detection/_outlier_detector.py` & `sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/_outlier_detector.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/ml/anomaly_detection/_outlier_detector_ensemble.py` & `sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/_outlier_detector_ensemble.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/ml/anomaly_detection/_outliercblof.py` & `sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/_outliercblof.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/ml/anomaly_detection/_outliercustom.py` & `sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/_outliercustom.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/ml/anomaly_detection/_outlierforest.py` & `sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/_outlierforest.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/ml/anomaly_detection/_outlierlof.py` & `sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/_outlierlof.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/ml/anomaly_detection/_outlierocsvm.py` & `sberpm-2.5.0rc0/sberpm/ml/anomaly_detection/_outlierocsvm.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/ml/chronometrage/_chronometrage.py` & `sberpm-2.5.0rc0/sberpm/ml/chronometrage/_chronometrage.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/ml/stages_clustering/file_obf/_stages_clustering.obfsbpm` & `sberpm-2.5.0rc0/sberpm/ml/stages_clustering/file_obf/_stages_clustering.obfsbpm`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/ml/utils/_perm_importance.py` & `sberpm-2.5.0rc0/sberpm/ml/utils/_perm_importance.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/models/_check_models.py` & `sberpm-2.5.0rc0/sberpm/models/_check_models.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/visual/__init__.py` & `sberpm-2.5.0rc0/sberpm/visual/__init__.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/visual/_chart_painter.py` & `sberpm-2.5.0rc0/sberpm/visual/_chart_painter.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/visual/_graph.py` & `sberpm-2.5.0rc0/sberpm/visual/_graph.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/visual/_graphviz_painter.py` & `sberpm-2.5.0rc0/sberpm/visual/_graphviz_painter.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/visual/_matplotlib_painter.py` & `sberpm-2.5.0rc0/sberpm/visual/_matplotlib_painter.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/visual/_types.py` & `sberpm-2.5.0rc0/sberpm/visual/_types.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm/visual/utils.py` & `sberpm-2.5.0rc0/sberpm/visual/utils.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm.egg-info/PKG-INFO` & `sberpm-2.5.0rc0/sberpm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sberpm
-Version: 2.4.1
+Version: 2.5.0rc0
 Summary: Library that is intended to operate with various process mining tasks.
 Author: Sberbank Process Mining Team
 Author-email: AABugaenko@sberbank.ru
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `sberpm-2.4.1/sberpm.egg-info/SOURCES.txt` & `sberpm-2.5.0rc0/sberpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/sberpm.egg-info/requires.txt` & `sberpm-2.5.0rc0/sberpm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/setup.py` & `sberpm-2.5.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/tutorials/chrono_data.xlsx` & `sberpm-2.5.0rc0/tutorials/chrono_data.xlsx`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/tutorials/example.xlsx` & `sberpm-2.5.0rc0/tutorials/example.xlsx`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/tutorials/tutorial_en.ipynb` & `sberpm-2.5.0rc0/tutorials/tutorial_en.ipynb`

 * *Files identical despite different names*

### Comparing `sberpm-2.4.1/tutorials/tutorial_ru.ipynb` & `sberpm-2.5.0rc0/tutorials/tutorial_ru.ipynb`

 * *Files identical despite different names*

