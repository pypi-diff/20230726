# Comparing `tmp/himut-1.0.3.tar.gz` & `tmp/himut-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "himut-1.0.3.tar", max compression
+gzip compressed data, was "himut-1.0.4.tar", max compression
```

## Comparing `himut-1.0.3.tar` & `himut-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1083 2022-08-16 10:27:29.953806 himut-1.0.3/LICENSE.rst
--rw-r--r--   0        0        0    16548 2023-07-25 06:50:06.813355 himut-1.0.3/README.md
--rw-r--r--   0        0        0     1794 2023-07-25 06:49:28.808092 himut-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       13 2022-12-26 01:47:01.932320 himut-1.0.3/src/himut/__init__.py
--rw-r--r--   0        0        0     6964 2023-05-01 21:16:48.649856 himut-1.0.3/src/himut/__main__.py
--rw-r--r--   0        0        0     8674 2023-07-05 11:23:05.684508 himut-1.0.3/src/himut/bamlib.py
--rw-r--r--   0        0        0    26185 2023-07-24 07:00:29.698271 himut-1.0.3/src/himut/caller.py
--rw-r--r--   0        0        0     5802 2023-01-13 14:27:47.919496 himut-1.0.3/src/himut/cslib.py
--rw-r--r--   0        0        0     5031 2023-06-27 11:24:04.480570 himut-1.0.3/src/himut/gtlib.py
--rw-r--r--   0        0        0     2902 2023-06-05 14:41:43.177400 himut-1.0.3/src/himut/haplib.py
--rw-r--r--   0        0        0    56142 2023-07-24 13:49:06.495540 himut-1.0.3/src/himut/mutlib.py
--rw-r--r--   0        0        0    19319 2023-04-06 13:41:47.554704 himut-1.0.3/src/himut/normcounts.py
--rw-r--r--   0        0        0    19090 2023-07-24 06:47:50.399492 himut-1.0.3/src/himut/parse_args.py
--rw-r--r--   0        0        0     9746 2023-07-14 06:33:49.445325 himut-1.0.3/src/himut/phaselib.py
--rw-r--r--   0        0        0        0 2022-08-16 10:27:29.957052 himut-1.0.3/src/himut/py.typed
--rw-r--r--   0        0        0     2531 2023-05-06 09:14:16.822447 himut-1.0.3/src/himut/reflib.py
--rw-r--r--   0        0        0     5200 2022-12-26 01:55:34.508267 himut-1.0.3/src/himut/somlib.py
--rw-r--r--   0        0        0    17735 2023-07-24 06:52:57.954939 himut-1.0.3/src/himut/util.py
--rw-r--r--   0        0        0    37909 2023-07-07 15:12:06.691326 himut-1.0.3/src/himut/vcflib.py
--rw-r--r--   0        0        0    17742 1970-01-01 00:00:00.000000 himut-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-08-16 10:27:29.953806 himut-1.0.4/LICENSE.rst
+-rw-r--r--   0        0        0    16487 2023-07-25 09:00:11.179479 himut-1.0.4/README.md
+-rw-r--r--   0        0        0     1794 2023-07-26 10:40:06.970509 himut-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       13 2022-12-26 01:47:01.932320 himut-1.0.4/src/himut/__init__.py
+-rw-r--r--   0        0        0     6964 2023-07-26 10:39:10.401341 himut-1.0.4/src/himut/__main__.py
+-rw-r--r--   0        0        0     8674 2023-07-05 11:23:05.684508 himut-1.0.4/src/himut/bamlib.py
+-rw-r--r--   0        0        0    26185 2023-07-24 07:00:29.698271 himut-1.0.4/src/himut/caller.py
+-rw-r--r--   0        0        0     5802 2023-01-13 14:27:47.919496 himut-1.0.4/src/himut/cslib.py
+-rw-r--r--   0        0        0     5031 2023-06-27 11:24:04.480570 himut-1.0.4/src/himut/gtlib.py
+-rw-r--r--   0        0        0     2902 2023-06-05 14:41:43.177400 himut-1.0.4/src/himut/haplib.py
+-rw-r--r--   0        0        0    56142 2023-07-24 13:49:06.495540 himut-1.0.4/src/himut/mutlib.py
+-rw-r--r--   0        0        0    19319 2023-04-06 13:41:47.554704 himut-1.0.4/src/himut/normcounts.py
+-rw-r--r--   0        0        0    19078 2023-07-26 10:38:46.558099 himut-1.0.4/src/himut/parse_args.py
+-rw-r--r--   0        0        0     9746 2023-07-14 06:33:49.445325 himut-1.0.4/src/himut/phaselib.py
+-rw-r--r--   0        0        0        0 2022-08-16 10:27:29.957052 himut-1.0.4/src/himut/py.typed
+-rw-r--r--   0        0        0     2531 2023-05-06 09:14:16.822447 himut-1.0.4/src/himut/reflib.py
+-rw-r--r--   0        0        0     5200 2022-12-26 01:55:34.508267 himut-1.0.4/src/himut/somlib.py
+-rw-r--r--   0        0        0    17735 2023-07-24 06:52:57.954939 himut-1.0.4/src/himut/util.py
+-rw-r--r--   0        0        0    37909 2023-07-07 15:12:06.691326 himut-1.0.4/src/himut/vcflib.py
+-rw-r--r--   0        0        0    17681 1970-01-01 00:00:00.000000 himut-1.0.4/PKG-INFO
```

### Comparing `himut-1.0.3/LICENSE.rst` & `himut-1.0.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `himut-1.0.3/README.md` & `himut-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 wget https://github.com/sjin09/himut/archive/refs/tags/v1.0.2.tar.gz
 tar -zxvf v1.0.3.tar.gz
 cd himut-1.0.3
 bash install.sh
 
 ## use miniamp2 and samtools to align, sort (and merge) PacBio CCS read alignments
 minimap2 "@RG\tSM:sample" -ax map-hifi --cs ref.fa pacbio.ccs.fastq.gz | samtools sort -o aln.sorted.bam # SM tag must be provided to retrieve sample ID
+samtools merge *.sorted.bam | samtools sort -o aln.mergeSorted.bam - ## if there are multiple BAM files, merge and sort the BAM files 
 samtools view -bh -F 0x900 aln.sorted.bam > aln.primary_alignments.sorted.bam # select primary alignments
-samtools index aln.primary_alignments.sorted.bam
-samtools merge *.primary_alignments.sorted.bam | samtools sort -o aln.primary_alignments.mergeSorted.bam - ## if there are multiple BAM files, merge and sort the BAM files
-samtools index aln.primary_alignments.mergeSorted.bam 
+samtools index aln.sorted.bam
+samtools index aln.primary_alignments.sorted.bam 
 
 ## germline mutation detection and haplotype phasing
 deepvariant.simg /opt/deepvariant/bin/run_deepvariant --model_type=PACBIO --ref ref.fa --reads=aln.primary_alignments.sorted.bam --output_vcf=germline.vcf ## use deepvariant to call germline mutations 
 bgzip -c germline.vcf > germline.vcf.bgz ## bgzip compress
 tabix -p vcf germline.vcf.bgz ## tabix index
 himut phase --bam aln.primary_alignments.sorted.bam --vcf germline.vcf.bgz -o germline.phased.vcf ## phsae
 bgzip -c germline.phased.vcf  > germline.phased.vcf.bgz ## bgzip compress
```

### Comparing `himut-1.0.3/pyproject.toml` & `himut-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "himut"
-version = "1.0.3"
+version = "1.0.4"
 description = "himut: single molecule somatic single-base substitution detection using PacBio CCS reads"
 authors = ["Sangjin Lee <sl17@sanger.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/sjin09/himut"
 repository = "https://github.com/sjin09/himut"
 classifiers = [
```

### Comparing `himut-1.0.3/src/himut/__main__.py` & `himut-1.0.4/src/himut/__main__.py`

 * *Files identical despite different names*

### Comparing `himut-1.0.3/src/himut/bamlib.py` & `himut-1.0.4/src/himut/bamlib.py`

 * *Files identical despite different names*

### Comparing `himut-1.0.3/src/himut/caller.py` & `himut-1.0.4/src/himut/caller.py`

 * *Files identical despite different names*

### Comparing `himut-1.0.3/src/himut/cslib.py` & `himut-1.0.4/src/himut/cslib.py`

 * *Files identical despite different names*

### Comparing `himut-1.0.3/src/himut/gtlib.py` & `himut-1.0.4/src/himut/gtlib.py`

 * *Files identical despite different names*

### Comparing `himut-1.0.3/src/himut/haplib.py` & `himut-1.0.4/src/himut/haplib.py`

 * *Files identical despite different names*

### Comparing `himut-1.0.3/src/himut/mutlib.py` & `himut-1.0.4/src/himut/mutlib.py`

 * *Files identical despite different names*

### Comparing `himut-1.0.3/src/himut/normcounts.py` & `himut-1.0.4/src/himut/normcounts.py`

 * *Files identical despite different names*

### Comparing `himut-1.0.3/src/himut/parse_args.py` & `himut-1.0.4/src/himut/parse_args.py`

 * *Files 0% similar despite different names*

```diff
@@ -679,20 +679,20 @@
     )
     parser_normcounts.add_argument(
         "--non_human_sample",
         required=False,
         action="store_true",
         help="human or non_human_sample",
     )
-    # parser_normcounts.add_argument(
-    #     "--reference_sample",
-    #     required=False,
-    #     action="store_true",
-    #     help="reads from the sample has been used to create the reference genome",
-    # )
+    parser_normcounts.add_argument(
+        "--reference_sample",
+        required=False,
+        action="store_true",
+        help="reads from the sample has been used to create the reference genome",
+    )
     parser_normcounts.add_argument(
         "-o",
         "--output",
         type=str,
         required=True,
         help="file to return normalised SBS96 counts",
     )
```

### Comparing `himut-1.0.3/src/himut/phaselib.py` & `himut-1.0.4/src/himut/phaselib.py`

 * *Files identical despite different names*

### Comparing `himut-1.0.3/src/himut/reflib.py` & `himut-1.0.4/src/himut/reflib.py`

 * *Files identical despite different names*

### Comparing `himut-1.0.3/src/himut/somlib.py` & `himut-1.0.4/src/himut/somlib.py`

 * *Files identical despite different names*

### Comparing `himut-1.0.3/src/himut/util.py` & `himut-1.0.4/src/himut/util.py`

 * *Files identical despite different names*

### Comparing `himut-1.0.3/src/himut/vcflib.py` & `himut-1.0.4/src/himut/vcflib.py`

 * *Files identical despite different names*

### Comparing `himut-1.0.3/PKG-INFO` & `himut-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: himut
-Version: 1.0.3
+Version: 1.0.4
 Summary: himut: single molecule somatic single-base substitution detection using PacBio CCS reads
 Home-page: https://github.com/sjin09/himut
 License: MIT
 Author: Sangjin Lee
 Author-email: sl17@sanger.ac.uk
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -38,18 +38,18 @@
 wget https://github.com/sjin09/himut/archive/refs/tags/v1.0.2.tar.gz
 tar -zxvf v1.0.3.tar.gz
 cd himut-1.0.3
 bash install.sh
 
 ## use miniamp2 and samtools to align, sort (and merge) PacBio CCS read alignments
 minimap2 "@RG\tSM:sample" -ax map-hifi --cs ref.fa pacbio.ccs.fastq.gz | samtools sort -o aln.sorted.bam # SM tag must be provided to retrieve sample ID
+samtools merge *.sorted.bam | samtools sort -o aln.mergeSorted.bam - ## if there are multiple BAM files, merge and sort the BAM files 
 samtools view -bh -F 0x900 aln.sorted.bam > aln.primary_alignments.sorted.bam # select primary alignments
-samtools index aln.primary_alignments.sorted.bam
-samtools merge *.primary_alignments.sorted.bam | samtools sort -o aln.primary_alignments.mergeSorted.bam - ## if there are multiple BAM files, merge and sort the BAM files
-samtools index aln.primary_alignments.mergeSorted.bam 
+samtools index aln.sorted.bam
+samtools index aln.primary_alignments.sorted.bam 
 
 ## germline mutation detection and haplotype phasing
 deepvariant.simg /opt/deepvariant/bin/run_deepvariant --model_type=PACBIO --ref ref.fa --reads=aln.primary_alignments.sorted.bam --output_vcf=germline.vcf ## use deepvariant to call germline mutations 
 bgzip -c germline.vcf > germline.vcf.bgz ## bgzip compress
 tabix -p vcf germline.vcf.bgz ## tabix index
 himut phase --bam aln.primary_alignments.sorted.bam --vcf germline.vcf.bgz -o germline.phased.vcf ## phsae
 bgzip -c germline.phased.vcf  > germline.phased.vcf.bgz ## bgzip compress
```

