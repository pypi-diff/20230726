# Comparing `tmp/cazomevolve-0.1.7.tar.gz` & `tmp/cazomevolve-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cazomevolve-0.1.7.tar", last modified: Tue Jul 18 16:57:15 2023, max compression
+gzip compressed data, was "cazomevolve-0.1.7.1.tar", last modified: Wed Jul 26 18:04:55 2023, max compression
```

## Comparing `cazomevolve-0.1.7.tar` & `cazomevolve-0.1.7.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.097237 cazomevolve-0.1.7/
--rw-rw-r--   0 em        (1000) em        (1000)     1067 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/LICENSE
--rw-rw-r--   0 em        (1000) em        (1000)    42889 2023-07-18 16:57:15.097237 cazomevolve-0.1.7/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)    42124 2023-07-18 12:14:26.000000 cazomevolve-0.1.7/README.md
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.961232 cazomevolve-0.1.7/cazomevolve/
--rw-rw-r--   0 em        (1000) em        (1000)     2094 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/__init__.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.977233 cazomevolve-0.1.7/cazomevolve/cazome/
--rw-rw-r--   0 em        (1000) em        (1000)     1517 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/cazome/__init__.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.981233 cazomevolve-0.1.7/cazomevolve/cazome/cazy/
--rw-rw-r--   0 em        (1000) em        (1000)     1548 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/cazome/cazy/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)     7022 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/cazome/cazy/get_cazy_cazymes.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.989233 cazomevolve-0.1.7/cazomevolve/cazome/dbcan/
--rw-rw-r--   0 em        (1000) em        (1000)     1548 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/cazome/dbcan/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)     6237 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py
--rw-rw-r--   0 em        (1000) em        (1000)     4895 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/cazome/dbcan/invoke_dbcan.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.993233 cazomevolve-0.1.7/cazomevolve/cazome/explore/
--rw-rw-r--   0 em        (1000) em        (1000)     1527 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/cazome/explore/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)    11615 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/cazome/explore/cazome_sizes.py
--rw-rw-r--   0 em        (1000) em        (1000)     6409 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/cazome/explore/cazy_classes.py
--rw-rw-r--   0 em        (1000) em        (1000)    17152 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/cazome/explore/cazy_families.py
--rw-rw-r--   0 em        (1000) em        (1000)    19985 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/cazome/explore/cooccurring_families.py
--rw-rw-r--   0 em        (1000) em        (1000)    20862 2023-07-18 16:28:28.000000 cazomevolve-0.1.7/cazomevolve/cazome/explore/explore_cazomes.py
--rw-rw-r--   0 em        (1000) em        (1000)     5445 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/cazome/explore/parse_data.py
--rw-rw-r--   0 em        (1000) em        (1000)    17853 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/cazome/explore/pca.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.993233 cazomevolve-0.1.7/cazomevolve/genomes/
--rw-rw-r--   0 em        (1000) em        (1000)     1540 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/genomes/__init__.py
--rwxrwxr-x   0 em        (1000) em        (1000)    11300 2023-07-18 11:44:58.000000 cazomevolve-0.1.7/cazomevolve/genomes/download_genomes.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.997233 cazomevolve-0.1.7/cazomevolve/scripts/
--rw-rw-r--   0 em        (1000) em        (1000)     1492 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/__init__.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.009234 cazomevolve-0.1.7/cazomevolve/scripts/bash/
--rw-rw-r--   0 em        (1000) em        (1000)     1568 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/bash/build_cazy_db.sh
--rwxrwxr-x   0 em        (1000) em        (1000)     2401 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/bash/download_acc_genomes.sh
--rw-rw-r--   0 em        (1000) em        (1000)     2078 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/build_cazy_db.py
--rw-rw-r--   0 em        (1000) em        (1000)     2462 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/cazomevolve_script.py
--rw-rw-r--   0 em        (1000) em        (1000)     3135 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/download_acc_genomes.py
--rw-rw-r--   0 em        (1000) em        (1000)     3063 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/get_fam_seqs.py
--rw-rw-r--   0 em        (1000) em        (1000)     2064 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/run_fam_blast.py
--rw-rw-r--   0 em        (1000) em        (1000)     1969 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/run_fam_diamond.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.953232 cazomevolve-0.1.7/cazomevolve/scripts/tree/
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.013234 cazomevolve-0.1.7/cazomevolve/scripts/tree/ani/
--rw-rw-r--   0 em        (1000) em        (1000)     2123 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/ani/build_anim_tree.R
--rw-rw-r--   0 em        (1000) em        (1000)     1123 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/ani/run_anim.sh
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.025235 cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/
--rw-rw-r--   0 em        (1000) em        (1000)     1863 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/align_scos.sh
--rw-rw-r--   0 em        (1000) em        (1000)     1928 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/annotate_genomes.sh
--rw-rw-r--   0 em        (1000) em        (1000)     1927 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/backtranslate.sh
--rw-rw-r--   0 em        (1000) em        (1000)     6330 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/concatenate_cds.py
--rw-rw-r--   0 em        (1000) em        (1000)     5189 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/extract_cds.py
--rw-rw-r--   0 em        (1000) em        (1000)     1718 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/find_orthologues.sh
--rw-rw-r--   0 em        (1000) em        (1000)     2073 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.029235 cazomevolve-0.1.7/cazomevolve/seq_diversity/
--rw-rw-r--   0 em        (1000) em        (1000)     1489 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/seq_diversity/__init__.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.033235 cazomevolve-0.1.7/cazomevolve/seq_diversity/explore/
--rw-rw-r--   0 em        (1000) em        (1000)     1489 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/seq_diversity/explore/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)     6473 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/seq_diversity/explore/cazy.py
--rw-rw-r--   0 em        (1000) em        (1000)     6192 2023-07-18 12:12:05.000000 cazomevolve-0.1.7/cazomevolve/seq_diversity/explore/parse.py
--rw-rw-r--   0 em        (1000) em        (1000)    11125 2023-07-17 22:21:48.000000 cazomevolve-0.1.7/cazomevolve/seq_diversity/explore/plot.py
--rwxrwxr-x   0 em        (1000) em        (1000)     1790 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/seq_diversity/get_fam_seqs.sh
--rwxrwxr-x   0 em        (1000) em        (1000)     1724 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/seq_diversity/run_blastp.sh
--rwxrwxr-x   0 em        (1000) em        (1000)     2036 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/seq_diversity/run_diamond.sh
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.041235 cazomevolve-0.1.7/cazomevolve/taxs/
--rw-rw-r--   0 em        (1000) em        (1000)     1513 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/taxs/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)    11322 2023-07-17 20:40:22.000000 cazomevolve-0.1.7/cazomevolve/taxs/add_taxs.py
--rw-rw-r--   0 em        (1000) em        (1000)     6971 2023-07-18 12:11:27.000000 cazomevolve-0.1.7/cazomevolve/taxs/ncbi.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.045235 cazomevolve-0.1.7/cazomevolve/utilities/
--rw-rw-r--   0 em        (1000) em        (1000)     1517 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/__init__.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.073236 cazomevolve-0.1.7/cazomevolve/utilities/parsers/
--rw-rw-r--   0 em        (1000) em        (1000)     1529 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)     4914 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/add_taxs_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     2260 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/build_cazy_db_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     6316 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/dl_acc_genomes_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     6780 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/download_genomes_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     6687 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/explore_cazomes_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     4021 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/get_cazy_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     3480 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/get_dbcan_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     2899 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/get_fam_seqs_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     3724 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/invoke_dbcan_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     4427 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/parse_cmd.py
--rw-rw-r--   0 em        (1000) em        (1000)     2257 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/run_blast_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     2372 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/run_diamond_parser.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.973233 cazomevolve-0.1.7/cazomevolve.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)    42889 2023-07-18 16:57:14.000000 cazomevolve-0.1.7/cazomevolve.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     3318 2023-07-18 16:57:14.000000 cazomevolve-0.1.7/cazomevolve.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-07-18 16:57:14.000000 cazomevolve-0.1.7/cazomevolve.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       76 2023-07-18 16:57:14.000000 cazomevolve-0.1.7/cazomevolve.egg-info/entry_points.txt
--rw-rw-r--   0 em        (1000) em        (1000)      161 2023-07-18 16:57:14.000000 cazomevolve-0.1.7/cazomevolve.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)       12 2023-07-18 16:57:14.000000 cazomevolve-0.1.7/cazomevolve.egg-info/top_level.txt
--rw-rw-r--   0 em        (1000) em        (1000)       38 2023-07-18 16:57:15.097237 cazomevolve-0.1.7/setup.cfg
--rw-rw-r--   0 em        (1000) em        (1000)     4157 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/setup.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.093237 cazomevolve-0.1.7/tests/
--rw-rw-r--   0 em        (1000) em        (1000)     5804 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_add_taxs.py
--rw-rw-r--   0 em        (1000) em        (1000)     1958 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_cazomevolve.py
--rw-rw-r--   0 em        (1000) em        (1000)     2585 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_explore_cazome_sizes.py
--rw-rw-r--   0 em        (1000) em        (1000)    13133 2023-07-18 16:36:56.000000 cazomevolve-0.1.7/tests/test_explore_cazomes.py
--rw-rw-r--   0 em        (1000) em        (1000)     1830 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_explore_classes.py
--rw-rw-r--   0 em        (1000) em        (1000)     2741 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_explore_cooccurring_families.py
--rw-rw-r--   0 em        (1000) em        (1000)     3625 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_explore_families.py
--rw-rw-r--   0 em        (1000) em        (1000)     2562 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_explore_parse_data.py
--rw-rw-r--   0 em        (1000) em        (1000)     5653 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_explore_pca.py
--rw-rw-r--   0 em        (1000) em        (1000)     4216 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_explore_upsetplot.py
--rw-rw-r--   0 em        (1000) em        (1000)     3373 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_genome_download.py
--rw-rw-r--   0 em        (1000) em        (1000)     4114 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_get_cazy.py
--rw-rw-r--   0 em        (1000) em        (1000)     3744 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_get_dbcan.py
--rw-rw-r--   0 em        (1000) em        (1000)     4157 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_invoke_dbcan.py
--rw-rw-r--   0 em        (1000) em        (1000)     3712 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_ncbi.py
--rw-rw-r--   0 em        (1000) em        (1000)     8722 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     5843 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_scripts.py
--rw-rw-r--   0 em        (1000) em        (1000)     4569 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_seq_diversity.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.072330 cazomevolve-0.1.7.1/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1067 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/LICENSE
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    42891 2023-07-26 18:04:55.072330 cazomevolve-0.1.7.1/PKG-INFO
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    42124 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/README.md
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.048329 cazomevolve-0.1.7.1/cazomevolve/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2096 2023-07-26 18:04:39.000000 cazomevolve-0.1.7.1/cazomevolve/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.048329 cazomevolve-0.1.7.1/cazomevolve/cazome/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1517 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/cazome/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.052330 cazomevolve-0.1.7.1/cazomevolve/cazome/cazy/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1548 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/cazome/cazy/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7022 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/cazome/cazy/get_cazy_cazymes.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.052330 cazomevolve-0.1.7.1/cazomevolve/cazome/dbcan/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1548 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/cazome/dbcan/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6457 2023-07-26 18:04:39.000000 cazomevolve-0.1.7.1/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4895 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/cazome/dbcan/invoke_dbcan.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.052330 cazomevolve-0.1.7.1/cazomevolve/cazome/explore/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1527 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/cazome/explore/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11615 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/cazome/explore/cazome_sizes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6409 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/cazome/explore/cazy_classes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    17152 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/cazome/explore/cazy_families.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    19985 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/cazome/explore/cooccurring_families.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    20862 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/cazome/explore/explore_cazomes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5445 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/cazome/explore/parse_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    17886 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/cazome/explore/pca.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.056330 cazomevolve-0.1.7.1/cazomevolve/genomes/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1540 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/genomes/__init__.py
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)    11300 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/genomes/download_genomes.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.056330 cazomevolve-0.1.7.1/cazomevolve/scripts/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1492 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.056330 cazomevolve-0.1.7.1/cazomevolve/scripts/bash/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1568 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/bash/build_cazy_db.sh
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)     2401 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/bash/download_acc_genomes.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2078 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/build_cazy_db.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2462 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/cazomevolve_script.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3135 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/download_acc_genomes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3063 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/get_fam_seqs.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2064 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/run_fam_blast.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1969 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/run_fam_diamond.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.044330 cazomevolve-0.1.7.1/cazomevolve/scripts/tree/
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.056330 cazomevolve-0.1.7.1/cazomevolve/scripts/tree/ani/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2123 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/tree/ani/build_anim_tree.R
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1123 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/tree/ani/run_anim.sh
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.060330 cazomevolve-0.1.7.1/cazomevolve/scripts/tree/phylo/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1863 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/tree/phylo/align_scos.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1928 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/tree/phylo/annotate_genomes.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1927 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/tree/phylo/backtranslate.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6330 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/tree/phylo/concatenate_cds.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5189 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/tree/phylo/extract_cds.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1718 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/tree/phylo/find_orthologues.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2073 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.060330 cazomevolve-0.1.7.1/cazomevolve/seq_diversity/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1489 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/seq_diversity/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.060330 cazomevolve-0.1.7.1/cazomevolve/seq_diversity/explore/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1489 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/seq_diversity/explore/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6473 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/seq_diversity/explore/cazy.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6192 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/seq_diversity/explore/parse.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11125 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/seq_diversity/explore/plot.py
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)     1790 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/seq_diversity/get_fam_seqs.sh
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)     1724 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/seq_diversity/run_blastp.sh
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)     2036 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/seq_diversity/run_diamond.sh
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.060330 cazomevolve-0.1.7.1/cazomevolve/taxs/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1513 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/taxs/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11322 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/taxs/add_taxs.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6971 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/taxs/ncbi.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.060330 cazomevolve-0.1.7.1/cazomevolve/utilities/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1517 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/utilities/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.064330 cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1529 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4914 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/add_taxs_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2260 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/build_cazy_db_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6316 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/dl_acc_genomes_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6780 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/download_genomes_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6687 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/explore_cazomes_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4021 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/get_cazy_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3480 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/get_dbcan_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2899 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/get_fam_seqs_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3724 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/invoke_dbcan_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4427 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/parse_cmd.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2257 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/run_blast_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2372 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/run_diamond_parser.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.048329 cazomevolve-0.1.7.1/cazomevolve.egg-info/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    42891 2023-07-26 18:04:55.000000 cazomevolve-0.1.7.1/cazomevolve.egg-info/PKG-INFO
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3318 2023-07-26 18:04:55.000000 cazomevolve-0.1.7.1/cazomevolve.egg-info/SOURCES.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)        1 2023-07-26 18:04:55.000000 cazomevolve-0.1.7.1/cazomevolve.egg-info/dependency_links.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)       76 2023-07-26 18:04:55.000000 cazomevolve-0.1.7.1/cazomevolve.egg-info/entry_points.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)      161 2023-07-26 18:04:55.000000 cazomevolve-0.1.7.1/cazomevolve.egg-info/requires.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)       12 2023-07-26 18:04:55.000000 cazomevolve-0.1.7.1/cazomevolve.egg-info/top_level.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)       38 2023-07-26 18:04:55.072330 cazomevolve-0.1.7.1/setup.cfg
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4161 2023-07-26 18:04:39.000000 cazomevolve-0.1.7.1/setup.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-26 18:04:55.072330 cazomevolve-0.1.7.1/tests/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5804 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_add_taxs.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1958 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_cazomevolve.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2585 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_explore_cazome_sizes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    13133 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_explore_cazomes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1830 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_explore_classes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2741 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_explore_cooccurring_families.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3625 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_explore_families.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2562 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_explore_parse_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5653 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_explore_pca.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4216 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_explore_upsetplot.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3373 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_genome_download.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4114 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_get_cazy.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3744 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_get_dbcan.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4157 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_invoke_dbcan.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3712 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_ncbi.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     8722 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5843 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_scripts.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4569 2023-07-26 18:00:35.000000 cazomevolve-0.1.7.1/tests/test_seq_diversity.py
```

### Comparing `cazomevolve-0.1.7/LICENSE` & `cazomevolve-0.1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/PKG-INFO` & `cazomevolve-0.1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cazomevolve
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: A bioinforamtic package for investigating the evolution of CAZomes
 Author: Emma E. M. Hobbs
 Author-email: eemh1@st-andrews.ac.uk
 License: MIT
 Keywords: bioinforamtics protein
 Platform: Posix
 Platform: MacOS X
```

### Comparing `cazomevolve-0.1.7/README.md` & `cazomevolve-0.1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/__init__.py` & `cazomevolve-0.1.7.1/cazomevolve/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 # SOFTWARE.
 """Bioinforamtic package for exploring the evolution of CAZomes"""
 
 
 import logging
 
 
-__version__ = "0.1.7"
+__version__ = "0.1.7.1"
 
 __citation__ = "???"
 
 
 def closing_message(job, args):
     """Write closing messsage to terminal
```

### Comparing `cazomevolve-0.1.7/cazomevolve/cazome/__init__.py` & `cazomevolve-0.1.7.1/cazomevolve/cazome/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/cazome/cazy/__init__.py` & `cazomevolve-0.1.7.1/cazomevolve/cazome/cazy/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/cazome/cazy/get_cazy_cazymes.py` & `cazomevolve-0.1.7.1/cazomevolve/cazome/cazy/get_cazy_cazymes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/cazome/dbcan/__init__.py` & `cazomevolve-0.1.7.1/cazomevolve/cazome/dbcan/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py` & `cazomevolve-0.1.7.1/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,17 +98,22 @@
     df = df[df['#ofTools'] != 1]
     
     for ri in tqdm(range(len(df)), desc=f"Parsing {output_dir.name}"):
         row = df.iloc[ri]
 
         protein_accession = row['Gene ID']
 
-        hmmer_fams = get_tool_fams(row[1])
-        hotpep_fams = get_tool_fams(row[2])
-        diamond_fams = get_tool_fams(row[3])
+        if list(df.columns)[1].startswith('EC#'):
+            hmmer_fams = get_tool_fams(row[2])
+            hotpep_fams = get_tool_fams(row[3])
+            diamond_fams = get_tool_fams(row[4])
+        else:
+            hmmer_fams = get_tool_fams(row[1])
+            hotpep_fams = get_tool_fams(row[2])
+            diamond_fams = get_tool_fams(row[3])
 
         # get the fams at least two tools agreed upon
         dbcan_fams = get_dbcan_consensus(hmmer_fams, hotpep_fams, diamond_fams)
 
         if len(dbcan_fams) > 0:
             try:
                 fam_annotations[protein_accession]
```

### Comparing `cazomevolve-0.1.7/cazomevolve/cazome/dbcan/invoke_dbcan.py` & `cazomevolve-0.1.7.1/cazomevolve/cazome/dbcan/invoke_dbcan.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/cazome/explore/__init__.py` & `cazomevolve-0.1.7.1/cazomevolve/cazome/explore/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/cazome/explore/cazome_sizes.py` & `cazomevolve-0.1.7.1/cazomevolve/cazome/explore/cazome_sizes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/cazome/explore/cazy_classes.py` & `cazomevolve-0.1.7.1/cazomevolve/cazome/explore/cazy_classes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/cazome/explore/cazy_families.py` & `cazomevolve-0.1.7.1/cazomevolve/cazome/explore/cazy_families.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/cazome/explore/cooccurring_families.py` & `cazomevolve-0.1.7.1/cazomevolve/cazome/explore/cooccurring_families.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/cazome/explore/explore_cazomes.py` & `cazomevolve-0.1.7.1/cazomevolve/cazome/explore/explore_cazomes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/cazome/explore/parse_data.py` & `cazomevolve-0.1.7.1/cazomevolve/cazome/explore/parse_data.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/cazome/explore/pca.py` & `cazomevolve-0.1.7.1/cazomevolve/cazome/explore/pca.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         in the dataset
     :param file_path: str/Path, path to write out figure. If none, image is not written to a file
     :param file_format: str, format to write out the image. Default, png
     :param dpi: int, resolution for saved figure
     
     Retrun numpy array with the explained variance per PC
     """
+    plt.clf()
     cumExpVar = np.cumsum(pca.explained_variance_ratio_)
 
     keepPC = [pc for pc in range(nComp) if cumExpVar[pc] >= threshold][0]
     print(
         'Number of features needed to explain {:1.2f} fraction of total variance is {:2d}. '.format(threshold, keepPC)
     )
 
@@ -129,14 +130,16 @@
     :param nComp: int, number of PCs to plot
     :param file_path: str/Path, path to write out figure. If none, image is not written to a file
     :param file_format: str, format to write out the image. Default, png
     :param dpi: int, resolution for saved figure
     
     Return nothing
     """
+    plt.clf()
+    
     PC_values = np.arange(nComp) + 1
     plt.plot(PC_values, pca.explained_variance_ratio_[0:nComp], 'o-', linewidth=2, color='blue')
     plt.xlabel('Principal Component')
     plt.ylabel('Variance Explained')
     if file_path is not None:
         plt.savefig(
             file_path,
```

### Comparing `cazomevolve-0.1.7/cazomevolve/genomes/__init__.py` & `cazomevolve-0.1.7.1/cazomevolve/genomes/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/genomes/download_genomes.py` & `cazomevolve-0.1.7.1/cazomevolve/genomes/download_genomes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/__init__.py` & `cazomevolve-0.1.7.1/cazomevolve/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/bash/build_cazy_db.sh` & `cazomevolve-0.1.7.1/cazomevolve/scripts/bash/build_cazy_db.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/bash/download_acc_genomes.sh` & `cazomevolve-0.1.7.1/cazomevolve/scripts/bash/download_acc_genomes.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/build_cazy_db.py` & `cazomevolve-0.1.7.1/cazomevolve/scripts/build_cazy_db.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/cazomevolve_script.py` & `cazomevolve-0.1.7.1/cazomevolve/scripts/cazomevolve_script.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/download_acc_genomes.py` & `cazomevolve-0.1.7.1/cazomevolve/scripts/download_acc_genomes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/get_fam_seqs.py` & `cazomevolve-0.1.7.1/cazomevolve/scripts/get_fam_seqs.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/run_fam_blast.py` & `cazomevolve-0.1.7.1/cazomevolve/scripts/run_fam_blast.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/run_fam_diamond.py` & `cazomevolve-0.1.7.1/cazomevolve/scripts/run_fam_diamond.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/tree/ani/build_anim_tree.R` & `cazomevolve-0.1.7.1/cazomevolve/scripts/tree/ani/build_anim_tree.R`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/tree/ani/run_anim.sh` & `cazomevolve-0.1.7.1/cazomevolve/scripts/tree/ani/run_anim.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/align_scos.sh` & `cazomevolve-0.1.7.1/cazomevolve/scripts/tree/phylo/align_scos.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/annotate_genomes.sh` & `cazomevolve-0.1.7.1/cazomevolve/scripts/tree/phylo/annotate_genomes.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/backtranslate.sh` & `cazomevolve-0.1.7.1/cazomevolve/scripts/tree/phylo/backtranslate.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/concatenate_cds.py` & `cazomevolve-0.1.7.1/cazomevolve/scripts/tree/phylo/concatenate_cds.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/extract_cds.py` & `cazomevolve-0.1.7.1/cazomevolve/scripts/tree/phylo/extract_cds.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/find_orthologues.sh` & `cazomevolve-0.1.7.1/cazomevolve/scripts/tree/phylo/find_orthologues.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh` & `cazomevolve-0.1.7.1/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/seq_diversity/__init__.py` & `cazomevolve-0.1.7.1/cazomevolve/seq_diversity/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/seq_diversity/explore/__init__.py` & `cazomevolve-0.1.7.1/cazomevolve/seq_diversity/explore/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/seq_diversity/explore/cazy.py` & `cazomevolve-0.1.7.1/cazomevolve/seq_diversity/explore/cazy.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/seq_diversity/explore/parse.py` & `cazomevolve-0.1.7.1/cazomevolve/seq_diversity/explore/parse.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/seq_diversity/explore/plot.py` & `cazomevolve-0.1.7.1/cazomevolve/seq_diversity/explore/plot.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/seq_diversity/get_fam_seqs.sh` & `cazomevolve-0.1.7.1/cazomevolve/seq_diversity/get_fam_seqs.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/seq_diversity/run_blastp.sh` & `cazomevolve-0.1.7.1/cazomevolve/seq_diversity/run_blastp.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/seq_diversity/run_diamond.sh` & `cazomevolve-0.1.7.1/cazomevolve/seq_diversity/run_diamond.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/taxs/__init__.py` & `cazomevolve-0.1.7.1/cazomevolve/taxs/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/taxs/add_taxs.py` & `cazomevolve-0.1.7.1/cazomevolve/taxs/add_taxs.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/taxs/ncbi.py` & `cazomevolve-0.1.7.1/cazomevolve/taxs/ncbi.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/utilities/__init__.py` & `cazomevolve-0.1.7.1/cazomevolve/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/utilities/parsers/__init__.py` & `cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/utilities/parsers/add_taxs_parser.py` & `cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/add_taxs_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/utilities/parsers/build_cazy_db_parser.py` & `cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/build_cazy_db_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/utilities/parsers/dl_acc_genomes_parser.py` & `cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/dl_acc_genomes_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/utilities/parsers/download_genomes_parser.py` & `cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/download_genomes_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/utilities/parsers/explore_cazomes_parser.py` & `cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/explore_cazomes_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/utilities/parsers/get_cazy_parser.py` & `cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/get_cazy_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/utilities/parsers/get_dbcan_parser.py` & `cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/get_dbcan_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/utilities/parsers/get_fam_seqs_parser.py` & `cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/get_fam_seqs_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/utilities/parsers/invoke_dbcan_parser.py` & `cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/invoke_dbcan_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/utilities/parsers/parse_cmd.py` & `cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/parse_cmd.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/utilities/parsers/run_blast_parser.py` & `cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/run_blast_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve/utilities/parsers/run_diamond_parser.py` & `cazomevolve-0.1.7.1/cazomevolve/utilities/parsers/run_diamond_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/cazomevolve.egg-info/PKG-INFO` & `cazomevolve-0.1.7.1/cazomevolve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cazomevolve
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: A bioinforamtic package for investigating the evolution of CAZomes
 Author: Emma E. M. Hobbs
 Author-email: eemh1@st-andrews.ac.uk
 License: MIT
 Keywords: bioinforamtics protein
 Platform: Posix
 Platform: MacOS X
```

### Comparing `cazomevolve-0.1.7/cazomevolve.egg-info/SOURCES.txt` & `cazomevolve-0.1.7.1/cazomevolve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/setup.py` & `cazomevolve-0.1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 # get long description from README.md
 with Path("README.md").open("r") as long_description_handle:
     long_description = long_description_handle.read()
 
 
 setuptools.setup(
     name="cazomevolve",
-    version="0.1.7",
+    version="0.1.7.1",
     # Metadata
     author="Emma E. M. Hobbs",
     author_email="eemh1@st-andrews.ac.uk",
     description="".join(
         [
             (
                 "A bioinforamtic package for investigating the evolution of CAZomes"
@@ -118,8 +118,8 @@
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Programming Language :: Python :: 3.8",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
-)
+)
```

### Comparing `cazomevolve-0.1.7/tests/test_add_taxs.py` & `cazomevolve-0.1.7.1/tests/test_add_taxs.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_cazomevolve.py` & `cazomevolve-0.1.7.1/tests/test_cazomevolve.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_explore_cazome_sizes.py` & `cazomevolve-0.1.7.1/tests/test_explore_cazome_sizes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_explore_cazomes.py` & `cazomevolve-0.1.7.1/tests/test_explore_cazomes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_explore_classes.py` & `cazomevolve-0.1.7.1/tests/test_explore_classes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_explore_cooccurring_families.py` & `cazomevolve-0.1.7.1/tests/test_explore_cooccurring_families.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_explore_families.py` & `cazomevolve-0.1.7.1/tests/test_explore_families.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_explore_parse_data.py` & `cazomevolve-0.1.7.1/tests/test_explore_parse_data.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_explore_pca.py` & `cazomevolve-0.1.7.1/tests/test_explore_pca.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_explore_upsetplot.py` & `cazomevolve-0.1.7.1/tests/test_explore_upsetplot.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_genome_download.py` & `cazomevolve-0.1.7.1/tests/test_genome_download.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_get_cazy.py` & `cazomevolve-0.1.7.1/tests/test_get_cazy.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_get_dbcan.py` & `cazomevolve-0.1.7.1/tests/test_get_dbcan.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_invoke_dbcan.py` & `cazomevolve-0.1.7.1/tests/test_invoke_dbcan.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_ncbi.py` & `cazomevolve-0.1.7.1/tests/test_ncbi.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_parser.py` & `cazomevolve-0.1.7.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_scripts.py` & `cazomevolve-0.1.7.1/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.7/tests/test_seq_diversity.py` & `cazomevolve-0.1.7.1/tests/test_seq_diversity.py`

 * *Files identical despite different names*

