# Comparing `tmp/tdasha-0.2.2.tar.gz` & `tmp/tdasha-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdasha-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tdasha-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tdasha-0.2.2.tar` & `tdasha-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-06-22 17:06:22.760869 tdasha-0.2.2/LICENSE
--rw-r--r--   0        0        0        8 2023-06-22 17:06:22.760869 tdasha-0.2.2/README.md
--rw-r--r--   0        0        0     1063 2023-06-22 17:06:22.760869 tdasha-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      388 2023-06-22 17:06:22.760869 tdasha-0.2.2/tdasha/__init__.py
--rw-r--r--   0        0        0    13900 2023-06-22 17:06:22.760869 tdasha-0.2.2/tdasha/compute.py
--rw-r--r--   0        0        0     3803 2023-06-22 17:06:22.760869 tdasha-0.2.2/tdasha/io.py
--rw-r--r--   0        0        0     8645 2023-06-22 17:06:22.760869 tdasha-0.2.2/tdasha/window.py
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 tdasha-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-26 15:55:42.077582 tdasha-0.2.3/LICENSE
+-rw-r--r--   0        0        0        8 2023-07-26 15:55:42.077582 tdasha-0.2.3/README.md
+-rw-r--r--   0        0        0     1063 2023-07-26 15:55:42.077582 tdasha-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      388 2023-07-26 15:55:42.077582 tdasha-0.2.3/tdasha/__init__.py
+-rw-r--r--   0        0        0     7085 2023-07-26 15:55:42.077582 tdasha-0.2.3/tdasha/compute.py
+-rw-r--r--   0        0        0     3811 2023-07-26 15:55:42.077582 tdasha-0.2.3/tdasha/io.py
+-rw-r--r--   0        0        0     8935 2023-07-26 15:55:42.081582 tdasha-0.2.3/tdasha/window.py
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 tdasha-0.2.3/PKG-INFO
```

### Comparing `tdasha-0.2.2/LICENSE` & `tdasha-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tdasha-0.2.2/pyproject.toml` & `tdasha-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tdasha-0.2.2/tdasha/io.py` & `tdasha-0.2.3/tdasha/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             time_frame = mat['Catalog'][0][i]
             t1 = time_frame[2].flatten()
             datenums = np.array(t1)
             t2= pd.to_datetime(datenums-719529, unit='D') #convert from Matlab's datenum format to human readable format
             time = [UTCDateTime(str(t)) for t in t2] # convert to list of obspy UTCDateTime objects
             
     if len(mag)==0:
-        print("Magnitude column not found in .mat file")
+        print("Magnitude column not found in .mat file. Abort!")
         sys.exit()
 
     return time, mag
 
 def read_csv(csv_file,  datenum= True, **kwargs):
     
     # df = pd.read_csv(csv_file, engine="pyarrow", **kwargs) #use pyarrow for faster input
```

### Comparing `tdasha-0.2.2/tdasha/window.py` & `tdasha-0.2.3/tdasha/window.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,21 +84,23 @@
         #     h = bandwidth
                 
         # use KDEpy to estimate bandwidth
         if bw == 'ls':
             args = self.filter_args(kwargs, self.h_plat) #filter kwargs
             h = self.h_plat(x, **args)
         elif bw == 'ss':
-            args = self.filter_args(kwargs, sskernel) #filter kwargs
+            args = self.filter_args(kwargs, sskernel) 
             kde = sskernel(x, **args)
             h = kde[2]
-        # elif bw == 'ssv': #don't know how to use multiple bandwidth values in a window yet.
-        
+        elif bw == 'ssv':
+            args = self.filter_args(kwargs, ssvkernel)
+            kde = ssvkernel(x, tin=np.linspace(min(x),max(x),len(x)), **args)
+            h = kde[2] #returns array of bandwidths since there is a variable bandwidth across the window
         elif type(bw)==str: 
-            args = self.filter_args(kwargs, FFTKDE) #filter kwargs
+            args = self.filter_args(kwargs, FFTKDE)
             h = FFTKDE(bw=bw, **args).fit(x).bw            
         elif type(bw)==float:
             h = bw # use user-provided value for bandwidth
         
 
         
         return h
@@ -138,14 +140,18 @@
         # x - the n-element column vector of data values
         # h - the optimal smoothing factor
         # ambd - the resultant n-element row vector of local scaling factors
                 
         n = len(x)
         c = np.sqrt(2 * np.pi)
         gau = []
+        
+        # if isinstance(h, np.ndarray): #test if bandwidth is a numpy array
+            # print("Adaptivle locally variable bandwidth used")
+
         for i in range(0,n):
             gau.append(sum(np.exp(- 0.5 * ((x[i] - x) / h) ** 2)) / c / n / h)
         
         g = np.exp(np.mean(np.log(gau)))
         ambd = np.sqrt(g / gau)
         return ambd
```

### Comparing `tdasha-0.2.2/PKG-INFO` & `tdasha-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdasha
-Version: 0.2.2
+Version: 0.2.3
 Summary: Time-dependent Anthropogenic Seismic Hazard Assessment
 Author: Stanisław Lasocki, Francis Tong
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

