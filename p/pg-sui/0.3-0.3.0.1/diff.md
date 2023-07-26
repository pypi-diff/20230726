# Comparing `tmp/pg-sui-0.3.tar.gz` & `tmp/pg-sui-0.3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg-sui-0.3.tar", last modified: Tue Jul 25 19:10:33 2023, max compression
+gzip compressed data, was "pg-sui-0.3.0.1.tar", last modified: Wed Jul 26 06:12:49 2023, max compression
```

## Comparing `pg-sui-0.3.tar` & `pg-sui-0.3.0.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:32.207312 pg-sui-0.3/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    35149 2023-07-16 18:34:37.000000 pg-sui-0.3/LICENSE
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      220 2023-07-23 06:06:57.000000 pg-sui-0.3/MANIFEST.in
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    14121 2023-07-25 19:10:32.204312 pg-sui-0.3/PKG-INFO
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    10444 2023-07-23 06:06:57.000000 pg-sui-0.3/README.md
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:30.174327 pg-sui-0.3/pg_sui.egg-info/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    14121 2023-07-25 19:10:28.000000 pg-sui-0.3/pg_sui.egg-info/PKG-INFO
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2994 2023-07-25 19:10:29.000000 pg-sui-0.3/pg_sui.egg-info/SOURCES.txt
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        1 2023-07-25 19:10:28.000000 pg-sui-0.3/pg_sui.egg-info/dependency_links.txt
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      331 2023-07-25 19:10:28.000000 pg-sui-0.3/pg_sui.egg-info/requires.txt
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)       22 2023-07-25 19:10:28.000000 pg-sui-0.3/pg_sui.egg-info/top_level.txt
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:30.202329 pg-sui-0.3/pgsui/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     1449 2023-07-23 06:06:59.000000 pg-sui-0.3/pgsui/__init__.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:30.236326 pg-sui-0.3/pgsui/data_processing/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:42.000000 pg-sui-0.3/pgsui/data_processing/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    42452 2023-07-24 01:34:13.000000 pg-sui-0.3/pgsui/data_processing/transformers.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:30.256330 pg-sui-0.3/pgsui/example_data/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:42.000000 pg-sui-0.3/pgsui/example_data/__init__.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:30.401326 pg-sui-0.3/pgsui/example_data/phylip_files/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/phylip_files/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)   238537 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/phylip_files/test.phy
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2897 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/phylip_files/test_n10.phy
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    13428 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/phylip_files/test_n100.phy
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     1960 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/phylip_files/test_n2.phy
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    60228 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/phylip_files/test_n500.phy
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:30.447326 pg-sui-0.3/pgsui/example_data/popmaps/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/popmaps/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     1954 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/popmaps/test.popmap
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:30.775325 pg-sui-0.3/pgsui/example_data/structure_files/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     6375 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.1row.10sites.str
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    50808 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.2row.100sites.str
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     7978 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.2row.10sites.str
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    17512 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.2row.30sites.str
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)   967410 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.2row.allsites.str
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     6609 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/test.pops.1row.10sites.str
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     8446 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/test.pops.2row.10sites.str
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)   967878 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/structure_files/test.pops.2row.allsites.str
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:31.133322 pg-sui-0.3/pgsui/example_data/trees/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    25575 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test.iqtree
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      134 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test.qmat
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    46013 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test.rate
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     4696 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test.tre
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      678 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test_n10.rate
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2577 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test_n100.rate
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    11387 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test_n500.rate
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    16235 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test_siterates.txt
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)       80 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test_siterates_n10.txt
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      804 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test_siterates_n100.txt
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     4008 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/trees/test_siterates_n500.txt
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:31.225320 pg-sui-0.3/pgsui/example_data/vcf_files/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)   380243 2023-07-23 04:24:43.000000 pg-sui-0.3/pgsui/example_data/vcf_files/test.vcf
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    72705 2023-07-23 06:06:59.000000 pg-sui-0.3/pgsui/example_data/vcf_files/test.vcf.gz
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2581 2023-07-23 06:06:59.000000 pg-sui-0.3/pgsui/example_data/vcf_files/test.vcf.gz.tbi
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:31.324319 pg-sui-0.3/pgsui/impute/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:44.000000 pg-sui-0.3/pgsui/impute/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    49767 2023-07-25 05:09:59.000000 pg-sui-0.3/pgsui/impute/estimators.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    51148 2023-07-24 06:54:52.000000 pg-sui-0.3/pgsui/impute/impute.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    53283 2023-07-23 06:06:59.000000 pg-sui-0.3/pgsui/impute/simple_imputers.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:31.417320 pg-sui-0.3/pgsui/impute/supervised/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:44.000000 pg-sui-0.3/pgsui/impute/supervised/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    35075 2023-07-23 06:06:59.000000 pg-sui-0.3/pgsui/impute/supervised/iterative_imputer_fixedparams.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    45443 2023-07-23 06:06:59.000000 pg-sui-0.3/pgsui/impute/supervised/iterative_imputer_gridsearch.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:31.570317 pg-sui-0.3/pgsui/impute/unsupervised/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:44.000000 pg-sui-0.3/pgsui/impute/unsupervised/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     9682 2023-07-23 06:06:59.000000 pg-sui-0.3/pgsui/impute/unsupervised/callbacks.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    29626 2023-07-24 07:18:02.000000 pg-sui-0.3/pgsui/impute/unsupervised/keras_classifiers.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:31.809313 pg-sui-0.3/pgsui/impute/unsupervised/models/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:45.000000 pg-sui-0.3/pgsui/impute/unsupervised/models/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    19704 2023-07-24 17:44:03.000000 pg-sui-0.3/pgsui/impute/unsupervised/models/autoencoder_model.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:31.884314 pg-sui-0.3/pgsui/impute/unsupervised/models/in_development/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:45.000000 pg-sui-0.3/pgsui/impute/unsupervised/models/in_development/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    15036 2023-07-23 04:24:45.000000 pg-sui-0.3/pgsui/impute/unsupervised/models/in_development/cnn_model.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    16939 2023-07-24 18:00:06.000000 pg-sui-0.3/pgsui/impute/unsupervised/models/nlpca_model.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    44658 2023-07-24 17:18:02.000000 pg-sui-0.3/pgsui/impute/unsupervised/models/ubp_model.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    21805 2023-07-24 17:30:15.000000 pg-sui-0.3/pgsui/impute/unsupervised/models/vae_model.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    51530 2023-07-24 21:25:03.000000 pg-sui-0.3/pgsui/impute/unsupervised/neural_network_imputers.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    50820 2023-07-25 05:36:56.000000 pg-sui-0.3/pgsui/impute/unsupervised/neural_network_methods.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     7471 2023-07-23 06:06:59.000000 pg-sui-0.3/pgsui/pg_sui.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:32.026312 pg-sui-0.3/pgsui/utils/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:45.000000 pg-sui-0.3/pgsui/utils/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    15705 2023-07-23 04:24:45.000000 pg-sui-0.3/pgsui/utils/misc.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    32470 2023-07-24 08:43:44.000000 pg-sui-0.3/pgsui/utils/plotting.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    17472 2023-07-24 20:47:26.000000 pg-sui-0.3/pgsui/utils/scorers.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    10143 2023-07-23 04:24:45.000000 pg-sui-0.3/pgsui/utils/sequence_tools.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)       38 2023-07-25 19:10:32.208311 pg-sui-0.3/setup.cfg
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     3087 2023-07-25 18:35:09.000000 pg-sui-0.3/setup.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:32.080312 pg-sui-0.3/simulation/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:45.000000 pg-sui-0.3/simulation/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    11345 2023-07-23 04:24:46.000000 pg-sui-0.3/simulation/sim_benchmarks.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    13793 2023-07-23 04:24:46.000000 pg-sui-0.3/simulation/sim_treeparams.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-25 19:10:32.185312 pg-sui-0.3/test/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:46.000000 pg-sui-0.3/test/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     6024 2023-07-23 04:24:46.000000 pg-sui-0.3/test/pg_sui_simtest.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    15871 2023-07-23 04:24:46.000000 pg-sui-0.3/test/pg_sui_testing.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     6773 2023-07-25 18:43:07.000000 pg-sui-0.3/test/test.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    14310 2023-07-23 04:24:46.000000 pg-sui-0.3/test/test_pgsui.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     5867 2023-07-24 00:02:54.000000 pg-sui-0.3/test/test_tkc.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:47.387278 pg-sui-0.3.0.1/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    35149 2023-07-16 18:34:37.000000 pg-sui-0.3.0.1/LICENSE
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      220 2023-07-23 06:06:57.000000 pg-sui-0.3.0.1/MANIFEST.in
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    14125 2023-07-26 06:12:47.384275 pg-sui-0.3.0.1/PKG-INFO
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    10444 2023-07-23 06:06:57.000000 pg-sui-0.3.0.1/README.md
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:45.087292 pg-sui-0.3.0.1/pg_sui.egg-info/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    14125 2023-07-26 06:12:43.000000 pg-sui-0.3.0.1/pg_sui.egg-info/PKG-INFO
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2994 2023-07-26 06:12:44.000000 pg-sui-0.3.0.1/pg_sui.egg-info/SOURCES.txt
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        1 2023-07-26 06:12:43.000000 pg-sui-0.3.0.1/pg_sui.egg-info/dependency_links.txt
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      331 2023-07-26 06:12:43.000000 pg-sui-0.3.0.1/pg_sui.egg-info/requires.txt
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)       22 2023-07-26 06:12:43.000000 pg-sui-0.3.0.1/pg_sui.egg-info/top_level.txt
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:45.121292 pg-sui-0.3.0.1/pgsui/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     1449 2023-07-23 06:06:59.000000 pg-sui-0.3.0.1/pgsui/__init__.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:45.168291 pg-sui-0.3.0.1/pgsui/data_processing/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:42.000000 pg-sui-0.3.0.1/pgsui/data_processing/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    43851 2023-07-26 05:38:41.000000 pg-sui-0.3.0.1/pgsui/data_processing/transformers.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:45.193290 pg-sui-0.3.0.1/pgsui/example_data/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:42.000000 pg-sui-0.3.0.1/pgsui/example_data/__init__.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:45.378289 pg-sui-0.3.0.1/pgsui/example_data/phylip_files/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/phylip_files/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)   238537 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/phylip_files/test.phy
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2897 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/phylip_files/test_n10.phy
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    13428 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/phylip_files/test_n100.phy
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     1960 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/phylip_files/test_n2.phy
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    60228 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/phylip_files/test_n500.phy
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:45.439289 pg-sui-0.3.0.1/pgsui/example_data/popmaps/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/popmaps/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     1954 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/popmaps/test.popmap
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:45.761286 pg-sui-0.3.0.1/pgsui/example_data/structure_files/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/structure_files/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     6375 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/structure_files/test.nopops.1row.10sites.str
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    50808 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/structure_files/test.nopops.2row.100sites.str
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     7978 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/structure_files/test.nopops.2row.10sites.str
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    17512 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/structure_files/test.nopops.2row.30sites.str
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)   967410 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/structure_files/test.nopops.2row.allsites.str
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     6609 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/structure_files/test.pops.1row.10sites.str
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     8446 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/structure_files/test.pops.2row.10sites.str
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)   967878 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/structure_files/test.pops.2row.allsites.str
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:46.154284 pg-sui-0.3.0.1/pgsui/example_data/trees/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/trees/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    25575 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/trees/test.iqtree
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      134 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/trees/test.qmat
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    46013 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/trees/test.rate
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     4696 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/trees/test.tre
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      678 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/trees/test_n10.rate
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2577 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/trees/test_n100.rate
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    11387 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/trees/test_n500.rate
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    16235 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/trees/test_siterates.txt
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)       80 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/trees/test_siterates_n10.txt
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      804 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/trees/test_siterates_n100.txt
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     4008 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/trees/test_siterates_n500.txt
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:46.259283 pg-sui-0.3.0.1/pgsui/example_data/vcf_files/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)   380243 2023-07-23 04:24:43.000000 pg-sui-0.3.0.1/pgsui/example_data/vcf_files/test.vcf
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    72705 2023-07-23 06:06:59.000000 pg-sui-0.3.0.1/pgsui/example_data/vcf_files/test.vcf.gz
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2581 2023-07-23 06:06:59.000000 pg-sui-0.3.0.1/pgsui/example_data/vcf_files/test.vcf.gz.tbi
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:46.386282 pg-sui-0.3.0.1/pgsui/impute/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:44.000000 pg-sui-0.3.0.1/pgsui/impute/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    49954 2023-07-26 05:38:56.000000 pg-sui-0.3.0.1/pgsui/impute/estimators.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    51148 2023-07-26 05:38:56.000000 pg-sui-0.3.0.1/pgsui/impute/impute.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    53283 2023-07-23 06:06:59.000000 pg-sui-0.3.0.1/pgsui/impute/simple_imputers.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:46.491281 pg-sui-0.3.0.1/pgsui/impute/supervised/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:44.000000 pg-sui-0.3.0.1/pgsui/impute/supervised/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    35075 2023-07-23 06:06:59.000000 pg-sui-0.3.0.1/pgsui/impute/supervised/iterative_imputer_fixedparams.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    45443 2023-07-23 06:06:59.000000 pg-sui-0.3.0.1/pgsui/impute/supervised/iterative_imputer_gridsearch.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:46.755278 pg-sui-0.3.0.1/pgsui/impute/unsupervised/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:44.000000 pg-sui-0.3.0.1/pgsui/impute/unsupervised/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     9682 2023-07-23 06:06:59.000000 pg-sui-0.3.0.1/pgsui/impute/unsupervised/callbacks.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    29626 2023-07-26 05:38:56.000000 pg-sui-0.3.0.1/pgsui/impute/unsupervised/keras_classifiers.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:46.919280 pg-sui-0.3.0.1/pgsui/impute/unsupervised/models/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:45.000000 pg-sui-0.3.0.1/pgsui/impute/unsupervised/models/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    19704 2023-07-26 05:38:56.000000 pg-sui-0.3.0.1/pgsui/impute/unsupervised/models/autoencoder_model.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:46.988278 pg-sui-0.3.0.1/pgsui/impute/unsupervised/models/in_development/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:45.000000 pg-sui-0.3.0.1/pgsui/impute/unsupervised/models/in_development/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    15036 2023-07-23 04:24:45.000000 pg-sui-0.3.0.1/pgsui/impute/unsupervised/models/in_development/cnn_model.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    16939 2023-07-26 05:38:56.000000 pg-sui-0.3.0.1/pgsui/impute/unsupervised/models/nlpca_model.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    44658 2023-07-26 05:38:56.000000 pg-sui-0.3.0.1/pgsui/impute/unsupervised/models/ubp_model.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    21805 2023-07-26 05:38:56.000000 pg-sui-0.3.0.1/pgsui/impute/unsupervised/models/vae_model.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    51530 2023-07-26 05:38:56.000000 pg-sui-0.3.0.1/pgsui/impute/unsupervised/neural_network_imputers.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    50820 2023-07-26 05:38:57.000000 pg-sui-0.3.0.1/pgsui/impute/unsupervised/neural_network_methods.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     7471 2023-07-23 06:06:59.000000 pg-sui-0.3.0.1/pgsui/pg_sui.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:47.125279 pg-sui-0.3.0.1/pgsui/utils/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:45.000000 pg-sui-0.3.0.1/pgsui/utils/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    15705 2023-07-23 04:24:45.000000 pg-sui-0.3.0.1/pgsui/utils/misc.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    32470 2023-07-26 05:38:57.000000 pg-sui-0.3.0.1/pgsui/utils/plotting.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    17472 2023-07-26 05:38:57.000000 pg-sui-0.3.0.1/pgsui/utils/scorers.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    10143 2023-07-23 04:24:45.000000 pg-sui-0.3.0.1/pgsui/utils/sequence_tools.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)       38 2023-07-26 06:12:47.388276 pg-sui-0.3.0.1/setup.cfg
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     3091 2023-07-26 06:12:21.000000 pg-sui-0.3.0.1/setup.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:47.270276 pg-sui-0.3.0.1/simulation/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:45.000000 pg-sui-0.3.0.1/simulation/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    11345 2023-07-23 04:24:46.000000 pg-sui-0.3.0.1/simulation/sim_benchmarks.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    13793 2023-07-23 04:24:46.000000 pg-sui-0.3.0.1/simulation/sim_treeparams.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-26 06:12:47.366279 pg-sui-0.3.0.1/test/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-23 04:24:46.000000 pg-sui-0.3.0.1/test/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     6024 2023-07-23 04:24:46.000000 pg-sui-0.3.0.1/test/pg_sui_simtest.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    15871 2023-07-23 04:24:46.000000 pg-sui-0.3.0.1/test/pg_sui_testing.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     6773 2023-07-26 05:38:57.000000 pg-sui-0.3.0.1/test/test.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    14310 2023-07-23 04:24:46.000000 pg-sui-0.3.0.1/test/test_pgsui.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     7041 2023-07-26 05:38:41.000000 pg-sui-0.3.0.1/test/test_tkc.py
```

### Comparing `pg-sui-0.3/LICENSE` & `pg-sui-0.3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/PKG-INFO` & `pg-sui-0.3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-sui
-Version: 0.3
+Version: 0.3.0.1
 Summary: Python machine and deep learning package to impute missing SNPs
 Home-page: https://github.com/btmartin721/PG-SUI
 Author: Bradley T. Martin and Tyler K. Chafin
 Author-email: evobio721@gmail.com
 Maintainer: Bradley T. Martin
 Maintainer-email: evobio721@gmail.com
 License: GNU General Public License v3 (GPLv3)
```

### Comparing `pg-sui-0.3/README.md` & `pg-sui-0.3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pg_sui.egg-info/PKG-INFO` & `pg-sui-0.3.0.1/pg_sui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-sui
-Version: 0.3
+Version: 0.3.0.1
 Summary: Python machine and deep learning package to impute missing SNPs
 Home-page: https://github.com/btmartin721/PG-SUI
 Author: Bradley T. Martin and Tyler K. Chafin
 Author-email: evobio721@gmail.com
 Maintainer: Bradley T. Martin
 Maintainer-email: evobio721@gmail.com
 License: GNU General Public License v3 (GPLv3)
```

### Comparing `pg-sui-0.3/pg_sui.egg-info/SOURCES.txt` & `pg-sui-0.3.0.1/pg_sui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/__init__.py` & `pg-sui-0.3.0.1/pgsui/__init__.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/data_processing/transformers.py` & `pg-sui-0.3.0.1/pgsui/data_processing/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -968,15 +968,15 @@
 
     def random_weighted_missing_data(self, X, inv=False):
         """Choose values for which to simulate missing data by biasing towards the minority or majority alleles, depending on whether inv is True or False.
 
         Args:
             X (np.ndarray): True values.
 
-            inv (bool, optional): If True, then biases towards choosing majority alleles. If False, then biases towards choosing minority alleles. Defaults to False.
+            inv (bool, optional): If True, then biases towards choosing majority alleles. If False, then generates a stratified random sample (class proportions ~= full dataset) Defaults to False.
 
         Returns:
             np.ndarray: X with simulated missing values.
 
         """
         # Get unique classes and their counts
         classes, counts = np.unique(X, return_counts=True)
@@ -1108,14 +1108,48 @@
             raise ValueError(f"Invalid shape of input X: {X.shape}")
 
         Xt = X.copy()
         mask_boolean = self.mask_ != 0
         Xt[mask_boolean] = mask_val
         return Xt
 
+    def write_mask(self, filename_prefix):
+        """Write mask to file.
+
+        Args:
+            filename_prefix (str): Prefix for the filenames to write to.
+        """
+        np.save(filename_prefix + "_mask.npy", self.mask_)
+        np.save(filename_prefix + "_original_missing_mask.npy", self.original_missing_mask_)
+
+    def read_mask(self, filename_prefix):
+        """Read mask from file.
+
+        Args:
+            filename_prefix (str): Prefix for the filenames to read from.
+
+        Returns:
+            tuple of np.ndarray: The read masks.
+        """
+        # Check if files exist
+        if not os.path.isfile(filename_prefix + "_mask.npy"):
+            raise FileNotFoundError(filename_prefix + "_mask.npy" + " does not exist.")
+        if not os.path.isfile(filename_prefix + "_original_missing_mask.npy"):
+            raise FileNotFoundError(filename_prefix + "_original_missing_mask.npy" + " does not exist.")
+
+        # Load mask from file
+        self.mask_ = np.load(filename_prefix + "_mask.npy")
+        self.original_missing_mask_ = np.load(filename_prefix + "_original_missing_mask.npy")
+
+        # Recalculate all_missing_mask_ from mask_ and original_missing_mask_
+        self.all_missing_mask_ = np.logical_or(self.mask_, self.original_missing_mask_)
+
+        return self.mask_, self.original_missing_mask_, self.all_missing_mask_
+
+
     @property
     def missing_count(self) -> int:
         """Count of masked genotypes in SimGenotypeData.mask
 
         Returns:
             int: Integer count of masked alleles.
         """
```

### Comparing `pg-sui-0.3/pgsui/example_data/phylip_files/test.phy` & `pg-sui-0.3.0.1/pgsui/example_data/phylip_files/test.phy`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/phylip_files/test_n10.phy` & `pg-sui-0.3.0.1/pgsui/example_data/phylip_files/test_n10.phy`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/phylip_files/test_n100.phy` & `pg-sui-0.3.0.1/pgsui/example_data/phylip_files/test_n100.phy`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/phylip_files/test_n2.phy` & `pg-sui-0.3.0.1/pgsui/example_data/phylip_files/test_n2.phy`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/phylip_files/test_n500.phy` & `pg-sui-0.3.0.1/pgsui/example_data/phylip_files/test_n500.phy`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/popmaps/test.popmap` & `pg-sui-0.3.0.1/pgsui/example_data/popmaps/test.popmap`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.1row.10sites.str` & `pg-sui-0.3.0.1/pgsui/example_data/structure_files/test.nopops.1row.10sites.str`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.2row.100sites.str` & `pg-sui-0.3.0.1/pgsui/example_data/structure_files/test.nopops.2row.100sites.str`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.2row.10sites.str` & `pg-sui-0.3.0.1/pgsui/example_data/structure_files/test.nopops.2row.10sites.str`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.2row.30sites.str` & `pg-sui-0.3.0.1/pgsui/example_data/structure_files/test.nopops.2row.30sites.str`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/structure_files/test.nopops.2row.allsites.str` & `pg-sui-0.3.0.1/pgsui/example_data/structure_files/test.nopops.2row.allsites.str`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/structure_files/test.pops.1row.10sites.str` & `pg-sui-0.3.0.1/pgsui/example_data/structure_files/test.pops.1row.10sites.str`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/structure_files/test.pops.2row.10sites.str` & `pg-sui-0.3.0.1/pgsui/example_data/structure_files/test.pops.2row.10sites.str`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/structure_files/test.pops.2row.allsites.str` & `pg-sui-0.3.0.1/pgsui/example_data/structure_files/test.pops.2row.allsites.str`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/trees/test.iqtree` & `pg-sui-0.3.0.1/pgsui/example_data/trees/test.iqtree`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/trees/test.rate` & `pg-sui-0.3.0.1/pgsui/example_data/trees/test.rate`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/trees/test.tre` & `pg-sui-0.3.0.1/pgsui/example_data/trees/test.tre`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/trees/test_n10.rate` & `pg-sui-0.3.0.1/pgsui/example_data/trees/test_n10.rate`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/trees/test_n100.rate` & `pg-sui-0.3.0.1/pgsui/example_data/trees/test_n100.rate`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/trees/test_n500.rate` & `pg-sui-0.3.0.1/pgsui/example_data/trees/test_n500.rate`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/trees/test_siterates.txt` & `pg-sui-0.3.0.1/pgsui/example_data/trees/test_siterates.txt`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/trees/test_siterates_n100.txt` & `pg-sui-0.3.0.1/pgsui/example_data/trees/test_siterates_n100.txt`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/trees/test_siterates_n500.txt` & `pg-sui-0.3.0.1/pgsui/example_data/trees/test_siterates_n500.txt`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/vcf_files/test.vcf` & `pg-sui-0.3.0.1/pgsui/example_data/vcf_files/test.vcf`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/vcf_files/test.vcf.gz` & `pg-sui-0.3.0.1/pgsui/example_data/vcf_files/test.vcf.gz`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/example_data/vcf_files/test.vcf.gz.tbi` & `pg-sui-0.3.0.1/pgsui/example_data/vcf_files/test.vcf.gz.tbi`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/impute/estimators.py` & `pg-sui-0.3.0.1/pgsui/impute/estimators.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,23 @@
     from .unsupervised.neural_network_imputers import VAE, UBP, SAE
 except (ModuleNotFoundError, ValueError, ImportError):
     from pgsui.impute.impute import Impute
     from pgsui.impute.unsupervised.neural_network_imputers import VAE, UBP, SAE
 
 
 class UnsupervisedImputer(Impute):
-    """prefix (str): Prefix for output directory. Defaults to "imputer".
+    """Parent class for unsupervised imputers. Contains all common arguments and code between unsupervised imputers.
 
-        gridparams (Dict[str, Any] or None, optional): Dictionary with keys=keyword arguments for the specified estimator and values=lists of parameter values or distributions. If ``gridparams=None``\, a grid search is not performed, otherwise ``gridparams`` will be used to specify parameter ranges or distributions for the grid search. If using ``gridsearch_method="gridsearch"``\, then the ``gridparams`` values can be lists or numpy arrays. If using ``gridsearch_method="randomized_gridsearch"``\, distributions can be specified by using scipy.stats.uniform(low, high) (for a uniform distribution) or scipy.stats.loguniform(low, high) (useful if range of values spans orders of magnitude). If using the genetic algorithm grid search by setting ``gridsearch_method="genetic_algorithm"``\, the parameters can be specified as ``sklearn_genetic.space`` objects. The grid search will determine the optimal parameters as those that maximize the scoring metrics. If it takes a long time, run it with a small subset of the data just to find the optimal parameters for the classifier, then run a full imputation using the optimal parameters. Defaults to None (no gridsearch performed).
+    Args:
+
+        genotype_data (GenotypeData object): GenotypeData instance that was used to read in the sequence data.
+
+        prefix (str): Prefix for output directory. Defaults to "imputer".
+
+        gridparams (Dict[str, Any] or None, optional): Dictionary with keys=keyword arguments for the specified estimator and values=lists of parameter values or distributions. If ``gridparams=None``\, a grid search is not performed, otherwise ``gridparams`` will be used to specify parameter ranges or distributions for the grid search. If using ``gridsearch_method="gridsearch"``\, then the ``gridparams`` values can be lists or numpy arrays. If using ``gridsearch_method="randomized_gridsearch"``\, distributions can be specified by using scipy.stats.uniform(low, high) (for a uniform distribution) or scipy.stats.loguniform(low, high) (useful if range of values spans orders of magnitude). If using the genetic algorithm grid search by setting ``gridsearch_method="genetic_algorithm"``\, the parameters can be specified as ``sklearn_genetic.space`` objects. The grid search will determine the optimal parameters as those that maximize the scoring metrics. If it takes a long time, run it with a small subset of the data just to find the optimal parameters for the classifier, then run a full imputation using the optimal parameters. Defaults to None (no gridsearch).
 
         validation_split (float, optional): Proportion of training dataset to set aside for loss validation during model training. Defaults to 0.2.
 
         column_subset (int or float, optional): If float is provided, gets the proportion of the dataset to randomly subset for the grid search or validation. Subsets ``int(n_features * column_subset)`` columns and Should be in the range [0, 1]. It can be small if the grid search or validation takes a long time. If int is provided, subset ``column_subset`` columns. Defaults to 1.0.
 
         epochs (int, optional): Number of epochs (cycles through the data) to run during training. Defaults to 100.
 
@@ -54,15 +60,15 @@
 
         l1_penalty (float, optional): L1 regularization penalty to apply. Adjust if the model is over or underfitting. If this value is too high, underfitting can occur, and vice versa. Defaults to 1e-6.
 
         l2_penalty (float, optional) L2 regularization penalty to apply. If this value is too high, underfitting can occur, and vice versa. Defaults to 1e-6.
 
         dropout_rate (float, optional): Neuron dropout rate during training. Dropout randomly disables ``dropout_rate`` proportion of neurons during training, which can reduce overfitting. E.g., if dropout_rate is set to 0.2, then 20% of the neurons are randomly dropped out per epoch. Adjust if the model is over or underfitting. Must be a float in the range [0, 1]. Defaults to 0.2.
 
-        sample_weights (str, Dict[int, float], or None, optional): Weights for the 012-encoded classes during training. If None, then does not weight classes. If set to "auto", then class weights are automatically calculated for each column to balance classes (reference, heterozygous, and alternate alleles). If a dictionary is passed, it must contain 0, 1, and 2 as the keys and the class weights as the values. E.g., {0: 1.0, 1: 1.0, 2: 1.0}. The dictionary is then used as the overall class weights. If you wanted to prevent the model from learning to predict heterozygotes, for example, you could set the class weights to {0: 1.0, 1: 0.0, 2: 1.0}. Defaults to None (no weighting).
+        sample_weights (str, Dict[int, float], or None, optional): Weights for the ACTG-encoded classes during training. If None, then does not weight classes. If set to "auto", then class weights are automatically calculated for each column to balance classes. If a dictionary is passed, it must contain "A", "C", "G", and "T" as the keys and the class weights as the values. E.g., {"A": 1.0, "C": 1.0, "G": 1.0, "T": 1.0}. The dictionary is then used as the overall class weights. Defaults to None (no weighting).
 
         gridsearch_method (str, optional): Grid search method to use. Supported options include: {"gridsearch", "randomized_gridsearch", "genetic_algorithm"}. "gridsearch" uses GridSearchCV to test every possible parameter combination. "randomized_gridsearch" picks ``grid_iter`` random combinations of parameters to test. "genetic_algorithm" uses a genetic algorithm via the sklearn-genetic-opt GASearchCV module to do the grid search. If doing a grid search, "randomized_search" takes the least amount of time because it does not have to test all parameters. "genetic_algorithm" takes the longest. See the scikit-learn GridSearchCV and RandomizedSearchCV documentation for the "gridsearch" and "randomized_gridsearch" options, and the sklearn-genetic-opt GASearchCV documentation for the "genetic_algorithm" option. Defaults to "gridsearch".
 
         grid_iter (int, optional): Number of iterations to use for randomized and genetic algorithm grid searches. For randomized grid search, ``grid_iter`` parameter combinations will be randomly sampled. For the genetic algorithm, this determines how many generations the genetic algorithm will run. Defaults to 80.
 
         scoring_metric (str, optional): Scoring metric to use for grid searches. The neural network imputers use a multimetric scorer and use different string values for the grid searches. Supported options include: {"accuracy", "hamming", "roc_auc_micro", "roc_auc_macro", "roc_auc_weighted", "average_precision_micro", "average_precision_macro", "average_precision_weighted", "f1_micro", "f1_macro", and "f1_weighted"}. All of the above metrics are calculated during the grid search, but the provided string just sets the metric that the grid search refits to (i.e., which one is used in the best estimator). See the scikit-learn documentation (https://scikit-learn.org/stable/modules/model_evaluation.html) for more information. Defaults to "f1_weighted".
 
@@ -90,19 +96,14 @@
 
         kwargs (Dict[str, Any], optional): Possible options include: {"testing": True/False}. If testing is True, a confusion matrix plot will be created showing model performance. Arrays of the true and predicted values will also be printed to STDOUT. testing defaults to False.
 
     Attributes:
         imputed (GenotypeData): New GenotypeData instance with imputed data.
 
         best_params (Dict[str, Any]): Best found parameters from grid search.
-
-    References:
-        .. [1] Gashler, M. S., Smith, M. R., Morris, R., & Martinez, T. (2016). Missing value imputation with unsupervised backpropagation. Computational Intelligence, 32(2), 196-215.
-
-        .. [2] Scholz, M., Kaplan, F., Guy, C. L., Kopka, J., & Selbig, J. (2005). Non-linear PCA: a missing data approach. Bioinformatics, 21(20), 3887-3895.
     """
 
     def __init__(
         self,
         genotype_data,
         clf,
         clf_type,
@@ -167,69 +168,76 @@
         else:
             df = X.copy()
 
         self.imputed, self.best_params = self.fit_predict(df)
 
 
 class SupervisedImputer(Impute):
-    """prefix (str): Prefix for imputed data's output directory.
+    """Parent class for the supervised imputers. Contains all common arguments and code between supervised imputers.
+
+
+    Args:
+
+        genotype_data (GenotypeData object): GenotypeData instance that was used to read in the sequence data.
 
-    gridparams (Dict[str, Any] or None or None, optional): Dictionary with keys=keyword arguments for the specified estimator and values=lists of parameter values or distributions. If ``gridparams=None``\, a grid search is not performed, otherwise ``gridparams`` will be used to specify parameter ranges or distributions for the grid search. If using ``gridsearch_method="gridsearch"``\, then the ``gridparams`` values can be lists or numpy arrays. If using ``gridsearch_method="randomized_gridsearch"``\, distributions can be specified by using scipy.stats.uniform(low, high) (for a uniform distribution) or scipy.stats.loguniform(low, high) (useful if range of values spans orders of magnitude). If using the genetic algorithm grid search by setting ``gridsearch_method="genetic_algorithm"``\, the parameters can be specified as ``sklearn_genetic.space`` objects. The grid search will determine the optimal parameters as those that maximize the scoring_methods. NOTE: Takes a long time, so you can run it with a small subset of the data using the ``column_subset`` argument just to find the optimal parameters for the classifier, then it will automatically run a full imputation using the optimal parameters. Defaults to None.
+        prefix (str): Prefix for imputed data's output directory.
 
-    do_validation (bool, optional): Whether to validate the imputation if not doing a grid search. This validation method randomly replaces between 15% and 50% of the known, non-missing genotypes in ``n_features * column_subset`` of the features. It then imputes the newly missing genotypes for which we know the true values and calculates validation scores. This procedure is replicated ``cv`` times and a mean, median, minimum, maximum, lower 95% confidence interval (CI) of the mean, and the upper 95% CI are calculated and saved to a CSV file. ``gridparams`` must be set to None for ``do_validation`` to work. Calculating a validation score can be turned off altogether by setting ``do_validation`` to False. Defaults to False.
+        gridparams (Dict[str, Any] or None, optional): Dictionary with keys=keyword arguments for the specified estimator and values=lists of parameter values or distributions. If ``gridparams=None``\, a grid search is not performed, otherwise ``gridparams`` will be used to specify parameter ranges or distributions for the grid search. If using ``gridsearch_method="gridsearch"``\, then the ``gridparams`` values can be lists or numpy arrays. If using ``gridsearch_method="randomized_gridsearch"``\, distributions can be specified by using scipy.stats.uniform(low, high) (for a uniform distribution) or scipy.stats.loguniform(low, high) (useful if range of values spans orders of magnitude). If using the genetic algorithm grid search by setting ``gridsearch_method="genetic_algorithm"``\, the parameters can be specified as ``sklearn_genetic.space`` objects. The grid search will determine the optimal parameters as those that maximize the scoring_methods. NOTE: Takes a long time, so you can run it with a small subset of the data using the ``column_subset`` argument just to find the optimal parameters for the classifier, then it will automatically run a full imputation using the optimal parameters. Defaults to None (no gridsearch).
 
-    column_subset (int or float, optional): If float, proportion of the dataset to randomly subset for the grid search or validation. Should be between 0 and 1, and should also be small, because the grid search or validation takes a long time. If int, subset ``column_subset`` columns. If float, subset ``int(n_features * column_subset)`` columns. Defaults to 0.1.
+        do_validation (bool, optional): Whether to validate the imputation if not doing a grid search. This validation method randomly replaces between 15% and 50% of the known, non-missing genotypes in ``n_features * column_subset`` of the features. It then imputes the newly missing genotypes for which we know the true values and calculates validation scores. This procedure is replicated ``cv`` times and a mean, median, minimum, maximum, lower 95% confidence interval (CI) of the mean, and the upper 95% CI are calculated and saved to a CSV file. ``gridparams`` must be set to None for ``do_validation`` to work. Calculating a validation score can be turned off altogether by setting ``do_validation`` to False. Defaults to False.
 
-    cv (int, optional): Number of folds for cross-validation during grid search. Defaults to 5.
+        column_subset (int or float, optional): If float, proportion of the dataset to randomly subset for the grid search or validation. Should be between 0 and 1, and should also be small, because the grid search or validation takes a long time. If int, subset ``column_subset`` columns. If float, subset ``int(n_features * column_subset)`` columns. Defaults to 0.1.
 
-    max_iter (int, optional): Maximum number of imputation rounds to perform before returning the imputations computed during the final round. A round is a single imputation of each feature with missing values. Defaults to 10.
+        cv (int, optional): Number of folds for cross-validation during grid search. Defaults to 5.
 
-    tol (float, optional): Tolerance of the stopping condition for the iterations. Defaults to 1e-3.
+        max_iter (int, optional): Maximum number of imputation rounds to perform before returning the imputations computed during the final round. A round is a single imputation of each feature with missing values. Defaults to 10.
 
-    n_nearest_features (int, optional): Number of other features to use to estimate the missing values of eacah feature column. If None, then all features will be used, but this can consume an  intractable amount of computing resources. Nearness between features is measured using the absolute correlation coefficient between each feature pair (after initial imputation). To ensure coverage of features throughout the imputation process, the neighbor features are not necessarily nearest, but are drawn with probability proportional to correlation for each imputed target feature. Can provide significant speed-up when the number of features is huge. Defaults to 10.
+        tol (float, optional): Tolerance of the stopping condition for the iterations. Defaults to 1e-3.
 
-    initial_strategy (str, optional): Which strategy to use for initializing the missing values in the training data (neighbor columns). IterativeImputer must initially impute the training data (neighbor columns) using a simple, quick imputation in order to predict the missing values for each target column. The ``initial_strategy`` argument specifies which method to use for this initial imputation. Valid options include: “most_frequent”, "populations", "phylogeny", or "nmf". "most_frequent" uses the overall mode of each column. "populations" uses the mode per population/ per column via a population map file and the ``ImputeAlleleFreq`` class. "phylogeny" uses an input phylogenetic tree and a rate matrix with the ``ImputePhylo`` class. "nmf" performs the imputaton via matrix factorization via the ``ImputeMF`` class. Note that the "mean" and "median" options from the original IterativeImputer are not supported because they are not sensible settings for the type of input data used here. Defaults to "populations".
+        n_nearest_features (int, optional): Number of other features to use to estimate the missing values of eacah feature column. If None, then all features will be used, but this can consume an  intractable amount of computing resources. Nearness between features is measured using the absolute correlation coefficient between each feature pair (after initial imputation). To ensure coverage of features throughout the imputation process, the neighbor features are not necessarily nearest, but are drawn with probability proportional to correlation for each imputed target feature. Reducing this can provide significant speed-up when the number of features is large. Defaults to 10.
 
-    str_encodings (dict(str: int), optional): Integer encodings for nucleotides if input file was in STRUCTURE format. Only used if ``initial_strategy="phylogeny"``\. Defaults to {"A": 1, "C": 2, "G": 3, "T": 4, "N": -9}.
+        initial_strategy (str, optional): Which strategy to use for initializing the missing values in the training data (neighbor columns). IterativeImputer must initially impute the training data (neighbor columns) using a simple, quick imputation in order to predict the missing values for each target column. The ``initial_strategy`` argument specifies which method to use for this initial imputation. Valid options include: “most_frequent”, "populations", "phylogeny", or "mf". "most_frequent" uses the overall mode of each column. "populations" uses the mode per population/ per column via a population map file and the ``ImputeAlleleFreq`` class. "phylogeny" uses an input phylogenetic tree and a rate matrix with the ``ImputePhylo`` class. "mf" performs the imputaton via matrix factorization with the ``ImputeMF`` class. Note that the "mean" and "median" options from the original IterativeImputer are not supported because they are not sensible settings for the type of input data used here. Defaults to "populations".
 
-    imputation_order (str, optional): The order in which the features will be imputed. Possible values: "ascending" (from features with fewest missing values to most), "descending" (from features with most missing values to fewest), "roman" (left to right), "arabic" (right to left), "random" (a random order for each round). Defaults to "ascending".
+        str_encodings (dict(str: int), optional): Integer encodings for nucleotides if input file was in STRUCTURE format. Only used if ``initial_strategy="phylogeny"``\. Defaults to {"A": 1, "C": 2, "G": 3, "T": 4, "N": -9}.
 
-    skip_complete (bool, optional): If True, then features with missing values during transform that did not have any missing values during fit will be imputed with the initial imputation method only. Set to True if you have many features with no missing values at both fit and transform time to save compute time. Defaults to False.
+        imputation_order (str, optional): The order in which the features will be imputed. Possible values: "ascending" (from features with fewest missing values to most), "descending" (from features with most missing values to fewest), "roman" (left to right), "arabic" (right to left), "random" (a random order for each round). Defaults to "ascending".
 
-    random_state (int or None, optional): The seed of the pseudo random number generator to use for the iterative imputer. Randomizes selection of etimator features if n_nearest_features is not None or the imputation_order is "random". Use an integer for determinism. If None, then uses a different random seed each time. Defaults to None.
+        skip_complete (bool, optional): If True, then features with missing values during transform that did not have any missing values during fit will be imputed with the initial imputation method only. Set to True if you have many features with no missing values at both fit and transform time to save compute time. Defaults to False.
 
-    gridsearch_method (str, optional): Grid search method to use. Supported options include: {"gridsearch", "randomized_gridsearch", and "genetic_algorithm"}. "gridsearch" uses GridSearchCV to test every possible parameter combination. "randomized_gridsearch" picks ``grid_iter`` random combinations of parameters to test. "genetic_algorithm" uses a genetic algorithm via sklearn-genetic-opt GASearchCV to do the grid search. If doing a grid search, "randomized_search" takes the least amount of time because it does not have to test all parameters. "genetic_algorithm" takes the longest. See the scikit-learn GridSearchCV and RandomizedSearchCV documentation for the "gridsearch" and "randomized_gridsearch" options, and the sklearn-genetic-opt GASearchCV documentation for the "genetic_algorithm" option. Defaults to "gridsearch".
+        random_state (int or None, optional): The seed of the pseudo random number generator to use for the iterative imputer. Randomizes selection of etimator features if n_nearest_features is not None or the imputation_order is "random". Use an integer for determinism. If None, then uses a different random seed each time. Defaults to None.
 
-    grid_iter (int, optional): Number of iterations for randomized and genetic algorithm grid searches. Defaults to 80.
+        gridsearch_method (str, optional): Grid search method to use. Supported options include: {"gridsearch", "randomized_gridsearch", and "genetic_algorithm"}. "gridsearch" uses GridSearchCV to test every possible parameter combination. "randomized_gridsearch" picks ``grid_iter`` random combinations of parameters to test. "genetic_algorithm" uses a genetic algorithm via sklearn-genetic-opt GASearchCV to do the grid search. If doing a grid search, "randomized_search" takes the least amount of time because it does not have to test all parameters. "genetic_algorithm" takes the longest. See the scikit-learn GridSearchCV and RandomizedSearchCV documentation for the "gridsearch" and "randomized_gridsearch" options, and the sklearn-genetic-opt GASearchCV documentation (https://sklearn-genetic-opt.readthedocs.io) for the "genetic_algorithm" option. Defaults to "gridsearch".
 
-    population_size (int or str, optional): For genetic algorithm grid search: Size of the initial population to sample randomly generated individuals. If set to "auto", then ``population_size`` is calculated as ``15 * n_parameters``\. If set to an integer, then uses the integer value as ``population_size``\. If you need to speed up the genetic algorithm grid search, try decreasing this parameter. See GASearchCV in the sklearn-genetic-opt documentation (https://sklearn-genetic-opt.readthedocs.io). Defaults to "auto".
+        grid_iter (int, optional): Number of iterations for randomized and genetic algorithm grid searches. Defaults to 80.
 
-    tournament_size (int, optional): For genetic algorithm grid search: Number of individuals to perform tournament selection. See GASearchCV documentation. Defaults to 3.
+        population_size (int or str, optional): For genetic algorithm grid search: Size of the initial population to sample randomly generated individuals. If set to "auto", then ``population_size`` is calculated as ``15 * n_parameters``\. If set to an integer, then uses the integer value as ``population_size``\. If you need to speed up the genetic algorithm grid search, try decreasing this parameter. See GASearchCV in the sklearn-genetic-opt documentation (https://sklearn-genetic-opt.readthedocs.io). Defaults to "auto".
 
-    elitism (bool, optional): For genetic algorithm grid search:     If True takes the tournament_size best solution to the next generation. See GASearchCV documentation. Defaults to True.
+        tournament_size (int, optional): For genetic algorithm grid search: Number of individuals to perform tournament selection. See GASearchCV documentation. Defaults to 3.
 
-    crossover_probability (float, optional): For genetic algorithm grid search: Probability of crossover operation between two individuals. See GASearchCV documentation. Defaults to 0.2.
+        elitism (bool, optional): For genetic algorithm grid search: If True takes the tournament_size best solution to the next generation. See GASearchCV documentation. Defaults to True.
 
-    mutation_probability (float, optional): For genetic algorithm grid search: Probability of child mutation. See GASearchCV documentation. Defaults to 0.8.
+        crossover_probability (float, optional): For genetic algorithm grid search: Probability of crossover operation between two individuals. See GASearchCV documentation. Defaults to 0.2.
 
-    ga_algorithm (str, optional): For genetic algorithm grid search: Evolutionary algorithm to use. Supported options include: {"eaMuPlusLambda", "eaMuCommaLambda", "eaSimple"}. If you need to speed up the genetic algorithm grid search, try setting ``algorithm`` to "euSimple", at the expense of evolutionary model robustness. See more details in the DEAP algorithms documentation (https://deap.readthedocs.io). Defaults to "eaMuPlusLambda".
+        mutation_probability (float, optional): For genetic algorithm grid search: Probability of child mutation. See GASearchCV documentation. Defaults to 0.8.
 
-    early_stop_gen (int, optional): If the genetic algorithm sees ``early_stop_gen`` consecutive generations without improvement in the scoring metric, an early stopping callback is implemented. This saves time by reducing the number of generations the genetic algorithm has to perform. Defaults to 5.
+        ga_algorithm (str, optional): For genetic algorithm grid search: Evolutionary algorithm to use. Supported options include: {"eaMuPlusLambda", "eaMuCommaLambda", "eaSimple"}. If you need to speed up the genetic algorithm grid search, try setting ``algorithm`` to "euSimple", at the expense of evolutionary model robustness. See more details in the DEAP algorithms documentation (https://deap.readthedocs.io). Defaults to "eaMuPlusLambda".
 
-    scoring_metric (str, optional): Scoring metric to use for grid searches. See the classification metrics in the scikit-learn documentation (https://scikit-learn.org/stable/modules/model_evaluation.html) for supported options. Defaults to "f1_weighted".
+        early_stop_gen (int, optional): If the genetic algorithm sees ``early_stop_gen`` consecutive generations without improvement in the scoring metric, an early stopping callback is implemented. This saves time by reducing the number of generations the genetic algorithm has to perform. Defaults to 5.
 
-    chunk_size (int or float, optional): Number of loci for which to perform IterativeImputer at one time. Useful for reducing the memory usage if you are running out of RAM. If integer is specified, selects ``chunk_size`` loci at a time. If a float is specified, selects ``math.ceil(total_loci * chunk_size)`` loci at a time]. Defaults to 1.0 (all features).
+        scoring_metric (str, optional): Scoring metric to use for grid searches. See the classification metrics in the scikit-learn documentation (https://scikit-learn.org/stable/modules/model_evaluation.html) for supported options. Defaults to "f1_weighted".
 
-    disable_progressbar (bool, optional): Whether or not to disable the tqdm progress bar when doing the imputation. If True, progress bar is disabled, which is useful when running the imputation on e.g. an HPC cluster. If the bar is disabled, a status update will be printed to standard output for each iteration and feature instead. If False, the tqdm progress bar will be used. Defaults to False.
+        chunk_size (int or float, optional): Number of loci for which to perform IterativeImputer at one time. Useful for reducing the memory usage if you are running out of RAM. If integer is specified, selects ``chunk_size`` loci at a time. If a float is specified, selects ``math.ceil(total_loci * chunk_size)`` loci at a time]. Defaults to 1.0 (all features).
 
-    progress_update_percent (int or None, optional): Print status updates for features every ``progress_update_percent``\%. IterativeImputer iterations will always be printed, but ``progress_update_percent`` involves iteration progress through the features of each IterativeImputer iteration. If None, then does not print progress through features. Defaults to None.
+        disable_progressbar (bool, optional): Whether or not to disable the tqdm progress bar when doing the imputation. If True, progress bar is disabled, which is useful when running the imputation on e.g. an HPC cluster. If the bar is disabled, a status update will be printed to standard output for each iteration and feature instead. If False, the tqdm progress bar will be used. Defaults to False.
 
-    n_jobs (int, optional): Number of parallel jobs to use. If ``gridparams`` is not None, n_jobs is used for the grid search. Otherwise it is used for the classifier. -1 means using all available processors. Defaults to -1 (all CPUs).
+        progress_update_percent (int or None, optional): Print status updates for features every ``progress_update_percent``\%. IterativeImputer iterations will always be printed, but ``progress_update_percent`` involves iteration progress through the features of each IterativeImputer iteration. If None, then does not print progress through features. Defaults to None.
 
-    verbose (int, optional): Verbosity flag, controls the debug messages that are issues as functions are evaluated. The higher, the more verbose. Possible values are 0, 1, or 2. Defaults to 0.
+        n_jobs (int, optional): Number of parallel jobs to use. If ``gridparams`` is not None, n_jobs is used for the grid search. Otherwise it is used for the classifier. -1 means using all available processors. Defaults to -1 (all CPUs).
+
+        verbose (int, optional): Verbosity flag, controls the debug messages that are issues as functions are evaluated. The higher, the more verbose. Possible values are 0, 1, or 2. Defaults to 0.
 
     Attributes:
         imputed (GenotypeData): New GenotypeData instance with imputed data.
 
         best_params (Dict[str, Any]): Best found parameters from grid search.
 
     """
@@ -292,14 +300,29 @@
             genotype_data.genotypes_012(fmt="pandas")
         )
 
 
 class ImputeKNN(SupervisedImputer):
     """Does K-Nearest Neighbors Iterative Imputation of missing data. Iterative imputation uses the n_nearest_features to inform the imputation at each feature (i.e., SNP site), using the N most correlated features per site. The N most correlated features are drawn with probability proportional to correlation for each imputed target feature to ensure coverage of features throughout the imputation process.
 
+    Args:
+        genotype_data (GenotypeData object): GenotypeData instance that was used to read in the sequence data.
+
+        n_neighbors (int, optional): Number of neighbors to use for K-Nearest Neighbors queries. Defaults to 5.
+
+        weights (str, optional): Weight function used in prediction. Possible values: 'Uniform': Uniform weights with all points in each neighborhood weighted equally; 'distance': Weight points by the inverse of their distance, in this case closer neighbors of a query point will have  a greater influence than neighbors that are further away; 'callable': A user-defined function that accepts an array of distances and returns an array of the same shape containing the weights. Defaults to "distance".
+
+        algorithm (str, optional): Algorithm used to compute the nearest neighbors. Possible values: 'ball_tree', 'kd_tree', 'brute', 'auto'. Defaults to "auto".
+
+        leaf_size (int, optional): Leaf size passed to BallTree or KDTree. This can affect the speed of the construction and query, as well as the memory required to store the tree. The optimal value depends on the nature of the problem. Defaults to 30.
+
+        p (int, optional): Power parameter for the Minkowski metric. When p=1, this is equivalent to using manhattan_distance (l1), and if p=2 it is equivalent to using euclidean distance (l2). For arbitrary p, minkowski_distance (l_p) is used. Defaults to 2.
+
+        metric (str, optional): The distance metric to use for the tree. The default metric is minkowski, and with p=2 this is equivalent to the standard Euclidean metric. See the documentation of sklearn.DistanceMetric for a list of available metrics. If metric is 'precomputed', X is assumed to be a distance matrix and must be square during fit. Defaults to "minkowski".
+
     Example:
         >>> data = GenotypeData(
         >>>     filename="test.str",
         >>>     filetype="auto",
         >>>     guidetree="test.tre",
         >>>     qmatrix_iqtree="test.iqtree"
         >>> )
@@ -317,33 +340,16 @@
         >>>     gridsearch_method="genetic_algorithm",
         >>>     n_nearest_features=10,
         >>>     n_estimators=100,
         >>>     initial_strategy="phylogeny",
         >>> )
         >>>
         >>> knn_gtdata = knn.imputed
-
-    Args:
-        genotype_data (GenotypeData object): GenotypeData instance that was used to read in the sequence data.
-
-        n_neighbors (int, optional): Number of neighbors to use for K-Nearest Neighbors queries. Defaults to 5.
-
-        weights (str, optional): Weight function used in prediction. Possible values: 'Uniform': Uniform weights with all points in each neighborhood weighted equally; 'distance': Weight points by the inverse of their distance, in this case closer neighbors of a query point will have  a greater influence than neighbors that are further away; 'callable': A user-defined function that accepts an array of distances and returns an array of the same shape containing the weights. Defaults to "distance".
-
-        algorithm (str, optional): Algorithm used to compute the nearest neighbors. Possible values: 'ball_tree', 'kd_tree', 'brute', 'auto'. Defaults to "auto".
-
-        leaf_size (int, optional): Leaf size passed to BallTree or KDTree. This can affect the speed of the construction and query, as well as the memory required to store the tree. The optimal value depends on the nature of the problem. Defaults to 30.
-
-        p (int, optional): Power parameter for the Minkowski metric. When p=1, this is equivalent to using manhattan_distance (l1), and if p=2 it is equivalent to using euclidean distance (l2). For arbitrary p, minkowski_distance (l_p) is used. Defaults to 2.
-
-        metric (str, optional): The distance metric to use for the tree. The default metric is minkowski, and with p=2 this is equivalent to the standard Euclidean metric. See the documentation of sklearn.DistanceMetric for a list of available metrics. If metric is 'precomputed', X is assumed to be a distance matrix and must be square during fit. Defaults to "minkowski".
     """
 
-    __doc__ += SupervisedImputer.__doc__
-
     def __init__(
         self,
         genotype_data: Any,
         *,
         n_neighbors: int = 5,
         weights: str = "distance",
         algorithm: str = "auto",
@@ -360,40 +366,14 @@
 
         super().__init__(genotype_data, self.clf, self.clf_type, **kwargs)
 
 
 class ImputeRandomForest(SupervisedImputer):
     """Does Random Forest or Extra Trees Iterative imputation of missing data. Iterative imputation uses the n_nearest_features to inform the imputation at each feature (i.e., SNP site), using the N most correlated features per site. The N most correlated features are drawn with probability proportional to correlation for each imputed target feature to ensure coverage of features throughout the imputation process.
 
-    Example:
-        >>> data = GenotypeData(
-        >>>     filename="test.str",
-        >>>     filetype="auto",
-        >>>     guidetree="test.tre",
-        >>>     qmatrix_iqtree="test.iqtree"
-        >>> )
-        >>>
-        >>> # Genetic Algorithm grid_params
-        >>> grid_params = {
-        >>>     "min_samples_leaf": Integer(1, 10),
-        >>>     "max_depth": Integer(2, 110),
-        >>> }
-        >>>
-        >>> rf = ImputeRandomForest(
-        >>>     genotype_data=data,
-        >>>     gridparams=grid_params,
-        >>>     cv=5,
-        >>>     gridsearch_method="genetic_algorithm",
-        >>>     n_nearest_features=10,
-        >>>     n_estimators=100,
-        >>>     initial_strategy="phylogeny",
-        >>> )
-        >>>
-        >>> rf_gtdata = rf.imputed
-
     Args:
         genotype_data (GenotypeData object): GenotypeData instance that was used to read in the sequence data.
 
         extra_trees (bool, optional): Whether to use ExtraTreesClassifier (If True) instead of RandomForestClassifier (If False). ExtraTreesClassifier is faster, but is not supported by the scikit-learn-intelex patch, whereas RandomForestClassifier is. If using an Intel CPU, the optimizations provided by the scikit-learn-intelex patch might make setting ``extratrees=False`` worthwhile. If you are not using an Intel CPU, the scikit-learn-intelex library is not supported and ExtraTreesClassifier will be faster with similar performance. NOTE: If using scikit-learn-intelex, ``criterion`` must be set to "gini" and ``oob_score`` to False, as those parameters are not currently supported herein. Defaults to True.
 
         n_estimators (int, optional): The number of trees in the forest. Increasing this value can improve the fit, but at the cost of compute time and resources. Defaults to 100.
 
@@ -414,17 +394,42 @@
         min_impurity_decrease (float, optional): A node will be split if this split induces a decrease of the impurity greater than or equal to this value. See ``sklearn.ensemble.ExtraTreesClassifier`` documentation for more information. Defaults to 0.0.
 
         bootstrap (bool, optional): Whether bootstrap samples are used when building trees. If False, the whole dataset is used to build each tree. Defaults to False.
 
         oob_score (bool, optional): Whether to use out-of-bag samples to estimate the generalization score. Only available if ``bootstrap=True``\. Defaults to False.
 
         max_samples (int or float, optional): If bootstrap is True, the number of samples to draw from X to train each base estimator. If None (default), then draws ``X.shape[0] samples``\. if int, then draws ``max_samples`` samples. If float, then draws ``int(max_samples * X.shape[0] samples)`` with ``max_samples`` in the interval (0, 1). Defaults to None.
-    """
 
-    __doc__ += SupervisedImputer.__doc__
+
+    Example:
+        >>> data = GenotypeData(
+        >>>     filename="test.str",
+        >>>     filetype="auto",
+        >>>     guidetree="test.tre",
+        >>>     qmatrix_iqtree="test.iqtree"
+        >>> )
+        >>>
+        >>> # Genetic Algorithm grid_params
+        >>> grid_params = {
+        >>>     "min_samples_leaf": Integer(1, 10),
+        >>>     "max_depth": Integer(2, 110),
+        >>> }
+        >>>
+        >>> rf = ImputeRandomForest(
+        >>>     genotype_data=data,
+        >>>     gridparams=grid_params,
+        >>>     cv=5,
+        >>>     gridsearch_method="genetic_algorithm",
+        >>>     n_nearest_features=10,
+        >>>     n_estimators=100,
+        >>>     initial_strategy="phylogeny",
+        >>> )
+        >>>
+        >>> rf_gtdata = rf.imputed
+    """
 
     def __init__(
         self,
         genotype_data: Any,
         *,
         extratrees: bool = True,
         n_estimators: int = 100,
@@ -470,40 +475,14 @@
 
         super().__init__(genotype_data, self.clf, self.clf_type, **kwargs)
 
 
 class ImputeXGBoost(SupervisedImputer):
     """Does XGBoost (Extreme Gradient Boosting) Iterative imputation of missing data. Iterative imputation uses the n_nearest_features to inform the imputation at each feature (i.e., SNP site), using the N most correlated features per site. The N most correlated features are drawn with probability proportional to correlation for each imputed target feature to ensure coverage of features throughout the imputation process.
 
-    Example:
-        >>> data = GenotypeData(
-        >>>     filename="test.str",
-        >>>     filetype="auto",
-        >>>     guidetree="test.tre",
-        >>>     qmatrix_iqtree="test.iqtree"
-        >>> )
-        >>>
-        >>> # Genetic Algorithm grid_params
-        >>> grid_params = {
-        >>>     "learning_rate": Continuous(lower=0.01, upper=0.1),
-        >>>     "max_depth": Integer(2, 110),
-        >>> }
-        >>>
-        >>> xgb = ImputeXGBoost(
-        >>>     genotype_data=data,
-        >>>     gridparams=grid_params,
-        >>>     cv=5,
-        >>>     gridsearch_method="genetic_algorithm",
-        >>>     n_nearest_features=10,
-        >>>     n_estimators=100,
-        >>>     initial_strategy="phylogeny",
-        >>> )
-        >>>
-        >>> xgb_gtdata = xgb.imputed
-
     Args:
         genotype_data (GenotypeData object): GenotypeData instance that was used to read in the sequence data.
 
         n_estimators (int, optional): The number of boosting rounds. Increasing this value can improve the fit, but at the cost of compute time and RAM usage. Defaults to 100.
 
         max_depth (int, optional): Maximum tree depth for base learners. Defaults to 3.
 
@@ -521,18 +500,41 @@
 
         colsample_bytree (float, optional): Subsample ratio of columns when constructing each tree. Defaults to 1.0.
 
         reg_lambda (float, optional): L2 regularization term on weights (xgb's lambda parameter). Defaults to 1.0.
 
         reg_alpha (float, optional): L1 regularization term on weights (xgb's alpha parameter). Defaults to 1.0.
 
+    Example:
+        >>> data = GenotypeData(
+        >>>     filename="test.str",
+        >>>     filetype="auto",
+        >>>     guidetree="test.tre",
+        >>>     qmatrix_iqtree="test.iqtree"
+        >>> )
+        >>>
+        >>> # Genetic Algorithm grid_params
+        >>> grid_params = {
+        >>>     "learning_rate": Continuous(lower=0.01, upper=0.1),
+        >>>     "max_depth": Integer(2, 110),
+        >>> }
+        >>>
+        >>> xgb = ImputeXGBoost(
+        >>>     genotype_data=data,
+        >>>     gridparams=grid_params,
+        >>>     cv=5,
+        >>>     gridsearch_method="genetic_algorithm",
+        >>>     n_nearest_features=10,
+        >>>     n_estimators=100,
+        >>>     initial_strategy="phylogeny",
+        >>> )
+        >>>
+        >>> xgb_gtdata = xgb.imputed
     """
 
-    __doc__ += SupervisedImputer.__doc__
-
     def __init__(
         self,
         genotype_data: Any,
         *,
         n_estimators: int = 100,
         max_depth: int = 3,
         learning_rate: float = 0.1,
@@ -556,14 +558,19 @@
 
         super().__init__(genotype_data, self.clf, self.clf_type, **kwargs)
 
 
 class ImputeVAE(UnsupervisedImputer):
     """Class to impute missing data using a Variational Autoencoder neural network model. For training, missing values are simulated and the model is trained on the simulated missing values. The real missing values are then predicted by the trained model. The strategy for simulating missing values can be set with the ``sim_strategy`` argument.
 
+    Args:
+        genotype_data (GenotypeData object): Input data initialized as GenotypeData object. Required positional argument.
+
+        kl_beta (float, optional): Weight to apply to Kullback-Liebler divergence loss. If the latent distribution is not learned well, this weight can be adjusted to adjust how much KL divergence affects the total loss. Should be in the range [0, 1]. If set to 1.0, the KL loss is unweighted. If set to 0.0, the KL loss is negated entirely and does not affect the total loss. Defaults to 1.0.
+
     Example:
         >>> data = GenotypeData(
         >>>    filename="test.str",
         >>>    filetype="auto",
         >>>    guidetree="test.tre",
         >>>    qmatrix_iqtree="test.iqtree"
         >>> )
@@ -572,35 +579,32 @@
         >>>     genotype_data=data,
         >>>     learning_rate=0.001,
         >>>     epochs=200,
         >>> )
         >>>
         >>> vae_gtdata = vae.imputed
 
-    Args:
-        genotype_data (GenotypeData object): Input data initialized as GenotypeData object. Required positional argument.
-
-        kl_beta (float, optional): Weight to apply to Kullback-Liebler divergence loss. If the latent distribution is not learned well, this weight can be adjusted to adjust how much KL divergence affects the total loss. Should be in the range [0, 1]. If set to 1.0, the KL loss is unweighted. If set to 0.0, the KL loss is negated entirely and does not affect the total loss. Defaults to 1.0.
     """
 
-    __doc__ += UnsupervisedImputer.__doc__
-
     def __init__(
         self,
         genotype_data,
         kl_beta=1.0,
         **kwargs,
     ):
         kwargs["kl_beta"] = kl_beta
         super().__init__(genotype_data, VAE, "classifier", **kwargs)
 
 
 class ImputeStandardAutoEncoder(UnsupervisedImputer):
     """Class to impute missing data using a standard Autoencoder (SAE) neural network model. For training, missing values are simulated and the model is trained on the simulated missing values. The real missing values are then predicted by the trained model. The strategy for simulating missing values can be set with the ``sim_strategy`` argument.
 
+    Args:
+        genotype_data (GenotypeData object): Input data initialized as GenotypeData object. Required positional argument.
+
     Example:
         >>> data = GenotypeData(
         >>>    filename="test.str",
         >>>    filetype="auto",
         >>>    guidetree="test.tre",
         >>>    qmatrix_iqtree="test.iqtree"
         >>> )
@@ -610,21 +614,16 @@
         >>>     learning_rate=0.001,
         >>>     n_components=5,
         >>>     epochs=200,
         >>> )
         >>>
         >>> # Get the imputed data.
         >>> sae_gtdata = sae.imputed
-
-    Args:
-        genotype_data (GenotypeData object): Input data initialized as GenotypeData object. Required positional argument.
     """
 
-    __doc__ += UnsupervisedImputer.__doc__
-
     def __init__(
         self,
         genotype_data,
         **kwargs,
     ):
         # Get local variables into dictionary object
         self.clf = SAE
@@ -632,15 +631,18 @@
 
         super().__init__(genotype_data, self.clf, self.clf_type, **kwargs)
 
 
 class ImputeUBP(UnsupervisedImputer):
     """Class to impute missing data using an unsupervised backpropagation (UBP) neural network model. For training, missing values are simulated and the model is trained on the simulated missing values. The real missing values are then predicted by the trained model. The strategy for simulating missing values can be set with the ``sim_strategy`` argument.
 
-    UBP [1]_ is an extension of NLPCA [2]_ with the input being randomly generated and of reduced dimensionality that gets trained to predict the supplied output based on only known values. It then uses the trained model to predict missing values. However, in contrast to NLPCA, UBP trains the model over three phases. The first is a single layer perceptron used to refine the randomly generated input. The second phase is a multi-layer perceptron that uses the refined reduced-dimension data from the first phase as input. In the second phase, the model weights are refined but not the input. In the third phase, the model weights and the inputs are then refined.
+    UBP [1]_ is an extension of NLPCA with the input being randomly generated and of reduced dimensionality that gets trained to predict the supplied output based on only known values. It then uses the trained model to predict missing values. However, in contrast to NLPCA, UBP trains the model over three phases. The first is a single layer perceptron used to refine the randomly generated input. The second phase is a multi-layer perceptron that uses the refined reduced-dimension data from the first phase as input. In the second phase, the model weights are refined but not the input. In the third phase, the model weights and the inputs are then refined.
+
+    Args:
+        genotype_data (GenotypeData object): Input data initialized as GenotypeData object. Required positional argument.
 
     Example:
         >>> data = GenotypeData(
         >>>    filename="test.str",
         >>>    filetype="auto",
         >>>    guidetree="test.tre",
         >>>    qmatrix_iqtree="test.iqtree"
@@ -651,20 +653,18 @@
         >>>     learning_rate=0.001,
         >>>     n_components=5
         >>> )
         >>>
         >>> # Get the imputed data.
         >>> ubp_gtdata = ubp.imputed
 
-    Args:
-        genotype_data (GenotypeData object): Input data initialized as GenotypeData object. Required positional argument.
+    References:
+        .. [1] Gashler, M. S., Smith, M. R., Morris, R., & Martinez, T. (2016). Missing value imputation with unsupervised backpropagation. Computational Intelligence, 32(2), 196-215.
     """
 
-    __doc__ += UnsupervisedImputer.__doc__
-
     nlpca = False
 
     def __init__(
         self,
         genotype_data,
         **kwargs,
     ):
@@ -677,14 +677,17 @@
 
 
 class ImputeNLPCA(ImputeUBP):
     """Class to impute missing data using inverse non-linear principal component analysis (NLPCA) neural network models. For training, missing values are simulated and the model is trained on the simulated missing values. The real missing values are then predicted by the trained model. The strategy for simulating missing values can be set with the ``sim_strategy`` argument.
 
     NLPCA [2]_ trains randomly generated, reduced-dimensionality input to predict the correct output. In the case of imputation, the model is trained only on known values, and the trained model is then used to predict the missing values.
 
+    Args:
+        genotype_data (GenotypeData object): Input data initialized as GenotypeData object. Required positional argument.
+
     Example:
         >>> data = GenotypeData(
         >>>    filename="test.str",
         >>>    filetype="auto",
         >>>    guidetree="test.tre",
         >>>    qmatrix_iqtree="test.iqtree"
         >>> )
@@ -693,17 +696,16 @@
         >>>     genotype_data=data,
         >>>     learning_rate=0.001,
         >>>     epochs=200
         >>> )
         >>>
         >>> nlpca_gtdata = nlpca.imputed
 
-    Args:
-        genotype_data (GenotypeData object): Input data initialized as GenotypeData object. Required positional argument.
-    """
+    References:
 
-    __doc__ += UnsupervisedImputer.__doc__
+        .. [2] Scholz, M., Kaplan, F., Guy, C. L., Kopka, J., & Selbig, J. (2005). Non-linear PCA: a missing data approach. Bioinformatics, 21(20), 3887-3895.
+    """
 
     nlpca = True
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `pg-sui-0.3/pgsui/impute/impute.py` & `pg-sui-0.3.0.1/pgsui/impute/impute.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/impute/simple_imputers.py` & `pg-sui-0.3.0.1/pgsui/impute/simple_imputers.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/impute/supervised/iterative_imputer_fixedparams.py` & `pg-sui-0.3.0.1/pgsui/impute/supervised/iterative_imputer_fixedparams.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/impute/supervised/iterative_imputer_gridsearch.py` & `pg-sui-0.3.0.1/pgsui/impute/supervised/iterative_imputer_gridsearch.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/impute/unsupervised/callbacks.py` & `pg-sui-0.3.0.1/pgsui/impute/unsupervised/callbacks.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/impute/unsupervised/keras_classifiers.py` & `pg-sui-0.3.0.1/pgsui/impute/unsupervised/keras_classifiers.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/impute/unsupervised/models/autoencoder_model.py` & `pg-sui-0.3.0.1/pgsui/impute/unsupervised/models/autoencoder_model.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/impute/unsupervised/models/in_development/cnn_model.py` & `pg-sui-0.3.0.1/pgsui/impute/unsupervised/models/in_development/cnn_model.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/impute/unsupervised/models/nlpca_model.py` & `pg-sui-0.3.0.1/pgsui/impute/unsupervised/models/nlpca_model.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/impute/unsupervised/models/ubp_model.py` & `pg-sui-0.3.0.1/pgsui/impute/unsupervised/models/ubp_model.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/impute/unsupervised/models/vae_model.py` & `pg-sui-0.3.0.1/pgsui/impute/unsupervised/models/vae_model.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/impute/unsupervised/neural_network_imputers.py` & `pg-sui-0.3.0.1/pgsui/impute/unsupervised/neural_network_imputers.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/impute/unsupervised/neural_network_methods.py` & `pg-sui-0.3.0.1/pgsui/impute/unsupervised/neural_network_methods.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/pg_sui.py` & `pg-sui-0.3.0.1/pgsui/pg_sui.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/utils/misc.py` & `pg-sui-0.3.0.1/pgsui/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/utils/plotting.py` & `pg-sui-0.3.0.1/pgsui/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/utils/scorers.py` & `pg-sui-0.3.0.1/pgsui/utils/scorers.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/pgsui/utils/sequence_tools.py` & `pg-sui-0.3.0.1/pgsui/utils/sequence_tools.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/setup.py` & `pg-sui-0.3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 NAME = "pg-sui"
-VERSION = "0.3"
+VERSION = "0.3.0.1"
 AUTHORS = "Bradley T. Martin and Tyler K. Chafin"
 AUTHOR_EMAIL = "evobio721@gmail.com"
 MAINTAINER = "Bradley T. Martin"
 DESCRIPTION = "Python machine and deep learning package to impute missing SNPs"
 LONG_DESCRIPTION = open("README.md").read()
 
 setup(
```

### Comparing `pg-sui-0.3/simulation/sim_benchmarks.py` & `pg-sui-0.3.0.1/simulation/sim_benchmarks.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/simulation/sim_treeparams.py` & `pg-sui-0.3.0.1/simulation/sim_treeparams.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/test/pg_sui_simtest.py` & `pg-sui-0.3.0.1/test/pg_sui_simtest.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/test/pg_sui_testing.py` & `pg-sui-0.3.0.1/test/pg_sui_testing.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/test/test.py` & `pg-sui-0.3.0.1/test/test.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/test/test_pgsui.py` & `pg-sui-0.3.0.1/test/test_pgsui.py`

 * *Files identical despite different names*

### Comparing `pg-sui-0.3/test/test_tkc.py` & `pg-sui-0.3.0.1/test/test_tkc.py`

 * *Files 26% similar despite different names*

```diff
@@ -86,14 +86,17 @@
         }
 
         instance = class_instance(
             self.simulated_data, 
             gridparams=param_grid, 
             **kwargs)
 
+        # Write the masks
+        self.transformer.write_mask(filename_prefix="mask_test")
+
         imputed_data = instance.imputed.genotypes_012(fmt="numpy")
 
         # Test that the imputed values are close to the original values
         accuracy = self.transformer.accuracy(
             self.genotype_data.genotypes_012(fmt="numpy"), imputed_data
         )
 
@@ -117,33 +120,59 @@
         )
         pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
             f"RECALL PER CLASS: {dict(zip(range(3), recall_scores))}"
         )
         pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
             f"AVERAGE PRECISION PER CLASS: {dict(zip(range(3), avg_precision_scores))}"
         )
+
+        # Read masks from file
+        self.transformer.read_mask(filename_prefix="mask_test")
+
+        # Recalculate accuracy after reading in the mask
+        accuracy_after_read = self.transformer.accuracy(
+            self.genotype_data.genotypes_012(fmt="numpy"), imputed_data
+        )
+
+        pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
+            f"OVERALL ACCURACY AFTER READ: {accuracy_after_read}"
+        )
+        pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
+            f"AUC-ROC PER CLASS AFTER READ: {dict(zip(range(3), auc_roc_scores))}"
+        )
+        pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
+            f"PRECISION PER CLASS AFTER READ: {dict(zip(range(3), precision_scores))}"
+        )
+        pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
+            f"RECALL PER CLASS AFTER READ: {dict(zip(range(3), recall_scores))}"
+        )
+        pprint.PrettyPrinter(indent=4, sort_dicts=True).pprint(
+            f"AVERAGE PRECISION PER CLASS AFTER READ: {dict(zip(range(3), avg_precision_scores))}"
+        )
+
+
         print("\n")
 
     # def test_ImputeKNN(self):
     #     self._test_class(ImputeKNN)
 
     # def test_ImputeRandomForest(self):
     #     self._test_class(ImputeRandomForest)
 
     # def test_ImputeXGBoost(self):
     #     self._test_class(ImputeXGBoost)
 
-    # def test_ImputeVAE(self):
-    #     self._test_class(ImputeVAE)
+    def test_ImputeVAE(self):
+        self._test_class(ImputeVAE)
 
     # def test_ImputeStandardAutoEncoder(self):
     #     self._test_class(ImputeStandardAutoEncoder)
 
-    def test_ImputeUBP(self):
-        self._test_class(ImputeUBP)
+    # def test_ImputeUBP(self):
+    #     self._test_class(ImputeUBP)
 
     # def test_ImputeNLPCA(self):
     #     self._test_class(ImputeNLPCA)
 
     # def test_ImputeKNN_grid(self):
     #     self._test_class(ImputeKNN, do_gridsearch=True)
```

