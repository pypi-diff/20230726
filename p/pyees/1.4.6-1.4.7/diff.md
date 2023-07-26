# Comparing `tmp/pyees-1.4.6.tar.gz` & `tmp/pyees-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.4.6.tar", last modified: Tue Jul 25 18:04:40 2023, max compression
+gzip compressed data, was "pyees-1.4.7.tar", last modified: Wed Jul 26 08:45:19 2023, max compression
```

## Comparing `pyees-1.4.6.tar` & `pyees-1.4.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 18:04:40.859134 pyees-1.4.6/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.4.6/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-07-25 18:04:40.864120 pyees-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 18:04:40.678614 pyees-1.4.6/pyees/
--rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.4.6/pyees/__init__.py
--rw-rw-rw-   0        0        0    18504 2023-07-16 06:55:05.000000 pyees-1.4.6/pyees/fit.py
--rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.4.6/pyees/profileFit.py
--rw-rw-rw-   0        0        0      818 2023-07-24 09:58:21.000000 pyees-1.4.6/pyees/profilePyees.py
--rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.4.6/pyees/prop.py
--rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.4.6/pyees/sheet.py
--rw-rw-rw-   0        0        0    10180 2023-07-21 06:44:16.000000 pyees-1.4.6/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.4.6/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7387 2023-07-17 06:54:59.000000 pyees-1.4.6/pyees/testFit.py
--rw-rw-rw-   0        0        0    13344 2023-07-25 17:57:15.000000 pyees-1.4.6/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2023-07-25 13:15:40.000000 pyees-1.4.6/pyees/testPyees.py
--rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.4.6/pyees/testSheet.py
--rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.4.6/pyees/testSolve.py
--rw-rw-rw-   0        0        0    10768 2023-07-21 11:19:40.000000 pyees-1.4.6/pyees/testUnit.py
--rw-rw-rw-   0        0        0    84469 2023-07-21 08:40:30.000000 pyees-1.4.6/pyees/testVariable.py
--rw-rw-rw-   0        0        0    39220 2023-07-25 18:03:03.000000 pyees-1.4.6/pyees/unit.py
--rw-rw-rw-   0        0        0    35531 2023-07-25 17:53:28.000000 pyees-1.4.6/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:04:40.838190 pyees-1.4.6/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-07-25 18:04:39.000000 pyees-1.4.6/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-07-25 18:04:39.000000 pyees-1.4.6/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 18:04:39.000000 pyees-1.4.6/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-25 18:04:39.000000 pyees-1.4.6/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-25 18:04:39.000000 pyees-1.4.6/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-25 18:04:40.891048 pyees-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-07-25 18:04:33.000000 pyees-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:45:19.823677 pyees-1.4.7/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.4.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-07-26 08:45:19.839304 pyees-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 08:45:19.479921 pyees-1.4.7/pyees/
+-rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.4.7/pyees/__init__.py
+-rw-rw-rw-   0        0        0    18504 2023-07-16 06:55:05.000000 pyees-1.4.7/pyees/fit.py
+-rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.4.7/pyees/profileFit.py
+-rw-rw-rw-   0        0        0      821 2023-07-26 08:41:19.000000 pyees-1.4.7/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.4.7/pyees/prop.py
+-rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.4.7/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10180 2023-07-21 06:44:16.000000 pyees-1.4.7/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.4.7/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7387 2023-07-17 06:54:59.000000 pyees-1.4.7/pyees/testFit.py
+-rw-rw-rw-   0        0        0    13344 2023-07-25 17:57:15.000000 pyees-1.4.7/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2023-07-25 13:15:40.000000 pyees-1.4.7/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.4.7/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.4.7/pyees/testSolve.py
+-rw-rw-rw-   0        0        0    10768 2023-07-21 11:19:40.000000 pyees-1.4.7/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    84469 2023-07-26 07:43:38.000000 pyees-1.4.7/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    38790 2023-07-26 08:45:02.000000 pyees-1.4.7/pyees/unit.py
+-rw-rw-rw-   0        0        0    35330 2023-07-26 08:43:22.000000 pyees-1.4.7/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:45:19.792428 pyees-1.4.7/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-07-26 08:45:17.000000 pyees-1.4.7/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-07-26 08:45:18.000000 pyees-1.4.7/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:45:17.000000 pyees-1.4.7/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-26 08:45:17.000000 pyees-1.4.7/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-26 08:45:17.000000 pyees-1.4.7/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-26 08:45:19.870555 pyees-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-07-26 08:45:10.000000 pyees-1.4.7/setup.py
```

### Comparing `pyees-1.4.6/LICENSE.txt` & `pyees-1.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.4.6/PKG-INFO` & `pyees-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.4.6
+Version: 1.4.7
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.4.6/README.md` & `pyees-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.4.6/pyees/fit.py` & `pyees-1.4.7/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.6/pyees/profileFit.py` & `pyees-1.4.7/pyees/profileFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.6/pyees/profilePyees.py` & `pyees-1.4.7/pyees/profilePyees.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,11 +18,11 @@
     air_speed = variable([6.5, 6, 5.5, 5, 4.5, 4, 3.5], 'm/s', [0.1, 0.15, 0.12, 0.13, 0.9, 1.1, 1.0])
     q = c * rho * v_dot * (t_in - t_out)
     q.convert('kW')
     
 pr.disable()
 s = io.StringIO()
 ps = pstats.Stats(pr, stream=s).sort_stats('tottime')
-ps.print_stats()
+ps.print_stats(100)
 
 with open('profile.txt', 'w+') as f:
     f.write(s.getvalue())
```

### Comparing `pyees-1.4.6/pyees/prop.py` & `pyees-1.4.7/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.6/pyees/sheet.py` & `pyees-1.4.7/pyees/sheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.6/pyees/solve.py` & `pyees-1.4.7/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.6/pyees/stackOverflowODR.py` & `pyees-1.4.7/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.6/pyees/testFit.py` & `pyees-1.4.7/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.6/pyees/testProp.py` & `pyees-1.4.7/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.6/pyees/testPyees.py` & `pyees-1.4.7/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.6/pyees/testSheet.py` & `pyees-1.4.7/pyees/testSheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.6/pyees/testSolve.py` & `pyees-1.4.7/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.6/pyees/testUnit.py` & `pyees-1.4.7/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.6/pyees/testVariable.py` & `pyees-1.4.7/pyees/testVariable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1536,19 +1536,19 @@
         a = variable([1, 2, 3], 'm')
         b = variable([4, 5, 6], 'm')
         c = variable([10, 11, 12], 'Pa')
         d = variable([13, 14, 15], 'Pa')
         b.addCovariance(d, [0.1, 0.2, 0.3], 'm-Pa')
         a.append(b)
         c.append(d) 
-        d = a * c
+        e = a * c
 
-        np.testing.assert_equal(d.value, np.array([1,2,3,4,5,6]) * np.array([10,11,12,13,14,15]))
-        self.assertTrue(d._unitObject == unit('m-Pa'))        
-        np.testing.assert_array_almost_equal(d.uncert, np.sqrt(2 * np.array([1,2,3,4,5,6]) * np.array([10,11,12,13,14,15]) * np.array([0,0,0,0.1,0.2,0.3])))
+        np.testing.assert_equal(e.value, np.array([1,2,3,4,5,6]) * np.array([10,11,12,13,14,15]))
+        self.assertTrue(e._unitObject == unit('m-Pa'))        
+        np.testing.assert_array_almost_equal(e.uncert, np.sqrt(2 * np.array([1,2,3,4,5,6]) * np.array([10,11,12,13,14,15]) * np.array([0,0,0,0.1,0.2,0.3])))
         
         
         a = variable([1, 2, 3], 'm')
         b = variable([4, 5, 6], 'm')
         c = variable([10, 11, 12], 'Pa')
         d = variable([13, 14, 15], 'Pa')
         b.addCovariance(c, [0.1, 0.2, 0.3], 'm-Pa')
```

### Comparing `pyees-1.4.6/pyees/unit.py` & `pyees-1.4.7/pyees/unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,28 +385,29 @@
         if converterToSI is None:
             self.getConverterToSI()
         else:
             self._converterToSI = converterToSI
 
     @staticmethod
     def _getUnitStrFromDict(unitDict):
-        upper, lower = [], []
+        upper, lower = '',''
         
         for u, item in unitDict.items():    
             for p, exp in item.items():
                 isUpper = exp > 0
                 if not isUpper: exp = - exp
                 exp = str(exp) if exp != 1 else ''
-                s = p+u+str(exp)
-                if isUpper: upper.append(s)
-                else: lower.append(s)
-        
-        out = '-'.join(upper)
-        if lower: out = out + '/' + '-'.join(lower)
-        return out
+                s = p + u + exp + '-'
+                if isUpper: upper += s
+                else: lower += s
+                
+        upper = upper[:-1]
+        if lower: upper += '/' + lower[:-1]
+        return upper
+
       
     def getUnitWithoutPrefix(self):
         
         upper, lower = [],[]
         
         for key, item in self.unitDict.items():
             exp = sum(item.values())
@@ -442,55 +443,57 @@
         return upper, lower
 
     @staticmethod
     def _splitUnitExponentAndPrefix(unitStr):
         prefixUnit, exponent = unit._removeExponentFromUnit(unitStr)
         u, prefix = unit._removePrefixFromUnit(prefixUnit)
         return u, prefix, exponent
-   
+       
     @staticmethod
     def _reduceDict(unitDict):
         
         ## loop over all units, and remove any prefixes, which has an exponenet of 0
+        n = len(unitDict)
+        keysToRemove = []
         for key, item in unitDict.items():
             prefixesToRemove = []
             for pre, exp in item.items():
                 if exp == 0:  prefixesToRemove.append(pre)
             for pre in prefixesToRemove: item.pop(pre)
-
-        ## remove the units, which has no items in their dictionary
-        keysToRemove = []
-        n = len(unitDict)
-        for key, item in unitDict.items():
-            if not item:
-                keysToRemove.append(key)
-                n -= 1
-                
+            if not item: keysToRemove.append(key)
+        n -= len(keysToRemove)        
+        
         ## if all the keys in unitDict has to be removed, then return the unit '1'
         if n == 0:
             ## return '1' if there are not other units
             return {'1': {'': 1}}
         
         ## remove the keys
         for key in keysToRemove: unitDict.pop(key)
         
         ## check if 1 is in the unit
         if '1' in unitDict:
-            if n > 1:
-                ## determine if there are any other units than '1' above the fraction line
-                otherUpper = sum([sum([1 if exp > 0 else 0 for exp in item.values()]) if (key != '1') else 0 for key, item in unitDict.items()])
-                            
+            if n > 1:     
+                otherUpper = False
+                for key, item in unitDict.items():
+                    if key == '1': continue
+                    for exp in item.values():
+                        if exp > 0:
+                            otherUpper = True
+                            break
+                    if otherUpper: break
+
+                    
                 ## if there are any other upper units, then remove 1
                 ## else set the exponent of the unit '1' to 1
                 if otherUpper:
                     unitDict.pop('1')
                     n -= 1
                 else: unitDict['1'][''] = 1
-            else:
-                unitDict['1'][''] = 1
+            else: unitDict['1'][''] = 1
                 
         ## make temperature units in to temperature differences, if there are any other units in the dict
         if n > 1:
             keysToChange = []
             for key in _temperature.keys():
                 if key in unitDict: keysToChange.append(key)
             for key in keysToChange: 
@@ -502,50 +505,40 @@
     @staticmethod
     def _getUnitDictSI(unitDict):
         out = {}
         for key, item in unitDict.items():
             exp = sum(item.values())
             unitSI = _knownUnits[key][0]
             for kkey, iitem in unitSI.items():
-                if kkey in out:
-                    for p,e in iitem.items():
-                        e = e * exp
-                        if p in out[kkey]:
-                            out[kkey][p] += e
-                        else:
-                            out[kkey][p] = e
-                else:
-                    out[kkey] = {}
-                    for p,e in iitem.items():
-                        out[kkey][p] = e * exp         
+                for p, e in iitem.items():
+                    e = e * exp
+                    if kkey in out: e = e + out[kkey][p]
+                    out[kkey] = {p: e}
+                    
                     
         out = unit._reduceDict(out)                 
         return out
 
     @staticmethod
     def _getUnitDict(unitStr):
         upper, lower = unit._splitCompositeUnit(unitStr)
 
         out = {}
-        
         nUpper = len(upper)
         for i, elem in enumerate(upper + lower):
             u, p, e = unit._splitUnitExponentAndPrefix(elem)
             if i > nUpper - 1: e = - e
             if not u in out:
                 out[u] = {p: e}
             else:
-                if not p in out[u]:
-                    out[u][p] = e
-                else:
-                    out[u][p] += e
-        
-        out = unit._reduceDict(out)
+                if p in out[u]: e += out[u][p]
+                out[u][p] = e
         
-        return out
+        return unit._reduceDict(out)
+    
    
     @ staticmethod
     def _formatUnitStr(unitStr):
         
         ## remove spaces
         unitStr = unitStr.replace(' ', '')
         
@@ -1012,11 +1005,7 @@
         if u == 'B':
             return _bellConversion()
         if u == 'Np':
             return _neperConversion()
         if u == 'oct':
             return _octaveConversion()
         return _bellConversion()
-
-    def __hash__(self):
-        return id(self)
-
```

### Comparing `pyees-1.4.6/pyees/variable.py` & `pyees-1.4.7/pyees/variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,19 @@
     
 class logarithmicVariables:
     def __init__(self):
         pass
     
     @staticmethod
     def __add__(a,b):
-        aUnit = str(a.unit)
-        bUnit =str(b.unit)
+        aUnit = a.unit
+        bUnit = b.unit
         
         aUnitWithoutPrefix = a._unitObject.getUnitWithoutPrefix()
         a.convert(aUnitWithoutPrefix)
-
         aConverter = a._unitObject.getLogarithmicConverter()
         a._unitStr = '1'
         a._unitObject = unit('')
         aConverter.convertToSignal(a)
        
         bUnitWithoutPrefix = b._unitObject.getUnitWithoutPrefix()
         b.convert(bUnitWithoutPrefix)
@@ -48,20 +47,19 @@
         c._unitObject = unit(aUnitWithoutPrefix)
         c.convert(aUnit)
 
         return c
 
     @staticmethod
     def __sub__(a,b):
-        aUnit = str(a.unit)
-        bUnit =str(b.unit)
+        aUnit = a.unit
+        bUnit = b.unit
         
         aUnitWithoutPrefix = a._unitObject.getUnitWithoutPrefix()
         a.convert(aUnitWithoutPrefix)
-
         aConverter = a._unitObject.getLogarithmicConverter()
         a._unitStr = '1'
         a._unitObject = unit('')
         aConverter.convertToSignal(a)
        
         bUnitWithoutPrefix = b._unitObject.getUnitWithoutPrefix()
         b.convert(bUnitWithoutPrefix)
@@ -232,29 +230,26 @@
     def __next__(self):
         if self.n == 0:
             self.n += 1
             return self
         raise StopIteration           
    
     def addCovariance(self, var, covariance: float, unitStr: str):
-        try:
-            float(covariance)
-        except TypeError:
-            raise ValueError(f'You tried to set the covariance between {self} and {var} with a non scalar value')
         
         covUnit = unit(unitStr)
         selfVarUnit = self._unitObject * var._unitObject
         if not covUnit.unitDictSI ==  selfVarUnit.unitDictSI:
             raise ValueError(f'The covariance of {covariance} [{unitStr}] does not match the units of {self} and {var}')
         
         covariance = covariance * covUnit._converterToSI.scale
         
         self.covariance[var] = covariance        
         var.covariance[self] = covariance
         
+        
     def _calculateUncertanty(self):
         
         variance = 0
         for var, grad in self.dependsOn.items():
             ## variance from the measurements     
             variance += (var._uncertSI * grad)**2
         
@@ -995,8 +990,7 @@
             if isinstance(uncert, np.ndarray):
                 raise ValueError('The lenght of the value has to be equal to the lenght of the uncertanty')      
     
     if isinstance(value, np.ndarray):
         return arrayVariable(value = value, unitStr = unit, uncert = uncert, nDigits = nDigits)
     else:
         return scalarVariable(value, unit, uncert, nDigits)
-
```

### Comparing `pyees-1.4.6/pyees.egg-info/PKG-INFO` & `pyees-1.4.7/pyees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.4.6
+Version: 1.4.7
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.4.6/setup.py` & `pyees-1.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.4.6',
+    version='1.4.7',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

