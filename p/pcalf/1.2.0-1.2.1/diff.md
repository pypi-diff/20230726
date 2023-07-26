# Comparing `tmp/pcalf-1.2.0.tar.gz` & `tmp/pcalf-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcalf-1.2.0.tar", last modified: Wed Jul 26 13:58:22 2023, max compression
+gzip compressed data, was "pcalf-1.2.1.tar", last modified: Wed Jul 26 13:59:45 2023, max compression
```

## Comparing `pcalf-1.2.0.tar` & `pcalf-1.2.1.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/
--rw-r--r--   0 mmillet    (501) staff       (20)     1069 2023-07-24 14:02:32.000000 pcalf-1.2.0/LICENSE.txt
--rw-r--r--   0 mmillet    (501) staff       (20)       44 2023-07-24 14:02:32.000000 pcalf-1.2.0/MANIFEST.in
--rw-r--r--   0 mmillet    (501) staff       (20)     8515 2023-07-26 13:58:22.000000 pcalf-1.2.0/PKG-INFO
--rw-r--r--   0 mmillet    (501) staff       (20)     8049 2023-07-26 13:16:48.000000 pcalf-1.2.0/README.md
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/
--rw-r--r--   0 mmillet    (501) staff       (20)     8196 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/__init__.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/__pycache__/
--rw-r--r--   0 mmillet    (501) staff       (20)      149 2023-07-24 14:09:01.000000 pcalf-1.2.0/pcalf/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/core/
--rw-r--r--   0 mmillet    (501) staff       (20)     8938 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/core/PcalfDB.py
--rw-r--r--   0 mmillet    (501) staff       (20)     2246 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/core/PcalfSnake.py
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/core/__init__.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/core/__pycache__/
--rw-r--r--   0 mmillet    (501) staff       (20)     9566 2023-07-26 13:14:00.000000 pcalf-1.2.0/pcalf/core/__pycache__/PcalfDB.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)     2243 2023-07-26 12:47:00.000000 pcalf-1.2.0/pcalf/core/__pycache__/PcalfSnake.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)      154 2023-07-24 14:09:01.000000 pcalf-1.2.0/pcalf/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)     7822 2023-07-26 09:03:50.000000 pcalf-1.2.0/pcalf/core/__pycache__/biohmm.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)    15626 2023-07-26 13:19:23.000000 pcalf-1.2.0/pcalf/core/__pycache__/bioseq.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)     1063 2023-07-24 14:09:02.000000 pcalf-1.2.0/pcalf/core/__pycache__/log.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)    18499 2023-07-26 13:19:22.000000 pcalf-1.2.0/pcalf/core/__pycache__/search.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)     8930 2023-07-26 09:01:06.000000 pcalf-1.2.0/pcalf/core/biohmm.py
--rw-r--r--   0 mmillet    (501) staff       (20)    17629 2023-07-26 12:34:35.000000 pcalf-1.2.0/pcalf/core/bioseq.py
--rw-r--r--   0 mmillet    (501) staff       (20)      993 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/core/log.py
--rw-r--r--   0 mmillet    (501) staff       (20)     5167 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/core/pcalf_db_scheme.sql
--rw-r--r--   0 mmillet    (501) staff       (20)    27381 2023-07-26 11:53:50.000000 pcalf-1.2.0/pcalf/core/search.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/datas/
--rw-r--r--   0 mmillet    (501) staff       (20)    29491 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/datas/Gly1.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)     3440 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/datas/Gly1.msa.fa
--rw-r--r--   0 mmillet    (501) staff       (20)    28897 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/datas/Gly2.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)     2819 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/datas/Gly2.msa.fa
--rw-r--r--   0 mmillet    (501) staff       (20)    27603 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/datas/Gly3.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)     3674 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/datas/Gly3.msa.fa
--rw-r--r--   0 mmillet    (501) staff       (20)   106797 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/datas/GlyX3.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)    11209 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/datas/GlyX3.msa.fa
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/datas/__init__.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/datas/__pycache__/
--rw-r--r--   0 mmillet    (501) staff       (20)      155 2023-07-24 14:09:01.000000 pcalf-1.2.0/pcalf/datas/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)      495 2023-07-26 07:22:49.000000 pcalf-1.2.0/pcalf/datas/accession.txt
--rw-r--r--   0 mmillet    (501) staff       (20)   192788 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/datas/all.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)    14739 2023-07-26 08:00:25.000000 pcalf-1.2.0/pcalf/datas/calcyanin.fasta
--rw-r--r--   0 mmillet    (501) staff       (20)    12236 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/datas/nterdb.fasta
--rw-r--r--   0 mmillet    (501) staff       (20)     6003 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/datas/nterdb.ref.tsv
--rw-r--r--   0 mmillet    (501) staff       (20)     3188 2023-07-26 07:44:17.000000 pcalf-1.2.0/pcalf/datas/nterdb.tsv
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/pcalf.egg-info/
--rw-r--r--   0 mmillet    (501) staff       (20)     8021 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/pcalf.egg-info/PKG-INFO
--rw-r--r--   0 mmillet    (501) staff       (20)      663 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/pcalf.egg-info/SOURCES.txt
--rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/pcalf.egg-info/dependency_links.txt
--rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/pcalf.egg-info/not-zip-safe
--rw-r--r--   0 mmillet    (501) staff       (20)      133 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/pcalf.egg-info/requires.txt
--rw-r--r--   0 mmillet    (501) staff       (20)       22 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/pcalf.egg-info/top_level.txt
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/report/
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/report/.ipynb_checkpoints/
--rw-r--r--   0 mmillet    (501) staff       (20)  1158450 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/report/.ipynb_checkpoints/Report-checkpoint.ipynb
--rw-r--r--   0 mmillet    (501) staff       (20)  1182597 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/report/Report.ipynb
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/report/__init__.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/report/__pycache__/
--rw-r--r--   0 mmillet    (501) staff       (20)      156 2023-07-26 13:36:26.000000 pcalf-1.2.0/pcalf/report/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)    17732 2023-07-26 13:36:26.000000 pcalf-1.2.0/pcalf/report/__pycache__/render.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)    79976 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/report/pcalf.svg
--rw-r--r--   0 mmillet    (501) staff       (20)    25860 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/report/render.py
--rw-r--r--   0 mmillet    (501) staff       (20)    71713 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/report/template.css
--rw-r--r--   0 mmillet    (501) staff       (20)    19121 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/report/template.html
--rw-r--r--   0 mmillet    (501) staff       (20)    23654 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/report/template.js
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/workflow/
--rw-r--r--   0 mmillet    (501) staff       (20)    10244 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/.DS_Store
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/workflow/.ipynb_checkpoints/
--rw-r--r--   0 mmillet    (501) staff       (20)    34112 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/.ipynb_checkpoints/Report-checkpoint.ipynb
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/workflow/annotate/
--rw-r--r--   0 mmillet    (501) staff       (20)     8196 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/annotate/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)     1715 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/annotate/Snakefile
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/annotate/__init__.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/workflow/annotate/__pycache__/
--rw-r--r--   0 mmillet    (501) staff       (20)      167 2023-07-26 13:14:00.000000 pcalf-1.2.0/pcalf/workflow/annotate/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/workflow/annotate/config/
--rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/annotate/config/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)      618 2023-07-26 12:15:45.000000 pcalf-1.2.0/pcalf/workflow/annotate/config/config.yaml
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/workflow/annotate/envs/
--rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/annotate/envs/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)      129 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/annotate/envs/biopython_1.79.yaml
--rw-r--r--   0 mmillet    (501) staff       (20)      135 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/annotate/envs/checkm.yaml
--rw-r--r--   0 mmillet    (501) staff       (20)      230 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/annotate/envs/gtdbtk_2.1.yaml
--rw-r--r--   0 mmillet    (501) staff       (20)      232 2023-07-26 13:16:41.000000 pcalf-1.2.0/pcalf/workflow/annotate/envs/ncbi_dataset_14.14.0.yaml
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/workflow/annotate/rules/
--rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/annotate/rules/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)     8241 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/annotate/rules/checkm.smk
--rw-r--r--   0 mmillet    (501) staff       (20)     4509 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/annotate/rules/gtdbtk.smk
--rw-r--r--   0 mmillet    (501) staff       (20)    14816 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/annotate/rules/gtdbtk_by_batch.smk
--rw-r--r--   0 mmillet    (501) staff       (20)      981 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/annotate/rules/ncbi_metadatas.smk
--rw-r--r--   0 mmillet    (501) staff       (20)     9235 2023-07-26 13:53:19.000000 pcalf-1.2.0/pcalf/workflow/annotate/rules/pcalf.smk
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/workflow/annotate/scripts/
--rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/annotate/scripts/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)     8201 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/annotate/scripts/ncbi_metadatas.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/workflow/datasets/
--rw-r--r--   0 mmillet    (501) staff       (20)     8196 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)      741 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/Snakefile
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/__init__.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/workflow/datasets/__pycache__/
--rw-r--r--   0 mmillet    (501) staff       (20)      167 2023-07-26 12:47:01.000000 pcalf-1.2.0/pcalf/workflow/datasets/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/workflow/datasets/config/
--rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/config/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)      169 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/config/config.yaml
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/workflow/datasets/envs/
--rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/envs/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)      129 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/envs/biopython_1.79.yaml
--rw-r--r--   0 mmillet    (501) staff       (20)      232 2023-07-26 13:16:43.000000 pcalf-1.2.0/pcalf/workflow/datasets/envs/ncbi_dataset_14.14.0.yaml
--rw-r--r--   0 mmillet    (501) staff       (20)      199 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/envs/ngd.yaml
--rw-r--r--   0 mmillet    (501) staff       (20)      141 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/envs/prodigal-2.6.yaml
--rw-r--r--   0 mmillet    (501) staff       (20)      154 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/envs/seqkit.yaml
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/workflow/datasets/rules/
--rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/rules/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)     4348 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/rules/download.smk
--rw-r--r--   0 mmillet    (501) staff       (20)     4721 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/rules/fetch.smk
--rw-r--r--   0 mmillet    (501) staff       (20)     3557 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/rules/translate.smk
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf/workflow/datasets/scripts/
--rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/scripts/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)     3085 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/scripts/datas.py
--rw-r--r--   0 mmillet    (501) staff       (20)     4227 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/scripts/fallback.py
--rw-r--r--   0 mmillet    (501) staff       (20)     1161 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/scripts/filter_accession_on_taxid.py
--rw-r--r--   0 mmillet    (501) staff       (20)     4845 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/scripts/get_ncbi_reports.py
--rwxr-xr-x   0 mmillet    (501) staff       (20)     6473 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/scripts/gimme_taxa.py
--rwxr-xr-x   0 mmillet    (501) staff       (20)     1464 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/scripts/log.py
--rw-r--r--   0 mmillet    (501) staff       (20)     1193 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/scripts/taxid_children.py
--rw-r--r--   0 mmillet    (501) staff       (20)     1515 2023-07-24 14:02:32.000000 pcalf-1.2.0/pcalf/workflow/datasets/scripts/utils.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/pcalf.egg-info/
--rw-r--r--   0 mmillet    (501) staff       (20)     8515 2023-07-26 13:58:21.000000 pcalf-1.2.0/pcalf.egg-info/PKG-INFO
--rw-r--r--   0 mmillet    (501) staff       (20)     3856 2023-07-26 13:58:21.000000 pcalf-1.2.0/pcalf.egg-info/SOURCES.txt
--rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-07-26 13:58:21.000000 pcalf-1.2.0/pcalf.egg-info/dependency_links.txt
--rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-07-24 14:06:20.000000 pcalf-1.2.0/pcalf.egg-info/not-zip-safe
--rw-r--r--   0 mmillet    (501) staff       (20)      133 2023-07-26 13:58:21.000000 pcalf-1.2.0/pcalf.egg-info/requires.txt
--rw-r--r--   0 mmillet    (501) staff       (20)        6 2023-07-26 13:58:21.000000 pcalf-1.2.0/pcalf.egg-info/top_level.txt
--rw-r--r--   0 mmillet    (501) staff       (20)       84 2023-07-24 14:02:32.000000 pcalf-1.2.0/pyproject.toml
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:58:22.000000 pcalf-1.2.0/scripts/
--rw-r--r--   0 mmillet    (501) staff       (20)    12734 2023-07-24 14:02:32.000000 pcalf-1.2.0/scripts/pcalf
--rw-r--r--   0 mmillet    (501) staff       (20)     8656 2023-07-26 12:20:10.000000 pcalf-1.2.0/scripts/pcalf-annotate-workflow
--rw-r--r--   0 mmillet    (501) staff       (20)     4197 2023-07-24 14:02:32.000000 pcalf-1.2.0/scripts/pcalf-datasets-workflow
--rw-r--r--   0 mmillet    (501) staff       (20)     1330 2023-07-24 14:02:32.000000 pcalf-1.2.0/scripts/pcalf-report
--rw-r--r--   0 mmillet    (501) staff       (20)       38 2023-07-26 13:58:22.000000 pcalf-1.2.0/setup.cfg
--rw-r--r--   0 mmillet    (501) staff       (20)     1205 2023-07-26 12:02:29.000000 pcalf-1.2.0/setup.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/
+-rw-r--r--   0 mmillet    (501) staff       (20)     1069 2023-07-24 14:02:32.000000 pcalf-1.2.1/LICENSE.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)       44 2023-07-24 14:02:32.000000 pcalf-1.2.1/MANIFEST.in
+-rw-r--r--   0 mmillet    (501) staff       (20)     8515 2023-07-26 13:59:45.000000 pcalf-1.2.1/PKG-INFO
+-rw-r--r--   0 mmillet    (501) staff       (20)     8049 2023-07-26 13:16:48.000000 pcalf-1.2.1/README.md
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8196 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)      149 2023-07-24 14:09:01.000000 pcalf-1.2.1/pcalf/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/core/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8938 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/core/PcalfDB.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     2246 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/core/PcalfSnake.py
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/core/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/core/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)     9566 2023-07-26 13:14:00.000000 pcalf-1.2.1/pcalf/core/__pycache__/PcalfDB.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     2243 2023-07-26 12:47:00.000000 pcalf-1.2.1/pcalf/core/__pycache__/PcalfSnake.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)      154 2023-07-24 14:09:01.000000 pcalf-1.2.1/pcalf/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     7822 2023-07-26 09:03:50.000000 pcalf-1.2.1/pcalf/core/__pycache__/biohmm.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)    15626 2023-07-26 13:19:23.000000 pcalf-1.2.1/pcalf/core/__pycache__/bioseq.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     1063 2023-07-24 14:09:02.000000 pcalf-1.2.1/pcalf/core/__pycache__/log.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)    18499 2023-07-26 13:19:22.000000 pcalf-1.2.1/pcalf/core/__pycache__/search.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     8930 2023-07-26 09:01:06.000000 pcalf-1.2.1/pcalf/core/biohmm.py
+-rw-r--r--   0 mmillet    (501) staff       (20)    17629 2023-07-26 12:34:35.000000 pcalf-1.2.1/pcalf/core/bioseq.py
+-rw-r--r--   0 mmillet    (501) staff       (20)      993 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/core/log.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     5167 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/core/pcalf_db_scheme.sql
+-rw-r--r--   0 mmillet    (501) staff       (20)    27381 2023-07-26 11:53:50.000000 pcalf-1.2.1/pcalf/core/search.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/datas/
+-rw-r--r--   0 mmillet    (501) staff       (20)    29491 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/Gly1.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)     3440 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/Gly1.msa.fa
+-rw-r--r--   0 mmillet    (501) staff       (20)    28897 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/Gly2.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)     2819 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/Gly2.msa.fa
+-rw-r--r--   0 mmillet    (501) staff       (20)    27603 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/Gly3.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)     3674 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/Gly3.msa.fa
+-rw-r--r--   0 mmillet    (501) staff       (20)   106797 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/GlyX3.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)    11209 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/GlyX3.msa.fa
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/datas/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)      155 2023-07-24 14:09:01.000000 pcalf-1.2.1/pcalf/datas/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)      495 2023-07-26 07:22:49.000000 pcalf-1.2.1/pcalf/datas/accession.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)   192788 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/all.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)    14739 2023-07-26 08:00:25.000000 pcalf-1.2.1/pcalf/datas/calcyanin.fasta
+-rw-r--r--   0 mmillet    (501) staff       (20)    12236 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/nterdb.fasta
+-rw-r--r--   0 mmillet    (501) staff       (20)     6003 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/nterdb.ref.tsv
+-rw-r--r--   0 mmillet    (501) staff       (20)     3188 2023-07-26 07:44:17.000000 pcalf-1.2.1/pcalf/datas/nterdb.tsv
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/pcalf.egg-info/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8021 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/pcalf.egg-info/PKG-INFO
+-rw-r--r--   0 mmillet    (501) staff       (20)      663 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/pcalf.egg-info/SOURCES.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/pcalf.egg-info/dependency_links.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/pcalf.egg-info/not-zip-safe
+-rw-r--r--   0 mmillet    (501) staff       (20)      133 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/pcalf.egg-info/requires.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)       22 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/pcalf.egg-info/top_level.txt
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/report/
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/report/.ipynb_checkpoints/
+-rw-r--r--   0 mmillet    (501) staff       (20)  1158450 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/report/.ipynb_checkpoints/Report-checkpoint.ipynb
+-rw-r--r--   0 mmillet    (501) staff       (20)  1182597 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/report/Report.ipynb
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/report/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/report/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)      156 2023-07-26 13:36:26.000000 pcalf-1.2.1/pcalf/report/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)    17732 2023-07-26 13:36:26.000000 pcalf-1.2.1/pcalf/report/__pycache__/render.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)    79976 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/report/pcalf.svg
+-rw-r--r--   0 mmillet    (501) staff       (20)    25860 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/report/render.py
+-rw-r--r--   0 mmillet    (501) staff       (20)    71713 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/report/template.css
+-rw-r--r--   0 mmillet    (501) staff       (20)    19121 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/report/template.html
+-rw-r--r--   0 mmillet    (501) staff       (20)    23654 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/report/template.js
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/
+-rw-r--r--   0 mmillet    (501) staff       (20)    10244 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/.DS_Store
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/.ipynb_checkpoints/
+-rw-r--r--   0 mmillet    (501) staff       (20)    34112 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/.ipynb_checkpoints/Report-checkpoint.ipynb
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/annotate/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8196 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)     1715 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/Snakefile
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/annotate/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)      167 2023-07-26 13:14:00.000000 pcalf-1.2.1/pcalf/workflow/annotate/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/annotate/config/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/config/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)      618 2023-07-26 12:15:45.000000 pcalf-1.2.1/pcalf/workflow/annotate/config/config.yaml
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/annotate/envs/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/envs/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)      129 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/envs/biopython_1.79.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      135 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/envs/checkm.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      230 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/envs/gtdbtk_2.1.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      232 2023-07-26 13:16:41.000000 pcalf-1.2.1/pcalf/workflow/annotate/envs/ncbi_dataset_14.14.0.yaml
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/annotate/rules/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/rules/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)     8241 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/rules/checkm.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)     4509 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/rules/gtdbtk.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)    14816 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/rules/gtdbtk_by_batch.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)      981 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/rules/ncbi_metadatas.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)     9235 2023-07-26 13:53:19.000000 pcalf-1.2.1/pcalf/workflow/annotate/rules/pcalf.smk
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/annotate/scripts/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/scripts/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)     8201 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/scripts/ncbi_metadatas.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/datasets/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8196 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)      741 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/Snakefile
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/datasets/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)      167 2023-07-26 12:47:01.000000 pcalf-1.2.1/pcalf/workflow/datasets/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/datasets/config/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/config/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)      169 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/config/config.yaml
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/datasets/envs/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/envs/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)      129 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/envs/biopython_1.79.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      232 2023-07-26 13:16:43.000000 pcalf-1.2.1/pcalf/workflow/datasets/envs/ncbi_dataset_14.14.0.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      199 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/envs/ngd.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      141 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/envs/prodigal-2.6.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      154 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/envs/seqkit.yaml
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/datasets/rules/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/rules/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)     4348 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/rules/download.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)     4721 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/rules/fetch.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)     3557 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/rules/translate.smk
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)     3085 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/datas.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     4227 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/fallback.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     1161 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/filter_accession_on_taxid.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     4845 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/get_ncbi_reports.py
+-rwxr-xr-x   0 mmillet    (501) staff       (20)     6473 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/gimme_taxa.py
+-rwxr-xr-x   0 mmillet    (501) staff       (20)     1464 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/log.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     1193 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/taxid_children.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     1515 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/utils.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf.egg-info/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8515 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf.egg-info/PKG-INFO
+-rw-r--r--   0 mmillet    (501) staff       (20)     3856 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf.egg-info/SOURCES.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf.egg-info/dependency_links.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-07-24 14:06:20.000000 pcalf-1.2.1/pcalf.egg-info/not-zip-safe
+-rw-r--r--   0 mmillet    (501) staff       (20)      133 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf.egg-info/requires.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)        6 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf.egg-info/top_level.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)       84 2023-07-24 14:02:32.000000 pcalf-1.2.1/pyproject.toml
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/scripts/
+-rw-r--r--   0 mmillet    (501) staff       (20)    12734 2023-07-24 14:02:32.000000 pcalf-1.2.1/scripts/pcalf
+-rw-r--r--   0 mmillet    (501) staff       (20)     8656 2023-07-26 12:20:10.000000 pcalf-1.2.1/scripts/pcalf-annotate-workflow
+-rw-r--r--   0 mmillet    (501) staff       (20)     4197 2023-07-24 14:02:32.000000 pcalf-1.2.1/scripts/pcalf-datasets-workflow
+-rw-r--r--   0 mmillet    (501) staff       (20)     1330 2023-07-24 14:02:32.000000 pcalf-1.2.1/scripts/pcalf-report
+-rw-r--r--   0 mmillet    (501) staff       (20)       38 2023-07-26 13:59:45.000000 pcalf-1.2.1/setup.cfg
+-rw-r--r--   0 mmillet    (501) staff       (20)     1205 2023-07-26 13:59:22.000000 pcalf-1.2.1/setup.py
```

### Comparing `pcalf-1.2.0/LICENSE.txt` & `pcalf-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/PKG-INFO` & `pcalf-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcalf
-Version: 1.2.0
+Version: 1.2.1
 Summary: Search calcyanin in a set of amino acid sequences
 Home-page: https://github.com/K2SOHIGH/pcalf
 Author: Maxime Millet
 Author-email: maxime.luc.millet@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pcalf-1.2.0/README.md` & `pcalf-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/.DS_Store` & `pcalf-1.2.1/pcalf/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/core/PcalfDB.py` & `pcalf-1.2.1/pcalf/core/PcalfDB.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/core/PcalfSnake.py` & `pcalf-1.2.1/pcalf/core/PcalfSnake.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/core/__pycache__/PcalfDB.cpython-39.pyc` & `pcalf-1.2.1/pcalf/core/__pycache__/PcalfDB.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/core/__pycache__/PcalfSnake.cpython-39.pyc` & `pcalf-1.2.1/pcalf/core/__pycache__/PcalfSnake.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/core/__pycache__/biohmm.cpython-39.pyc` & `pcalf-1.2.1/pcalf/core/__pycache__/biohmm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/core/__pycache__/bioseq.cpython-39.pyc` & `pcalf-1.2.1/pcalf/core/__pycache__/bioseq.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/core/__pycache__/log.cpython-39.pyc` & `pcalf-1.2.1/pcalf/core/__pycache__/log.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/core/__pycache__/search.cpython-39.pyc` & `pcalf-1.2.1/pcalf/core/__pycache__/search.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/core/biohmm.py` & `pcalf-1.2.1/pcalf/core/biohmm.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/core/bioseq.py` & `pcalf-1.2.1/pcalf/core/bioseq.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/core/log.py` & `pcalf-1.2.1/pcalf/core/log.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/core/pcalf_db_scheme.sql` & `pcalf-1.2.1/pcalf/core/pcalf_db_scheme.sql`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/core/search.py` & `pcalf-1.2.1/pcalf/core/search.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/datas/Gly1.hmm` & `pcalf-1.2.1/pcalf/datas/Gly1.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/datas/Gly1.msa.fa` & `pcalf-1.2.1/pcalf/datas/Gly1.msa.fa`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/datas/Gly2.hmm` & `pcalf-1.2.1/pcalf/datas/Gly2.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/datas/Gly2.msa.fa` & `pcalf-1.2.1/pcalf/datas/Gly2.msa.fa`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/datas/Gly3.hmm` & `pcalf-1.2.1/pcalf/datas/Gly3.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/datas/Gly3.msa.fa` & `pcalf-1.2.1/pcalf/datas/Gly3.msa.fa`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/datas/GlyX3.hmm` & `pcalf-1.2.1/pcalf/datas/GlyX3.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/datas/GlyX3.msa.fa` & `pcalf-1.2.1/pcalf/datas/GlyX3.msa.fa`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/datas/all.hmm` & `pcalf-1.2.1/pcalf/datas/all.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/datas/calcyanin.fasta` & `pcalf-1.2.1/pcalf/datas/calcyanin.fasta`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/datas/nterdb.fasta` & `pcalf-1.2.1/pcalf/datas/nterdb.fasta`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/datas/nterdb.ref.tsv` & `pcalf-1.2.1/pcalf/datas/nterdb.ref.tsv`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/datas/nterdb.tsv` & `pcalf-1.2.1/pcalf/datas/nterdb.tsv`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/pcalf.egg-info/PKG-INFO` & `pcalf-1.2.1/pcalf/pcalf.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/pcalf.egg-info/SOURCES.txt` & `pcalf-1.2.1/pcalf/pcalf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/report/.ipynb_checkpoints/Report-checkpoint.ipynb` & `pcalf-1.2.1/pcalf/report/.ipynb_checkpoints/Report-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/report/Report.ipynb` & `pcalf-1.2.1/pcalf/report/Report.ipynb`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/report/__pycache__/render.cpython-39.pyc` & `pcalf-1.2.1/pcalf/report/__pycache__/render.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/report/pcalf.svg` & `pcalf-1.2.1/pcalf/report/pcalf.svg`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/report/render.py` & `pcalf-1.2.1/pcalf/report/render.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/report/template.css` & `pcalf-1.2.1/pcalf/report/template.css`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/report/template.html` & `pcalf-1.2.1/pcalf/report/template.html`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/report/template.js` & `pcalf-1.2.1/pcalf/report/template.js`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/.DS_Store` & `pcalf-1.2.1/pcalf/workflow/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/.ipynb_checkpoints/Report-checkpoint.ipynb` & `pcalf-1.2.1/pcalf/workflow/.ipynb_checkpoints/Report-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/annotate/.DS_Store` & `pcalf-1.2.1/pcalf/workflow/annotate/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/annotate/Snakefile` & `pcalf-1.2.1/pcalf/workflow/annotate/Snakefile`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/annotate/config/.DS_Store` & `pcalf-1.2.1/pcalf/workflow/annotate/config/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/annotate/config/config.yaml` & `pcalf-1.2.1/pcalf/workflow/annotate/config/config.yaml`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/annotate/envs/.DS_Store` & `pcalf-1.2.1/pcalf/workflow/annotate/envs/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/annotate/rules/.DS_Store` & `pcalf-1.2.1/pcalf/workflow/annotate/rules/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/annotate/rules/checkm.smk` & `pcalf-1.2.1/pcalf/workflow/annotate/rules/checkm.smk`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/annotate/rules/gtdbtk.smk` & `pcalf-1.2.1/pcalf/workflow/annotate/rules/gtdbtk.smk`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/annotate/rules/gtdbtk_by_batch.smk` & `pcalf-1.2.1/pcalf/workflow/annotate/rules/gtdbtk_by_batch.smk`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/annotate/rules/ncbi_metadatas.smk` & `pcalf-1.2.1/pcalf/workflow/annotate/rules/ncbi_metadatas.smk`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/annotate/rules/pcalf.smk` & `pcalf-1.2.1/pcalf/workflow/annotate/rules/pcalf.smk`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/annotate/scripts/.DS_Store` & `pcalf-1.2.1/pcalf/workflow/annotate/scripts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/annotate/scripts/ncbi_metadatas.py` & `pcalf-1.2.1/pcalf/workflow/annotate/scripts/ncbi_metadatas.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/.DS_Store` & `pcalf-1.2.1/pcalf/workflow/datasets/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/Snakefile` & `pcalf-1.2.1/pcalf/workflow/datasets/Snakefile`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/config/.DS_Store` & `pcalf-1.2.1/pcalf/workflow/datasets/config/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/envs/.DS_Store` & `pcalf-1.2.1/pcalf/workflow/datasets/envs/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/rules/.DS_Store` & `pcalf-1.2.1/pcalf/workflow/datasets/rules/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/rules/download.smk` & `pcalf-1.2.1/pcalf/workflow/datasets/rules/download.smk`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/rules/fetch.smk` & `pcalf-1.2.1/pcalf/workflow/datasets/rules/fetch.smk`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/rules/translate.smk` & `pcalf-1.2.1/pcalf/workflow/datasets/rules/translate.smk`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/scripts/.DS_Store` & `pcalf-1.2.1/pcalf/workflow/datasets/scripts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/scripts/datas.py` & `pcalf-1.2.1/pcalf/workflow/datasets/scripts/datas.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/scripts/fallback.py` & `pcalf-1.2.1/pcalf/workflow/datasets/scripts/fallback.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/scripts/filter_accession_on_taxid.py` & `pcalf-1.2.1/pcalf/workflow/datasets/scripts/filter_accession_on_taxid.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/scripts/get_ncbi_reports.py` & `pcalf-1.2.1/pcalf/workflow/datasets/scripts/get_ncbi_reports.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/scripts/gimme_taxa.py` & `pcalf-1.2.1/pcalf/workflow/datasets/scripts/gimme_taxa.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/scripts/log.py` & `pcalf-1.2.1/pcalf/workflow/datasets/scripts/log.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/scripts/taxid_children.py` & `pcalf-1.2.1/pcalf/workflow/datasets/scripts/taxid_children.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf/workflow/datasets/scripts/utils.py` & `pcalf-1.2.1/pcalf/workflow/datasets/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/pcalf.egg-info/PKG-INFO` & `pcalf-1.2.1/pcalf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcalf
-Version: 1.2.0
+Version: 1.2.1
 Summary: Search calcyanin in a set of amino acid sequences
 Home-page: https://github.com/K2SOHIGH/pcalf
 Author: Maxime Millet
 Author-email: maxime.luc.millet@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pcalf-1.2.0/pcalf.egg-info/SOURCES.txt` & `pcalf-1.2.1/pcalf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/scripts/pcalf` & `pcalf-1.2.1/scripts/pcalf`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/scripts/pcalf-annotate-workflow` & `pcalf-1.2.1/scripts/pcalf-annotate-workflow`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/scripts/pcalf-datasets-workflow` & `pcalf-1.2.1/scripts/pcalf-datasets-workflow`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/scripts/pcalf-report` & `pcalf-1.2.1/scripts/pcalf-report`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.0/setup.py` & `pcalf-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pcalf',
-    version='1.2.0',
+    version='1.2.1',
     description='Search calcyanin in a set of amino acid sequences',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url='https://github.com/K2SOHIGH/pcalf',
     author='Maxime Millet',
     author_email='maxime.luc.millet@gmail.com',
     license='MIT',
```

