# Comparing `tmp/calisp-3.0.8.tar.gz` & `tmp/calisp-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calisp-3.0.8.tar", last modified: Thu Dec 30 17:43:25 2021, max compression
+gzip compressed data, was "calisp-3.0.9.tar", last modified: Thu Jun 23 16:28:02 2022, max compression
```

## Comparing `calisp-3.0.8.tar` & `calisp-3.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kinestetika  (1000) kinestetika  (1000)        0 2021-12-30 17:43:25.721921 calisp-3.0.8/
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     7331 2021-12-30 17:43:25.721921 calisp-3.0.8/PKG-INFO
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     6559 2021-12-13 16:54:31.000000 calisp-3.0.8/README.md
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)      103 2021-11-25 17:22:28.000000 calisp-3.0.8/pyproject.toml
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)       78 2021-12-30 17:43:25.721921 calisp-3.0.8/setup.cfg
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     1403 2021-12-13 16:54:31.000000 calisp-3.0.8/setup.py
-drwxr-xr-x   0 kinestetika  (1000) kinestetika  (1000)        0 2021-12-30 17:43:25.675254 calisp-3.0.8/src/
-drwxr-xr-x   0 kinestetika  (1000) kinestetika  (1000)        0 2021-12-30 17:43:25.708587 calisp-3.0.8/src/calisp/
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)        0 2021-11-25 17:22:28.000000 calisp-3.0.8/src/calisp/__init__.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     5861 2021-12-13 16:54:31.000000 calisp-3.0.8/src/calisp/data_store.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     6487 2021-12-13 16:58:18.000000 calisp-3.0.8/src/calisp/element_count_and_mass_utils.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     9332 2021-12-13 16:45:40.000000 calisp-3.0.8/src/calisp/isotopic_pattern_utils.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)    19702 2021-12-13 16:54:31.000000 calisp-3.0.8/src/calisp/main.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     7601 2021-12-13 16:24:23.000000 calisp-3.0.8/src/calisp/peptide_spectrum_match_files.py
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)    35798 2021-11-25 17:22:28.000000 calisp-3.0.8/src/calisp/unimod.py
-drwxr-xr-x   0 kinestetika  (1000) kinestetika  (1000)        0 2021-12-30 17:43:25.721921 calisp-3.0.8/src/calisp.egg-info/
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)     7331 2021-12-30 17:43:25.000000 calisp-3.0.8/src/calisp.egg-info/PKG-INFO
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)      460 2021-12-30 17:43:25.000000 calisp-3.0.8/src/calisp.egg-info/SOURCES.txt
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)        1 2021-12-30 17:43:25.000000 calisp-3.0.8/src/calisp.egg-info/dependency_links.txt
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)       45 2021-12-30 17:43:25.000000 calisp-3.0.8/src/calisp.egg-info/entry_points.txt
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)      103 2021-12-30 17:43:25.000000 calisp-3.0.8/src/calisp.egg-info/requires.txt
--rw-r--r--   0 kinestetika  (1000) kinestetika  (1000)        7 2021-12-30 17:43:25.000000 calisp-3.0.8/src/calisp.egg-info/top_level.txt
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2022-06-23 16:28:02.822000 calisp-3.0.9/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     7343 2022-06-23 16:28:02.825333 calisp-3.0.9/PKG-INFO
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6591 2022-06-23 14:34:23.000000 calisp-3.0.9/README.md
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)      103 2022-06-23 14:34:23.000000 calisp-3.0.9/pyproject.toml
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)       78 2022-06-23 16:28:02.825333 calisp-3.0.9/setup.cfg
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     1403 2022-06-23 14:53:53.000000 calisp-3.0.9/setup.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2022-06-23 16:28:02.822000 calisp-3.0.9/src/
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2022-06-23 16:28:02.822000 calisp-3.0.9/src/calisp/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        0 2022-06-23 14:34:23.000000 calisp-3.0.9/src/calisp/__init__.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     5861 2022-06-23 14:34:23.000000 calisp-3.0.9/src/calisp/data_store.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     6487 2022-06-23 14:34:23.000000 calisp-3.0.9/src/calisp/element_count_and_mass_utils.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     9332 2022-06-23 14:34:23.000000 calisp-3.0.9/src/calisp/isotopic_pattern_utils.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    19883 2022-06-23 16:27:43.000000 calisp-3.0.9/src/calisp/main.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     7601 2022-06-23 14:34:23.000000 calisp-3.0.9/src/calisp/peptide_spectrum_match_files.py
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)    35798 2022-06-23 14:34:23.000000 calisp-3.0.9/src/calisp/unimod.py
+drwxr-xr-x   0 mstrous   (1000) mstrous   (1000)        0 2022-06-23 16:28:02.822000 calisp-3.0.9/src/calisp.egg-info/
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)     7343 2022-06-23 16:28:02.000000 calisp-3.0.9/src/calisp.egg-info/PKG-INFO
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)      460 2022-06-23 16:28:02.000000 calisp-3.0.9/src/calisp.egg-info/SOURCES.txt
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        1 2022-06-23 16:28:02.000000 calisp-3.0.9/src/calisp.egg-info/dependency_links.txt
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)       44 2022-06-23 16:28:02.000000 calisp-3.0.9/src/calisp.egg-info/entry_points.txt
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)      103 2022-06-23 16:28:02.000000 calisp-3.0.9/src/calisp.egg-info/requires.txt
+-rw-r--r--   0 mstrous   (1000) mstrous   (1000)        7 2022-06-23 16:28:02.000000 calisp-3.0.9/src/calisp.egg-info/top_level.txt
```

### Comparing `calisp-3.0.8/PKG-INFO` & `calisp-3.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: calisp
-Version: 3.0.8
+Version: 3.0.9
 Summary: Isotope analysis of proteomics data
 Home-page: https://github.com/kinestetika/Calisp
 Author: Marc Strous
 Author-email: mstrous@ucalgary.ca
 License: MIT
 Project-URL: Source, https://github.com/kinestetika/Calisp
 Keywords: proteomics isotope mass-spectrometry 13C
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -74,17 +73,17 @@
 
 >pip install --upgrade calisp jupyter matplotlib jinja2
 
 **Usage:**
 
 >source calisp/bin/activate
 
->calisp.py --spectrum_file [path to .mzML file or folder with .mzML files] --peptide_file [path to .mzML file or folder 
- with .mzML files] --output_file [folder where calisp.py will save results files] --threads [# of threads used, 
- default 4] --isotope [15N, 3H etc, default 13C], --bin_delimiter [character that separates the bin ID from the
+>calisp.py --spectrum_file [path to .mzML file or folder with .mzML files] --peptide_file [path to .peptideSpectrumMatch file 
+ or folder with .PeptideSpectrumMatch files] --output_file [folder where calisp.py will save results files] --threads [# of 
+ threads used, default 4] --isotope [15N, 3H etc, default 13C], --bin_delimiter [character that separates the bin ID from the
  remainder of protein IDs, default '_'], --mass_accuracy [accuracy of peak m/z identifications, default 10 ppm]
  --compute_clumps [use only if you want to compute clumpiness]
 
 **Column names of the Pandas DataFrame created by calisp.py:**
 
 In the saved dataframe, each row contains one isotopic pattern, defined by the following columns:
 
@@ -114,9 +113,7 @@
 Kleiner M, Kouris A, Jensen M, Liu Y, McCalder J, Strous M (2021) Ultra-sensitive Protein-SIP to quantify activity 
 and substrate uptake in microbiomes with stable isotopes. bioRxiv.
 doi: [https://doi.org/10.1101/2021.03.29.437612](https://doi.org/10.1101/2021.03.29.437612)
 
 M Kösters, J Leufken, S Schulze, K Sugimoto, J Klein, R P Zahedi, M Hippler, S A Leidel, C Fufezan; pymzML v2.0: 
 introducing a highly compressed and seekable gzip format, Bioinformatics, 
 doi: [https://doi.org/10.1093/bioinformatics/bty046](https://doi.org/10.1093/bioinformatics/bty046)
-
-
```

### Comparing `calisp-3.0.8/README.md` & `calisp-3.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,17 @@
 
 >pip install --upgrade calisp jupyter matplotlib jinja2
 
 **Usage:**
 
 >source calisp/bin/activate
 
->calisp.py --spectrum_file [path to .mzML file or folder with .mzML files] --peptide_file [path to .mzML file or folder 
- with .mzML files] --output_file [folder where calisp.py will save results files] --threads [# of threads used, 
- default 4] --isotope [15N, 3H etc, default 13C], --bin_delimiter [character that separates the bin ID from the
+>calisp.py --spectrum_file [path to .mzML file or folder with .mzML files] --peptide_file [path to .peptideSpectrumMatch file 
+ or folder with .PeptideSpectrumMatch files] --output_file [folder where calisp.py will save results files] --threads [# of 
+ threads used, default 4] --isotope [15N, 3H etc, default 13C], --bin_delimiter [character that separates the bin ID from the
  remainder of protein IDs, default '_'], --mass_accuracy [accuracy of peak m/z identifications, default 10 ppm]
  --compute_clumps [use only if you want to compute clumpiness]
 
 **Column names of the Pandas DataFrame created by calisp.py:**
 
 In the saved dataframe, each row contains one isotopic pattern, defined by the following columns:
```

### Comparing `calisp-3.0.8/setup.py` & `calisp-3.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='calisp',
-    version='3.0.8',
+    version='3.0.9',
     packages=setuptools.find_packages(where='src'),
     url='https://github.com/kinestetika/Calisp',
     license='MIT',
     author='Marc Strous',
     author_email='mstrous@ucalgary.ca',
     description='Isotope analysis of proteomics data',
     long_description=long_description,
```

### Comparing `calisp-3.0.8/src/calisp/data_store.py` & `calisp-3.0.9/src/calisp/data_store.py`

 * *Files identical despite different names*

### Comparing `calisp-3.0.8/src/calisp/element_count_and_mass_utils.py` & `calisp-3.0.9/src/calisp/element_count_and_mass_utils.py`

 * *Files identical despite different names*

### Comparing `calisp-3.0.8/src/calisp/isotopic_pattern_utils.py` & `calisp-3.0.9/src/calisp/isotopic_pattern_utils.py`

 * *Files identical despite different names*

### Comparing `calisp-3.0.8/src/calisp/main.py` & `calisp-3.0.9/src/calisp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from tqdm import tqdm
 
 from calisp import isotopic_pattern_utils
 from calisp import data_store
 from calisp import element_count_and_mass_utils
 from calisp.peptide_spectrum_match_files import PeptideSpectrumMatchFileReader
 
-VERSION = '3.0.8'
+VERSION = '3.0.9'
 START_TIME = time.monotonic()
 LOG_TOPICS = set()
 MASS_ACCURACY = 1e-5
 COMPUTE_CLUMPS = False
 
 
 def format_runtime():
@@ -50,14 +50,15 @@
                                                              '34S', '36S'],
                         help='The target isotope. Default: 13C')
     parser.add_argument('--compute_clumps', default=False, action='store_true',
                         help='To compute clumpiness of carbon assimilation. Only use when samples are labeled to'
                              'saturation. Estimation of clumpiness takes much additional time.')
 
     args = parser.parse_args()
+
     log(f'isotope:        {args.isotope} '
         f'[matrix{isotopic_pattern_utils.ELEMENT_ROW_INDEX, isotopic_pattern_utils.ISOTOPE_COLUMN_INDEX}]')
     log(f'peptide_file:   {args.peptide_file}')
     log(f'spectrum_file:  {args.spectrum_file}')
     log(f'output_file:    {args.output_file}')
     log(f'mass_accuracy:  {args.mass_accuracy} ppm')
     log(f'bin_delimiter:  {args.bin_delimiter}')
@@ -278,15 +279,16 @@
             f'"{os.path.basename(experiment_filename)}"...')
         with PeptideSpectrumMatchFileReader(experiment_filename, bin_delimiter=args.bin_delimiter) as peptide_reader:
             psm_as_dict = []
             for psm in peptide_reader:
                 psm_as_dict.append(psm)
         psm_data = pd.DataFrame(columns=data_store.DATAFRAME_COLUMNS)
         psm_data = psm_data.astype(data_store.DATAFRAME_DATATYPES)
-        psm_data = psm_data.append(psm_as_dict, ignore_index=True)
+        psm_data = pd.concat([psm_data, pd.DataFrame(psm_as_dict)], ignore_index=True)
+        # psm_data.append(psm_as_dict, ignore_index=True)
         log(f'Parsed {len(psm_data.index)} PSMs from file.')
         spectrum_file_counter = 0
 
         ms_runs = psm_data["ms_run"].unique()
         for ms_run in ms_runs:
             try:
                 ms_run_file = my_data_store.ms_run_address_book[ms_run]
@@ -343,15 +345,16 @@
                 all_patterns = []
                 for patterns in list(tqdm(executor.map(subsample_ms1_spectra, tasks, chunksize=25), total=len(tasks))):
                     for p in patterns:
                         if p['reassigned']:
                             patterns_reassigned_count += 1
                         del p['reassigned']
                     all_patterns.extend(patterns)
-            pattern_data = pattern_data.append(all_patterns, ignore_index=True)
+            pattern_data = pd.concat([pattern_data, pd.DataFrame(all_patterns)], ignore_index=True)
+            # pattern_data = pattern_data.append(all_patterns, ignore_index=True)
             log(f'Subsampled and analyzed {len(pattern_data.index)} isotopic patterns, '
                 f'reassigned {patterns_reassigned_count / len(pattern_data.index) * 100:.1f}% of patterns to '
                 f'their nearest PSM. Now flagging overlap between patterns...')
 
             # (4) check for contamination (the same ms1 peaks shared by multiple peptide spectra
             with ProcessPoolExecutor(max_workers=args.threads) as executor:
                 precursor_ids = pattern_data['pattern_precursor_id'].unique()
```

### Comparing `calisp-3.0.8/src/calisp/peptide_spectrum_match_files.py` & `calisp-3.0.9/src/calisp/peptide_spectrum_match_files.py`

 * *Files identical despite different names*

### Comparing `calisp-3.0.8/src/calisp/unimod.py` & `calisp-3.0.9/src/calisp/unimod.py`

 * *Files identical despite different names*

### Comparing `calisp-3.0.8/src/calisp.egg-info/PKG-INFO` & `calisp-3.0.9/src/calisp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: calisp
-Version: 3.0.8
+Version: 3.0.9
 Summary: Isotope analysis of proteomics data
 Home-page: https://github.com/kinestetika/Calisp
 Author: Marc Strous
 Author-email: mstrous@ucalgary.ca
 License: MIT
 Project-URL: Source, https://github.com/kinestetika/Calisp
 Keywords: proteomics isotope mass-spectrometry 13C
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -74,17 +73,17 @@
 
 >pip install --upgrade calisp jupyter matplotlib jinja2
 
 **Usage:**
 
 >source calisp/bin/activate
 
->calisp.py --spectrum_file [path to .mzML file or folder with .mzML files] --peptide_file [path to .mzML file or folder 
- with .mzML files] --output_file [folder where calisp.py will save results files] --threads [# of threads used, 
- default 4] --isotope [15N, 3H etc, default 13C], --bin_delimiter [character that separates the bin ID from the
+>calisp.py --spectrum_file [path to .mzML file or folder with .mzML files] --peptide_file [path to .peptideSpectrumMatch file 
+ or folder with .PeptideSpectrumMatch files] --output_file [folder where calisp.py will save results files] --threads [# of 
+ threads used, default 4] --isotope [15N, 3H etc, default 13C], --bin_delimiter [character that separates the bin ID from the
  remainder of protein IDs, default '_'], --mass_accuracy [accuracy of peak m/z identifications, default 10 ppm]
  --compute_clumps [use only if you want to compute clumpiness]
 
 **Column names of the Pandas DataFrame created by calisp.py:**
 
 In the saved dataframe, each row contains one isotopic pattern, defined by the following columns:
 
@@ -114,9 +113,7 @@
 Kleiner M, Kouris A, Jensen M, Liu Y, McCalder J, Strous M (2021) Ultra-sensitive Protein-SIP to quantify activity 
 and substrate uptake in microbiomes with stable isotopes. bioRxiv.
 doi: [https://doi.org/10.1101/2021.03.29.437612](https://doi.org/10.1101/2021.03.29.437612)
 
 M Kösters, J Leufken, S Schulze, K Sugimoto, J Klein, R P Zahedi, M Hippler, S A Leidel, C Fufezan; pymzML v2.0: 
 introducing a highly compressed and seekable gzip format, Bioinformatics, 
 doi: [https://doi.org/10.1093/bioinformatics/bty046](https://doi.org/10.1093/bioinformatics/bty046)
-
-
```

