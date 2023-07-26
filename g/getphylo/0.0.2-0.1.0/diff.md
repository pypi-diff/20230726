# Comparing `tmp/getphylo-0.0.2.tar.gz` & `tmp/getphylo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/getphylo-0.0.2.tar", last modified: Mon Apr 17 14:47:42 2023, max compression
+gzip compressed data, was "getphylo-0.1.0.tar", last modified: Wed Jul 26 14:52:12 2023, max compression
```

## Comparing `getphylo-0.0.2.tar` & `getphylo-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 thoboo    (1000) thoboo    (1000)        0 2023-04-17 14:47:42.000000 getphylo-0.0.2/
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     3595 2023-04-17 14:47:42.000000 getphylo-0.0.2/PKG-INFO
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     2605 2023-03-28 11:14:23.000000 getphylo-0.0.2/README.md
-drwxr-xr-x   0 thoboo    (1000) thoboo    (1000)        0 2023-04-17 14:47:42.000000 getphylo-0.0.2/getphylo/
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)       46 2023-03-13 14:27:01.000000 getphylo-0.0.2/getphylo/__init__.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)      565 2023-04-14 12:17:34.000000 getphylo-0.0.2/getphylo/__main__.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     8497 2023-04-17 14:16:15.000000 getphylo-0.0.2/getphylo/align.py
-drwxr-xr-x   0 thoboo    (1000) thoboo    (1000)        0 2023-04-17 14:47:42.000000 getphylo-0.0.2/getphylo/ext/
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)       57 2023-03-28 11:14:23.000000 getphylo-0.0.2/getphylo/ext/__init__.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     1729 2023-04-14 12:17:34.000000 getphylo-0.0.2/getphylo/ext/diamond.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)      584 2023-04-14 12:17:34.000000 getphylo-0.0.2/getphylo/ext/fasttree.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)      602 2023-04-14 12:17:34.000000 getphylo-0.0.2/getphylo/ext/muscle.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     6083 2023-04-17 14:42:21.000000 getphylo-0.0.2/getphylo/extract.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     4039 2023-04-17 14:44:09.000000 getphylo-0.0.2/getphylo/main.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     5705 2023-04-14 12:17:34.000000 getphylo-0.0.2/getphylo/parser.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)    12460 2023-04-17 14:25:38.000000 getphylo-0.0.2/getphylo/screen.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     1218 2023-04-17 14:14:39.000000 getphylo-0.0.2/getphylo/trees.py
-drwxr-xr-x   0 thoboo    (1000) thoboo    (1000)        0 2023-04-17 14:47:42.000000 getphylo-0.0.2/getphylo/utils/
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)       47 2023-03-28 11:14:23.000000 getphylo-0.0.2/getphylo/utils/__init__.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)      439 2023-04-14 12:17:34.000000 getphylo-0.0.2/getphylo/utils/checkpoint.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     1370 2023-04-14 12:17:34.000000 getphylo-0.0.2/getphylo/utils/errors.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     5461 2023-04-17 13:29:57.000000 getphylo-0.0.2/getphylo/utils/io.py
-drwxr-xr-x   0 thoboo    (1000) thoboo    (1000)        0 2023-04-17 14:47:42.000000 getphylo-0.0.2/getphylo.egg-info/
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     3595 2023-04-17 14:47:42.000000 getphylo-0.0.2/getphylo.egg-info/PKG-INFO
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)      564 2023-04-17 14:47:42.000000 getphylo-0.0.2/getphylo.egg-info/SOURCES.txt
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)        1 2023-04-17 14:47:42.000000 getphylo-0.0.2/getphylo.egg-info/dependency_links.txt
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)       59 2023-04-17 14:47:42.000000 getphylo-0.0.2/getphylo.egg-info/entry_points.txt
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)        4 2023-04-17 14:47:42.000000 getphylo-0.0.2/getphylo.egg-info/requires.txt
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)        9 2023-04-17 14:47:42.000000 getphylo-0.0.2/getphylo.egg-info/top_level.txt
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)       38 2023-04-17 14:47:42.000000 getphylo-0.0.2/setup.cfg
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)      717 2023-04-17 14:47:29.000000 getphylo-0.0.2/setup.py
+drwxr-xr-x   0 thoboo    (1000) thoboo    (1000)        0 2023-07-26 14:52:12.217290 getphylo-0.1.0/
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     2621 2023-07-26 14:52:12.217290 getphylo-0.1.0/PKG-INFO
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     1953 2023-07-26 13:13:37.000000 getphylo-0.1.0/README.md
+drwxr-xr-x   0 thoboo    (1000) thoboo    (1000)        0 2023-07-26 14:52:12.217290 getphylo-0.1.0/getphylo/
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)       46 2023-07-26 13:13:37.000000 getphylo-0.1.0/getphylo/__init__.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)      565 2023-07-26 13:13:37.000000 getphylo-0.1.0/getphylo/__main__.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     8499 2023-07-26 14:47:57.000000 getphylo-0.1.0/getphylo/align.py
+drwxr-xr-x   0 thoboo    (1000) thoboo    (1000)        0 2023-07-26 14:52:12.217290 getphylo-0.1.0/getphylo/ext/
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)       57 2023-07-26 13:13:37.000000 getphylo-0.1.0/getphylo/ext/__init__.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     1729 2023-07-26 13:13:37.000000 getphylo-0.1.0/getphylo/ext/diamond.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)      584 2023-07-26 13:13:37.000000 getphylo-0.1.0/getphylo/ext/fasttree.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)      602 2023-07-26 13:13:37.000000 getphylo-0.1.0/getphylo/ext/muscle.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     6247 2023-07-26 14:34:53.000000 getphylo-0.1.0/getphylo/extract.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     4039 2023-07-26 13:15:40.000000 getphylo-0.1.0/getphylo/main.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     5665 2023-07-26 13:13:37.000000 getphylo-0.1.0/getphylo/parser.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)    13220 2023-07-26 13:59:37.000000 getphylo-0.1.0/getphylo/screen.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     1218 2023-07-26 13:13:37.000000 getphylo-0.1.0/getphylo/trees.py
+drwxr-xr-x   0 thoboo    (1000) thoboo    (1000)        0 2023-07-26 14:52:12.217290 getphylo-0.1.0/getphylo/utils/
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)       47 2023-07-26 13:13:37.000000 getphylo-0.1.0/getphylo/utils/__init__.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)      439 2023-07-26 13:13:37.000000 getphylo-0.1.0/getphylo/utils/checkpoint.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     1370 2023-07-26 13:29:13.000000 getphylo-0.1.0/getphylo/utils/errors.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     5479 2023-07-26 13:36:43.000000 getphylo-0.1.0/getphylo/utils/io.py
+drwxr-xr-x   0 thoboo    (1000) thoboo    (1000)        0 2023-07-26 14:52:12.217290 getphylo-0.1.0/getphylo.egg-info/
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     2621 2023-07-26 14:52:12.000000 getphylo-0.1.0/getphylo.egg-info/PKG-INFO
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)      564 2023-07-26 14:52:12.000000 getphylo-0.1.0/getphylo.egg-info/SOURCES.txt
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)        1 2023-07-26 14:52:12.000000 getphylo-0.1.0/getphylo.egg-info/dependency_links.txt
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)       59 2023-07-26 14:52:12.000000 getphylo-0.1.0/getphylo.egg-info/entry_points.txt
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)        4 2023-07-26 14:52:12.000000 getphylo-0.1.0/getphylo.egg-info/requires.txt
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)        9 2023-07-26 14:52:12.000000 getphylo-0.1.0/getphylo.egg-info/top_level.txt
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)       38 2023-07-26 14:52:12.217290 getphylo-0.1.0/setup.cfg
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)      717 2023-07-26 13:15:00.000000 getphylo-0.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `getphylo-0.0.2/getphylo/__main__.py` & `getphylo-0.1.0/getphylo/__main__.py`

 * *Files identical despite different names*

### Comparing `getphylo-0.0.2/getphylo/align.py` & `getphylo-0.1.0/getphylo/align.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,27 +120,29 @@
         if seq_flag and taxon_name not in line:
             extracted_alignment.extend(line[:-1])
     extracted_alignment_string = ''.join(extracted_alignment)
     return extracted_alignment_string
 
 def format_partition_data(partition_data: List) -> List:
     '''
-    Takes the partition data [locus, locus_length] and reformats it as a partition file (e.g. p1 = 1-50, p2 = 51-110)
+    Takes the partition data [locus, locus_length] and reformats it as a partition file 
+    (e.g. p1 = 1-50, p2 = 51-110)
         Arguments:
             partition_data: a list of [locus, locus_length] lists
         Returns:
             partition_lines: list of lines in the partition format
     '''
+    model = 'WAG'
     partition_lines = []
     partition_start = 1
     for partition in partition_data:
         locus, length = partition[0], partition[1]
         locus = os.path.splitext(os.path.basename(locus))[0]
         partition_end = partition_start + length - 1
-        partition_lines.append('%s = %s-%s' % (locus, partition_start, partition_end))
+        partition_lines.append('%s, %s = %s-%s' % (model, locus, partition_start, partition_end))
         partition_start += length
     return partition_lines
 
 def make_combined_alignment(gbks: List, output: str) -> None:
     '''
     Create a combined alignment from single locus alignments
         Arguments:
@@ -151,43 +153,45 @@
     '''
     combined_alignment_path = os.path.join(output, 'aligned_fasta/combined_alignment.fasta')
     partition_path = os.path.join(output, 'partition.txt')
     if os.path.exists(combined_alignment_path):
         logging.error(
             'ALERT: aligned_fasta/combined_alignment.fasta already exists. Exiting!'
             )
-        raise FileAlreadyExistsError('%s alread exists.' % combined_alignemnt_path)
-    else:
-        combined_alignment = []
-        partition_data = []
-        taxa = glob.glob(gbks)
-        assert taxa, gbks
-        loci = glob.glob(os.path.join(output, 'aligned_fasta/*.fasta'))
-        for taxon in taxa:
-            taxon_name = os.path.splitext(os.path.basename(taxon))[0]
-            sequence_data = []
-            for locus in loci:
-                alignment = io.read_file(locus)
-                locus_length = get_locus_length(alignment)
+        raise FileAlreadyExistsError('%s alread exists.' % combined_alignment_path)
+    combined_alignment = []
+    partition_data = []
+    taxa = glob.glob(gbks)
+    assert taxa, gbks
+    loci = glob.glob(os.path.join(output, 'aligned_fasta/*.fasta'))
+    first_taxa = True
+    for taxon in taxa:
+        taxon_name = os.path.splitext(os.path.basename(taxon))[0]
+        sequence_data = []
+        for locus in loci:
+            alignment = io.read_file(locus)
+            locus_length = get_locus_length(alignment)
+            if first_taxa is True:
                 partition_data.append([locus, locus_length])
-                locus_alignment = get_locus_alignment(alignment, taxon_name)
-                if len(locus_alignment) == locus_length:
-                    sequence_data.append(locus_alignment)
-                else:
-                    sequence_data.append('X' * locus_length)
-            sequence_string = ''.join(sequence_data)
-            assert sequence_data
-            if sequence_string.count('X') == len(sequence_string):
-                logging.error('[ALERT]: %s has no sequence data and has been removed.', taxon_name)
+            locus_alignment = get_locus_alignment(alignment, taxon_name)
+            if len(locus_alignment) == locus_length:
+                sequence_data.append(locus_alignment)
             else:
-                combined_alignment.append(f'>{taxon_name}')
-                combined_alignment.append(sequence_string)
-        partition_data = format_partition_data(partition_data)  
-        io.write_to_file(combined_alignment_path, combined_alignment)
-        io.write_to_file(partition_path, partition_data)
+                sequence_data.append('?' * locus_length)
+        sequence_string = ''.join(sequence_data)
+        assert sequence_data
+        if sequence_string.count('?') == len(sequence_string):
+            logging.error('[ALERT]: %s has no sequence data and has been removed.', taxon_name)
+        else:
+            combined_alignment.append(f'>{taxon_name}')
+            combined_alignment.append(sequence_string)
+        first_taxa = False
+    partition_data = format_partition_data(partition_data)
+    io.write_to_file(combined_alignment_path, combined_alignment)
+    io.write_to_file(partition_path, partition_data)
 
 def make_alignments(checkpoint: Checkpoint, output: str, loci: List, gbks: List, cpus: int) -> None:
     '''
     Main routine for align.
         Arguments:
             checkpoint: checkpoint defined by the user
             output: path to the output directory
```

### Comparing `getphylo-0.0.2/getphylo/ext/diamond.py` & `getphylo-0.1.0/getphylo/ext/diamond.py`

 * *Files identical despite different names*

### Comparing `getphylo-0.0.2/getphylo/ext/fasttree.py` & `getphylo-0.1.0/getphylo/ext/fasttree.py`

 * *Files identical despite different names*

### Comparing `getphylo-0.0.2/getphylo/ext/muscle.py` & `getphylo-0.1.0/getphylo/ext/muscle.py`

 * *Files identical despite different names*

### Comparing `getphylo-0.0.2/getphylo/extract.py` & `getphylo-0.1.0/getphylo/extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 '''
 Build fasta and diamond databases from genbank files
 
 Functions:
-build_diamond_databases(output:str) -> None:
+build_diamond_databases(output:str) -> None
 extract_cdses(
     gbks: str, output: str, tag_label: str, ignore_bad_annotations: bool, ignore_bad_records: bool
-    ) -> None:
+    ) -> None
 get_cds_from_genbank(
-    filename: str, output: str, tag_label: str, ignore_bad_annotations: bool
-    ) -> None:
+    filename: str, output: str, tag_label: str, ignore_bad_annotations: bool,
+    ignore_bad_records: bool) -> None
 extract_data(
     checkpoint: Checkpoint, output: str, gbks: str, tag_label: str,
     ignore_bad_annotations: bool, ignore_bad_records: bool
-    ) -> None:
+    ) -> None
 '''
 import logging
 import os
 import glob
 from getphylo.ext import diamond
 from getphylo.utils import io
 from getphylo.utils.checkpoint import Checkpoint
@@ -36,15 +36,15 @@
     fasta_files_path = os.path.join(output, 'fasta/*.fasta')
     args_list = []
     for filename in glob.glob(fasta_files_path):
         dmnd_database = os.path.basename(io.change_extension(filename, "dmnd"))
         dmnd_database = os.path.join(dmnd_folder, dmnd_database)
         args = [filename, dmnd_database]
         args_list.append(args)
-    io.run_in_parallel(diamond.make_diamond_database, args_list, cpus) 
+    io.run_in_parallel(diamond.make_diamond_database, args_list, cpus)
 
 def extract_cdses(
         gbks: str, output: str, tag_label: str,
         ignore_bad_annotations: bool, ignore_bad_records: bool, cpus: int
     ) -> None:
     '''
     Produce a fasta file from each genbank provided
@@ -54,27 +54,29 @@
             tag_args:
             cpus: number of cpus available
         Returns:
             None
     '''
     io.make_folder(os.path.join(output, 'fasta'))
     filenames = glob.glob(gbks)
-    args_list = [[filename, output, tag_label, ignore_bad_annotations] for filename in filenames]
+    args_list = [[
+        filename, output, tag_label, ignore_bad_annotations, ignore_bad_records
+        ] for filename in filenames]
     try:
         io.run_in_parallel(get_cds_from_genbank, args_list, cpus)
     except BadAnnotationError:
         raise BadAnnotationError(
-            'Some files were not parsed correctly, check the logging file for more information.'
+           'Some files were not parsed correctly, check the logging file for more information.'
             'If you want to skip these files,'
             'rerun the analysis with the --ignore-bad-records flag.'
             )
 
 def get_cds_from_genbank(
-        filename: str, output: str, tag_label: str, ignore_bad_annotations: bool
-    ) -> None:
+        filename: str, output: str, tag_label: str, ignore_bad_annotations: bool,
+    ignore_bad_records: bool) -> None:
     '''
     Extract CDS translations from genbank files into ./fasta/*.fasta
         Arguments:
             filename: the name of the genbank file being read
             output: path to the output folder
             tag_label: the string defining the tag label (e.g. 'locus_tag')
             ignore_bad_annotations:
@@ -106,20 +108,22 @@
                             raise BadAnnotationError(
                                 f'Some features are missing the {tag_label} annotations.'
                                 'Ensure the genbank file is correctly annotated or use'
                                 '--ignore-bad-annotations flag.'
                             )
                     else:
                         warning_flag = True
-            if warning_flag == True:
+            if warning_flag is True:
                 logging.warning('%s has missing translations!', record.id)
     except ValueError as error:
-        raise BadRecordError(error)
+        if not ignore_bad_records:
+            raise BadRecordError(error)
     if not lines:
-        raise BadAnnotationError(f'No CDS Features in {filename}')
+        if not ignore_bad_annotations:
+            raise BadAnnotationError(f'No CDS Features in {filename}')
     filename = io.change_extension(os.path.basename(filename), "fasta")
     filename = os.path.join(output, 'fasta', filename)
     io.write_to_file(filename, lines)
 
 def extract_data(
         checkpoint: Checkpoint, output: str, gbks: str, tag_label: str,
         ignore_bad_annotations: bool, ignore_bad_records: bool, cpus: int
```

### Comparing `getphylo-0.0.2/getphylo/main.py` & `getphylo-0.1.0/getphylo/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         Returns: None'''
     logging_level = logging.DEBUG
     logging.basicConfig(
         #filename='getphylo.log',
         level=logging_level,
         format='[%(asctime)s] %(levelname)-10s: %(message)s',
         datefmt='%H:%M:%S')
-    logging.info("Running getphylo version 0.0.2.")
+    logging.info("Running getphylo version 0.1.0.")
 
 def check_seed(checkpoint: Checkpoint, gbk_search_string: str) -> str:
     '''Set a seed for a new analysis and raise an error if continuing an old analysis.
         Arguments:
             checkpoint: the checkpoint supplied by the user
             gbk_search_string: the string used to filter the glob (e.g. '*.gbk')
         Returns:
```

### Comparing `getphylo-0.0.2/getphylo/parser.py` & `getphylo-0.1.0/getphylo/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,16 +22,15 @@
         """,
         epilog="Written by Dr. Thom Booth, 2022.",
         formatter_class=RawTextHelpFormatter
         )
     parser.add_argument(
         '-b',
         '--build-all',
-        default=-False,
-        type=bool,
+        action='store_true',
         help=(
             'build phylogenetic trees for all loci, not just concatenated alignment '
             '(default: %(default)s)'
         )
         )
     parser.add_argument(
         '-cp',
@@ -81,23 +80,21 @@
         default="*.gbk",
         type=str,
         help='string indicating the genbank files to use in the phylogeny (default: %(default)s)'
         )
     parser.add_argument(
         '-ia',
         '--ignore-bad-annotations',
-        default=False,
-        type=bool,
+        action='store_true',
         help='ignore missing annotations - NOT RECCOMMENDED (default: %(default)s)'
         )
     parser.add_argument(
         '-ir',
         '--ignore-bad-records',
-        default=False,
-        type=bool,
+        action='store_true',
         help='ignore poorly formated records - NOT RECCOMMENDED (default: %(default)s)'
         )
     parser.add_argument(
         '-l',
         '--logging',
         default='ERROR',
         choices=list(logging._nameToLevel.keys()),
```

### Comparing `getphylo-0.0.2/getphylo/screen.py` & `getphylo-0.1.0/getphylo/screen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,33 @@
 '''
 Screen fasta files and blast databases for singletons and extract sequences
 
 Functions:
-get_target_proteins(checkpoint: Checkpoint, output: str, seed: str, thresholds: List) -> None
+    get_unique_hits_from_tsv(file: str) -> List
+    get_seed_paths(seed: str, output: str) -> Tuple[str, str, str]
+    get_singletons_from_seed(seed, output, thresholds, random_seed_number)
+    get_loci_from_file(file: str) -> List
+    search_candidates(output: str, cpus: int) -> None
+    score_locus(locus: str, files: List) -> Tuple[int, bool, List]
+    process_final_loci(final_loci: List, minimum_loci: int, output: str) -> None
+    do_thresholding(
+        target_loci: List, presence_threshold: float, maximum_loci: int, output: str
+    ) -> List
+    threshold_loci(target_loci: List, thresholds: List, output: str) -> List
+    write_pa_table(pa_table: List, loci: List, output: str) -> None
+    get_target_proteins(
+        checkpoint: Checkpoint, output: str, seed: str, thresholds: List,
+        cpus: int, random_seed_number: int
+    ) -> None
 '''
 import os
 import glob
 import logging
 from collections import Counter
-import random 
+import random
 from typing import List, Tuple
 
 from getphylo.ext import diamond
 from getphylo.utils import io
 from getphylo.utils.checkpoint import Checkpoint
 from getphylo.utils.errors import(
     FileAlreadyExistsError,
```

### Comparing `getphylo-0.0.2/getphylo/trees.py` & `getphylo-0.1.0/getphylo/trees.py`

 * *Files identical despite different names*

### Comparing `getphylo-0.0.2/getphylo/utils/errors.py` & `getphylo-0.1.0/getphylo/utils/errors.py`

 * *Files identical despite different names*

### Comparing `getphylo-0.0.2/getphylo/utils/io.py` & `getphylo-0.1.0/getphylo/utils/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,27 +84,26 @@
         Returns:
             None
     '''
     if os.path.exists(name):
         raise FolderExistsError(
             f'ALERT: The directory {name} already exists.'
             )
-    else:
-        os.mkdir(name)
+    os.mkdir(name)
 
 def read_file(filename: str) -> List[str]:
     '''
     Return a files contents as a list of lines
         Arguments:
             filename: The file to be read
         Returns:
             _file.readlines(): list of strings for each line of the file
     '''
-    _file = open(filename, "r")
-    return _file.readlines()
+    with open(filename) as _file:
+        return _file.readlines()
 
 def read_tsv(filename: str) -> List[str]:
     '''
     Read lines from a .tsv file.
         Arguments:
             filename: the path to the file to be read
         Returns:
@@ -123,19 +122,19 @@
         Aruments:
             command: string containing the command for the terminal
         Returns:
             process: the process being run
     '''
     command = command.split(" ")
     logging.debug(command)
-    process = subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
-    process.communicate()
-    if process.returncode != 0:
-        raise RuntimeError('Failed to run: ' + str(command))
-    return process
+    with subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT) as process:
+        process.communicate()
+        if process.returncode != 0:
+            raise RuntimeError('Failed to run: ' + str(command))
+        return process
 
 def run_in_parallel(function: Callable, args_list: Iterable[List], cpus: int) -> List:
     '''
     Run a given function on avaliable cpus. If only 1 cpu is available, run as normal.
         Arguments:
             function: the function to be called
             args_list: Iterable of lists containing the arguments for each call of the function
@@ -146,26 +145,26 @@
     if cpus <= 1:
         return_value = [function(*args) for args in args_list]
     else:
         for item in args_list:
             try:
                 iter(item)
             except TypeError as error:
-                raise GetphyloError(error)
+                raise GetphyloError from error
         with multiprocessing.Pool(cpus) as pool:
             results = pool.starmap_async(function, args_list)
-            return_value = [result for result in results.get()]
+            return_value = results.get()
     return return_value
 
 def write_to_file(filename: str, write_lines: List[str]) -> None:
     '''
     Write a list line by line into a new file.
         Arguments:
             filename: path to the new file being written
             write_lines: list of strings to be written to the file
         Returns:
             None
     '''
-    file = open(filename, "a")
-    for line in write_lines:
-        file.write(line + '\n')
-    file.close()
+    with open(filename, "a") as _file:
+        for line in write_lines:
+            _file.write(line + '\n')
+        _file.close()
```

### Comparing `getphylo-0.0.2/getphylo.egg-info/SOURCES.txt` & `getphylo-0.1.0/getphylo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `getphylo-0.0.2/setup.py` & `getphylo-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setup(
     name="getphylo",
-    version="0.0.2",
+    version="0.1.0",
     author="Thomas J. Booth",
     author_email="thoboo@biosustain.dtu.dk",
     packages=find_packages(),
     description="a python package for automated generation of heuristic phylogenetic trees from genbank files",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/DrBoothTJ/getphylo",
```

