# Comparing `tmp/mpnp-0.1.5-py3-none-any.whl.zip` & `tmp/mpnp-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 20872 bytes, number of entries: 9
--rw-rw-r--  2.0 unx     1302 b- defN 22-Dec-04 21:23 mpnp/data_preprocessing.py
+Zip file size: 20958 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx     1375 b- defN 23-Jun-13 11:30 mpnp/data_preprocessing.py
 -rw-rw-r--  2.0 unx    33039 b- defN 23-Apr-08 00:32 mpnp/experiment.py
 -rw-rw-r--  2.0 unx    17652 b- defN 23-Apr-08 01:04 mpnp/notebook_application.py
--rw-rw-r--  2.0 unx     3931 b- defN 23-Apr-07 21:39 mpnp/utilities.py
--rw-rw-r--  2.0 unx    15087 b- defN 23-Apr-08 02:45 mpnp-0.1.5.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     1162 b- defN 23-Apr-08 02:45 mpnp-0.1.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-08 02:45 mpnp-0.1.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Apr-08 02:45 mpnp-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      694 b- defN 23-Apr-08 02:45 mpnp-0.1.5.dist-info/RECORD
-9 files, 72964 bytes uncompressed, 19692 bytes compressed:  73.0%
+-rw-rw-r--  2.0 unx     4146 b- defN 23-Jun-13 11:42 mpnp/utilities.py
+-rw-rw-r--  2.0 unx    15087 b- defN 23-Jul-26 02:30 mpnp-0.1.6.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     1162 b- defN 23-Jul-26 02:30 mpnp-0.1.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-26 02:30 mpnp-0.1.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jul-26 02:30 mpnp-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      694 b- defN 23-Jul-26 02:30 mpnp-0.1.6.dist-info/RECORD
+9 files, 73252 bytes uncompressed, 19778 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: mpnp/notebook_application.py
 Comment: 
 
 Filename: mpnp/utilities.py
 Comment: 
 
-Filename: mpnp-0.1.5.dist-info/LICENSE.txt
+Filename: mpnp-0.1.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: mpnp-0.1.5.dist-info/METADATA
+Filename: mpnp-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: mpnp-0.1.5.dist-info/WHEEL
+Filename: mpnp-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: mpnp-0.1.5.dist-info/top_level.txt
+Filename: mpnp-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: mpnp-0.1.5.dist-info/RECORD
+Filename: mpnp-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mpnp/data_preprocessing.py

```diff
@@ -19,16 +19,20 @@
 def v_discretization( y, bins = 3, decreasing = False ):
 
 
 	ndim = y.ndim
 	if ndim > 1: ndim = y.shape[ 1 ]
 
 
+	nbins = bins
+	if type( bins ) is not int: nbins = len( bins ) - 1
+
+
 	hists = []
-	count = [ 0 ] * bins
+	count = [ 0 ] * nbins
 	mat_count = []
 
 
 
 	if ndim == 1: 
 		hists.append( np.histogram( y, bins = bins ) )
 		mat_count.append( count )
@@ -45,25 +49,25 @@
 
 	for i in range( y.shape[ 0 ] ):
 
 		row = [ -1 ] * ndim
 
 		for j in range( ndim ): 
 			
-			for b in range( bins ):
+			for b in range( nbins ):
 
 				if ndim == 1: y_ij = y[ i ]
 				else: y_ij = y[ i, j ]
 
-				if ( y_ij >= hists[ j ][ 1 ][ b ] ) and ( ( y_ij < hists[ j ][ 1 ][ b + 1 ] ) or ( b == bins - 1 ) ):
+				if ( y_ij >= hists[ j ][ 1 ][ b ] ) and ( ( y_ij < hists[ j ][ 1 ][ b + 1 ] ) or ( b == nbins - 1 ) ):
 
 					mat_count[ j, b ] += 1
 					
 					if decreasing == False: row[ j ] = b
-					else: row[ j ] = ( bins - 1 ) - b
+					else: row[ j ] = ( nbins - 1 ) - b
 
 					break
 
 		mat.append( row )
 
 	mat = np.array( mat )
```

## mpnp/utilities.py

```diff
@@ -1,39 +1,45 @@
 #coding=utf-8
 from datetime import datetime
 import platform
 import numpy as np
 import os
 from sklearn.feature_extraction.text import TfidfVectorizer
 import csv
+import sys
 
 
 
 
 
 
 
 
 
 
 
-def create_readme( author = '', msg = '', folder = './', authorization_header = True ):
+def create_readme( author = '', msg = '', folder = './', authorization_header = True, by_date = False ):
 
 
-	writer = open( folder + 'README.txt', 'w' )
+	now = datetime.now()
+
+	file_name = 'README'
+	if by_date == True: file_name += '_' + now.strftime( '%d%m%Y' )
+	file_name += '.txt'
+
+	writer = open( folder + file_name, 'w' )
 	separator = '-----------------------------------\n\n\n'
 
 	text = ''
 	line = ''
 
 	line = 'Author: ' + author + '\n'
 	writer.write( line )
 	text += line
 
-	now = datetime.now()
 	line = now.strftime( '%d/%m/%Y %H:%M:%S' ) + '\n\n'
 	writer.write( line )
 	text += line
 
 	if authorization_header == True: 
 		line = 'This project can not be used without its author\'s full and express authorization.\n'
 		writer.write( line )
@@ -65,14 +71,18 @@
 	writer.write( line )
 	text += line
 
 	line = 'Python Implementation: ' + platform.python_implementation() + '\n'
 	writer.write( line )
 	text += line
 
+	line = 'sys.prefix: ' + sys.prefix + '\n'
+	writer.write( line )
+	text += line
+
 	writer.write( separator )
 	text += separator
 
 
 	line = 'Python Packages (pip freeze):\n\n'
 	writer.write( line )
 	text += line
```

## Comparing `mpnp-0.1.5.dist-info/LICENSE.txt` & `mpnp-0.1.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `mpnp-0.1.5.dist-info/METADATA` & `mpnp-0.1.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpnp
-Version: 0.1.5
+Version: 0.1.6
 Summary: Mário Popolin Neto Package.
 Home-page: https://gitlab.com/popolinneto/mpnp
 Author: Mario Popolin Neto
 Author-email: mariopopolin@gmail.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International
 Platform: UNKNOWN
 Classifier: License :: Free for non-commercial use
```

## Comparing `mpnp-0.1.5.dist-info/RECORD` & `mpnp-0.1.6.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-mpnp/data_preprocessing.py,sha256=73g8AfaSPkFBJKExW3PaRco6ktZjrdurKoz4WgXkn5w,1302
+mpnp/data_preprocessing.py,sha256=NimJ20tQJasn_iDubx7TiJxAX5dI8yUbJTqgb3ZzALU,1375
 mpnp/experiment.py,sha256=SlSgFwOIKpiljXPGKxYjUjpKTKm2IEdHDmRen49zDyU,33039
 mpnp/notebook_application.py,sha256=YC-RZw8-qvgjxog7gt5G59qVrzOL9V8O1oX4nv4JkF4,17652
-mpnp/utilities.py,sha256=dQk6IOmIbV7IHKZbIGGiwLRsEL25ErlbN5TBR3jwiDI,3931
-mpnp-0.1.5.dist-info/LICENSE.txt,sha256=FB_n6crTurfb2TE61kPWEyNzpPkCqBLCMzwIAUTqw1U,15087
-mpnp-0.1.5.dist-info/METADATA,sha256=Nu0kyvavX8LtrZ3rayzEN0t6npp_qcCwEBii_LLioag,1162
-mpnp-0.1.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mpnp-0.1.5.dist-info/top_level.txt,sha256=5sfiEMoCLdFC3hCESBpvs7cZ_s0BsZ-4Zo_VbEm36u4,5
-mpnp-0.1.5.dist-info/RECORD,,
+mpnp/utilities.py,sha256=zE7IiioaBm6wAaESDMTKkY9keT-1v5eCCT9Z0clYlHw,4146
+mpnp-0.1.6.dist-info/LICENSE.txt,sha256=FB_n6crTurfb2TE61kPWEyNzpPkCqBLCMzwIAUTqw1U,15087
+mpnp-0.1.6.dist-info/METADATA,sha256=FQ04B_yhgfF_TH145Frap-oaPSIZ_OsYEoqPf73GrfU,1162
+mpnp-0.1.6.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+mpnp-0.1.6.dist-info/top_level.txt,sha256=5sfiEMoCLdFC3hCESBpvs7cZ_s0BsZ-4Zo_VbEm36u4,5
+mpnp-0.1.6.dist-info/RECORD,,
```

