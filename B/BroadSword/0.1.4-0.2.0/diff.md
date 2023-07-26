# Comparing `tmp/BroadSword-0.1.4.tar.gz` & `tmp/BroadSword-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BroadSword-0.1.4.tar", last modified: Mon Jul 17 22:20:41 2023, max compression
+gzip compressed data, was "BroadSword-0.2.0.tar", last modified: Wed Jul 26 21:07:37 2023, max compression
```

## Comparing `BroadSword-0.1.4.tar` & `BroadSword-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:20:41.540843 BroadSword-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-17 22:20:29.000000 BroadSword-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-17 22:20:41.540843 BroadSword-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-17 22:20:29.000000 BroadSword-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 22:20:29.000000 BroadSword-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-17 22:20:41.540843 BroadSword-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:20:41.532843 BroadSword-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:20:41.536843 BroadSword-0.1.4/src/BroadSword/
--rw-r--r--   0 runner    (1001) docker     (123)    29722 2023-07-17 22:20:29.000000 BroadSword-0.1.4/src/BroadSword/BroadSword.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:20:29.000000 BroadSword-0.1.4/src/BroadSword/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20584 2023-07-17 22:20:29.000000 BroadSword-0.1.4/src/BroadSword/libmatrices.so
--rw-r--r--   0 runner    (1001) docker     (123)    33748 2023-07-17 22:20:29.000000 BroadSword-0.1.4/src/BroadSword/libmatrices_ARM64.dylib
--rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-07-17 22:20:29.000000 BroadSword-0.1.4/src/BroadSword/libmatrices_x86_64.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-17 22:20:29.000000 BroadSword-0.1.4/src/BroadSword/matrices.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:20:41.540843 BroadSword-0.1.4/src/BroadSword.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-17 22:20:41.000000 BroadSword-0.1.4/src/BroadSword.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-17 22:20:41.000000 BroadSword-0.1.4/src/BroadSword.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:20:41.000000 BroadSword-0.1.4/src/BroadSword.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-17 22:20:41.000000 BroadSword-0.1.4/src/BroadSword.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 22:20:41.000000 BroadSword-0.1.4/src/BroadSword.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:20:41.000000 BroadSword-0.1.4/src/BroadSword.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:07:37.052719 BroadSword-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-26 21:07:25.000000 BroadSword-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-26 21:07:37.052719 BroadSword-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-26 21:07:25.000000 BroadSword-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-26 21:07:25.000000 BroadSword-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-26 21:07:37.056719 BroadSword-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:07:37.052719 BroadSword-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:07:37.052719 BroadSword-0.2.0/src/BroadSword/
+-rw-r--r--   0 runner    (1001) docker     (123)    55658 2023-07-26 21:07:25.000000 BroadSword-0.2.0/src/BroadSword/BroadSword.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:07:25.000000 BroadSword-0.2.0/src/BroadSword/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20584 2023-07-26 21:07:25.000000 BroadSword-0.2.0/src/BroadSword/libmatrices.so
+-rw-r--r--   0 runner    (1001) docker     (123)    33748 2023-07-26 21:07:25.000000 BroadSword-0.2.0/src/BroadSword/libmatrices_ARM64.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-07-26 21:07:25.000000 BroadSword-0.2.0/src/BroadSword/libmatrices_x86_64.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-26 21:07:25.000000 BroadSword-0.2.0/src/BroadSword/matrices.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:07:37.052719 BroadSword-0.2.0/src/BroadSword.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-26 21:07:37.000000 BroadSword-0.2.0/src/BroadSword.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-26 21:07:37.000000 BroadSword-0.2.0/src/BroadSword.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:07:37.000000 BroadSword-0.2.0/src/BroadSword.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-26 21:07:37.000000 BroadSword-0.2.0/src/BroadSword.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 21:07:37.000000 BroadSword-0.2.0/src/BroadSword.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:07:36.000000 BroadSword-0.2.0/src/BroadSword.egg-info/zip-safe
```

### Comparing `BroadSword-0.1.4/LICENSE` & `BroadSword-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.4/PKG-INFO` & `BroadSword-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BroadSword
-Version: 0.1.4
+Version: 0.2.0
 Summary: Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/Cody-Somers/BroadSword
 Author: Cody Somers
 Author-email: cas003@usask.ca
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,37 +12,25 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BroadSword
 Converting the BroadSword program written by Teak Boyko from the Canadian Light Source in Saskatoon, SK, CA.
 The program has been transcribed into python so that it can be compatible with jupyter notebook.
-It still makes use of C functions as the runtime in pure Python is too long to be practically usable.
+Execution should be < 30s in the majority of cases. However when certain conditions do not align it can take > 2min. The program will warn the user of such an event.
 
 Go to the [github](https://github.com/Cody-Somers/BroadSword/tree/main) to find an example program to better understand the input file requirements.
 
 ## Installation
 
 Install the package from PyPi with the pip package manager. This is the recommended way to obtain a copy for your local machine and will install all required dependencies.
 
 ```
     $ pip install BroadSword
 ```
-After installing BroadSword the following lines may appear in the terminal.
-```
-Collecting BroadSword
-  Using cached BroadSword-0.0.15-py3-none-any.whl (21 kB)
-Requirement already satisfied: numpy in ./opt/anaconda3/lib/python3.9/site-packages (from BroadSword) (1.20.3)
-.
-.
-.
-Installing collected packages: BroadSword
-Successfully installed BroadSword-0.0.15
-```
-Take note of location that the package was installed to, as this will be needed when running the program. In this case "opt/anaconda3/lib/python3.9/site-packages"
 
 You will also need [Jupyter Notebook](https://github.com/jupyter) together with python 3 on your local machine.
 
 ## Example Program
 
 ```
 # Specify the base directory for the location of the data files
@@ -55,64 +43,71 @@
 from bokeh.io import output_notebook
 output_notebook(hide_banner=True)
 
 # Create an instance of the class
 broad = Broaden()
 
 # Load the experimental and calculations
-broad.loadExp(basedir,"N_test_XES.txt","N_test_XAS.txt",fermi=0.44996547)
-broad.loadCalc(basedir,"N1_emis.txspec","N1_abs.txspec","N1_half.txspec",fermis=0.45062079,binds=27.176237)
-broad.loadCalc(".","N2_emis.txspec","N2_abs.txspec","N2_half.txspec",fermis=0.45091878,binds=27.177975)
-broad.loadCalc(".","N3_emis.txspec","N3_abs.txspec","N3_half.txspec",fermis=0.45090808,binds=27.122234,sites=1.245)
-broad.loadCalc(".","N4_emis.txspec","N4_abs.txspec","N4_half.txspec",fermis=0.45088602,binds=27.177070,edge="L2")
+broad.loadExp(basedir,XES="N_test_XES.txt",XANES="N_test_XAS.txt",GS_fermi=0.44996547,headerlines=[2,2])
+broad.loadCalc(basedir,XES="N1_emis.txspec",XAS="N1_abs.txspec",GS_bindingEnergy=27.176237,XANES="N1_half.txspec",ES_fermi=0.45062079,sites=1,edge="L2")
+broad.loadCalc(basedir,XES="N2_emis.txspec",XAS="N2_abs.txspec",GS_bindingEnergy=27.177975,XANES="N2_half.txspec",ES_fermi=0.45091878)
+broad.loadCalc(basedir,XES="N3_emis.txspec",XAS="N3_abs.txspec",GS_bindingEnergy=27.122234,XANES="N3_half.txspec",ES_fermi=0.45090808)
+broad.loadCalc(basedir,XES="N4_emis.txspec",XAS="N4_abs.txspec",GS_bindingEnergy=27.177070,XANES="N4_half.txspec",ES_fermi=0.45088602)
+
+# broad.loadCalc(basedir,XES="N1_emis.txspec",XAS="N1_abs.txspec",GS_bindingEnergy=27.177070) # Minimum required inputs to broaden a spectra.
 
 # Initialize the broadening parameters
 broad.initResolution(corelifetime=0.15,specResolution=1200,monoResolution=5000,disorder=0.5,XESscaling=0.5,XASscaling=0.5)
 # Optionally you can scale specific bands in XEN. Use printBands() to determine where the bands are located.
 # Then add the new argument XESbandScaling into initResolution()
 # broad.printBands()
 # XESbandScaling=[[0.1,0.2,0.2,0.4],[0.2,0.2,0.4,0.2],[0.3,0.2,0.1,0.5],[0.3,0.5,0.4,0.2]])
 
 # Shift the spectra until the calculation aligns with the experimental
-broad.Shift(XESshift=19.2,XASshift=20.2)
+broad.Shift(XESshift=19.2,XASshift=20.2,separate=False)
 # Optionally you can shift specific bands in XES.
 # Add the new argument into Shift()
 # XESbandshift=[[30,33,30,20],[15,19.2,19.2,19.2],[30,33,30,20],[15,19.2,19.2,19.2]])
 
 # Broaden the spectra
-broad.broaden("/Users/cas003/opt/anaconda3/lib/python3.9/site-packages/BroadSword/")
+broad.broaden(separate=False)
 
 # Export the broadened calculated spectra
-# broad.export("Nitrogen")
+# broad.export(filename="GeP2N4",element="N",individual=False)
 ```
 
 ### Functions
 Below are the functions with their input criteria. If needed the docstrings will appear in Jupyter notebook using "shift+tab"
 
 ```
-def loadExp(self, basedir, XES, XANES, fermi):
-# Loads the measured experimental data (no headers allowed). Fermi energy is from the calculated ground state
+def loadExp(self, basedir, XES, XANES, GS_fermi, headerlines=[0,0]):
+# Loads the measured experimental data. Fermi energy is from the calculated ground state
 
-def loadCalc(self, basedir, XES, XAS, XANES, fermis, binds, edge="K", sites=1):
-# Loads the calculated data (no headers allowed). Fermis is the energy from the calculated excited state. Binding is from the ground state.
+def loadCalc(self, basedir, XES, XAS, GS_bindingEnergy, XANES=0, ES_fermi=0,  edge="K", sites=1, headerlines=[0,0,0]):
+# Loads the calculated data. The header lines are an array describing the number of header lines in the [XES, XAS, XANES] respectively.
+# Fermis is the energy from the calculated excited state. Binding is from the ground state.
 # Specifying the edge and number of sites are only required if they differ from the K edge and you have a different number of atoms between different inequivalent atoms.
 
 def printBands(self):
 # Prints out the location of the bands
 
 def initResolution(self, corelifetime, specResolution, monoResolution, disorder, XESscaling, XASscaling, XESbandScaling=0)
 # Specifies the broadening parameters based on instrument, general disorder, and lifetime broadening.
 # An optional variable to scale the bands individually is available
 
-def Shift(self,XESshift, XASshift, XESbandshift=0):
+def Shift(self,XESshift, XASshift, XESbandshift=0, separate=False):
 # Shifts the calculated spectra based on user input.
 # An optional variable to shift the bands individually is available
+# separate describes whether or not to create a separate plot for XES and XAS
 
-def broaden(self, libpath="./")
+def broaden(self, separate=True)
 # Broadens the calculated spectra. The library path will need to specified as described in the Installation segment
+# separate describes whether or not to create a separate plot for XES and XAS
 
-def export(self, filename)
+def export(self, filename, element, individual=False)
 # Exports the broadened data as a .csv file.
+# Set the filename and then the elemental edge, as well as if the broadened spectra for each individual inequivalent site should be export.
+# Ex: filename=C3N3, element=N, ouput would be C3N3_N_XES.csv
 ```
-### Comments
+### Post Script
 
 Shifting only takes ~1s to plot. Comment out the broad.broaden() function and shift the unbroadened spectra first until it is in the proper position. Then include broad.broaden() in the notebook since this can take ~30s to compute.
```

### Comparing `BroadSword-0.1.4/README.md` & `BroadSword-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,21 @@
 # BroadSword
 Converting the BroadSword program written by Teak Boyko from the Canadian Light Source in Saskatoon, SK, CA.
 The program has been transcribed into python so that it can be compatible with jupyter notebook.
-It still makes use of C functions as the runtime in pure Python is too long to be practically usable.
+Execution should be < 30s in the majority of cases. However when certain conditions do not align it can take > 2min. The program will warn the user of such an event.
 
 Go to the [github](https://github.com/Cody-Somers/BroadSword/tree/main) to find an example program to better understand the input file requirements.
 
 ## Installation
 
 Install the package from PyPi with the pip package manager. This is the recommended way to obtain a copy for your local machine and will install all required dependencies.
 
 ```
     $ pip install BroadSword
 ```
-After installing BroadSword the following lines may appear in the terminal.
-```
-Collecting BroadSword
-  Using cached BroadSword-0.0.15-py3-none-any.whl (21 kB)
-Requirement already satisfied: numpy in ./opt/anaconda3/lib/python3.9/site-packages (from BroadSword) (1.20.3)
-.
-.
-.
-Installing collected packages: BroadSword
-Successfully installed BroadSword-0.0.15
-```
-Take note of location that the package was installed to, as this will be needed when running the program. In this case "opt/anaconda3/lib/python3.9/site-packages"
 
 You will also need [Jupyter Notebook](https://github.com/jupyter) together with python 3 on your local machine.
 
 ## Example Program
 
 ```
 # Specify the base directory for the location of the data files
@@ -40,64 +28,71 @@
 from bokeh.io import output_notebook
 output_notebook(hide_banner=True)
 
 # Create an instance of the class
 broad = Broaden()
 
 # Load the experimental and calculations
-broad.loadExp(basedir,"N_test_XES.txt","N_test_XAS.txt",fermi=0.44996547)
-broad.loadCalc(basedir,"N1_emis.txspec","N1_abs.txspec","N1_half.txspec",fermis=0.45062079,binds=27.176237)
-broad.loadCalc(".","N2_emis.txspec","N2_abs.txspec","N2_half.txspec",fermis=0.45091878,binds=27.177975)
-broad.loadCalc(".","N3_emis.txspec","N3_abs.txspec","N3_half.txspec",fermis=0.45090808,binds=27.122234,sites=1.245)
-broad.loadCalc(".","N4_emis.txspec","N4_abs.txspec","N4_half.txspec",fermis=0.45088602,binds=27.177070,edge="L2")
+broad.loadExp(basedir,XES="N_test_XES.txt",XANES="N_test_XAS.txt",GS_fermi=0.44996547,headerlines=[2,2])
+broad.loadCalc(basedir,XES="N1_emis.txspec",XAS="N1_abs.txspec",GS_bindingEnergy=27.176237,XANES="N1_half.txspec",ES_fermi=0.45062079,sites=1,edge="L2")
+broad.loadCalc(basedir,XES="N2_emis.txspec",XAS="N2_abs.txspec",GS_bindingEnergy=27.177975,XANES="N2_half.txspec",ES_fermi=0.45091878)
+broad.loadCalc(basedir,XES="N3_emis.txspec",XAS="N3_abs.txspec",GS_bindingEnergy=27.122234,XANES="N3_half.txspec",ES_fermi=0.45090808)
+broad.loadCalc(basedir,XES="N4_emis.txspec",XAS="N4_abs.txspec",GS_bindingEnergy=27.177070,XANES="N4_half.txspec",ES_fermi=0.45088602)
+
+# broad.loadCalc(basedir,XES="N1_emis.txspec",XAS="N1_abs.txspec",GS_bindingEnergy=27.177070) # Minimum required inputs to broaden a spectra.
 
 # Initialize the broadening parameters
 broad.initResolution(corelifetime=0.15,specResolution=1200,monoResolution=5000,disorder=0.5,XESscaling=0.5,XASscaling=0.5)
 # Optionally you can scale specific bands in XEN. Use printBands() to determine where the bands are located.
 # Then add the new argument XESbandScaling into initResolution()
 # broad.printBands()
 # XESbandScaling=[[0.1,0.2,0.2,0.4],[0.2,0.2,0.4,0.2],[0.3,0.2,0.1,0.5],[0.3,0.5,0.4,0.2]])
 
 # Shift the spectra until the calculation aligns with the experimental
-broad.Shift(XESshift=19.2,XASshift=20.2)
+broad.Shift(XESshift=19.2,XASshift=20.2,separate=False)
 # Optionally you can shift specific bands in XES.
 # Add the new argument into Shift()
 # XESbandshift=[[30,33,30,20],[15,19.2,19.2,19.2],[30,33,30,20],[15,19.2,19.2,19.2]])
 
 # Broaden the spectra
-broad.broaden("/Users/cas003/opt/anaconda3/lib/python3.9/site-packages/BroadSword/")
+broad.broaden(separate=False)
 
 # Export the broadened calculated spectra
-# broad.export("Nitrogen")
+# broad.export(filename="GeP2N4",element="N",individual=False)
 ```
 
 ### Functions
 Below are the functions with their input criteria. If needed the docstrings will appear in Jupyter notebook using "shift+tab"
 
 ```
-def loadExp(self, basedir, XES, XANES, fermi):
-# Loads the measured experimental data (no headers allowed). Fermi energy is from the calculated ground state
+def loadExp(self, basedir, XES, XANES, GS_fermi, headerlines=[0,0]):
+# Loads the measured experimental data. Fermi energy is from the calculated ground state
 
-def loadCalc(self, basedir, XES, XAS, XANES, fermis, binds, edge="K", sites=1):
-# Loads the calculated data (no headers allowed). Fermis is the energy from the calculated excited state. Binding is from the ground state.
+def loadCalc(self, basedir, XES, XAS, GS_bindingEnergy, XANES=0, ES_fermi=0,  edge="K", sites=1, headerlines=[0,0,0]):
+# Loads the calculated data. The header lines are an array describing the number of header lines in the [XES, XAS, XANES] respectively.
+# Fermis is the energy from the calculated excited state. Binding is from the ground state.
 # Specifying the edge and number of sites are only required if they differ from the K edge and you have a different number of atoms between different inequivalent atoms.
 
 def printBands(self):
 # Prints out the location of the bands
 
 def initResolution(self, corelifetime, specResolution, monoResolution, disorder, XESscaling, XASscaling, XESbandScaling=0)
 # Specifies the broadening parameters based on instrument, general disorder, and lifetime broadening.
 # An optional variable to scale the bands individually is available
 
-def Shift(self,XESshift, XASshift, XESbandshift=0):
+def Shift(self,XESshift, XASshift, XESbandshift=0, separate=False):
 # Shifts the calculated spectra based on user input.
 # An optional variable to shift the bands individually is available
+# separate describes whether or not to create a separate plot for XES and XAS
 
-def broaden(self, libpath="./")
+def broaden(self, separate=True)
 # Broadens the calculated spectra. The library path will need to specified as described in the Installation segment
+# separate describes whether or not to create a separate plot for XES and XAS
 
-def export(self, filename)
+def export(self, filename, element, individual=False)
 # Exports the broadened data as a .csv file.
+# Set the filename and then the elemental edge, as well as if the broadened spectra for each individual inequivalent site should be export.
+# Ex: filename=C3N3, element=N, ouput would be C3N3_N_XES.csv
 ```
-### Comments
+### Post Script
 
 Shifting only takes ~1s to plot. Comment out the broad.broaden() function and shift the unbroadened spectra first until it is in the proper position. Then include broad.broaden() in the notebook since this can take ~30s to compute.
```

### Comparing `BroadSword-0.1.4/setup.cfg` & `BroadSword-0.2.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = BroadSword
-version = 0.1.4
+version = 0.2.0
 author = Cody Somers
 author_email = cas003@usask.ca
 description = Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Cody-Somers/BroadSword
 project_urls =
```

### Comparing `BroadSword-0.1.4/src/BroadSword/libmatrices.so` & `BroadSword-0.2.0/src/BroadSword/libmatrices.so`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.4/src/BroadSword/libmatrices_ARM64.dylib` & `BroadSword-0.2.0/src/BroadSword/libmatrices_ARM64.dylib`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.4/src/BroadSword/libmatrices_x86_64.dylib` & `BroadSword-0.2.0/src/BroadSword/libmatrices_x86_64.dylib`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.4/src/BroadSword/matrices.c` & `BroadSword-0.2.0/src/BroadSword/matrices.c`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.4/src/BroadSword.egg-info/PKG-INFO` & `BroadSword-0.2.0/src/BroadSword.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BroadSword
-Version: 0.1.4
+Version: 0.2.0
 Summary: Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/Cody-Somers/BroadSword
 Author: Cody Somers
 Author-email: cas003@usask.ca
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,37 +12,25 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BroadSword
 Converting the BroadSword program written by Teak Boyko from the Canadian Light Source in Saskatoon, SK, CA.
 The program has been transcribed into python so that it can be compatible with jupyter notebook.
-It still makes use of C functions as the runtime in pure Python is too long to be practically usable.
+Execution should be < 30s in the majority of cases. However when certain conditions do not align it can take > 2min. The program will warn the user of such an event.
 
 Go to the [github](https://github.com/Cody-Somers/BroadSword/tree/main) to find an example program to better understand the input file requirements.
 
 ## Installation
 
 Install the package from PyPi with the pip package manager. This is the recommended way to obtain a copy for your local machine and will install all required dependencies.
 
 ```
     $ pip install BroadSword
 ```
-After installing BroadSword the following lines may appear in the terminal.
-```
-Collecting BroadSword
-  Using cached BroadSword-0.0.15-py3-none-any.whl (21 kB)
-Requirement already satisfied: numpy in ./opt/anaconda3/lib/python3.9/site-packages (from BroadSword) (1.20.3)
-.
-.
-.
-Installing collected packages: BroadSword
-Successfully installed BroadSword-0.0.15
-```
-Take note of location that the package was installed to, as this will be needed when running the program. In this case "opt/anaconda3/lib/python3.9/site-packages"
 
 You will also need [Jupyter Notebook](https://github.com/jupyter) together with python 3 on your local machine.
 
 ## Example Program
 
 ```
 # Specify the base directory for the location of the data files
@@ -55,64 +43,71 @@
 from bokeh.io import output_notebook
 output_notebook(hide_banner=True)
 
 # Create an instance of the class
 broad = Broaden()
 
 # Load the experimental and calculations
-broad.loadExp(basedir,"N_test_XES.txt","N_test_XAS.txt",fermi=0.44996547)
-broad.loadCalc(basedir,"N1_emis.txspec","N1_abs.txspec","N1_half.txspec",fermis=0.45062079,binds=27.176237)
-broad.loadCalc(".","N2_emis.txspec","N2_abs.txspec","N2_half.txspec",fermis=0.45091878,binds=27.177975)
-broad.loadCalc(".","N3_emis.txspec","N3_abs.txspec","N3_half.txspec",fermis=0.45090808,binds=27.122234,sites=1.245)
-broad.loadCalc(".","N4_emis.txspec","N4_abs.txspec","N4_half.txspec",fermis=0.45088602,binds=27.177070,edge="L2")
+broad.loadExp(basedir,XES="N_test_XES.txt",XANES="N_test_XAS.txt",GS_fermi=0.44996547,headerlines=[2,2])
+broad.loadCalc(basedir,XES="N1_emis.txspec",XAS="N1_abs.txspec",GS_bindingEnergy=27.176237,XANES="N1_half.txspec",ES_fermi=0.45062079,sites=1,edge="L2")
+broad.loadCalc(basedir,XES="N2_emis.txspec",XAS="N2_abs.txspec",GS_bindingEnergy=27.177975,XANES="N2_half.txspec",ES_fermi=0.45091878)
+broad.loadCalc(basedir,XES="N3_emis.txspec",XAS="N3_abs.txspec",GS_bindingEnergy=27.122234,XANES="N3_half.txspec",ES_fermi=0.45090808)
+broad.loadCalc(basedir,XES="N4_emis.txspec",XAS="N4_abs.txspec",GS_bindingEnergy=27.177070,XANES="N4_half.txspec",ES_fermi=0.45088602)
+
+# broad.loadCalc(basedir,XES="N1_emis.txspec",XAS="N1_abs.txspec",GS_bindingEnergy=27.177070) # Minimum required inputs to broaden a spectra.
 
 # Initialize the broadening parameters
 broad.initResolution(corelifetime=0.15,specResolution=1200,monoResolution=5000,disorder=0.5,XESscaling=0.5,XASscaling=0.5)
 # Optionally you can scale specific bands in XEN. Use printBands() to determine where the bands are located.
 # Then add the new argument XESbandScaling into initResolution()
 # broad.printBands()
 # XESbandScaling=[[0.1,0.2,0.2,0.4],[0.2,0.2,0.4,0.2],[0.3,0.2,0.1,0.5],[0.3,0.5,0.4,0.2]])
 
 # Shift the spectra until the calculation aligns with the experimental
-broad.Shift(XESshift=19.2,XASshift=20.2)
+broad.Shift(XESshift=19.2,XASshift=20.2,separate=False)
 # Optionally you can shift specific bands in XES.
 # Add the new argument into Shift()
 # XESbandshift=[[30,33,30,20],[15,19.2,19.2,19.2],[30,33,30,20],[15,19.2,19.2,19.2]])
 
 # Broaden the spectra
-broad.broaden("/Users/cas003/opt/anaconda3/lib/python3.9/site-packages/BroadSword/")
+broad.broaden(separate=False)
 
 # Export the broadened calculated spectra
-# broad.export("Nitrogen")
+# broad.export(filename="GeP2N4",element="N",individual=False)
 ```
 
 ### Functions
 Below are the functions with their input criteria. If needed the docstrings will appear in Jupyter notebook using "shift+tab"
 
 ```
-def loadExp(self, basedir, XES, XANES, fermi):
-# Loads the measured experimental data (no headers allowed). Fermi energy is from the calculated ground state
+def loadExp(self, basedir, XES, XANES, GS_fermi, headerlines=[0,0]):
+# Loads the measured experimental data. Fermi energy is from the calculated ground state
 
-def loadCalc(self, basedir, XES, XAS, XANES, fermis, binds, edge="K", sites=1):
-# Loads the calculated data (no headers allowed). Fermis is the energy from the calculated excited state. Binding is from the ground state.
+def loadCalc(self, basedir, XES, XAS, GS_bindingEnergy, XANES=0, ES_fermi=0,  edge="K", sites=1, headerlines=[0,0,0]):
+# Loads the calculated data. The header lines are an array describing the number of header lines in the [XES, XAS, XANES] respectively.
+# Fermis is the energy from the calculated excited state. Binding is from the ground state.
 # Specifying the edge and number of sites are only required if they differ from the K edge and you have a different number of atoms between different inequivalent atoms.
 
 def printBands(self):
 # Prints out the location of the bands
 
 def initResolution(self, corelifetime, specResolution, monoResolution, disorder, XESscaling, XASscaling, XESbandScaling=0)
 # Specifies the broadening parameters based on instrument, general disorder, and lifetime broadening.
 # An optional variable to scale the bands individually is available
 
-def Shift(self,XESshift, XASshift, XESbandshift=0):
+def Shift(self,XESshift, XASshift, XESbandshift=0, separate=False):
 # Shifts the calculated spectra based on user input.
 # An optional variable to shift the bands individually is available
+# separate describes whether or not to create a separate plot for XES and XAS
 
-def broaden(self, libpath="./")
+def broaden(self, separate=True)
 # Broadens the calculated spectra. The library path will need to specified as described in the Installation segment
+# separate describes whether or not to create a separate plot for XES and XAS
 
-def export(self, filename)
+def export(self, filename, element, individual=False)
 # Exports the broadened data as a .csv file.
+# Set the filename and then the elemental edge, as well as if the broadened spectra for each individual inequivalent site should be export.
+# Ex: filename=C3N3, element=N, ouput would be C3N3_N_XES.csv
 ```
-### Comments
+### Post Script
 
 Shifting only takes ~1s to plot. Comment out the broad.broaden() function and shift the unbroadened spectra first until it is in the proper position. Then include broad.broaden() in the notebook since this can take ~30s to compute.
```

