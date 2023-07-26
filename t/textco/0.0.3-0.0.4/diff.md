# Comparing `tmp/textco-0.0.3.tar.gz` & `tmp/textco-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textco-0.0.3.tar", last modified: Wed Jul 26 17:22:17 2023, max compression
+gzip compressed data, was "textco-0.0.4.tar", last modified: Wed Jul 26 17:25:31 2023, max compression
```

## Comparing `textco-0.0.3.tar` & `textco-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 17:22:17.026370 textco-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-07-20 20:17:27.000000 textco-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      731 2023-07-26 17:22:17.026370 textco-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-07-20 20:16:36.000000 textco-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-26 17:22:17.026370 textco-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1044 2023-07-26 17:22:02.000000 textco-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:22:17.019826 textco-0.0.3/textco/
--rw-rw-rw-   0        0        0       23 2023-07-26 16:54:05.000000 textco-0.0.3/textco/__init__.py
--rw-rw-rw-   0        0        0     3678 2023-07-26 17:21:45.000000 textco-0.0.3/textco/textco.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:22:17.026370 textco-0.0.3/textco.egg-info/
--rw-rw-rw-   0        0        0      731 2023-07-26 17:22:16.000000 textco-0.0.3/textco.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-07-26 17:22:16.000000 textco-0.0.3/textco.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 17:22:16.000000 textco-0.0.3/textco.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 17:22:16.000000 textco-0.0.3/textco.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 17:25:31.819277 textco-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-07-20 20:17:27.000000 textco-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      731 2023-07-26 17:25:31.819277 textco-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-07-20 20:16:36.000000 textco-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-26 17:25:31.819277 textco-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2023-07-26 17:25:16.000000 textco-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:25:31.797146 textco-0.0.4/textco/
+-rw-rw-rw-   0        0        0       23 2023-07-26 16:54:05.000000 textco-0.0.4/textco/__init__.py
+-rw-rw-rw-   0        0        0     3677 2023-07-26 17:25:01.000000 textco-0.0.4/textco/textco.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:25:31.819277 textco-0.0.4/textco.egg-info/
+-rw-rw-rw-   0        0        0      731 2023-07-26 17:25:31.000000 textco-0.0.4/textco.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-07-26 17:25:31.000000 textco-0.0.4/textco.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 17:25:31.000000 textco-0.0.4/textco.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 17:25:31.000000 textco-0.0.4/textco.egg-info/top_level.txt
```

### Comparing `textco-0.0.3/LICENSE.txt` & `textco-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `textco-0.0.3/PKG-INFO` & `textco-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textco
-Version: 0.0.3
+Version: 0.0.4
 Summary: TEXT analytsis COpilot
 Home-page: UNKNOWN
 Author: Dr Anna Sung and Prof Kelvin Leong
 Author-email: <k.leong@chester.ac.uk>
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

### Comparing `textco-0.0.3/setup.py` & `textco-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '00.00.03' 
+VERSION = '00.00.04' 
 DESCRIPTION = 'TEXT analytsis COpilot'
 LONG_DESCRIPTION = 'This Python package will help you to analyse text'
 
 
 setup(
         name="textco", 
         version=VERSION,
```

### Comparing `textco-0.0.3/textco/textco.py` & `textco-0.0.4/textco/textco.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,167 +64,167 @@
 000003f0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
 00000400: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 0d0a 0d0a  ************....
 00000410: 0d0a 6465 6620 636f 756e 7428 293a 0d0a  ..def count():..
 00000420: 2020 2320 5374 6570 2031 3a20 496e 7374    # Step 1: Inst
 00000430: 616c 6c20 6e65 6365 7373 6172 7920 6c69  all necessary li
 00000440: 6272 6172 6965 7320 2869 6620 6e6f 7420  braries (if not 
 00000450: 616c 7265 6164 7920 696e 7374 616c 6c65  already installe
-00000460: 6429 0d0a 2020 2170 6970 2069 6e73 7461  d)..  !pip insta
-00000470: 6c6c 2070 616e 6461 7320 6e6c 746b 0d0a  ll pandas nltk..
-00000480: 0d0a 2020 2320 5374 6570 2032 3a20 496d  ..  # Step 2: Im
-00000490: 706f 7274 2074 6865 2072 6571 7569 7265  port the require
-000004a0: 6420 6c69 6272 6172 6965 730d 0a20 2069  d libraries..  i
-000004b0: 6d70 6f72 7420 7061 6e64 6173 2061 7320  mport pandas as 
-000004c0: 7064 0d0a 2020 6672 6f6d 2063 6f6c 6c65  pd..  from colle
-000004d0: 6374 696f 6e73 2069 6d70 6f72 7420 436f  ctions import Co
-000004e0: 756e 7465 720d 0a20 2069 6d70 6f72 7420  unter..  import 
-000004f0: 696f 0d0a 2020 6672 6f6d 2067 6f6f 676c  io..  from googl
-00000500: 652e 636f 6c61 6220 696d 706f 7274 2066  e.colab import f
-00000510: 696c 6573 0d0a 2020 696d 706f 7274 206e  iles..  import n
-00000520: 6c74 6b0d 0a20 2066 726f 6d20 6e6c 746b  ltk..  from nltk
-00000530: 2e75 7469 6c20 696d 706f 7274 206e 6772  .util import ngr
-00000540: 616d 730d 0a20 2069 6d70 6f72 7420 6373  ams..  import cs
-00000550: 760d 0a0d 0a20 2023 2053 7465 7020 333a  v....  # Step 3:
-00000560: 2046 756e 6374 696f 6e20 746f 2070 6572   Function to per
-00000570: 666f 726d 2077 6f72 6420 636f 756e 7420  form word count 
-00000580: 616e 616c 7973 6973 2077 6974 6820 6e2d  analysis with n-
-00000590: 6772 616d 730d 0a20 2064 6566 2077 6f72  grams..  def wor
-000005a0: 645f 636f 756e 745f 616e 616c 7973 6973  d_count_analysis
-000005b0: 2863 7376 5f66 696c 652c 2074 6578 745f  (csv_file, text_
-000005c0: 636f 6c75 6d6e 2c20 6e29 3a0d 0a20 2020  column, n):..   
-000005d0: 2020 2023 2052 6561 6420 7468 6520 4353     # Read the CS
-000005e0: 5620 6669 6c65 2069 6e74 6f20 6120 7061  V file into a pa
-000005f0: 6e64 6173 2044 6174 6146 7261 6d65 0d0a  ndas DataFrame..
-00000600: 2020 2020 2020 6466 203d 2070 642e 7265        df = pd.re
-00000610: 6164 5f63 7376 2863 7376 5f66 696c 6529  ad_csv(csv_file)
-00000620: 0d0a 0d0a 2020 2020 2020 2320 436f 6d62  ....      # Comb
-00000630: 696e 6520 616c 6c20 7468 6520 7465 7874  ine all the text
-00000640: 2064 6174 6120 696e 746f 2061 2073 696e   data into a sin
-00000650: 676c 6520 7374 7269 6e67 0d0a 2020 2020  gle string..    
-00000660: 2020 7465 7874 5f64 6174 6120 3d20 2220    text_data = " 
-00000670: 222e 6a6f 696e 2864 665b 7465 7874 5f63  ".join(df[text_c
-00000680: 6f6c 756d 6e5d 2e61 7374 7970 6528 7374  olumn].astype(st
-00000690: 7229 2e74 6f6c 6973 7428 2929 0d0a 0d0a  r).tolist())....
-000006a0: 2020 2020 2020 2320 546f 6b65 6e69 7a65        # Tokenize
-000006b0: 2074 6865 2074 6578 7420 6461 7461 2028   the text data (
-000006c0: 7370 6c69 7420 696e 746f 2077 6f72 6473  split into words
-000006d0: 290d 0a20 2020 2020 2077 6f72 6473 203d  )..      words =
-000006e0: 2074 6578 745f 6461 7461 2e73 706c 6974   text_data.split
-000006f0: 2829 0d0a 0d0a 2020 2020 2020 2320 4765  ()....      # Ge
-00000700: 6e65 7261 7465 206e 2d67 7261 6d73 2066  nerate n-grams f
-00000710: 726f 6d20 7468 6520 776f 7264 730d 0a20  rom the words.. 
-00000720: 2020 2020 206e 5f67 7261 6d73 203d 206c       n_grams = l
-00000730: 6973 7428 6e67 7261 6d73 2877 6f72 6473  ist(ngrams(words
-00000740: 2c20 6e29 290d 0a0d 0a20 2020 2020 2023  , n))....      #
-00000750: 2050 6572 666f 726d 206e 2d67 7261 6d20   Perform n-gram 
-00000760: 636f 756e 7420 7573 696e 6720 7468 6520  count using the 
-00000770: 436f 756e 7465 7220 636c 6173 730d 0a20  Counter class.. 
-00000780: 2020 2020 206e 5f67 7261 6d5f 636f 756e       n_gram_coun
-00000790: 7420 3d20 436f 756e 7465 7228 6e5f 6772  t = Counter(n_gr
-000007a0: 616d 7329 0d0a 0d0a 2020 2020 2020 7265  ams)....      re
-000007b0: 7475 726e 206e 5f67 7261 6d5f 636f 756e  turn n_gram_coun
-000007c0: 740d 0a0d 0a20 2023 2053 7465 7020 343a  t....  # Step 4:
-000007d0: 2041 6c6c 6f77 2074 6865 2075 7365 7220   Allow the user 
-000007e0: 746f 2075 706c 6f61 6420 7468 6520 4353  to upload the CS
-000007f0: 5620 6669 6c65 0d0a 2020 7570 6c6f 6164  V file..  upload
-00000800: 6564 203d 2066 696c 6573 2e75 706c 6f61  ed = files.uploa
-00000810: 6428 290d 0a0d 0a20 2023 2053 7465 7020  d()....  # Step 
-00000820: 353a 2050 6572 666f 726d 2077 6f72 6420  5: Perform word 
-00000830: 636f 756e 7420 616e 616c 7973 6973 2061  count analysis a
-00000840: 6e64 2064 6973 706c 6179 2074 6865 2072  nd display the r
-00000850: 6573 756c 7473 0d0a 2020 6966 206c 656e  esults..  if len
-00000860: 2875 706c 6f61 6465 6429 203e 2030 3a0d  (uploaded) > 0:.
-00000870: 0a20 2020 2020 2023 2047 6574 2074 6865  .      # Get the
-00000880: 2075 706c 6f61 6465 6420 6669 6c65 206e   uploaded file n
-00000890: 616d 650d 0a20 2020 2020 2063 7376 5f66  ame..      csv_f
-000008a0: 696c 655f 6e61 6d65 203d 206c 6973 7428  ile_name = list(
-000008b0: 7570 6c6f 6164 6564 2e6b 6579 7328 2929  uploaded.keys())
-000008c0: 5b30 5d0d 0a0d 0a20 2020 2020 2023 2047  [0]....      # G
-000008d0: 6574 2074 6865 2063 6f6c 756d 6e20 6e61  et the column na
-000008e0: 6d65 2074 6861 7420 636f 6e74 6169 6e73  me that contains
-000008f0: 2074 6578 7420 6461 7461 0d0a 2020 2020   text data..    
-00000900: 2020 7465 7874 5f63 6f6c 756d 6e20 3d20    text_column = 
-00000910: 696e 7075 7428 2245 6e74 6572 2074 6865  input("Enter the
-00000920: 2063 6f6c 756d 6e20 6e61 6d65 2063 6f6e   column name con
-00000930: 7461 696e 696e 6720 7465 7874 2064 6174  taining text dat
-00000940: 613a 2022 290d 0a0d 0a20 2020 2020 2023  a: ")....      #
-00000950: 2047 6574 2074 6865 2064 6573 6972 6564   Get the desired
-00000960: 206e 2d67 7261 6d20 6c65 6e67 7468 2066   n-gram length f
-00000970: 726f 6d20 7468 6520 7573 6572 0d0a 2020  rom the user..  
-00000980: 2020 2020 6e20 3d20 696e 7428 696e 7075      n = int(inpu
-00000990: 7428 2245 6e74 6572 2074 6865 2064 6573  t("Enter the des
-000009a0: 6972 6564 206e 2d67 7261 6d20 6c65 6e67  ired n-gram leng
-000009b0: 7468 2028 652e 672e 2c20 3220 666f 7220  th (e.g., 2 for 
-000009c0: 6269 6772 616d 732c 2033 2066 6f72 2074  bigrams, 3 for t
-000009d0: 7269 6772 616d 732c 2065 7463 2e29 3a20  rigrams, etc.): 
-000009e0: 2229 290d 0a0d 0a20 2020 2020 2023 2047  "))....      # G
-000009f0: 6574 2074 6865 206e 756d 6265 7220 6f66  et the number of
-00000a00: 2072 756c 6573 2074 6865 2075 7365 7220   rules the user 
-00000a10: 7761 6e74 7320 746f 2067 656e 6572 6174  wants to generat
-00000a20: 650d 0a20 2020 2020 206e 756d 5f72 756c  e..      num_rul
-00000a30: 6573 203d 2069 6e74 2869 6e70 7574 2822  es = int(input("
-00000a40: 456e 7465 7220 7468 6520 6e75 6d62 6572  Enter the number
-00000a50: 206f 6620 7275 6c65 7320 796f 7520 7761   of rules you wa
-00000a60: 6e74 2074 6f20 6765 6e65 7261 7465 3a20  nt to generate: 
-00000a70: 2229 290d 0a0d 0a20 2020 2020 2023 2050  "))....      # P
-00000a80: 6572 666f 726d 2077 6f72 6420 636f 756e  erform word coun
-00000a90: 7420 616e 616c 7973 6973 2077 6974 6820  t analysis with 
-00000aa0: 6e2d 6772 616d 730d 0a20 2020 2020 206e  n-grams..      n
-00000ab0: 5f67 7261 6d5f 636f 756e 745f 7265 7375  _gram_count_resu
-00000ac0: 6c74 203d 2077 6f72 645f 636f 756e 745f  lt = word_count_
-00000ad0: 616e 616c 7973 6973 2869 6f2e 4279 7465  analysis(io.Byte
-00000ae0: 7349 4f28 7570 6c6f 6164 6564 5b63 7376  sIO(uploaded[csv
-00000af0: 5f66 696c 655f 6e61 6d65 5d29 2c20 7465  _file_name]), te
-00000b00: 7874 5f63 6f6c 756d 6e2c 206e 290d 0a0d  xt_column, n)...
-00000b10: 0a20 2020 2020 2023 2047 6574 2074 6865  .      # Get the
-00000b20: 2074 6f70 206e 206e 2d67 7261 6d73 2061   top n n-grams a
-00000b30: 6e64 2074 6865 6972 2063 6f75 6e74 730d  nd their counts.
-00000b40: 0a20 2020 2020 2074 6f70 5f6e 5f6e 5f67  .      top_n_n_g
-00000b50: 7261 6d73 203d 206e 5f67 7261 6d5f 636f  rams = n_gram_co
-00000b60: 756e 745f 7265 7375 6c74 2e6d 6f73 745f  unt_result.most_
-00000b70: 636f 6d6d 6f6e 286e 756d 5f72 756c 6573  common(num_rules
-00000b80: 290d 0a0d 0a20 2020 2020 2023 2044 6973  )....      # Dis
-00000b90: 706c 6179 2074 6865 2074 6f70 206e 206e  play the top n n
-00000ba0: 2d67 7261 6d73 2061 6e64 2074 6865 6972  -grams and their
-00000bb0: 2063 6f75 6e74 730d 0a20 2020 2020 2070   counts..      p
-00000bc0: 7269 6e74 2866 225c 6e54 6f70 207b 6e75  rint(f"\nTop {nu
-00000bd0: 6d5f 7275 6c65 737d 207b 6e7d 2d67 7261  m_rules} {n}-gra
-00000be0: 6d73 3a22 290d 0a20 2020 2020 2066 6f72  ms:")..      for
-00000bf0: 206e 5f67 7261 6d2c 2063 6f75 6e74 2069   n_gram, count i
-00000c00: 6e20 746f 705f 6e5f 6e5f 6772 616d 733a  n top_n_n_grams:
-00000c10: 0d0a 2020 2020 2020 2020 2020 7072 696e  ..          prin
-00000c20: 7428 6622 7b27 2027 2e6a 6f69 6e28 6e5f  t(f"{' '.join(n_
-00000c30: 6772 616d 297d 3a20 7b63 6f75 6e74 7d22  gram)}: {count}"
-00000c40: 290d 0a0d 0a20 2020 2020 2023 2053 6176  )....      # Sav
-00000c50: 6520 7468 6520 746f 7020 6e20 6e2d 6772  e the top n n-gr
-00000c60: 616d 7320 616e 6420 7468 6569 7220 636f  ams and their co
-00000c70: 756e 7473 2074 6f20 6120 4353 5620 6669  unts to a CSV fi
-00000c80: 6c65 0d0a 2020 2020 2020 6f75 7470 7574  le..      output
-00000c90: 5f66 696c 655f 6e61 6d65 203d 2066 2274  _file_name = f"t
-00000ca0: 6f70 5f7b 6e7d 5f67 7261 6d73 2e63 7376  op_{n}_grams.csv
-00000cb0: 220d 0a20 2020 2020 2077 6974 6820 6f70  "..      with op
-00000cc0: 656e 286f 7574 7075 745f 6669 6c65 5f6e  en(output_file_n
-00000cd0: 616d 652c 2027 7727 2c20 6e65 776c 696e  ame, 'w', newlin
-00000ce0: 653d 2727 2920 6173 2063 7376 6669 6c65  e='') as csvfile
-00000cf0: 3a0d 0a20 2020 2020 2020 2020 2063 7376  :..          csv
-00000d00: 5f77 7269 7465 7220 3d20 6373 762e 7772  _writer = csv.wr
-00000d10: 6974 6572 2863 7376 6669 6c65 290d 0a20  iter(csvfile).. 
-00000d20: 2020 2020 2020 2020 2063 7376 5f77 7269           csv_wri
-00000d30: 7465 722e 7772 6974 6572 6f77 285b 6622  ter.writerow([f"
-00000d40: 546f 7020 7b6e 7d2d 6772 616d 7322 2c20  Top {n}-grams", 
-00000d50: 2243 6f75 6e74 225d 290d 0a20 2020 2020  "Count"])..     
-00000d60: 2020 2020 2066 6f72 206e 5f67 7261 6d2c       for n_gram,
-00000d70: 2063 6f75 6e74 2069 6e20 746f 705f 6e5f   count in top_n_
-00000d80: 6e5f 6772 616d 733a 0d0a 2020 2020 2020  n_grams:..      
-00000d90: 2020 2020 2020 2020 6373 765f 7772 6974          csv_writ
-00000da0: 6572 2e77 7269 7465 726f 7728 5b27 2027  er.writerow([' '
-00000db0: 2e6a 6f69 6e28 6e5f 6772 616d 292c 2063  .join(n_gram), c
-00000dc0: 6f75 6e74 5d29 0d0a 0d0a 2020 2020 2020  ount])....      
-00000dd0: 2320 5072 6f76 6964 6520 6120 6c69 6e6b  # Provide a link
-00000de0: 2074 6f20 646f 776e 6c6f 6164 2074 6865   to download the
-00000df0: 2043 5356 2066 696c 650d 0a20 2020 2020   CSV file..     
-00000e00: 2070 7269 6e74 2866 225c 6e52 6573 756c   print(f"\nResul
-00000e10: 7473 2073 6176 6564 2074 6f3a 207b 6f75  ts saved to: {ou
-00000e20: 7470 7574 5f66 696c 655f 6e61 6d65 7d22  tput_file_name}"
-00000e30: 290d 0a20 2065 6c73 653a 0d0a 2020 2020  )..  else:..    
-00000e40: 2020 7072 696e 7428 224e 6f20 6669 6c65    print("No file
-00000e50: 2075 706c 6f61 6465 642e 2229 0d0a        uploaded.")..
+00000460: 6429 0d0a 2020 7069 7020 696e 7374 616c  d)..  pip instal
+00000470: 6c20 7061 6e64 6173 206e 6c74 6b0d 0a0d  l pandas nltk...
+00000480: 0a20 2023 2053 7465 7020 323a 2049 6d70  .  # Step 2: Imp
+00000490: 6f72 7420 7468 6520 7265 7175 6972 6564  ort the required
+000004a0: 206c 6962 7261 7269 6573 0d0a 2020 696d   libraries..  im
+000004b0: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
+000004c0: 640d 0a20 2066 726f 6d20 636f 6c6c 6563  d..  from collec
+000004d0: 7469 6f6e 7320 696d 706f 7274 2043 6f75  tions import Cou
+000004e0: 6e74 6572 0d0a 2020 696d 706f 7274 2069  nter..  import i
+000004f0: 6f0d 0a20 2066 726f 6d20 676f 6f67 6c65  o..  from google
+00000500: 2e63 6f6c 6162 2069 6d70 6f72 7420 6669  .colab import fi
+00000510: 6c65 730d 0a20 2069 6d70 6f72 7420 6e6c  les..  import nl
+00000520: 746b 0d0a 2020 6672 6f6d 206e 6c74 6b2e  tk..  from nltk.
+00000530: 7574 696c 2069 6d70 6f72 7420 6e67 7261  util import ngra
+00000540: 6d73 0d0a 2020 696d 706f 7274 2063 7376  ms..  import csv
+00000550: 0d0a 0d0a 2020 2320 5374 6570 2033 3a20  ....  # Step 3: 
+00000560: 4675 6e63 7469 6f6e 2074 6f20 7065 7266  Function to perf
+00000570: 6f72 6d20 776f 7264 2063 6f75 6e74 2061  orm word count a
+00000580: 6e61 6c79 7369 7320 7769 7468 206e 2d67  nalysis with n-g
+00000590: 7261 6d73 0d0a 2020 6465 6620 776f 7264  rams..  def word
+000005a0: 5f63 6f75 6e74 5f61 6e61 6c79 7369 7328  _count_analysis(
+000005b0: 6373 765f 6669 6c65 2c20 7465 7874 5f63  csv_file, text_c
+000005c0: 6f6c 756d 6e2c 206e 293a 0d0a 2020 2020  olumn, n):..    
+000005d0: 2020 2320 5265 6164 2074 6865 2043 5356    # Read the CSV
+000005e0: 2066 696c 6520 696e 746f 2061 2070 616e   file into a pan
+000005f0: 6461 7320 4461 7461 4672 616d 650d 0a20  das DataFrame.. 
+00000600: 2020 2020 2064 6620 3d20 7064 2e72 6561       df = pd.rea
+00000610: 645f 6373 7628 6373 765f 6669 6c65 290d  d_csv(csv_file).
+00000620: 0a0d 0a20 2020 2020 2023 2043 6f6d 6269  ...      # Combi
+00000630: 6e65 2061 6c6c 2074 6865 2074 6578 7420  ne all the text 
+00000640: 6461 7461 2069 6e74 6f20 6120 7369 6e67  data into a sing
+00000650: 6c65 2073 7472 696e 670d 0a20 2020 2020  le string..     
+00000660: 2074 6578 745f 6461 7461 203d 2022 2022   text_data = " "
+00000670: 2e6a 6f69 6e28 6466 5b74 6578 745f 636f  .join(df[text_co
+00000680: 6c75 6d6e 5d2e 6173 7479 7065 2873 7472  lumn].astype(str
+00000690: 292e 746f 6c69 7374 2829 290d 0a0d 0a20  ).tolist()).... 
+000006a0: 2020 2020 2023 2054 6f6b 656e 697a 6520       # Tokenize 
+000006b0: 7468 6520 7465 7874 2064 6174 6120 2873  the text data (s
+000006c0: 706c 6974 2069 6e74 6f20 776f 7264 7329  plit into words)
+000006d0: 0d0a 2020 2020 2020 776f 7264 7320 3d20  ..      words = 
+000006e0: 7465 7874 5f64 6174 612e 7370 6c69 7428  text_data.split(
+000006f0: 290d 0a0d 0a20 2020 2020 2023 2047 656e  )....      # Gen
+00000700: 6572 6174 6520 6e2d 6772 616d 7320 6672  erate n-grams fr
+00000710: 6f6d 2074 6865 2077 6f72 6473 0d0a 2020  om the words..  
+00000720: 2020 2020 6e5f 6772 616d 7320 3d20 6c69      n_grams = li
+00000730: 7374 286e 6772 616d 7328 776f 7264 732c  st(ngrams(words,
+00000740: 206e 2929 0d0a 0d0a 2020 2020 2020 2320   n))....      # 
+00000750: 5065 7266 6f72 6d20 6e2d 6772 616d 2063  Perform n-gram c
+00000760: 6f75 6e74 2075 7369 6e67 2074 6865 2043  ount using the C
+00000770: 6f75 6e74 6572 2063 6c61 7373 0d0a 2020  ounter class..  
+00000780: 2020 2020 6e5f 6772 616d 5f63 6f75 6e74      n_gram_count
+00000790: 203d 2043 6f75 6e74 6572 286e 5f67 7261   = Counter(n_gra
+000007a0: 6d73 290d 0a0d 0a20 2020 2020 2072 6574  ms)....      ret
+000007b0: 7572 6e20 6e5f 6772 616d 5f63 6f75 6e74  urn n_gram_count
+000007c0: 0d0a 0d0a 2020 2320 5374 6570 2034 3a20  ....  # Step 4: 
+000007d0: 416c 6c6f 7720 7468 6520 7573 6572 2074  Allow the user t
+000007e0: 6f20 7570 6c6f 6164 2074 6865 2043 5356  o upload the CSV
+000007f0: 2066 696c 650d 0a20 2075 706c 6f61 6465   file..  uploade
+00000800: 6420 3d20 6669 6c65 732e 7570 6c6f 6164  d = files.upload
+00000810: 2829 0d0a 0d0a 2020 2320 5374 6570 2035  ()....  # Step 5
+00000820: 3a20 5065 7266 6f72 6d20 776f 7264 2063  : Perform word c
+00000830: 6f75 6e74 2061 6e61 6c79 7369 7320 616e  ount analysis an
+00000840: 6420 6469 7370 6c61 7920 7468 6520 7265  d display the re
+00000850: 7375 6c74 730d 0a20 2069 6620 6c65 6e28  sults..  if len(
+00000860: 7570 6c6f 6164 6564 2920 3e20 303a 0d0a  uploaded) > 0:..
+00000870: 2020 2020 2020 2320 4765 7420 7468 6520        # Get the 
+00000880: 7570 6c6f 6164 6564 2066 696c 6520 6e61  uploaded file na
+00000890: 6d65 0d0a 2020 2020 2020 6373 765f 6669  me..      csv_fi
+000008a0: 6c65 5f6e 616d 6520 3d20 6c69 7374 2875  le_name = list(u
+000008b0: 706c 6f61 6465 642e 6b65 7973 2829 295b  ploaded.keys())[
+000008c0: 305d 0d0a 0d0a 2020 2020 2020 2320 4765  0]....      # Ge
+000008d0: 7420 7468 6520 636f 6c75 6d6e 206e 616d  t the column nam
+000008e0: 6520 7468 6174 2063 6f6e 7461 696e 7320  e that contains 
+000008f0: 7465 7874 2064 6174 610d 0a20 2020 2020  text data..     
+00000900: 2074 6578 745f 636f 6c75 6d6e 203d 2069   text_column = i
+00000910: 6e70 7574 2822 456e 7465 7220 7468 6520  nput("Enter the 
+00000920: 636f 6c75 6d6e 206e 616d 6520 636f 6e74  column name cont
+00000930: 6169 6e69 6e67 2074 6578 7420 6461 7461  aining text data
+00000940: 3a20 2229 0d0a 0d0a 2020 2020 2020 2320  : ")....      # 
+00000950: 4765 7420 7468 6520 6465 7369 7265 6420  Get the desired 
+00000960: 6e2d 6772 616d 206c 656e 6774 6820 6672  n-gram length fr
+00000970: 6f6d 2074 6865 2075 7365 720d 0a20 2020  om the user..   
+00000980: 2020 206e 203d 2069 6e74 2869 6e70 7574     n = int(input
+00000990: 2822 456e 7465 7220 7468 6520 6465 7369  ("Enter the desi
+000009a0: 7265 6420 6e2d 6772 616d 206c 656e 6774  red n-gram lengt
+000009b0: 6820 2865 2e67 2e2c 2032 2066 6f72 2062  h (e.g., 2 for b
+000009c0: 6967 7261 6d73 2c20 3320 666f 7220 7472  igrams, 3 for tr
+000009d0: 6967 7261 6d73 2c20 6574 632e 293a 2022  igrams, etc.): "
+000009e0: 2929 0d0a 0d0a 2020 2020 2020 2320 4765  ))....      # Ge
+000009f0: 7420 7468 6520 6e75 6d62 6572 206f 6620  t the number of 
+00000a00: 7275 6c65 7320 7468 6520 7573 6572 2077  rules the user w
+00000a10: 616e 7473 2074 6f20 6765 6e65 7261 7465  ants to generate
+00000a20: 0d0a 2020 2020 2020 6e75 6d5f 7275 6c65  ..      num_rule
+00000a30: 7320 3d20 696e 7428 696e 7075 7428 2245  s = int(input("E
+00000a40: 6e74 6572 2074 6865 206e 756d 6265 7220  nter the number 
+00000a50: 6f66 2072 756c 6573 2079 6f75 2077 616e  of rules you wan
+00000a60: 7420 746f 2067 656e 6572 6174 653a 2022  t to generate: "
+00000a70: 2929 0d0a 0d0a 2020 2020 2020 2320 5065  ))....      # Pe
+00000a80: 7266 6f72 6d20 776f 7264 2063 6f75 6e74  rform word count
+00000a90: 2061 6e61 6c79 7369 7320 7769 7468 206e   analysis with n
+00000aa0: 2d67 7261 6d73 0d0a 2020 2020 2020 6e5f  -grams..      n_
+00000ab0: 6772 616d 5f63 6f75 6e74 5f72 6573 756c  gram_count_resul
+00000ac0: 7420 3d20 776f 7264 5f63 6f75 6e74 5f61  t = word_count_a
+00000ad0: 6e61 6c79 7369 7328 696f 2e42 7974 6573  nalysis(io.Bytes
+00000ae0: 494f 2875 706c 6f61 6465 645b 6373 765f  IO(uploaded[csv_
+00000af0: 6669 6c65 5f6e 616d 655d 292c 2074 6578  file_name]), tex
+00000b00: 745f 636f 6c75 6d6e 2c20 6e29 0d0a 0d0a  t_column, n)....
+00000b10: 2020 2020 2020 2320 4765 7420 7468 6520        # Get the 
+00000b20: 746f 7020 6e20 6e2d 6772 616d 7320 616e  top n n-grams an
+00000b30: 6420 7468 6569 7220 636f 756e 7473 0d0a  d their counts..
+00000b40: 2020 2020 2020 746f 705f 6e5f 6e5f 6772        top_n_n_gr
+00000b50: 616d 7320 3d20 6e5f 6772 616d 5f63 6f75  ams = n_gram_cou
+00000b60: 6e74 5f72 6573 756c 742e 6d6f 7374 5f63  nt_result.most_c
+00000b70: 6f6d 6d6f 6e28 6e75 6d5f 7275 6c65 7329  ommon(num_rules)
+00000b80: 0d0a 0d0a 2020 2020 2020 2320 4469 7370  ....      # Disp
+00000b90: 6c61 7920 7468 6520 746f 7020 6e20 6e2d  lay the top n n-
+00000ba0: 6772 616d 7320 616e 6420 7468 6569 7220  grams and their 
+00000bb0: 636f 756e 7473 0d0a 2020 2020 2020 7072  counts..      pr
+00000bc0: 696e 7428 6622 5c6e 546f 7020 7b6e 756d  int(f"\nTop {num
+00000bd0: 5f72 756c 6573 7d20 7b6e 7d2d 6772 616d  _rules} {n}-gram
+00000be0: 733a 2229 0d0a 2020 2020 2020 666f 7220  s:")..      for 
+00000bf0: 6e5f 6772 616d 2c20 636f 756e 7420 696e  n_gram, count in
+00000c00: 2074 6f70 5f6e 5f6e 5f67 7261 6d73 3a0d   top_n_n_grams:.
+00000c10: 0a20 2020 2020 2020 2020 2070 7269 6e74  .          print
+00000c20: 2866 227b 2720 272e 6a6f 696e 286e 5f67  (f"{' '.join(n_g
+00000c30: 7261 6d29 7d3a 207b 636f 756e 747d 2229  ram)}: {count}")
+00000c40: 0d0a 0d0a 2020 2020 2020 2320 5361 7665  ....      # Save
+00000c50: 2074 6865 2074 6f70 206e 206e 2d67 7261   the top n n-gra
+00000c60: 6d73 2061 6e64 2074 6865 6972 2063 6f75  ms and their cou
+00000c70: 6e74 7320 746f 2061 2043 5356 2066 696c  nts to a CSV fil
+00000c80: 650d 0a20 2020 2020 206f 7574 7075 745f  e..      output_
+00000c90: 6669 6c65 5f6e 616d 6520 3d20 6622 746f  file_name = f"to
+00000ca0: 705f 7b6e 7d5f 6772 616d 732e 6373 7622  p_{n}_grams.csv"
+00000cb0: 0d0a 2020 2020 2020 7769 7468 206f 7065  ..      with ope
+00000cc0: 6e28 6f75 7470 7574 5f66 696c 655f 6e61  n(output_file_na
+00000cd0: 6d65 2c20 2777 272c 206e 6577 6c69 6e65  me, 'w', newline
+00000ce0: 3d27 2729 2061 7320 6373 7666 696c 653a  ='') as csvfile:
+00000cf0: 0d0a 2020 2020 2020 2020 2020 6373 765f  ..          csv_
+00000d00: 7772 6974 6572 203d 2063 7376 2e77 7269  writer = csv.wri
+00000d10: 7465 7228 6373 7666 696c 6529 0d0a 2020  ter(csvfile)..  
+00000d20: 2020 2020 2020 2020 6373 765f 7772 6974          csv_writ
+00000d30: 6572 2e77 7269 7465 726f 7728 5b66 2254  er.writerow([f"T
+00000d40: 6f70 207b 6e7d 2d67 7261 6d73 222c 2022  op {n}-grams", "
+00000d50: 436f 756e 7422 5d29 0d0a 2020 2020 2020  Count"])..      
+00000d60: 2020 2020 666f 7220 6e5f 6772 616d 2c20      for n_gram, 
+00000d70: 636f 756e 7420 696e 2074 6f70 5f6e 5f6e  count in top_n_n
+00000d80: 5f67 7261 6d73 3a0d 0a20 2020 2020 2020  _grams:..       
+00000d90: 2020 2020 2020 2063 7376 5f77 7269 7465         csv_write
+00000da0: 722e 7772 6974 6572 6f77 285b 2720 272e  r.writerow([' '.
+00000db0: 6a6f 696e 286e 5f67 7261 6d29 2c20 636f  join(n_gram), co
+00000dc0: 756e 745d 290d 0a0d 0a20 2020 2020 2023  unt])....      #
+00000dd0: 2050 726f 7669 6465 2061 206c 696e 6b20   Provide a link 
+00000de0: 746f 2064 6f77 6e6c 6f61 6420 7468 6520  to download the 
+00000df0: 4353 5620 6669 6c65 0d0a 2020 2020 2020  CSV file..      
+00000e00: 7072 696e 7428 6622 5c6e 5265 7375 6c74  print(f"\nResult
+00000e10: 7320 7361 7665 6420 746f 3a20 7b6f 7574  s saved to: {out
+00000e20: 7075 745f 6669 6c65 5f6e 616d 657d 2229  put_file_name}")
+00000e30: 0d0a 2020 656c 7365 3a0d 0a20 2020 2020  ..  else:..     
+00000e40: 2070 7269 6e74 2822 4e6f 2066 696c 6520   print("No file 
+00000e50: 7570 6c6f 6164 6564 2e22 290d 0a         uploaded.")..
```

### Comparing `textco-0.0.3/textco.egg-info/PKG-INFO` & `textco-0.0.4/textco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textco
-Version: 0.0.3
+Version: 0.0.4
 Summary: TEXT analytsis COpilot
 Home-page: UNKNOWN
 Author: Dr Anna Sung and Prof Kelvin Leong
 Author-email: <k.leong@chester.ac.uk>
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

