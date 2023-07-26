# Comparing `tmp/twinstop-0.0.2.tar.gz` & `tmp/twinstop-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinstop-0.0.2.tar", last modified: Wed Jul 26 09:00:54 2023, max compression
+gzip compressed data, was "twinstop-0.0.3.tar", last modified: Wed Jul 26 10:38:39 2023, max compression
```

## Comparing `twinstop-0.0.2.tar` & `twinstop-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 09:00:54.426179 twinstop-0.0.2/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-07-25 10:35:28.000000 twinstop-0.0.2/LICENSE
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-26 09:00:54.426179 twinstop-0.0.2/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      132 2023-07-25 10:35:28.000000 twinstop-0.0.2/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 twinstop-0.0.2/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1057 2023-07-26 09:00:54.426179 twinstop-0.0.2/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 twinstop-0.0.2/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 09:00:54.422179 twinstop-0.0.2/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 09:00:54.426179 twinstop-0.0.2/src/twinstop/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       93 2023-07-25 10:19:10.000000 twinstop-0.0.2/src/twinstop/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-07-26 08:55:34.000000 twinstop-0.0.2/src/twinstop/_version.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4384 2023-07-25 13:13:21.000000 twinstop-0.0.2/src/twinstop/block_selection.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 09:00:54.426179 twinstop-0.0.2/src/twinstop/data_files/
--rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     2003 2023-07-25 13:30:48.000000 twinstop-0.0.2/src/twinstop/data_files/Matrix_BLOSUM62sel.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.0.2/src/twinstop/data_files/logistic_regression_model.def.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.0.2/src/twinstop/data_files/logistic_regression_model.pre.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1462 2023-07-25 14:46:08.000000 twinstop-0.0.2/src/twinstop/data_files/logistic_regression_model.sen.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4142 2023-07-25 14:46:08.000000 twinstop-0.0.2/src/twinstop/data_files/scaler.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   111754 2023-07-25 14:16:44.000000 twinstop-0.0.2/src/twinstop/denovo_selenoproteins_h3.bkp.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   111812 2023-07-25 14:44:05.000000 twinstop-0.0.2/src/twinstop/denovo_selenoproteins_h3.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6979 2023-07-25 13:13:21.000000 twinstop-0.0.2/src/twinstop/test_alignment_methods.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 09:00:54.426179 twinstop-0.0.2/src/twinstop.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-26 09:00:54.000000 twinstop-0.0.2/src/twinstop.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      693 2023-07-26 09:00:54.000000 twinstop-0.0.2/src/twinstop.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-07-26 09:00:54.000000 twinstop-0.0.2/src/twinstop.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      209 2023-07-26 09:00:54.000000 twinstop-0.0.2/src/twinstop.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        9 2023-07-26 09:00:54.000000 twinstop-0.0.2/src/twinstop.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 10:38:39.975844 twinstop-0.0.3/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-07-25 10:35:28.000000 twinstop-0.0.3/LICENSE
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-26 10:38:39.975844 twinstop-0.0.3/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      132 2023-07-25 10:35:28.000000 twinstop-0.0.3/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 twinstop-0.0.3/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1065 2023-07-26 10:38:39.975844 twinstop-0.0.3/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 twinstop-0.0.3/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 10:38:39.975844 twinstop-0.0.3/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 10:38:39.975844 twinstop-0.0.3/src/twinstop/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       93 2023-07-25 10:19:10.000000 twinstop-0.0.3/src/twinstop/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-07-26 10:37:53.000000 twinstop-0.0.3/src/twinstop/_version.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4156 2023-07-26 09:06:02.000000 twinstop-0.0.3/src/twinstop/block_selection.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 10:38:39.975844 twinstop-0.0.3/src/twinstop/data_files/
+-rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     2003 2023-07-25 13:30:48.000000 twinstop-0.0.3/src/twinstop/data_files/Matrix_BLOSUM62sel.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.0.3/src/twinstop/data_files/logistic_regression_model.def.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.0.3/src/twinstop/data_files/logistic_regression_model.pre.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1462 2023-07-25 14:46:08.000000 twinstop-0.0.3/src/twinstop/data_files/logistic_regression_model.sen.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4142 2023-07-25 14:46:08.000000 twinstop-0.0.3/src/twinstop/data_files/scaler.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   111812 2023-07-25 14:44:05.000000 twinstop-0.0.3/src/twinstop/denovo_selenoproteins_h3.bkp2.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   112541 2023-07-26 10:36:55.000000 twinstop-0.0.3/src/twinstop/denovo_selenoproteins_h3.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6979 2023-07-25 13:13:21.000000 twinstop-0.0.3/src/twinstop/test_alignment_methods.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 10:38:39.975844 twinstop-0.0.3/src/twinstop.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-26 10:38:39.000000 twinstop-0.0.3/src/twinstop.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      694 2023-07-26 10:38:39.000000 twinstop-0.0.3/src/twinstop.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-07-26 10:38:39.000000 twinstop-0.0.3/src/twinstop.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      217 2023-07-26 10:38:39.000000 twinstop-0.0.3/src/twinstop.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        9 2023-07-26 10:38:39.000000 twinstop-0.0.3/src/twinstop.egg-info/top_level.txt
```

### Comparing `twinstop-0.0.2/LICENSE` & `twinstop-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.2/PKG-INFO` & `twinstop-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinstop
-Version: 0.0.2
+Version: 0.0.3
 Summary: twinstop identifies selenoproteins in close related transcriptomes
 Home-page: https://github.com/marco-mariotti/twinstop
 Author: Marco Mariotti and Sergio Sanchez Moragues
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `twinstop-0.0.2/setup.cfg` & `twinstop-0.0.3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 	= src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	biopython >= 1.78, <=1.81
 	easyterm >= 1.0.0
 	easybioinfo >= 0.2.1
-	extend_orfs >= 0.0.27
+	extend-orfs-pyranges >= 0.1.1
 	file-chunk-iterators >= 0.0.1
 	pyranges >= 0.0.120
 	pandas >= 1.3.5
 	pyfaidx >= 0.7.2
 	multiprocess >= 0.70.14
 	numpy >= 1.21.5
 	scikit-learn >= 1.3.0
```

### Comparing `twinstop-0.0.2/src/twinstop/block_selection.py` & `twinstop-0.0.3/src/twinstop/block_selection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,124 +1,118 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon May  2 10:38:33 2022
-
-@author: Toño
-"""
-
+# -*- coding: utf-8 -*-
+
 import os
 twinstop_libpath=os.path.dirname(os.path.realpath(__file__)) +"/data_files/"
-def block_dict(query_seq, subj_seq, dictionary):
-    '''
-    Takes two protein sequences (one from the query and the other from the subject), 
-    divides them into blocks according to the stops '*' present in both and then 
-    saves in a list of dictionaries the start, end and score (matrix Blosum62)
-    of each block. Afterward, the block with better score is selected and the
-    data of the score, start, end and sequence from both query and subject is
-    updated in the general dataframe.
-
-    Parameters
-    ----------
-    query_seq : String
-        Aligned protein sequence of the query
-    subj_seq : String
-        Aligned protein sequence of the subject
-    dictionary : Dictionary of tuples
-        Matrix Blosum62 values
-
-    Returns
-    -------
-    best_block[0] : Dictionary with the 'Start', 'End' and 'Score' values of the
-    best scored fragment of each alignment.
-    '''
-
-    list_stops = list() # create a list to save stops index
-
-    for index, x in enumerate(query_seq):
-        # we count the start and the end of the sequence always as stops
-        if index == 0 or index == len(query_seq) - 1:
-            # if x != '*' and subj_seq[index] != '*':
-            list_stops.append(index)
-            continue
-        # save all the indexes of stops
-        if x == '*' or subj_seq[index] == '*':
-            list_stops.append(index)
-
-    block_dict_list = list() # creates a list
-    for idx, x in enumerate(list_stops):
-        if x == list_stops[-1]:
-            break # necessary to skip an error
-        block_dict = dict() # creates a dictionary
-        # we skip the 1st and last index of the fragments (stops)
-        ######################################
-        #### MM: never scoring the first and last position --> fix it
-        block_dict['Align_Start'] = x + 1
-        block_dict['Align_End'] = list_stops[idx + 1]
-        block_dict['Score'] = score(query_seq[x: list_stops[idx + 1]], subj_seq[x: list_stops[idx + 1]], dictionary)
-        block_dict_list.append(block_dict) # create a list of dictionaries
-    # dictionaries of each alignment are sorted by 'Score'
-    # reverse=True to have the best scored one at the beginning
-    # lambda input: output
-    best_block = sorted(block_dict_list, key=lambda x: x['Score'], reverse=True)
-
-    return best_block[0] # return the dictionary with the values of the best fragment 
-
-def score(query_frag, subj_frag, dictionary):
-    '''
-    Calculates the score using matrix Blosum62
-
-    Parameters
-    ----------
-    query_frag : String
-        Protein sequence from the query
-    subj_frag : String
-        Protein sequence from the subject
-    dictionary : Dictionary
-        Matrix Blosum Values
-
-    Returns
-    -------
-    Score : Int
-        Value according to matrix Blosum62
-    '''
-
-    score = 0
-    for index, x in enumerate(query_frag):
-        if x == '-' or subj_frag[index] == '-':
-            continue
-        score += dictionary[(x, subj_frag[index])]
-
-    return score
-
-def dictionary_seleno():
-    '''
-    Creates a dictionary of tuples with the values of the BLOSUM62 Matrix.
-
-    Returns
-    -------
-    dictionary_sel : <dict>
-        Dictionary of tuples with the values of the BLOSUM62 Matrix.
-    '''
-
-    print(f'Writing the dictionary BLOSUM62')
-    dictionary_sel = dict()
-
-    with open(twinstop_libpath+'Matrix_BLOSUM62sel.txt', 'r') as fr:
-        for index, row in enumerate(fr):
-            # creates a list, using ' ' as sep.
-            spt = row.split(' ')
-            # deletes blank spaces.
-            spt = list(filter(None, spt))
-            if index == 0:
-                # delete empty spaces.
-                header = [x.strip() for x in spt]
-                continue
-            # deletes '\n' characters.
-            spt = [x.strip() for x in spt]
-            # converts the values (<str>) into <int>.
-            ints = [int(x) for x in spt[1:]]
-            keys = [(spt[0], aa) for aa in header]
-            # creation of the dictionary:
-            for ik, k in enumerate(keys):
-                dictionary_sel[k] = ints[ik]
-
-    return dictionary_sel
+def block_dict(query_seq, subj_seq, dictionary):
+    '''
+    Takes two protein sequences (one from the query and the other from the subject), 
+    divides them into blocks according to the stops '*' present in both and then 
+    saves in a list of dictionaries the start, end and score (matrix Blosum62)
+    of each block. Afterward, the block with better score is selected and the
+    data of the score, start, end and sequence from both query and subject is
+    updated in the general dataframe.
+
+    Parameters
+    ----------
+    query_seq : String
+        Aligned protein sequence of the query
+    subj_seq : String
+        Aligned protein sequence of the subject
+    dictionary : Dictionary of tuples
+        Matrix Blosum62 values
+
+    Returns
+    -------
+    best_block[0] : Dictionary with the 'Start', 'End' and 'Score' values of the
+    best scored fragment of each alignment.
+    '''
+
+    list_stops = list() # create a list to save stops index
+
+    for index, x in enumerate(query_seq):
+        # we count the start and the end of the sequence always as stops
+        if index == 0 or index == len(query_seq) - 1:
+            # if x != '*' and subj_seq[index] != '*':
+            list_stops.append(index)
+            continue
+        # save all the indexes of stops
+        if x == '*' or subj_seq[index] == '*':
+            list_stops.append(index)
+
+    block_dict_list = list() # creates a list
+    for idx, x in enumerate(list_stops):
+        if x == list_stops[-1]:
+            break # necessary to skip an error
+        block_dict = dict() # creates a dictionary
+        # we skip the 1st and last index of the fragments (stops)
+        ######################################
+        #### MM: never scoring the first and last position --> fix it
+        block_dict['Align_Start'] = x + 1
+        block_dict['Align_End'] = list_stops[idx + 1]
+        block_dict['Score'] = score(query_seq[x: list_stops[idx + 1]], subj_seq[x: list_stops[idx + 1]], dictionary)
+        block_dict_list.append(block_dict) # create a list of dictionaries
+    # dictionaries of each alignment are sorted by 'Score'
+    # reverse=True to have the best scored one at the beginning
+    # lambda input: output
+    best_block = sorted(block_dict_list, key=lambda x: x['Score'], reverse=True)
+
+    return best_block[0] # return the dictionary with the values of the best fragment 
+
+def score(query_frag, subj_frag, dictionary):
+    '''
+    Calculates the score using matrix Blosum62
+
+    Parameters
+    ----------
+    query_frag : String
+        Protein sequence from the query
+    subj_frag : String
+        Protein sequence from the subject
+    dictionary : Dictionary
+        Matrix Blosum Values
+
+    Returns
+    -------
+    Score : Int
+        Value according to matrix Blosum62
+    '''
+
+    score = 0
+    for index, x in enumerate(query_frag):
+        if x == '-' or subj_frag[index] == '-':
+            continue
+        score += dictionary[(x, subj_frag[index])]
+
+    return score
+
+def dictionary_seleno():
+    '''
+    Creates a dictionary of tuples with the values of the BLOSUM62 Matrix.
+
+    Returns
+    -------
+    dictionary_sel : <dict>
+        Dictionary of tuples with the values of the BLOSUM62 Matrix.
+    '''
+
+    dictionary_sel = dict()
+
+    with open(twinstop_libpath+'Matrix_BLOSUM62sel.txt', 'r') as fr:
+        for index, row in enumerate(fr):
+            # creates a list, using ' ' as sep.
+            spt = row.split(' ')
+            # deletes blank spaces.
+            spt = list(filter(None, spt))
+            if index == 0:
+                # delete empty spaces.
+                header = [x.strip() for x in spt]
+                continue
+            # deletes '\n' characters.
+            spt = [x.strip() for x in spt]
+            # converts the values (<str>) into <int>.
+            ints = [int(x) for x in spt[1:]]
+            keys = [(spt[0], aa) for aa in header]
+            # creation of the dictionary:
+            for ik, k in enumerate(keys):
+                dictionary_sel[k] = ints[ik]
+
+    return dictionary_sel
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `twinstop-0.0.2/src/twinstop/data_files/Matrix_BLOSUM62sel.txt` & `twinstop-0.0.3/src/twinstop/data_files/Matrix_BLOSUM62sel.txt`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.2/src/twinstop/data_files/logistic_regression_model.def.pkl` & `twinstop-0.0.3/src/twinstop/data_files/logistic_regression_model.def.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.2/src/twinstop/data_files/logistic_regression_model.pre.pkl` & `twinstop-0.0.3/src/twinstop/data_files/logistic_regression_model.pre.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.2/src/twinstop/data_files/logistic_regression_model.sen.pkl` & `twinstop-0.0.3/src/twinstop/data_files/logistic_regression_model.sen.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.2/src/twinstop/data_files/scaler.pkl` & `twinstop-0.0.3/src/twinstop/data_files/scaler.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.2/src/twinstop/denovo_selenoproteins_h3.bkp.py` & `twinstop-0.0.3/src/twinstop/denovo_selenoproteins_h3.bkp2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1792,15 +1792,15 @@
 def time_mem_usage(initial_time):
     time_usage = datetime.now() - initial_time
     write(f'Time usage: {time_usage}')
     peak_memory, current_memory = get_proc_status(('VmHWM', 'VmRSS'))
     write(f'Memory peak: {peak_memory}')
     write(f'Current memory use: {current_memory}')
 
-def regression_filter(candidates, lr_filepath):
+def regression_filter(candidates, lr_filepath, ncpus):
     scaler_filepath=twinstop_libpath + 'scaler.pkl'
     if candidates.isnull().values.any():
         maxdnds = 3
         # print(candidates['dN_dS_up'].isnull().values.any())
         # print(candidates['dN_dS_down'].isnull().values.any())
         candidates['dN_dS_up'] = candidates['dN_dS_up'].where(~candidates['dN_dS_up'].isna(), maxdnds)
         candidates['dN_dS_up'] = candidates['dN_dS_up'].where(candidates['dN_dS_up'] <= maxdnds, maxdnds)
@@ -1859,14 +1859,16 @@
 
     # X = X.reindex(columns=list(scaler.feature_names_in_))
     # stand_cand = scaler.transform(X)
 
     with open(lr_filepath, 'rb') as file:
         lr = pickle.load(file)
 
+    lr.n_jobs=ncpus
+        
     return lr.predict(X_stand)
 
 def preprocessing_candidates(candidates_df, q_file, subj_file, sp4_subj_gff): ### sp4_subj_gff ????
     abbreviations = dict(
         {'Chlorella_sorokiniana_nt': 'Cs', 'Chlamydomonas_acidophila_nt': 'Ca', 'Chlamydomonas_leiostraca': 'Cl',
          'Chlorella_sp_H2S_nt': 'CH2S', 'Smittium_culicis_2024_RNAseq_assembly': 'Sc',
          'Smittium_lentaquaticum_9068_RNAseq_assembly': 'Sl', 'Smittium_simulii_9019_RNAseq_assembly': 'Ss',
@@ -2244,15 +2246,16 @@
     if opt['model'] == 'd':
         lr_filepath=twinstop_libpath+'logistic_regression_model.def.pkl'
     elif opt['model'] == 'p':
         lr_filepath=twinstop_libpath+'logistic_regression_model.pre.pkl'
     elif opt['model'] == 's':
         lr_filepath=twinstop_libpath+'logistic_regression_model.sen.pkl'
 
-    lr_preds, y = regression_filter(candidates_df, lr_filepath)
+        
+    lr_preds, y = regression_filter(candidates_df, lr_filepath, ncpus=n_cpu)
     # mispredictions = candidates_df.true_positive.reset_index(drop=True)\
     #     .compare(pd.Series(lr_preds, name='true_positive')).value_counts()
     if benchmark:
         (_, fp_ml, fn_ml, tp_ml) = confusion_matrix(y, lr_preds).ravel()
         write(f'\nPrecision: {round(tp_ml / (tp_ml + fp_ml), 4)}')
         write(f'\nSensitivity: {round(tp_ml / (tp_ml + fn_ml), 4)}')
```

### Comparing `twinstop-0.0.2/src/twinstop/denovo_selenoproteins_h3.py` & `twinstop-0.0.3/src/twinstop/denovo_selenoproteins_h3.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 help_msg = """Twinstop is a de novo selenoprotein identification pipeline.
 It is based on the evolutionary conservation around the UGA-coding selenocysteine between two homologous
 selenoproteins from two closely related transcriptomes.
 
 ### Inputs/Outputs:
 
 # Compulsory args:
--q : <str> query file path. It must be a nucleotide transcriptome in fasta format.
--t : <str> db file path. It must be a nucleotide transcriptome in fasta format (makeblastdb beforehand).
--o : <str> folder path where all output files generated by Twinstop will be saved.
+-q : <str> query file path: a transcriptome in fasta format
+-s : <str> subject file path: a nucleotide transcriptome in fasta format, with with makeblastdb run beforehand
+-o : <str> output folder path, where files generated by Twinstop will be saved
 
 # Optional args:
 -c : <int> nº of CPUs used to run BLAST. The default is '1' CPUs.
 -force : <int> controls the rerun of the phases of Twinstop. The number represents the phase from which Twinstop
                will start the rerun (only in the case that the output file from previous phases have already been created).
                The default is to run only phases for which no output is detected.
                For a list of phases, run:  twinstop -h phases
@@ -50,15 +50,15 @@
 
 phases_help="""
 TBD
 """
 
 def_opt = {
     'q': '',
-    't': '',
+    's': '',
     'o': 'twinstop_out/',
     'c': 1,
     'n': 1,
     'n_chunks': 10,
     'n_lines': 2500000,
     'cds_q': False,
     'cds_t': False,
@@ -93,15 +93,16 @@
 import pickle
 import multiprocess as mp
 import numpy as np
 from datetime import datetime
 from easyterm import command_line_options, check_file_presence, write
 from easybioinfo import count_coding_changes, count_coding_sites, translate
 from Bio import pairwise2
-from extend_orfs import extend_orfs
+
+from extend_orfs_pyranges import extend_orfs
 from file_chunk_iterators import (
     iterate_file_in_chunks, iterate_file_in_chunks_with_key, buf_count_newlines_gen)
 
 # external scripts:
 from ._version import __version__
 from .block_selection import dictionary_seleno, score, block_dict
 from .test_alignment_methods import multiprocessing, mafft
@@ -1861,32 +1862,32 @@
     # stand_cand = scaler.transform(X)
 
     with open(lr_filepath, 'rb') as file:
         lr = pickle.load(file)
 
     lr.n_jobs=ncpus
         
-    return lr.predict(X_stand)
+    return lr.predict(X_stand), y
 
-def preprocessing_candidates(candidates_df, q_file, subj_file, sp4_subj_gff): ### sp4_subj_gff ????
+def preprocessing_candidates(candidates_df, q_file, subj_file, sp4_subj_gff=None):
     abbreviations = dict(
         {'Chlorella_sorokiniana_nt': 'Cs', 'Chlamydomonas_acidophila_nt': 'Ca', 'Chlamydomonas_leiostraca': 'Cl',
          'Chlorella_sp_H2S_nt': 'CH2S', 'Smittium_culicis_2024_RNAseq_assembly': 'Sc',
          'Smittium_lentaquaticum_9068_RNAseq_assembly': 'Sl', 'Smittium_simulii_9019_RNAseq_assembly': 'Ss',
          'Tetraselmis_striata_nt': 'Tst', 'Tetraselmis_suecica_nt': 'Ts', 'Homo_sapiens': 'Hs', 'Mus_musculus': 'Mm',
          'Thalassiosira_antartica_nt': 'Ta', 'Thalassiosira_minuscula_nt': 'Tm'})
     try:
         candidates_df['Run_info'] = (abbreviations[os.path.basename(q_file).split('.')[0]] + '_vs_' +
                                      abbreviations[os.path.basename(subj_file).split('.')[0]])
     except:
         candidates_df['Run_info'] = (os.path.basename(q_file).split('.')[0] +
                                      '_vs_' + os.path.basename(subj_file).split('.')[0])
     candidates_df[['sec_start', 'sec_end']] = \
         candidates_df.apply(find_sec_pos, axis=1, result_type='expand')
-    if benchmark:
+    if not sp4_subj_gff == None:
         true_positives = candidates_df[['ID', 'Chromosome', 'sec_start', 'sec_end']] \
             .merge(sp4_subj_gff[['Chromosome', 'sec_start', 'sec_end']],
                    on=['Chromosome', 'sec_start', 'sec_end'], how='inner')
     # true_positives = true_positives[true_positives.sec_start_ts.eq(true_positives.sec_start_sp4)]
     # print(candidates_df.dtypes)
     # print(candidates_df['sec_start_ts'] == candidates_df['sec_start_sp4'])
     # print(true_positive)
@@ -1991,15 +1992,15 @@
     opt = command_line_options(def_opt, help_msg,
                                advanced_help_msg={'phases':phases_help}
     )
     # os.path.abspath(relative/absolute path) gets the absolute path of a file
     q_file = os.path.abspath(opt['q'])
     # checks if query file exists
     check_file_presence(q_file, 'Given path for query file does not exist')
-    subj_file = os.path.abspath(opt['t'])
+    subj_file = os.path.abspath(opt['s'])
     # checks if subject file exists
     check_file_presence(subj_file, 'Given path for subject file does not exist')
 
     output_folder = opt['o']
     # if output folder does not exist, it is created
     if not os.path.exists(output_folder):
         os.makedirs(output_folder)
@@ -2045,16 +2046,24 @@
     # benchmark variable is defined as global to use it all across the script without the need of being imported
     global benchmark, debugging
     benchmark = opt['benchmark']
     debugging = opt['debugging']
 
     if benchmark:
         # read table of the Selenoprofiles4 selenocysteines prediction for subject (control selenoproteins)
-        sp4_prediction_subj = pd.read_table(opt['sp4_prediction_subj'], sep='\t', header=None,
-                                            names=["Transcript", "Sel_family", "n", "Subj_ID"], index_col=False)
+        sp4_subj_gff = pd.read_csv(opt['sp4_subj_gff'], sep="\t", header=None, index_col=False)
+        sp4_subj_gff.columns = ['Chromosome', 'source', 'feature', 'sec_start', 'sec_end',
+                                'score', 'strand', 'frame', 'attribute', 'subj_id']
+        sp4_prediction_subj = pd.DataFrame()
+        sp4_prediction_subj['Transcript'] = sp4_subj_gff.Chromosome
+        sp4_prediction_subj[['Sel_family', 'n']] = sp4_subj_gff.apply(
+            lambda x: x['attribute'].split(':')[1].split('.')[:2], axis=1, result_type='expand')
+        sp4_prediction_subj['Subj_ID'] = sp4_subj_gff.subj_id
+        # sp4_prediction_subj = pd.read_table(opt['sp4_prediction_subj'], sep='\t', header=None,
+        #                                     names=["Transcript", "Sel_family", "n", "Subj_ID"], index_col=False)
         sp4_prediction_query = pd.read_table(opt['sp4_prediction_query'], sep='\t', header=None,
                                              names=["Transcript", "Sel_family", "n", "Query_ID"], index_col=False)
         # I want to get rid of the selenoprotein families which are unreachable for this script (terminal selenocysteines)
         # selenos_annot_query = pd.DataFrame(sp4_prediction_query.Name.str.split(n=3, pat=".").to_list(),
         #                                    columns=['Sel_family', 'Nº', 'Stop_codon', 'rest'])
         # selenos_annot_query.drop(labels='rest', axis=1, inplace=True)
         # selenos_annot_query['Transcript'] = sp4_prediction_query.Transcript
@@ -2184,25 +2193,26 @@
         # else:
         #     chunking(path_pairwise_outfile, n_chunks, 0, UGA_alignments,
         #              n_cpu, None, path_candidates_outfile, n)
         #     candidates_df = pd.read_csv(path_candidates_outfile, sep='\t', header=0, index_col=False)
     else:
         write(f'Reading {path_candidates_outfile}')
         candidates_df = pd.read_csv(path_candidates_outfile, sep='\t', header=0, index_col=False)
-        candidates_df = candidates_df \
-            .sort_values(by='Score', ascending=False, ignore_index=True) \
-            .drop_duplicates('Chromosome', ignore_index=True)
-        candidates_df.to_csv(path_or_buf=path_candidates_outfile, sep='\t', index=False)
+        # candidates_df = candidates_df \
+        #     .sort_values(by='Score', ascending=False, ignore_index=True) \
+        #     .drop_duplicates('Chromosome', ignore_index=True)
+        # candidates_df.to_csv(path_or_buf=path_candidates_outfile, sep='\t', index=False)
         # here there is a control to prevent empty dfs to be passed to the next phase causing an error
         if len(candidates_df) == 0:
             write(f'Empty file {candidates_df}')
     
     write(f'\nCandidates outfile cointains: {buf_count_newlines_gen(path_candidates_outfile)} candidates')
     write(f'\nNº of unique subject transcripts: {len(candidates_df.Chromosome.unique())}')
-    write(f'\nTP: {available_selenos.Transcript.isin(candidates_df.Chromosome).sum()}/{len(available_selenos)}')
+    if benchmark:
+        write(f'\nTP: {available_selenos.Transcript.isin(candidates_df.Chromosome).sum()}/{len(available_selenos)}')
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
     write('\n### PHASE 7: EVO-CONSERVATION')
 
@@ -2222,54 +2232,56 @@
     # print(sp4_subj_gff)
     # sp4_subj_gff.columns = ['Chromosome', 'source', 'feature', 'sec_start', 'sec_end',
     #                         'score', 'strand', 'frame', 'attribute', 'subj_id']
     # sp4_subj_gff['sec_start'] -= 1
     # sp4_subj_gff = sp4_subj_gff[sp4_subj_gff['feature'] == 'Selenocysteine'].reset_index(drop=True)
     # print(sp4_subj_gff)
     if not os.path.exists(path_selenocandidates_outfile) or n_section < 8:
-        candidates_df = preprocessing_candidates(candidates_df, q_file, subj_file)
+        if benchmark:
+            candidates_df = preprocessing_candidates(candidates_df, q_file, subj_file, sp4_subj_gff=sp4_subj_gff)
+            tp = candidates_df[candidates_df.true_positive == True].shape[0]
+            fp = candidates_df[candidates_df.true_positive == False].shape[0]
+            fn = available_selenos.shape[0] - tp
+            precision = round(tp / (tp + fp), 4)
+            recall = round(tp / (tp + fn), 4)
+            write(f'\nPrecision: {precision}')
+            write(f'\nSensitivity: {recall}')
+        else:
+            candidates_df = preprocessing_candidates(candidates_df, q_file, subj_file)
+
+        if opt['model'] == 'd':
+            lr_filepath = twinstop_libpath + 'logistic_regression_model.def.pkl'
+        elif opt['model'] == 'p':
+            lr_filepath = twinstop_libpath + 'logistic_regression_model.pre.pkl'
+        elif opt['model'] == 's':
+            lr_filepath = twinstop_libpath + 'logistic_regression_model.sen.pkl'
+
+        lr_preds, y = regression_filter(candidates_df, lr_filepath)
+        candidates_df = candidates_df[lr_preds]
         candidates_df.to_csv(path_or_buf=path_selenocandidates_outfile, sep='\t', index=False)
+
+        if benchmark:
+            (_, fp_ml, fn_ml, tp_ml) = confusion_matrix(y, lr_preds).ravel()
+            precision_ml = round(tp_ml / (tp_ml + fp_ml), 4)
+            recall_ml = round(tp_ml / (tp_ml + fn_ml), 4)
+            write(f'\nPrecision_lr: {precision_ml}')
+            write(f'\nSensitivity_lr: {recall_ml}\n')
+            write(f'\nPrecision Twinstop: {precision_ml}')
+            write(f'\nSensitivity Twinstop: {recall * recall_ml}\n')
     else:
         candidates_df = pd.read_csv(path_selenocandidates_outfile, sep='\t', header=0, index_col=False)
 
-    # print(candidates_df.dtypes)
-    if benchmark:
-        tp = candidates_df[candidates_df.true_positive == True].shape[0]
-        fp = candidates_df[candidates_df.true_positive == False].shape[0]
-        fn = available_selenos.shape[0] - tp
-        write(f'\nPrecision: {round(tp / (tp + fp), 4)}')
-        write(f'\nSensitivity: {round(tp / (tp + fn), 4)}')
-
     write(f'\nSelenocandidates outfile cointains: {buf_count_newlines_gen(path_selenocandidates_outfile)} candidates')
-    write(f'\nNº of unique subject transcripts: {len(candidates_df.Chromosome.unique())}')
+    # write(f'\nNº of unique subject transcripts: {len(candidates_df.Chromosome.unique())}')
     # write(f'\nTP: {available_selenos.Transcript.isin(candidates_df.Chromosome).sum()}/{len(available_selenos)}')
 
-    if opt['model'] == 'd':
-        lr_filepath=twinstop_libpath+'logistic_regression_model.def.pkl'
-    elif opt['model'] == 'p':
-        lr_filepath=twinstop_libpath+'logistic_regression_model.pre.pkl'
-    elif opt['model'] == 's':
-        lr_filepath=twinstop_libpath+'logistic_regression_model.sen.pkl'
-
-        
-    lr_preds, y = regression_filter(candidates_df, lr_filepath, ncpus=n_cpu)
-    # mispredictions = candidates_df.true_positive.reset_index(drop=True)\
-    #     .compare(pd.Series(lr_preds, name='true_positive')).value_counts()
-    if benchmark:
-        (_, fp_ml, fn_ml, tp_ml) = confusion_matrix(y, lr_preds).ravel()
-        write(f'\nPrecision: {round(tp_ml / (tp_ml + fp_ml), 4)}')
-        write(f'\nSensitivity: {round(tp_ml / (tp_ml + fn_ml), 4)}')
-
-    write(f'\nSelenocandidates outfile cointains: {buf_count_newlines_gen(path_selenocandidates_outfile)} candidates')
-    write(f'\nNº of unique subject transcripts: {len(candidates_df.Chromosome.unique())}')
-
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
-    # raise SystemError
+
     write('\n### PHASE 8: BLASTP FOR ANNOTATION')
 
     if not 'Annot_Title' in candidates_df and opt['annot_candidates']:
         candidates_df = run_blastp(candidates_df, opt['annotation_db'], n_cpu,
                                    path_blastp_outfile, path_fasta_query_prot_seq)
         candidates_df.sort_values(by='Density_Score', inplace=True,
                                   ignore_index=True, ascending=False)
```

### Comparing `twinstop-0.0.2/src/twinstop/test_alignment_methods.py` & `twinstop-0.0.3/src/twinstop/test_alignment_methods.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.2/src/twinstop.egg-info/PKG-INFO` & `twinstop-0.0.3/src/twinstop.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinstop
-Version: 0.0.2
+Version: 0.0.3
 Summary: twinstop identifies selenoproteins in close related transcriptomes
 Home-page: https://github.com/marco-mariotti/twinstop
 Author: Marco Mariotti and Sergio Sanchez Moragues
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `twinstop-0.0.2/src/twinstop.egg-info/SOURCES.txt` & `twinstop-0.0.3/src/twinstop.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/twinstop/__init__.py
 src/twinstop/_version.py
 src/twinstop/block_selection.py
-src/twinstop/denovo_selenoproteins_h3.bkp.py
+src/twinstop/denovo_selenoproteins_h3.bkp2.py
 src/twinstop/denovo_selenoproteins_h3.py
 src/twinstop/test_alignment_methods.py
 src/twinstop.egg-info/PKG-INFO
 src/twinstop.egg-info/SOURCES.txt
 src/twinstop.egg-info/dependency_links.txt
 src/twinstop.egg-info/requires.txt
 src/twinstop.egg-info/top_level.txt
```

