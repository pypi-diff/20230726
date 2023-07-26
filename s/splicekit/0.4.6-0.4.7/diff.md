# Comparing `tmp/splicekit-0.4.6.tar.gz` & `tmp/splicekit-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splicekit-0.4.6.tar", last modified: Mon Jul  3 14:01:22 2023, max compression
+gzip compressed data, was "splicekit-0.4.7.tar", last modified: Wed Jul 26 10:31:55 2023, max compression
```

## Comparing `splicekit-0.4.6.tar` & `splicekit-0.4.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-03 14:01:22.103729 splicekit-0.4.6/
--rw-rw-r--   0 rotg     (2023757) games       (20)    23915 2023-07-03 14:01:22.103334 splicekit-0.4.6/PKG-INFO
--rwxrwxr-x   0 rotg     (2023757) games       (20)    23517 2023-06-19 14:13:26.000000 splicekit-0.4.6/README.md
--rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-07-03 14:01:22.103829 splicekit-0.4.6/setup.cfg
--rw-rw-r--   0 rotg     (2023757) games       (20)     1150 2023-06-12 17:55:56.000000 splicekit-0.4.6/setup.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-03 14:01:22.087579 splicekit-0.4.6/splicekit/
--rw-rw-r--   0 rotg     (2023757) games       (20)    13844 2023-07-03 13:59:07.000000 splicekit-0.4.6/splicekit/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-03 14:01:22.090896 splicekit-0.4.6/splicekit/clusterlogfc/
--rw-rw-r--   0 rotg     (2023757) games       (20)     5584 2023-05-05 11:49:03.000000 splicekit-0.4.6/splicekit/clusterlogfc/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-03 14:01:22.091634 splicekit-0.4.6/splicekit/config/
--rw-rw-r--   0 rotg     (2023757) games       (20)      951 2023-06-07 13:26:10.000000 splicekit-0.4.6/splicekit/config/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-03 14:01:22.101415 splicekit-0.4.6/splicekit/core/
--rw-rw-r--   0 rotg     (2023757) games       (20)      119 2023-06-20 11:22:13.000000 splicekit-0.4.6/splicekit/core/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     6667 2023-05-05 06:13:11.000000 splicekit-0.4.6/splicekit/core/anchors.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    16752 2023-05-24 07:18:50.000000 splicekit-0.4.6/splicekit/core/annotation.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     3988 2023-01-31 12:27:24.000000 splicekit-0.4.6/splicekit/core/delta_dar.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     5407 2023-05-05 08:10:13.000000 splicekit-0.4.6/splicekit/core/exons.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)    30130 2023-06-30 14:19:04.000000 splicekit-0.4.6/splicekit/core/features.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     5662 2023-05-05 06:13:26.000000 splicekit-0.4.6/splicekit/core/genes.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1059 2023-06-07 14:32:33.000000 splicekit-0.4.6/splicekit/core/jbrowse2.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     9033 2023-06-08 11:52:41.000000 splicekit-0.4.6/splicekit/core/jbrowse2_create.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2948 2023-04-26 12:12:45.000000 splicekit-0.4.6/splicekit/core/juan.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    18195 2023-06-21 14:33:41.000000 splicekit-0.4.6/splicekit/core/junctions.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    37713 2023-05-04 06:56:59.000000 splicekit-0.4.6/splicekit/core/motifs.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1663 2023-05-02 18:35:35.000000 splicekit-0.4.6/splicekit/core/patterns.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2420 2023-05-03 10:54:22.000000 splicekit-0.4.6/splicekit/core/promisc.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     9045 2023-05-03 09:57:04.000000 splicekit-0.4.6/splicekit/core/report.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1527 2023-05-09 07:27:49.000000 splicekit-0.4.6/splicekit/folders.setup
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-03 14:01:22.102271 splicekit-0.4.6/splicekit/judge/
--rw-rw-r--   0 rotg     (2023757) games       (20)    26830 2023-06-08 11:49:08.000000 splicekit-0.4.6/splicekit/judge/__init__.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)     5402 2023-05-05 10:18:19.000000 splicekit-0.4.6/splicekit/splicecompare
--rwxrwxr-x   0 rotg     (2023757) games       (20)     5117 2023-06-30 14:16:46.000000 splicekit-0.4.6/splicekit/splicekit
--rw-rw-r--   0 rotg     (2023757) games       (20)     1638 2023-06-06 07:56:19.000000 splicekit-0.4.6/splicekit/splicekit.config.template
--rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-07-03 14:00:08.000000 splicekit-0.4.6/splicekit/version
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-03 14:01:22.090456 splicekit-0.4.6/splicekit.egg-info/
--rw-rw-r--   0 rotg     (2023757) games       (20)    23915 2023-07-03 14:01:21.000000 splicekit-0.4.6/splicekit.egg-info/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)      850 2023-07-03 14:01:21.000000 splicekit-0.4.6/splicekit.egg-info/SOURCES.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-07-03 14:01:21.000000 splicekit-0.4.6/splicekit.egg-info/dependency_links.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-05-09 07:35:55.000000 splicekit-0.4.6/splicekit.egg-info/not-zip-safe
--rw-rw-r--   0 rotg     (2023757) games       (20)       62 2023-07-03 14:01:21.000000 splicekit-0.4.6/splicekit.egg-info/requires.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)       10 2023-07-03 14:01:21.000000 splicekit-0.4.6/splicekit.egg-info/top_level.txt
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-26 10:31:55.180852 splicekit-0.4.7/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    23985 2023-07-26 10:31:55.180386 splicekit-0.4.7/PKG-INFO
+-rwxrwxr-x   0 rotg     (2023757) games       (20)    23644 2023-07-19 11:40:35.000000 splicekit-0.4.7/README.md
+-rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-07-26 10:31:55.180939 splicekit-0.4.7/setup.cfg
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1182 2023-07-26 10:31:35.000000 splicekit-0.4.7/setup.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-26 10:31:55.160889 splicekit-0.4.7/splicekit/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    13883 2023-07-18 08:00:13.000000 splicekit-0.4.7/splicekit/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-26 10:31:55.164603 splicekit-0.4.7/splicekit/clusterlogfc/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5584 2023-05-05 11:49:03.000000 splicekit-0.4.7/splicekit/clusterlogfc/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-26 10:31:55.165507 splicekit-0.4.7/splicekit/config/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      951 2023-06-07 13:26:10.000000 splicekit-0.4.7/splicekit/config/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-26 10:31:55.177656 splicekit-0.4.7/splicekit/core/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      119 2023-06-20 11:22:13.000000 splicekit-0.4.7/splicekit/core/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     6667 2023-05-05 06:13:11.000000 splicekit-0.4.7/splicekit/core/anchors.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    16752 2023-05-24 07:18:50.000000 splicekit-0.4.7/splicekit/core/annotation.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     3988 2023-01-31 12:27:24.000000 splicekit-0.4.7/splicekit/core/delta_dar.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5407 2023-05-05 08:10:13.000000 splicekit-0.4.7/splicekit/core/exons.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)    30130 2023-06-30 14:19:04.000000 splicekit-0.4.7/splicekit/core/features.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5662 2023-05-05 06:13:26.000000 splicekit-0.4.7/splicekit/core/genes.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1059 2023-06-07 14:32:33.000000 splicekit-0.4.7/splicekit/core/jbrowse2.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     9036 2023-07-19 11:36:02.000000 splicekit-0.4.7/splicekit/core/jbrowse2_create.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2948 2023-04-26 12:12:45.000000 splicekit-0.4.7/splicekit/core/juan.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    18195 2023-06-21 14:33:41.000000 splicekit-0.4.7/splicekit/core/junctions.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    37713 2023-05-04 06:56:59.000000 splicekit-0.4.7/splicekit/core/motifs.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1663 2023-05-02 18:35:35.000000 splicekit-0.4.7/splicekit/core/patterns.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2420 2023-05-03 10:54:22.000000 splicekit-0.4.7/splicekit/core/promisc.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    10102 2023-07-19 11:36:02.000000 splicekit-0.4.7/splicekit/core/report.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1527 2023-05-09 07:27:49.000000 splicekit-0.4.7/splicekit/folders.setup
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-26 10:31:55.178893 splicekit-0.4.7/splicekit/judge/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    26830 2023-06-08 11:49:08.000000 splicekit-0.4.7/splicekit/judge/__init__.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     5402 2023-05-05 10:18:19.000000 splicekit-0.4.7/splicekit/splicecompare
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     5117 2023-06-30 14:16:46.000000 splicekit-0.4.7/splicekit/splicekit
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1638 2023-06-06 07:56:19.000000 splicekit-0.4.7/splicekit/splicekit.config.template
+-rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-07-26 10:31:46.000000 splicekit-0.4.7/splicekit/version
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-26 10:31:55.164072 splicekit-0.4.7/splicekit.egg-info/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    23985 2023-07-26 10:31:54.000000 splicekit-0.4.7/splicekit.egg-info/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)      850 2023-07-26 10:31:54.000000 splicekit-0.4.7/splicekit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-07-26 10:31:54.000000 splicekit-0.4.7/splicekit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-05-09 07:35:55.000000 splicekit-0.4.7/splicekit.egg-info/not-zip-safe
+-rw-rw-r--   0 rotg     (2023757) games       (20)       91 2023-07-26 10:31:54.000000 splicekit-0.4.7/splicekit.egg-info/requires.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)       10 2023-07-26 10:31:54.000000 splicekit-0.4.7/splicekit.egg-info/top_level.txt
```

### Comparing `splicekit-0.4.6/PKG-INFO` & `splicekit-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: splicekit
-Version: 0.4.6
+Version: 0.4.7
 Summary: splicekit: comprehensive toolkit for splicing analysis from short-read RNA-seq
 Home-page: https://github.com/bedapub/splicekit
 Author: Roche, PMDA Spliceosome team
 Author-email: gregor.rot@gmail.com
 Keywords: splicekit,splicing,transcriptomics,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
+## splicekit: a toolkit for splicing analysis from short-read RNA-seq
 
 A comprehensive platform for splicing analysis of RNA-seq short-read sequencing data. <b>splicekit</b> input are read alignments in BAM format (look at [datasets](datasets) for details on how to run examples).
 
 [What is splicekit?](#what_do)<br>
 [Installation](#initial_setup)<br>
 [Quick start](#quick_start)<br>
 [Software dependencies](#software_dep)<br>
```

### Comparing `splicekit-0.4.6/README.md` & `splicekit-0.4.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# splicekit
+<picture><img src="media/splicekit_logo.png" height="30"/></picture>
+## splicekit: a toolkit for splicing analysis from short-read RNA-seq
 
 A comprehensive platform for splicing analysis of RNA-seq short-read sequencing data. <b>splicekit</b> input are read alignments in BAM format (look at [datasets](datasets) for details on how to run examples).
 
 [What is splicekit?](#what_do)<br>
 [Installation](#initial_setup)<br>
 [Quick start](#quick_start)<br>
 [Software dependencies](#software_dep)<br>
```

### Comparing `splicekit-0.4.6/setup.py` & `splicekit-0.4.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,9 +23,9 @@
     author_email='gregor.rot@gmail.com',
     url='https://github.com/bedapub/splicekit',
     keywords=['splicekit', 'splicing', 'transcriptomics', 'bioinformatics'],
     include_package_data=True,
     package_data={
         'splicekit': ['folders.setup', 'splicekit.config.template', 'version'],
     },
-    install_requires=["pybio", "scanRBP", "pysam", "numpy", "psutil", "bs4", "requests", "rangehttpserver"],
+    install_requires=["python-dateutil>=2.8.2", "pybio", "scanRBP", "pysam", "numpy>=1.20", "psutil", "bs4", "requests", "rangehttpserver"],
 )
```

### Comparing `splicekit-0.4.6/splicekit/__init__.py` & `splicekit-0.4.7/splicekit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,14 +130,15 @@
     splicekit.core.features.read_genes()
     os.system("rm -f data/comparison_genes_data/*.tab > /dev/null 2>&1")
     splicekit.core.features.save_comps_feature_data("genes")
 
 def features():
     junctions_master()
     anchors()
+    splicekit.core.delta_dar.compute()
     junctions()
     exons()
     genes()
 
 def anchors():
     for anchor_type in ["donor", "acceptor"]:
         os.system(f"rm -f reference/{anchor_type}_anchors.gtf > /dev/null 2>&1")
@@ -232,12 +233,12 @@
 
 def process(force=False):
     setup()
     annotation()
     features()
     edgeR()
     juan()
+    judge_process()
     motifs()
     promisc()
-    judge_process()
     clusterlogfc_process()
     jbrowse2_process(force_samples=force, force_annotation=force)
```

### Comparing `splicekit-0.4.6/splicekit/clusterlogfc/__init__.py` & `splicekit-0.4.7/splicekit/clusterlogfc/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/config/__init__.py` & `splicekit-0.4.7/splicekit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/core/anchors.py` & `splicekit-0.4.7/splicekit/core/anchors.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/core/annotation.py` & `splicekit-0.4.7/splicekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/core/delta_dar.py` & `splicekit-0.4.7/splicekit/core/delta_dar.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/core/exons.py` & `splicekit-0.4.7/splicekit/core/exons.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/core/features.py` & `splicekit-0.4.7/splicekit/core/features.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/core/genes.py` & `splicekit-0.4.7/splicekit/core/genes.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/core/jbrowse2.py` & `splicekit-0.4.7/splicekit/core/jbrowse2.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/core/jbrowse2_create.py` & `splicekit-0.4.7/splicekit/core/jbrowse2_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 dirs_to_check = ['logs/logs_jbrowse/', 'jobs/jobs_jbrowse/','results/results_jbrowse/'] 
 
 def check_genome():
     '''jbrowse requires index genome assembly'''
     if not os.path.exists(genome_fa + '.fai'):
         print('[jbrowse] No fasta index file found. Creating it...')
         print(f'[jbrowse/samtools] Indexing genome {genome_fa}')
-        os.sys(f'{container} samtools faidx {genome_fa}')
+        os.system(f'{container} samtools faidx {genome_fa}')
         print(f'[jbrowse/samtools] Indexing genome done')
 
 
 def write_sample_jobs(force_samples):
     
     # clean up previous jobs
     os.system(f'rm -r jobs/jobs_jbrowse/*')
@@ -127,16 +127,16 @@
         print('[jbrowse2] annotation fully parsed')
 
         # now we add each sample's files in different track categories  --------------------------------------------------------------------------------------------------------------------------
         for sample in bam_files:
             sample_id = sample.replace('.bam', '')
             cram_fname = dirs_to_check[2] + sample.replace('.bam', '.cram')
             bigwig_fname = dirs_to_check[2] + sample.replace('.bam', '.bw')
-            os.system(f'cd jbrowse2/splicekit_data; {container} jbrowse add-track ../../{bigwig_fname} --name {sample_id}.bw --trackId {sample_id}.bw  --category "Coverage" --load symlink')
-            os.system(f'cd jbrowse2/splicekit_data; {container} jbrowse add-track ../../{cram_fname} --name {sample_id}.cram --trackId {sample_id}.cram --category "Reads" --load symlink')
+            os.system(f'cd jbrowse2/splicekit_data; {container} jbrowse add-track ../../{bigwig_fname} --name {sample_id}_bw --trackId {sample_id}_bw  --category "Coverage" --load symlink')
+            os.system(f'cd jbrowse2/splicekit_data; {container} jbrowse add-track ../../{cram_fname} --name {sample_id}_cram --trackId {sample_id}_cram --category "Reads" --load symlink')
     else:
         print('[jbrowse] config.json already existing in jbrowse2/splicekit_data --> use "splicekit jbrowse2_create annotation -force" to overwrite')
 
 def process(force_samples=False, force_annotation=False):
     #os.system(f'rm -r jbrowse2/splicekit_data/*') # clean up before starting
     check_genome()
     # clean up previous jobs
```

### Comparing `splicekit-0.4.6/splicekit/core/juan.py` & `splicekit-0.4.7/splicekit/core/juan.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/core/junctions.py` & `splicekit-0.4.7/splicekit/core/junctions.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/core/motifs.py` & `splicekit-0.4.7/splicekit/core/motifs.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/core/patterns.py` & `splicekit-0.4.7/splicekit/core/patterns.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/core/promisc.py` & `splicekit-0.4.7/splicekit/core/promisc.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/core/report.py` & `splicekit-0.4.7/splicekit/core/report.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import sys
 import gzip
 import pybio
 import glob
 import splicekit.config as config
 import splicekit.core.annotation as annotation
 import splicekit.core.features as features
+import numpy as np
 
 def toint(temp):
     try:
         temp = str(int(temp))
         return temp
     except:
         return temp
@@ -35,33 +36,52 @@
         while r:
             r = r.replace("\r", "").replace("\n", "").split("\t")
             data = dict(zip(header, r))
             database[data["junction_id"]] = data
             r = f.readline()
         f.close()        
 
+    # since we construct {sample_id}_{treatment_id} and {treatment_id} can still contain _,
+    # we go back to the original samples table to extract {sample_id}
+    samples = []
+    f = open("samples.tab", "rt")
+    header = f.readline().replace("\r", "").replace("\n", "").split("\t")
+    r = f.readline()
+    while r:
+        r = r.replace("\r", "").replace("\n", "").split("\t")
+        data = dict(zip(header, r))
+        samples.append(data["sample_id"])
+        r = f.readline()
+    f.close()
+
     # read comparisons, to determine which tracks (samples) to show in JBrowse
     f = open("annotation/comparisons.tab", "rt")
     r = f.readline()
     r = f.readline()
     while r:
         compound_samples = []
         dmso_samples = []
         r = r.replace("\r", "").replace("\n", "").split("\t")
         comparison = r[0]
         temp = r[1].split(",")
         for el in temp:
-            temp2 = toint("_".join(el.split("_")[:-1]))
-            if temp2 not in compound_samples:
-                compound_samples.append(temp2)
+            my_sample = ""
+            for sample_id in samples:
+                if el.startswith(sample_id+"_") and len(my_sample)<len(sample_id):
+                    my_sample = sample_id
+            if my_sample not in compound_samples and my_sample!="":
+                compound_samples.append(my_sample)
         temp = r[2].split(",")
         for el in temp:
-            temp2 = toint("_".join(el.split("_")[:-1]))
-            if temp2 not in dmso_samples:
-                dmso_samples.append(temp2)
+            my_sample = ""
+            for sample_id in samples:
+                if el.startswith(sample_id+"_") and len(my_sample)<len(sample_id):
+                    my_sample = sample_id
+            if my_sample not in dmso_samples and my_sample!="":
+                dmso_samples.append(my_sample)
         comparisons[comparison] = (compound_samples, dmso_samples)
         r = f.readline()
     f.close()
 
     if feature_name=="genes":
         rfiles = glob.glob(f"results/results_edgeR_{feature_name}/*difffeature.tab")
     else:
@@ -78,18 +98,18 @@
         compound = bname.split("_"+config.control_name)[0]
         f = open(fname, "rt")
         header = f.readline().replace("\n", "").replace("\r", "").split("\t")
         r = f.readline()
         while r:
             r = r.replace("\n", "").replace("\r", "").split("\t")
             data = dict(zip(header, r))
-            tracks_fixed = ["gene-refseq", "transcript-refseq", "transcript-ensembl"] # New JBrowse2
+            tracks_fixed = ["annotation_track"] # New JBrowse2
             tracks_samples, tracks_dmso = comparisons[comparison] 
-            tracks_samples = [track+'_bw' for track in tracks_samples] # New JBrowse2 --> bigwig files are called by id_bw 
-            tracks_dmso = [track+'_bw' for track in tracks_dmso] # New JBrowse2 --> bigwig files are called by id_bw 
+            tracks_samples = [track+'_bw' for track in tracks_samples] # New JBrowse2 --> bigwig files are called by id_bw
+            tracks_dmso = [track+'_bw' for track in tracks_dmso] # New JBrowse2 --> bigwig files are called by id_bw
             tracks = ",".join(tracks_samples[:3]+tracks_dmso[:3]+tracks_fixed)
             f_from=int(data["feature_start"])
             f_to=int(data["feature_stop"])
             delta = round(abs(f_from-f_to)*0.15) # 15% surrounding
             loc_from=int(data["feature_start"])-delta
             loc_to=int(data["feature_stop"])+delta
             row = [comparison, compound, "", data["feature_id"]]
@@ -101,15 +121,15 @@
                 junction_first_exon = f"first_exon_start_{first_exon_start}"
             else:
                 first_exon_start = None
                 junction_first_exon = ""
             if feature_name=="junctions":
                 row.append(junction_first_exon)
             row += [data["gene_id"], data["gene_name"], "{chr}:{f_from}..{f_to}".format(chr=data["chr"], f_from=data["feature_start"], f_to=data["feature_stop"])]
-            row.append("{jbrowse_url}&assembly=hg38&loc={chr}:{loc_from}..{loc_to}&tracks={tracks}".format(jbrowse_url=config.jbrowse2_url.format(compound=compound), compound=compound, chr=data["chr"], loc_from=loc_from, loc_to=loc_to, tracks=tracks))
+            row.append("{jbrowse_url}&assembly=GenomeSequence&loc={chr}:{loc_from}..{loc_to}&tracks={tracks}".format(jbrowse_url=config.jbrowse2_url.format(compound=compound), compound=compound, chr=data["chr"], loc_from=loc_from, loc_to=loc_to, tracks=tracks))
             row += [data["sum_feature_test"], data["sum_feature_control"]]
             row += [data["test_pfi"], data["control_pfi"], data["delta_pfi"]]
             if feature_name=="junctions":
                 row.append(database[data["feature_id"]]["annotated"]) 
                 row.append(database[data["feature_id"]]["donor_anchor_id"])
                 row.append(database[data["feature_id"]]["acceptor_anchor_id"])
                 row.append(data["donor_DAI"])
@@ -118,33 +138,36 @@
                 row.append(data["delta_DAI_pvalue"])
             if feature_name=="exons":
                 row.append(data["test_PSI"])
                 row.append(data["control_PSI"])
                 row.append(data["delta_PSI"])
             if feature_name=="genes":
                 row += [float(data["logFC"]), data["F"], float(data["PValue"]), float(data["FDR"])]
+                row += [float(data["logFC"])* -np.log10(float(data["PValue"]))] # add pi value
+
             else:
                 row += [float(data["logFC"]), data["exon.F"], float(data["P.Value"]), float(data["FDR"])]
+                row += [float(data["logFC"])* -np.log10(float(data["P.Value"]))] # add pi value
             results_all.append(row)
             if float(data["FDR"])<=config.edgeR_FDR_thr:
                 results.append(row)
             r = f.readline()
         f.close()
         count += 1
         print("Processed", fname, "{a}/{b} ({pdone}% done)".format(a=count, b=len(rfiles), pdone="%.2f" % (count/len(rfiles)*100)))
 
     # sort by FDR
     results_all.sort(key = lambda el: el[-1])
     results.sort(key = lambda el: el[-1])
     headers = {}
-    headers["genes"] = ["result_id", "comparison", "compound", "rank", "feature_id", "chr", "strand", "feature_start", "feature_stop", "feature_len", "gene_id", "gene_name", "jbrowse_loc", "jbrowse_url", "sum_feature_test", "sum_feature_control", "test_pfi", "control_pfi", "delta_pfi", "logFC", "exon.F", "p_value", "fdr"]
-    headers["junctions"] = ["result_id", "comparison", "compound", "rank", "feature_id", "chr", "strand", "feature_start", "feature_stop", "feature_len", "UTR", "gene_id", "gene_name", "jbrowse_loc", "jbrowse_url", "sum_feature_test", "sum_feature_control", "test_pfi", "control_pfi", "delta_pfi", "annotated", "donor_anchor_id", "acceptor_anchor_id", "donor_DAI", "acceptor_DAI", "delta_DAI", "delta_DAI_pvalue", "logFC", "exon.F", "p_value", "fdr"]
-    headers["exons"] = ["result_id", "comparison", "compound", "rank", "feature_id", "chr", "strand", "feature_start", "feature_stop", "feature_len", "gene_id", "gene_name", "jbrowse_loc", "jbrowse_url", "sum_feature_test", "sum_feature_control", "test_pfi", "control_pfi", "delta_pfi", "test_PSI", "control_PSI", "delta_PSI", "logFC", "exon.F", "p_value", "fdr"]
-    headers["donor_anchors"] = ["result_id", "comparison", "compound", "rank", "feature_id", "chr", "strand", "feature_start", "feature_stop", "feature_len", "gene_id", "gene_name", "jbrowse_loc", "jbrowse_url", "sum_feature_test", "sum_feature_control", "test_pfi", "control_pfi", "delta_pfi", "logFC", "exon.F", "p_value", "fdr"]
-    headers["acceptor_anchors"] = ["result_id", "comparison", "compound", "rank", "feature_id", "chr", "strand", "feature_start", "feature_stop", "feature_len", "gene_id", "gene_name", "jbrowse_loc", "jbrowse_url", "sum_feature_test", "sum_feature_control", "test_pfi", "control_pfi", "delta_pfi", "logFC", "exon.F", "p_value", "fdr"]
+    headers["genes"] = ["result_id", "comparison", "compound", "rank", "feature_id", "chr", "strand", "feature_start", "feature_stop", "feature_len", "gene_id", "gene_name", "jbrowse_loc", "jbrowse_url", "sum_feature_test", "sum_feature_control", "test_pfi", "control_pfi", "delta_pfi", "logFC", "exon.F", "p_value", "fdr","pi_value"]
+    headers["junctions"] = ["result_id", "comparison", "compound", "rank", "feature_id", "chr", "strand", "feature_start", "feature_stop", "feature_len", "UTR", "gene_id", "gene_name", "jbrowse_loc", "jbrowse_url", "sum_feature_test", "sum_feature_control", "test_pfi", "control_pfi", "delta_pfi", "annotated", "donor_anchor_id", "acceptor_anchor_id", "donor_DAI", "acceptor_DAI", "delta_DAI", "delta_DAI_pvalue", "logFC", "exon.F", "p_value", "fdr","pi_value"]
+    headers["exons"] = ["result_id", "comparison", "compound", "rank", "feature_id", "chr", "strand", "feature_start", "feature_stop", "feature_len", "gene_id", "gene_name", "jbrowse_loc", "jbrowse_url", "sum_feature_test", "sum_feature_control", "test_pfi", "control_pfi", "delta_pfi", "test_PSI", "control_PSI", "delta_PSI", "logFC", "exon.F", "p_value", "fdr","pi_value"]
+    headers["donor_anchors"] = ["result_id", "comparison", "compound", "rank", "feature_id", "chr", "strand", "feature_start", "feature_stop", "feature_len", "gene_id", "gene_name", "jbrowse_loc", "jbrowse_url", "sum_feature_test", "sum_feature_control", "test_pfi", "control_pfi", "delta_pfi", "logFC", "exon.F", "p_value", "fdr","pi_value"]
+    headers["acceptor_anchors"] = ["result_id", "comparison", "compound", "rank", "feature_id", "chr", "strand", "feature_start", "feature_stop", "feature_len", "gene_id", "gene_name", "jbrowse_loc", "jbrowse_url", "sum_feature_test", "sum_feature_control", "test_pfi", "control_pfi", "delta_pfi", "logFC", "exon.F", "p_value", "fdr","pi_value"]
     f = open(f"results/results_edgeR_{feature_name}.tab", "wt")
     f.write("\t".join(headers[feature_name]) + "\n")
     f_all = open(f"results/results_edgeR_{feature_name}_all.tab", "wt")
     f_all.write("\t".join(headers[feature_name]) + "\n")
     if len(results_all)>0:
         assert(len(headers[feature_name])==len(results_all[0])+1) # header and data columns must match, +1 for result_id
     result_id = 1
```

### Comparing `splicekit-0.4.6/splicekit/folders.setup` & `splicekit-0.4.7/splicekit/folders.setup`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/judge/__init__.py` & `splicekit-0.4.7/splicekit/judge/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/splicecompare` & `splicekit-0.4.7/splicekit/splicecompare`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/splicekit` & `splicekit-0.4.7/splicekit/splicekit`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit/splicekit.config.template` & `splicekit-0.4.7/splicekit/splicekit.config.template`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.6/splicekit.egg-info/PKG-INFO` & `splicekit-0.4.7/splicekit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: splicekit
-Version: 0.4.6
+Version: 0.4.7
 Summary: splicekit: comprehensive toolkit for splicing analysis from short-read RNA-seq
 Home-page: https://github.com/bedapub/splicekit
 Author: Roche, PMDA Spliceosome team
 Author-email: gregor.rot@gmail.com
 Keywords: splicekit,splicing,transcriptomics,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
+## splicekit: a toolkit for splicing analysis from short-read RNA-seq
 
 A comprehensive platform for splicing analysis of RNA-seq short-read sequencing data. <b>splicekit</b> input are read alignments in BAM format (look at [datasets](datasets) for details on how to run examples).
 
 [What is splicekit?](#what_do)<br>
 [Installation](#initial_setup)<br>
 [Quick start](#quick_start)<br>
 [Software dependencies](#software_dep)<br>
```

### Comparing `splicekit-0.4.6/splicekit.egg-info/SOURCES.txt` & `splicekit-0.4.7/splicekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

